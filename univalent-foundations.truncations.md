---
title: Formalisation of the Symmetry Book
---

<pre class="Agda"><a id="60" class="Symbol">{-#</a> <a id="64" class="Keyword">OPTIONS</a> <a id="72" class="Pragma">--without-K</a> <a id="84" class="Pragma">--exact-split</a> <a id="98" class="Pragma">--allow-unsolved-metas</a> <a id="121" class="Symbol">#-}</a>

<a id="126" class="Keyword">module</a> <a id="133" href="univalent-foundations.truncations.html" class="Module">univalent-foundations.truncations</a> <a id="167" class="Keyword">where</a>

<a id="174" class="Keyword">open</a> <a id="179" class="Keyword">import</a> <a id="186" href="foundation.html" class="Module">foundation</a>
<a id="197" class="Keyword">open</a> <a id="202" class="Keyword">import</a> <a id="209" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="234" class="Keyword">open</a> <a id="239" class="Keyword">import</a> <a id="246" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
<a id="270" class="Keyword">open</a> <a id="275" class="Keyword">import</a> <a id="282" href="univalent-foundations.html" class="Module">univalent-foundations</a>

</pre>
# Truncations

## The condition on a map to be a truncation

<pre class="Agda"><a id="precomp-Trunc"></a><a id="379" href="univalent-foundations.truncations.html#379" class="Function">precomp-Trunc</a> <a id="393" class="Symbol">:</a>
  <a id="397" class="Symbol">{</a><a id="398" href="univalent-foundations.truncations.html#398" class="Bound">l1</a> <a id="401" href="univalent-foundations.truncations.html#401" class="Bound">l2</a> <a id="404" href="univalent-foundations.truncations.html#404" class="Bound">l3</a> <a id="407" class="Symbol">:</a> <a id="409" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="414" class="Symbol">}</a> <a id="416" class="Symbol">{</a><a id="417" href="univalent-foundations.truncations.html#417" class="Bound">k</a> <a id="419" class="Symbol">:</a> <a id="421" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="422" class="Symbol">}</a> <a id="424" class="Symbol">{</a><a id="425" href="univalent-foundations.truncations.html#425" class="Bound">A</a> <a id="427" class="Symbol">:</a> <a id="429" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="432" href="univalent-foundations.truncations.html#398" class="Bound">l1</a><a id="434" class="Symbol">}</a> <a id="436" class="Symbol">{</a><a id="437" href="univalent-foundations.truncations.html#437" class="Bound">B</a> <a id="439" class="Symbol">:</a> <a id="441" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="444" href="univalent-foundations.truncations.html#401" class="Bound">l2</a><a id="446" class="Symbol">}</a> <a id="448" class="Symbol">(</a><a id="449" href="univalent-foundations.truncations.html#449" class="Bound">f</a> <a id="451" class="Symbol">:</a> <a id="453" href="univalent-foundations.truncations.html#425" class="Bound">A</a> <a id="455" class="Symbol">→</a> <a id="457" href="univalent-foundations.truncations.html#437" class="Bound">B</a><a id="458" class="Symbol">)</a>
  <a id="462" class="Symbol">(</a><a id="463" href="univalent-foundations.truncations.html#463" class="Bound">C</a> <a id="465" class="Symbol">:</a> <a id="467" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="485" href="univalent-foundations.truncations.html#404" class="Bound">l3</a> <a id="488" href="univalent-foundations.truncations.html#417" class="Bound">k</a><a id="489" class="Symbol">)</a> <a id="491" class="Symbol">→</a>
  <a id="495" class="Symbol">(</a><a id="496" href="univalent-foundations.truncations.html#437" class="Bound">B</a> <a id="498" class="Symbol">→</a> <a id="500" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="520" href="univalent-foundations.truncations.html#463" class="Bound">C</a><a id="521" class="Symbol">)</a> <a id="523" class="Symbol">→</a> <a id="525" class="Symbol">(</a><a id="526" href="univalent-foundations.truncations.html#425" class="Bound">A</a> <a id="528" class="Symbol">→</a> <a id="530" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="550" href="univalent-foundations.truncations.html#463" class="Bound">C</a><a id="551" class="Symbol">)</a>
<a id="553" href="univalent-foundations.truncations.html#379" class="Function">precomp-Trunc</a> <a id="567" href="univalent-foundations.truncations.html#567" class="Bound">f</a> <a id="569" href="univalent-foundations.truncations.html#569" class="Bound">C</a> <a id="571" class="Symbol">=</a> <a id="573" href="foundation-core.functions.html#925" class="Function">precomp</a> <a id="581" href="univalent-foundations.truncations.html#567" class="Bound">f</a> <a id="583" class="Symbol">(</a><a id="584" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="604" href="univalent-foundations.truncations.html#569" class="Bound">C</a><a id="605" class="Symbol">)</a>

<a id="is-truncation"></a><a id="608" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="622" class="Symbol">:</a>
  <a id="626" class="Symbol">{</a><a id="627" href="univalent-foundations.truncations.html#627" class="Bound">l1</a> <a id="630" href="univalent-foundations.truncations.html#630" class="Bound">l2</a> <a id="633" class="Symbol">:</a> <a id="635" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="640" class="Symbol">}</a> <a id="642" class="Symbol">(</a><a id="643" href="univalent-foundations.truncations.html#643" class="Bound">l</a> <a id="645" class="Symbol">:</a> <a id="647" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="652" class="Symbol">)</a> <a id="654" class="Symbol">{</a><a id="655" href="univalent-foundations.truncations.html#655" class="Bound">k</a> <a id="657" class="Symbol">:</a> <a id="659" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="660" class="Symbol">}</a> <a id="662" class="Symbol">{</a><a id="663" href="univalent-foundations.truncations.html#663" class="Bound">A</a> <a id="665" class="Symbol">:</a> <a id="667" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="670" href="univalent-foundations.truncations.html#627" class="Bound">l1</a><a id="672" class="Symbol">}</a>
  <a id="676" class="Symbol">(</a><a id="677" href="univalent-foundations.truncations.html#677" class="Bound">B</a> <a id="679" class="Symbol">:</a> <a id="681" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="699" href="univalent-foundations.truncations.html#630" class="Bound">l2</a> <a id="702" href="univalent-foundations.truncations.html#655" class="Bound">k</a><a id="703" class="Symbol">)</a> <a id="705" class="Symbol">→</a> <a id="707" class="Symbol">(</a><a id="708" href="univalent-foundations.truncations.html#663" class="Bound">A</a> <a id="710" class="Symbol">→</a> <a id="712" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="732" href="univalent-foundations.truncations.html#677" class="Bound">B</a><a id="733" class="Symbol">)</a> <a id="735" class="Symbol">→</a>
  <a id="739" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="742" class="Symbol">(</a><a id="743" href="univalent-foundations.truncations.html#627" class="Bound">l1</a> <a id="746" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="748" href="univalent-foundations.truncations.html#630" class="Bound">l2</a> <a id="751" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="753" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="758" href="univalent-foundations.truncations.html#643" class="Bound">l</a><a id="759" class="Symbol">)</a>
<a id="761" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="775" href="univalent-foundations.truncations.html#775" class="Bound">l</a> <a id="777" class="Symbol">{</a><a id="778" href="univalent-foundations.truncations.html#778" class="Bound">k</a><a id="779" class="Symbol">}</a> <a id="781" href="univalent-foundations.truncations.html#781" class="Bound">B</a> <a id="783" href="univalent-foundations.truncations.html#783" class="Bound">f</a> <a id="785" class="Symbol">=</a>
  <a id="789" class="Symbol">(</a><a id="790" href="univalent-foundations.truncations.html#790" class="Bound">C</a> <a id="792" class="Symbol">:</a> <a id="794" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="812" href="univalent-foundations.truncations.html#775" class="Bound">l</a> <a id="814" href="univalent-foundations.truncations.html#778" class="Bound">k</a><a id="815" class="Symbol">)</a> <a id="817" class="Symbol">→</a> <a id="819" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a> <a id="828" class="Symbol">(</a><a id="829" href="univalent-foundations.truncations.html#379" class="Function">precomp-Trunc</a> <a id="843" href="univalent-foundations.truncations.html#783" class="Bound">f</a> <a id="845" href="univalent-foundations.truncations.html#790" class="Bound">C</a><a id="846" class="Symbol">)</a>
</pre>
## The universal property of truncations

<pre class="Agda"><a id="universal-property-truncation"></a><a id="903" href="univalent-foundations.truncations.html#903" class="Function">universal-property-truncation</a> <a id="933" class="Symbol">:</a>
  <a id="937" class="Symbol">(</a><a id="938" href="univalent-foundations.truncations.html#938" class="Bound">l</a> <a id="940" class="Symbol">:</a> <a id="942" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="947" class="Symbol">)</a> <a id="949" class="Symbol">{</a><a id="950" href="univalent-foundations.truncations.html#950" class="Bound">l1</a> <a id="953" href="univalent-foundations.truncations.html#953" class="Bound">l2</a> <a id="956" class="Symbol">:</a> <a id="958" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="963" class="Symbol">}</a> <a id="965" class="Symbol">{</a><a id="966" href="univalent-foundations.truncations.html#966" class="Bound">k</a> <a id="968" class="Symbol">:</a> <a id="970" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="971" class="Symbol">}</a> <a id="973" class="Symbol">{</a><a id="974" href="univalent-foundations.truncations.html#974" class="Bound">A</a> <a id="976" class="Symbol">:</a> <a id="978" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="981" href="univalent-foundations.truncations.html#950" class="Bound">l1</a><a id="983" class="Symbol">}</a>
  <a id="987" class="Symbol">(</a><a id="988" href="univalent-foundations.truncations.html#988" class="Bound">B</a> <a id="990" class="Symbol">:</a> <a id="992" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="1010" href="univalent-foundations.truncations.html#953" class="Bound">l2</a> <a id="1013" href="univalent-foundations.truncations.html#966" class="Bound">k</a><a id="1014" class="Symbol">)</a> <a id="1016" class="Symbol">(</a><a id="1017" href="univalent-foundations.truncations.html#1017" class="Bound">f</a> <a id="1019" class="Symbol">:</a> <a id="1021" href="univalent-foundations.truncations.html#974" class="Bound">A</a> <a id="1023" class="Symbol">→</a> <a id="1025" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="1045" href="univalent-foundations.truncations.html#988" class="Bound">B</a><a id="1046" class="Symbol">)</a> <a id="1048" class="Symbol">→</a>
  <a id="1052" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="1055" class="Symbol">(</a><a id="1056" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1061" href="univalent-foundations.truncations.html#938" class="Bound">l</a> <a id="1063" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1065" href="univalent-foundations.truncations.html#950" class="Bound">l1</a> <a id="1068" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1070" href="univalent-foundations.truncations.html#953" class="Bound">l2</a><a id="1072" class="Symbol">)</a>
<a id="1074" href="univalent-foundations.truncations.html#903" class="Function">universal-property-truncation</a> <a id="1104" href="univalent-foundations.truncations.html#1104" class="Bound">l</a> <a id="1106" class="Symbol">{</a><a id="1107" class="Argument">k</a> <a id="1109" class="Symbol">=</a> <a id="1111" href="univalent-foundations.truncations.html#1111" class="Bound">k</a><a id="1112" class="Symbol">}</a> <a id="1114" class="Symbol">{</a><a id="1115" href="univalent-foundations.truncations.html#1115" class="Bound">A</a><a id="1116" class="Symbol">}</a> <a id="1118" href="univalent-foundations.truncations.html#1118" class="Bound">B</a> <a id="1120" href="univalent-foundations.truncations.html#1120" class="Bound">f</a> <a id="1122" class="Symbol">=</a>
  <a id="1126" class="Symbol">(</a><a id="1127" href="univalent-foundations.truncations.html#1127" class="Bound">C</a> <a id="1129" class="Symbol">:</a> <a id="1131" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="1149" href="univalent-foundations.truncations.html#1104" class="Bound">l</a> <a id="1151" href="univalent-foundations.truncations.html#1111" class="Bound">k</a><a id="1152" class="Symbol">)</a> <a id="1154" class="Symbol">(</a><a id="1155" href="univalent-foundations.truncations.html#1155" class="Bound">g</a> <a id="1157" class="Symbol">:</a> <a id="1159" href="univalent-foundations.truncations.html#1115" class="Bound">A</a> <a id="1161" class="Symbol">→</a> <a id="1163" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="1183" href="univalent-foundations.truncations.html#1127" class="Bound">C</a><a id="1184" class="Symbol">)</a> <a id="1186" class="Symbol">→</a>
  <a id="1190" href="foundation-core.contractible-types.html#925" class="Function">is-contr</a> <a id="1199" class="Symbol">(</a><a id="1200" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="1202" class="Symbol">(</a><a id="1203" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="1227" href="univalent-foundations.truncations.html#1111" class="Bound">k</a> <a id="1229" href="univalent-foundations.truncations.html#1118" class="Bound">B</a> <a id="1231" href="univalent-foundations.truncations.html#1127" class="Bound">C</a><a id="1232" class="Symbol">)</a> <a id="1234" class="Symbol">(λ</a> <a id="1237" href="univalent-foundations.truncations.html#1237" class="Bound">h</a> <a id="1239" class="Symbol">→</a> <a id="1241" class="Symbol">(</a><a id="1242" href="univalent-foundations.truncations.html#1237" class="Bound">h</a> <a id="1244" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="1246" href="univalent-foundations.truncations.html#1120" class="Bound">f</a><a id="1247" class="Symbol">)</a> <a id="1249" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="1251" href="univalent-foundations.truncations.html#1155" class="Bound">g</a><a id="1252" class="Symbol">))</a>

<a id="1256" class="Keyword">module</a> <a id="1263" href="univalent-foundations.truncations.html#1263" class="Module">_</a>
  <a id="1267" class="Symbol">{</a><a id="1268" href="univalent-foundations.truncations.html#1268" class="Bound">l1</a> <a id="1271" href="univalent-foundations.truncations.html#1271" class="Bound">l2</a> <a id="1274" class="Symbol">:</a> <a id="1276" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1281" class="Symbol">}</a> <a id="1283" class="Symbol">{</a><a id="1284" href="univalent-foundations.truncations.html#1284" class="Bound">k</a> <a id="1286" class="Symbol">:</a> <a id="1288" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="1289" class="Symbol">}</a> <a id="1291" class="Symbol">{</a><a id="1292" href="univalent-foundations.truncations.html#1292" class="Bound">A</a> <a id="1294" class="Symbol">:</a> <a id="1296" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="1299" href="univalent-foundations.truncations.html#1268" class="Bound">l1</a><a id="1301" class="Symbol">}</a> <a id="1303" class="Symbol">(</a><a id="1304" href="univalent-foundations.truncations.html#1304" class="Bound">B</a> <a id="1306" class="Symbol">:</a> <a id="1308" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="1326" href="univalent-foundations.truncations.html#1271" class="Bound">l2</a> <a id="1329" href="univalent-foundations.truncations.html#1284" class="Bound">k</a><a id="1330" class="Symbol">)</a>
  <a id="1334" class="Symbol">(</a><a id="1335" href="univalent-foundations.truncations.html#1335" class="Bound">f</a> <a id="1337" class="Symbol">:</a> <a id="1339" href="univalent-foundations.truncations.html#1292" class="Bound">A</a> <a id="1341" class="Symbol">→</a> <a id="1343" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="1363" href="univalent-foundations.truncations.html#1304" class="Bound">B</a><a id="1364" class="Symbol">)</a>
  <a id="1368" class="Keyword">where</a>

  <a id="1377" class="Keyword">abstract</a>
    <a id="1390" href="univalent-foundations.truncations.html#1390" class="Function">is-truncation-universal-property-truncation</a> <a id="1434" class="Symbol">:</a>
      <a id="1442" class="Symbol">({</a><a id="1444" href="univalent-foundations.truncations.html#1444" class="Bound">l</a> <a id="1446" class="Symbol">:</a> <a id="1448" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1453" class="Symbol">}</a> <a id="1455" class="Symbol">→</a> <a id="1457" href="univalent-foundations.truncations.html#903" class="Function">universal-property-truncation</a> <a id="1487" href="univalent-foundations.truncations.html#1444" class="Bound">l</a> <a id="1489" href="univalent-foundations.truncations.html#1304" class="Bound">B</a> <a id="1491" href="univalent-foundations.truncations.html#1335" class="Bound">f</a><a id="1492" class="Symbol">)</a> <a id="1494" class="Symbol">→</a>
      <a id="1502" class="Symbol">({</a><a id="1504" href="univalent-foundations.truncations.html#1504" class="Bound">l</a> <a id="1506" class="Symbol">:</a> <a id="1508" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1513" class="Symbol">}</a> <a id="1515" class="Symbol">→</a> <a id="1517" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="1531" href="univalent-foundations.truncations.html#1504" class="Bound">l</a> <a id="1533" href="univalent-foundations.truncations.html#1304" class="Bound">B</a> <a id="1535" href="univalent-foundations.truncations.html#1335" class="Bound">f</a><a id="1536" class="Symbol">)</a>
    <a id="1542" href="univalent-foundations.truncations.html#1390" class="Function">is-truncation-universal-property-truncation</a> <a id="1586" href="univalent-foundations.truncations.html#1586" class="Bound">H</a> <a id="1588" href="univalent-foundations.truncations.html#1588" class="Bound">C</a> <a id="1590" class="Symbol">=</a>
      <a id="1598" href="foundation-core.contractible-maps.html#2368" class="Function">is-equiv-is-contr-map</a>
        <a id="1628" class="Symbol">(</a> <a id="1630" class="Symbol">λ</a> <a id="1632" href="univalent-foundations.truncations.html#1632" class="Bound">g</a> <a id="1634" class="Symbol">→</a>
          <a id="1646" href="foundation-core.contractible-types.html#3230" class="Function">is-contr-equiv</a>
            <a id="1673" class="Symbol">(</a> <a id="1675" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="1677" class="Symbol">(</a><a id="1678" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="1702" href="univalent-foundations.truncations.html#1284" class="Bound">k</a> <a id="1704" href="univalent-foundations.truncations.html#1304" class="Bound">B</a> <a id="1706" href="univalent-foundations.truncations.html#1588" class="Bound">C</a><a id="1707" class="Symbol">)</a> <a id="1709" class="Symbol">(λ</a> <a id="1712" href="univalent-foundations.truncations.html#1712" class="Bound">h</a> <a id="1714" class="Symbol">→</a> <a id="1716" class="Symbol">(</a><a id="1717" href="univalent-foundations.truncations.html#1712" class="Bound">h</a> <a id="1719" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="1721" href="univalent-foundations.truncations.html#1335" class="Bound">f</a><a id="1722" class="Symbol">)</a> <a id="1724" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="1726" href="univalent-foundations.truncations.html#1632" class="Bound">g</a><a id="1727" class="Symbol">))</a>
            <a id="1742" class="Symbol">(</a> <a id="1744" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a> <a id="1754" class="Symbol">(λ</a> <a id="1757" href="univalent-foundations.truncations.html#1757" class="Bound">h</a> <a id="1759" class="Symbol">→</a> <a id="1761" href="foundation.function-extensionality.html#1283" class="Function">equiv-funext</a><a id="1773" class="Symbol">))</a>
            <a id="1788" class="Symbol">(</a> <a id="1790" href="univalent-foundations.truncations.html#1586" class="Bound">H</a> <a id="1792" href="univalent-foundations.truncations.html#1588" class="Bound">C</a> <a id="1794" href="univalent-foundations.truncations.html#1632" class="Bound">g</a><a id="1795" class="Symbol">))</a>

  <a id="1801" class="Keyword">abstract</a>
    <a id="1814" href="univalent-foundations.truncations.html#1814" class="Function">universal-property-truncation-is-truncation</a> <a id="1858" class="Symbol">:</a>
      <a id="1866" class="Symbol">({</a><a id="1868" href="univalent-foundations.truncations.html#1868" class="Bound">l</a> <a id="1870" class="Symbol">:</a> <a id="1872" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1877" class="Symbol">}</a> <a id="1879" class="Symbol">→</a> <a id="1881" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="1895" href="univalent-foundations.truncations.html#1868" class="Bound">l</a> <a id="1897" href="univalent-foundations.truncations.html#1304" class="Bound">B</a> <a id="1899" href="univalent-foundations.truncations.html#1335" class="Bound">f</a><a id="1900" class="Symbol">)</a> <a id="1902" class="Symbol">→</a>
      <a id="1910" class="Symbol">({</a><a id="1912" href="univalent-foundations.truncations.html#1912" class="Bound">l</a> <a id="1914" class="Symbol">:</a> <a id="1916" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1921" class="Symbol">}</a> <a id="1923" class="Symbol">→</a> <a id="1925" href="univalent-foundations.truncations.html#903" class="Function">universal-property-truncation</a> <a id="1955" href="univalent-foundations.truncations.html#1912" class="Bound">l</a> <a id="1957" href="univalent-foundations.truncations.html#1304" class="Bound">B</a> <a id="1959" href="univalent-foundations.truncations.html#1335" class="Bound">f</a><a id="1960" class="Symbol">)</a>
    <a id="1966" href="univalent-foundations.truncations.html#1814" class="Function">universal-property-truncation-is-truncation</a> <a id="2010" href="univalent-foundations.truncations.html#2010" class="Bound">H</a> <a id="2012" href="univalent-foundations.truncations.html#2012" class="Bound">C</a> <a id="2014" href="univalent-foundations.truncations.html#2014" class="Bound">g</a> <a id="2016" class="Symbol">=</a>
      <a id="2024" href="foundation-core.contractible-types.html#3739" class="Function">is-contr-equiv&#39;</a>
        <a id="2048" class="Symbol">(</a> <a id="2050" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="2052" class="Symbol">(</a><a id="2053" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="2077" href="univalent-foundations.truncations.html#1284" class="Bound">k</a> <a id="2079" href="univalent-foundations.truncations.html#1304" class="Bound">B</a> <a id="2081" href="univalent-foundations.truncations.html#2012" class="Bound">C</a><a id="2082" class="Symbol">)</a> <a id="2084" class="Symbol">(λ</a> <a id="2087" href="univalent-foundations.truncations.html#2087" class="Bound">h</a> <a id="2089" class="Symbol">→</a> <a id="2091" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="2094" class="Symbol">(</a><a id="2095" href="univalent-foundations.truncations.html#2087" class="Bound">h</a> <a id="2097" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="2099" href="univalent-foundations.truncations.html#1335" class="Bound">f</a><a id="2100" class="Symbol">)</a> <a id="2102" href="univalent-foundations.truncations.html#2014" class="Bound">g</a><a id="2103" class="Symbol">))</a>
        <a id="2114" class="Symbol">(</a> <a id="2116" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a> <a id="2126" class="Symbol">(λ</a> <a id="2129" href="univalent-foundations.truncations.html#2129" class="Bound">h</a> <a id="2131" class="Symbol">→</a> <a id="2133" href="foundation.function-extensionality.html#1283" class="Function">equiv-funext</a><a id="2145" class="Symbol">))</a>
        <a id="2156" class="Symbol">(</a> <a id="2158" href="foundation-core.contractible-maps.html#3850" class="Function">is-contr-map-is-equiv</a> <a id="2180" class="Symbol">(</a><a id="2181" href="univalent-foundations.truncations.html#2010" class="Bound">H</a> <a id="2183" href="univalent-foundations.truncations.html#2012" class="Bound">C</a><a id="2184" class="Symbol">)</a> <a id="2186" href="univalent-foundations.truncations.html#2014" class="Bound">g</a><a id="2187" class="Symbol">)</a>

  <a id="2192" href="univalent-foundations.truncations.html#2192" class="Function">map-is-truncation</a> <a id="2210" class="Symbol">:</a>
    <a id="2216" class="Symbol">({</a><a id="2218" href="univalent-foundations.truncations.html#2218" class="Bound">l</a> <a id="2220" class="Symbol">:</a> <a id="2222" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2227" class="Symbol">}</a> <a id="2229" class="Symbol">→</a> <a id="2231" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="2245" href="univalent-foundations.truncations.html#2218" class="Bound">l</a> <a id="2247" href="univalent-foundations.truncations.html#1304" class="Bound">B</a> <a id="2249" href="univalent-foundations.truncations.html#1335" class="Bound">f</a><a id="2250" class="Symbol">)</a> <a id="2252" class="Symbol">→</a>
    <a id="2258" class="Symbol">({</a><a id="2260" href="univalent-foundations.truncations.html#2260" class="Bound">l</a> <a id="2262" class="Symbol">:</a> <a id="2264" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2269" class="Symbol">}</a> <a id="2271" class="Symbol">(</a><a id="2272" href="univalent-foundations.truncations.html#2272" class="Bound">C</a> <a id="2274" class="Symbol">:</a> <a id="2276" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="2294" href="univalent-foundations.truncations.html#2260" class="Bound">l</a> <a id="2296" href="univalent-foundations.truncations.html#1284" class="Bound">k</a><a id="2297" class="Symbol">)</a> <a id="2299" class="Symbol">(</a><a id="2300" href="univalent-foundations.truncations.html#2300" class="Bound">g</a> <a id="2302" class="Symbol">:</a> <a id="2304" href="univalent-foundations.truncations.html#1292" class="Bound">A</a> <a id="2306" class="Symbol">→</a> <a id="2308" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="2328" href="univalent-foundations.truncations.html#2272" class="Bound">C</a><a id="2329" class="Symbol">)</a> <a id="2331" class="Symbol">→</a>
    <a id="2337" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="2361" href="univalent-foundations.truncations.html#1284" class="Bound">k</a> <a id="2363" href="univalent-foundations.truncations.html#1304" class="Bound">B</a> <a id="2365" href="univalent-foundations.truncations.html#2272" class="Bound">C</a><a id="2366" class="Symbol">)</a>
  <a id="2370" href="univalent-foundations.truncations.html#2192" class="Function">map-is-truncation</a> <a id="2388" href="univalent-foundations.truncations.html#2388" class="Bound">H</a> <a id="2390" href="univalent-foundations.truncations.html#2390" class="Bound">C</a> <a id="2392" href="univalent-foundations.truncations.html#2392" class="Bound">g</a> <a id="2394" class="Symbol">=</a>
    <a id="2400" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2404" class="Symbol">(</a><a id="2405" href="foundation-core.contractible-types.html#1018" class="Function">center</a> <a id="2412" class="Symbol">(</a><a id="2413" href="univalent-foundations.truncations.html#1814" class="Function">universal-property-truncation-is-truncation</a> <a id="2457" href="univalent-foundations.truncations.html#2388" class="Bound">H</a> <a id="2459" href="univalent-foundations.truncations.html#2390" class="Bound">C</a> <a id="2461" href="univalent-foundations.truncations.html#2392" class="Bound">g</a><a id="2462" class="Symbol">))</a>

  <a id="2468" href="univalent-foundations.truncations.html#2468" class="Function">triangle-is-truncation</a> <a id="2491" class="Symbol">:</a>
    <a id="2497" class="Symbol">(</a><a id="2498" href="univalent-foundations.truncations.html#2498" class="Bound">H</a> <a id="2500" class="Symbol">:</a> <a id="2502" class="Symbol">{</a><a id="2503" href="univalent-foundations.truncations.html#2503" class="Bound">l</a> <a id="2505" class="Symbol">:</a> <a id="2507" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2512" class="Symbol">}</a> <a id="2514" class="Symbol">→</a> <a id="2516" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="2530" href="univalent-foundations.truncations.html#2503" class="Bound">l</a> <a id="2532" href="univalent-foundations.truncations.html#1304" class="Bound">B</a> <a id="2534" href="univalent-foundations.truncations.html#1335" class="Bound">f</a><a id="2535" class="Symbol">)</a> <a id="2537" class="Symbol">→</a>
    <a id="2543" class="Symbol">{</a><a id="2544" href="univalent-foundations.truncations.html#2544" class="Bound">l</a> <a id="2546" class="Symbol">:</a> <a id="2548" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2553" class="Symbol">}</a> <a id="2555" class="Symbol">(</a><a id="2556" href="univalent-foundations.truncations.html#2556" class="Bound">C</a> <a id="2558" class="Symbol">:</a> <a id="2560" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="2578" href="univalent-foundations.truncations.html#2544" class="Bound">l</a> <a id="2580" href="univalent-foundations.truncations.html#1284" class="Bound">k</a><a id="2581" class="Symbol">)</a> <a id="2583" class="Symbol">(</a><a id="2584" href="univalent-foundations.truncations.html#2584" class="Bound">g</a> <a id="2586" class="Symbol">:</a> <a id="2588" href="univalent-foundations.truncations.html#1292" class="Bound">A</a> <a id="2590" class="Symbol">→</a> <a id="2592" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="2612" href="univalent-foundations.truncations.html#2556" class="Bound">C</a><a id="2613" class="Symbol">)</a> <a id="2615" class="Symbol">→</a>
    <a id="2621" class="Symbol">(</a><a id="2622" href="univalent-foundations.truncations.html#2192" class="Function">map-is-truncation</a> <a id="2640" href="univalent-foundations.truncations.html#2498" class="Bound">H</a> <a id="2642" href="univalent-foundations.truncations.html#2556" class="Bound">C</a> <a id="2644" href="univalent-foundations.truncations.html#2584" class="Bound">g</a> <a id="2646" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="2648" href="univalent-foundations.truncations.html#1335" class="Bound">f</a><a id="2649" class="Symbol">)</a> <a id="2651" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="2653" href="univalent-foundations.truncations.html#2584" class="Bound">g</a>
  <a id="2657" href="univalent-foundations.truncations.html#2468" class="Function">triangle-is-truncation</a> <a id="2680" href="univalent-foundations.truncations.html#2680" class="Bound">H</a> <a id="2682" href="univalent-foundations.truncations.html#2682" class="Bound">C</a> <a id="2684" href="univalent-foundations.truncations.html#2684" class="Bound">g</a> <a id="2686" class="Symbol">=</a>
    <a id="2692" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2696" class="Symbol">(</a><a id="2697" href="foundation-core.contractible-types.html#1018" class="Function">center</a> <a id="2704" class="Symbol">(</a><a id="2705" href="univalent-foundations.truncations.html#1814" class="Function">universal-property-truncation-is-truncation</a> <a id="2749" href="univalent-foundations.truncations.html#2680" class="Bound">H</a> <a id="2751" href="univalent-foundations.truncations.html#2682" class="Bound">C</a> <a id="2753" href="univalent-foundations.truncations.html#2684" class="Bound">g</a><a id="2754" class="Symbol">))</a>
</pre>
## Equivalences into k-truncated types are truncations

<pre class="Agda"><a id="2826" class="Keyword">abstract</a>
  <a id="is-truncation-id"></a><a id="2837" href="univalent-foundations.truncations.html#2837" class="Function">is-truncation-id</a> <a id="2854" class="Symbol">:</a>
    <a id="2860" class="Symbol">{</a><a id="2861" href="univalent-foundations.truncations.html#2861" class="Bound">l1</a> <a id="2864" class="Symbol">:</a> <a id="2866" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2871" class="Symbol">}</a> <a id="2873" class="Symbol">{</a><a id="2874" href="univalent-foundations.truncations.html#2874" class="Bound">k</a> <a id="2876" class="Symbol">:</a> <a id="2878" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="2879" class="Symbol">}</a> <a id="2881" class="Symbol">{</a><a id="2882" href="univalent-foundations.truncations.html#2882" class="Bound">A</a> <a id="2884" class="Symbol">:</a> <a id="2886" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="2889" href="univalent-foundations.truncations.html#2861" class="Bound">l1</a><a id="2891" class="Symbol">}</a> <a id="2893" class="Symbol">(</a><a id="2894" href="univalent-foundations.truncations.html#2894" class="Bound">H</a> <a id="2896" class="Symbol">:</a> <a id="2898" href="foundation-core.truncated-types.html#1466" class="Function">is-trunc</a> <a id="2907" href="univalent-foundations.truncations.html#2874" class="Bound">k</a> <a id="2909" href="univalent-foundations.truncations.html#2882" class="Bound">A</a><a id="2910" class="Symbol">)</a> <a id="2912" class="Symbol">→</a>
    <a id="2918" class="Symbol">{</a><a id="2919" href="univalent-foundations.truncations.html#2919" class="Bound">l</a> <a id="2921" class="Symbol">:</a> <a id="2923" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2928" class="Symbol">}</a> <a id="2930" class="Symbol">→</a> <a id="2932" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="2946" href="univalent-foundations.truncations.html#2919" class="Bound">l</a> <a id="2948" class="Symbol">(</a><a id="2949" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="2954" href="univalent-foundations.truncations.html#2882" class="Bound">A</a> <a id="2956" href="univalent-foundations.truncations.html#2894" class="Bound">H</a><a id="2957" class="Symbol">)</a> <a id="2959" href="foundation-core.functions.html#309" class="Function">id</a>
  <a id="2964" href="univalent-foundations.truncations.html#2837" class="Function">is-truncation-id</a> <a id="2981" href="univalent-foundations.truncations.html#2981" class="Bound">H</a> <a id="2983" href="univalent-foundations.truncations.html#2983" class="Bound">B</a> <a id="2985" class="Symbol">=</a>
    <a id="2991" href="foundation.equivalences.html#9064" class="Function">is-equiv-precomp-is-equiv</a> <a id="3017" href="foundation-core.functions.html#309" class="Function">id</a> <a id="3020" href="foundation-core.equivalences.html#2309" class="Function">is-equiv-id</a> <a id="3032" class="Symbol">(</a><a id="3033" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3053" href="univalent-foundations.truncations.html#2983" class="Bound">B</a><a id="3054" class="Symbol">)</a>

<a id="3057" class="Keyword">abstract</a>
  <a id="is-truncation-equiv"></a><a id="3068" href="univalent-foundations.truncations.html#3068" class="Function">is-truncation-equiv</a> <a id="3088" class="Symbol">:</a>
    <a id="3094" class="Symbol">{</a><a id="3095" href="univalent-foundations.truncations.html#3095" class="Bound">l1</a> <a id="3098" href="univalent-foundations.truncations.html#3098" class="Bound">l2</a> <a id="3101" class="Symbol">:</a> <a id="3103" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3108" class="Symbol">}</a> <a id="3110" class="Symbol">{</a><a id="3111" href="univalent-foundations.truncations.html#3111" class="Bound">k</a> <a id="3113" class="Symbol">:</a> <a id="3115" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="3116" class="Symbol">}</a> <a id="3118" class="Symbol">{</a><a id="3119" href="univalent-foundations.truncations.html#3119" class="Bound">A</a> <a id="3121" class="Symbol">:</a> <a id="3123" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="3126" href="univalent-foundations.truncations.html#3095" class="Bound">l1</a><a id="3128" class="Symbol">}</a> <a id="3130" class="Symbol">(</a><a id="3131" href="univalent-foundations.truncations.html#3131" class="Bound">B</a> <a id="3133" class="Symbol">:</a> <a id="3135" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="3153" href="univalent-foundations.truncations.html#3098" class="Bound">l2</a> <a id="3156" href="univalent-foundations.truncations.html#3111" class="Bound">k</a><a id="3157" class="Symbol">)</a>
    <a id="3163" class="Symbol">(</a><a id="3164" href="univalent-foundations.truncations.html#3164" class="Bound">e</a> <a id="3166" class="Symbol">:</a> <a id="3168" href="univalent-foundations.truncations.html#3119" class="Bound">A</a> <a id="3170" href="foundation-core.equivalences.html#1607" class="Function Operator">≃</a> <a id="3172" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3192" href="univalent-foundations.truncations.html#3131" class="Bound">B</a><a id="3193" class="Symbol">)</a> <a id="3195" class="Symbol">→</a>
    <a id="3201" class="Symbol">{</a><a id="3202" href="univalent-foundations.truncations.html#3202" class="Bound">l</a> <a id="3204" class="Symbol">:</a> <a id="3206" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3211" class="Symbol">}</a> <a id="3213" class="Symbol">→</a> <a id="3215" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="3229" href="univalent-foundations.truncations.html#3202" class="Bound">l</a> <a id="3231" href="univalent-foundations.truncations.html#3131" class="Bound">B</a> <a id="3233" class="Symbol">(</a><a id="3234" href="foundation-core.equivalences.html#1807" class="Function">map-equiv</a> <a id="3244" href="univalent-foundations.truncations.html#3164" class="Bound">e</a><a id="3245" class="Symbol">)</a>
  <a id="3249" href="univalent-foundations.truncations.html#3068" class="Function">is-truncation-equiv</a> <a id="3269" href="univalent-foundations.truncations.html#3269" class="Bound">B</a> <a id="3271" href="univalent-foundations.truncations.html#3271" class="Bound">e</a> <a id="3273" href="univalent-foundations.truncations.html#3273" class="Bound">C</a> <a id="3275" class="Symbol">=</a>
    <a id="3281" href="foundation.equivalences.html#9064" class="Function">is-equiv-precomp-is-equiv</a>
      <a id="3313" class="Symbol">(</a> <a id="3315" href="foundation-core.equivalences.html#1807" class="Function">map-equiv</a> <a id="3325" href="univalent-foundations.truncations.html#3271" class="Bound">e</a><a id="3326" class="Symbol">)</a>
      <a id="3334" class="Symbol">(</a> <a id="3336" href="foundation-core.equivalences.html#1862" class="Function">is-equiv-map-equiv</a> <a id="3355" href="univalent-foundations.truncations.html#3271" class="Bound">e</a><a id="3356" class="Symbol">)</a>
      <a id="3364" class="Symbol">(</a> <a id="3366" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3386" href="univalent-foundations.truncations.html#3273" class="Bound">C</a><a id="3387" class="Symbol">)</a>
</pre>
## The dependent universal property of truncations

<pre class="Agda"><a id="precomp-Π-Truncated-Type"></a><a id="3450" href="univalent-foundations.truncations.html#3450" class="Function">precomp-Π-Truncated-Type</a> <a id="3475" class="Symbol">:</a>
  <a id="3479" class="Symbol">{</a><a id="3480" href="univalent-foundations.truncations.html#3480" class="Bound">l1</a> <a id="3483" href="univalent-foundations.truncations.html#3483" class="Bound">l2</a> <a id="3486" href="univalent-foundations.truncations.html#3486" class="Bound">l3</a> <a id="3489" class="Symbol">:</a> <a id="3491" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3496" class="Symbol">}</a> <a id="3498" class="Symbol">{</a><a id="3499" href="univalent-foundations.truncations.html#3499" class="Bound">k</a> <a id="3501" class="Symbol">:</a> <a id="3503" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="3504" class="Symbol">}</a> <a id="3506" class="Symbol">{</a><a id="3507" href="univalent-foundations.truncations.html#3507" class="Bound">A</a> <a id="3509" class="Symbol">:</a> <a id="3511" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="3514" href="univalent-foundations.truncations.html#3480" class="Bound">l1</a><a id="3516" class="Symbol">}</a> <a id="3518" class="Symbol">{</a><a id="3519" href="univalent-foundations.truncations.html#3519" class="Bound">B</a> <a id="3521" class="Symbol">:</a> <a id="3523" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="3526" href="univalent-foundations.truncations.html#3483" class="Bound">l2</a><a id="3528" class="Symbol">}</a> <a id="3530" class="Symbol">(</a><a id="3531" href="univalent-foundations.truncations.html#3531" class="Bound">f</a> <a id="3533" class="Symbol">:</a> <a id="3535" href="univalent-foundations.truncations.html#3507" class="Bound">A</a> <a id="3537" class="Symbol">→</a> <a id="3539" href="univalent-foundations.truncations.html#3519" class="Bound">B</a><a id="3540" class="Symbol">)</a>
  <a id="3544" class="Symbol">(</a><a id="3545" href="univalent-foundations.truncations.html#3545" class="Bound">C</a> <a id="3547" class="Symbol">:</a> <a id="3549" href="univalent-foundations.truncations.html#3519" class="Bound">B</a> <a id="3551" class="Symbol">→</a> <a id="3553" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="3571" href="univalent-foundations.truncations.html#3486" class="Bound">l3</a> <a id="3574" href="univalent-foundations.truncations.html#3499" class="Bound">k</a><a id="3575" class="Symbol">)</a> <a id="3577" class="Symbol">→</a>
  <a id="3581" class="Symbol">((</a><a id="3583" href="univalent-foundations.truncations.html#3583" class="Bound">b</a> <a id="3585" class="Symbol">:</a> <a id="3587" href="univalent-foundations.truncations.html#3519" class="Bound">B</a><a id="3588" class="Symbol">)</a> <a id="3590" class="Symbol">→</a> <a id="3592" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3612" class="Symbol">(</a><a id="3613" href="univalent-foundations.truncations.html#3545" class="Bound">C</a> <a id="3615" href="univalent-foundations.truncations.html#3583" class="Bound">b</a><a id="3616" class="Symbol">))</a> <a id="3619" class="Symbol">→</a>
  <a id="3623" class="Symbol">((</a><a id="3625" href="univalent-foundations.truncations.html#3625" class="Bound">a</a> <a id="3627" class="Symbol">:</a> <a id="3629" href="univalent-foundations.truncations.html#3507" class="Bound">A</a><a id="3630" class="Symbol">)</a> <a id="3632" class="Symbol">→</a> <a id="3634" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3654" class="Symbol">(</a><a id="3655" href="univalent-foundations.truncations.html#3545" class="Bound">C</a> <a id="3657" class="Symbol">(</a><a id="3658" href="univalent-foundations.truncations.html#3531" class="Bound">f</a> <a id="3660" href="univalent-foundations.truncations.html#3625" class="Bound">a</a><a id="3661" class="Symbol">)))</a>
<a id="3665" href="univalent-foundations.truncations.html#3450" class="Function">precomp-Π-Truncated-Type</a> <a id="3690" href="univalent-foundations.truncations.html#3690" class="Bound">f</a> <a id="3692" href="univalent-foundations.truncations.html#3692" class="Bound">C</a> <a id="3694" href="univalent-foundations.truncations.html#3694" class="Bound">h</a> <a id="3696" href="univalent-foundations.truncations.html#3696" class="Bound">a</a> <a id="3698" class="Symbol">=</a> <a id="3700" href="univalent-foundations.truncations.html#3694" class="Bound">h</a> <a id="3702" class="Symbol">(</a><a id="3703" href="univalent-foundations.truncations.html#3690" class="Bound">f</a> <a id="3705" href="univalent-foundations.truncations.html#3696" class="Bound">a</a><a id="3706" class="Symbol">)</a>

<a id="dependent-universal-property-truncation"></a><a id="3709" href="univalent-foundations.truncations.html#3709" class="Function">dependent-universal-property-truncation</a> <a id="3749" class="Symbol">:</a>
  <a id="3753" class="Symbol">{</a><a id="3754" href="univalent-foundations.truncations.html#3754" class="Bound">l1</a> <a id="3757" href="univalent-foundations.truncations.html#3757" class="Bound">l2</a> <a id="3760" class="Symbol">:</a> <a id="3762" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3767" class="Symbol">}</a> <a id="3769" class="Symbol">(</a><a id="3770" href="univalent-foundations.truncations.html#3770" class="Bound">l</a> <a id="3772" class="Symbol">:</a> <a id="3774" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="3779" class="Symbol">)</a> <a id="3781" class="Symbol">{</a><a id="3782" href="univalent-foundations.truncations.html#3782" class="Bound">k</a> <a id="3784" class="Symbol">:</a> <a id="3786" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="3787" class="Symbol">}</a> <a id="3789" class="Symbol">{</a><a id="3790" href="univalent-foundations.truncations.html#3790" class="Bound">A</a> <a id="3792" class="Symbol">:</a> <a id="3794" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="3797" href="univalent-foundations.truncations.html#3754" class="Bound">l1</a><a id="3799" class="Symbol">}</a> <a id="3801" class="Symbol">(</a><a id="3802" href="univalent-foundations.truncations.html#3802" class="Bound">B</a> <a id="3804" class="Symbol">:</a> <a id="3806" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="3824" href="univalent-foundations.truncations.html#3757" class="Bound">l2</a> <a id="3827" href="univalent-foundations.truncations.html#3782" class="Bound">k</a><a id="3828" class="Symbol">)</a>
  <a id="3832" class="Symbol">(</a><a id="3833" href="univalent-foundations.truncations.html#3833" class="Bound">f</a> <a id="3835" class="Symbol">:</a> <a id="3837" href="univalent-foundations.truncations.html#3790" class="Bound">A</a> <a id="3839" class="Symbol">→</a> <a id="3841" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3861" href="univalent-foundations.truncations.html#3802" class="Bound">B</a><a id="3862" class="Symbol">)</a> <a id="3864" class="Symbol">→</a> <a id="3866" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="3869" class="Symbol">(</a><a id="3870" href="univalent-foundations.truncations.html#3754" class="Bound">l1</a> <a id="3873" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="3875" href="univalent-foundations.truncations.html#3757" class="Bound">l2</a> <a id="3878" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="3880" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="3885" href="univalent-foundations.truncations.html#3770" class="Bound">l</a><a id="3886" class="Symbol">)</a>
<a id="3888" href="univalent-foundations.truncations.html#3709" class="Function">dependent-universal-property-truncation</a> <a id="3928" href="univalent-foundations.truncations.html#3928" class="Bound">l</a> <a id="3930" class="Symbol">{</a><a id="3931" href="univalent-foundations.truncations.html#3931" class="Bound">k</a><a id="3932" class="Symbol">}</a> <a id="3934" href="univalent-foundations.truncations.html#3934" class="Bound">B</a> <a id="3936" href="univalent-foundations.truncations.html#3936" class="Bound">f</a> <a id="3938" class="Symbol">=</a>
  <a id="3942" class="Symbol">(</a><a id="3943" href="univalent-foundations.truncations.html#3943" class="Bound">X</a> <a id="3945" class="Symbol">:</a> <a id="3947" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="3967" href="univalent-foundations.truncations.html#3934" class="Bound">B</a> <a id="3969" class="Symbol">→</a> <a id="3971" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="3989" href="univalent-foundations.truncations.html#3928" class="Bound">l</a> <a id="3991" href="univalent-foundations.truncations.html#3931" class="Bound">k</a><a id="3992" class="Symbol">)</a> <a id="3994" class="Symbol">→</a>
  <a id="3998" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a> <a id="4007" class="Symbol">(</a><a id="4008" href="univalent-foundations.truncations.html#3450" class="Function">precomp-Π-Truncated-Type</a> <a id="4033" href="univalent-foundations.truncations.html#3936" class="Bound">f</a> <a id="4035" href="univalent-foundations.truncations.html#3943" class="Bound">X</a><a id="4036" class="Symbol">)</a>

<a id="4039" class="Keyword">module</a> <a id="4046" href="univalent-foundations.truncations.html#4046" class="Module">_</a>
  <a id="4050" class="Symbol">{</a><a id="4051" href="univalent-foundations.truncations.html#4051" class="Bound">l1</a> <a id="4054" href="univalent-foundations.truncations.html#4054" class="Bound">l2</a> <a id="4057" class="Symbol">:</a> <a id="4059" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4064" class="Symbol">}</a> <a id="4066" class="Symbol">{</a><a id="4067" href="univalent-foundations.truncations.html#4067" class="Bound">k</a> <a id="4069" class="Symbol">:</a> <a id="4071" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="4072" class="Symbol">}</a> <a id="4074" class="Symbol">{</a><a id="4075" href="univalent-foundations.truncations.html#4075" class="Bound">A</a> <a id="4077" class="Symbol">:</a> <a id="4079" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="4082" href="univalent-foundations.truncations.html#4051" class="Bound">l1</a><a id="4084" class="Symbol">}</a> <a id="4086" class="Symbol">(</a><a id="4087" href="univalent-foundations.truncations.html#4087" class="Bound">B</a> <a id="4089" class="Symbol">:</a> <a id="4091" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="4109" href="univalent-foundations.truncations.html#4054" class="Bound">l2</a> <a id="4112" href="univalent-foundations.truncations.html#4067" class="Bound">k</a><a id="4113" class="Symbol">)</a>
  <a id="4117" class="Symbol">(</a><a id="4118" href="univalent-foundations.truncations.html#4118" class="Bound">f</a> <a id="4120" class="Symbol">:</a> <a id="4122" href="univalent-foundations.truncations.html#4075" class="Bound">A</a> <a id="4124" class="Symbol">→</a> <a id="4126" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="4146" href="univalent-foundations.truncations.html#4087" class="Bound">B</a><a id="4147" class="Symbol">)</a>
  <a id="4151" class="Keyword">where</a>

  <a id="4160" class="Keyword">abstract</a>
    <a id="4173" href="univalent-foundations.truncations.html#4173" class="Function">dependent-universal-property-truncation-is-truncation</a> <a id="4227" class="Symbol">:</a>
      <a id="4235" class="Symbol">({</a><a id="4237" href="univalent-foundations.truncations.html#4237" class="Bound">l</a> <a id="4239" class="Symbol">:</a> <a id="4241" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4246" class="Symbol">}</a> <a id="4248" class="Symbol">→</a> <a id="4250" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="4264" href="univalent-foundations.truncations.html#4237" class="Bound">l</a> <a id="4266" href="univalent-foundations.truncations.html#4087" class="Bound">B</a> <a id="4268" href="univalent-foundations.truncations.html#4118" class="Bound">f</a><a id="4269" class="Symbol">)</a> <a id="4271" class="Symbol">→</a>
      <a id="4279" class="Symbol">{</a><a id="4280" href="univalent-foundations.truncations.html#4280" class="Bound">l</a> <a id="4282" class="Symbol">:</a> <a id="4284" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="4289" class="Symbol">}</a> <a id="4291" class="Symbol">→</a> <a id="4293" href="univalent-foundations.truncations.html#3709" class="Function">dependent-universal-property-truncation</a> <a id="4333" href="univalent-foundations.truncations.html#4280" class="Bound">l</a> <a id="4335" href="univalent-foundations.truncations.html#4087" class="Bound">B</a> <a id="4337" href="univalent-foundations.truncations.html#4118" class="Bound">f</a>
    <a id="4343" href="univalent-foundations.truncations.html#4173" class="Function">dependent-universal-property-truncation-is-truncation</a> <a id="4397" href="univalent-foundations.truncations.html#4397" class="Bound">H</a> <a id="4399" href="univalent-foundations.truncations.html#4399" class="Bound">X</a> <a id="4401" class="Symbol">=</a>
      <a id="4409" href="foundation-core.functoriality-dependent-pair-types.html#10750" class="Function">is-fiberwise-equiv-is-equiv-map-Σ</a>
        <a id="4451" class="Symbol">(</a> <a id="4453" class="Symbol">λ</a> <a id="4455" class="Symbol">(</a><a id="4456" href="univalent-foundations.truncations.html#4456" class="Bound">h</a> <a id="4458" class="Symbol">:</a> <a id="4460" href="univalent-foundations.truncations.html#4075" class="Bound">A</a> <a id="4462" class="Symbol">→</a> <a id="4464" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="4484" href="univalent-foundations.truncations.html#4087" class="Bound">B</a><a id="4485" class="Symbol">)</a> <a id="4487" class="Symbol">→</a>
          <a id="4499" class="Symbol">(</a><a id="4500" href="univalent-foundations.truncations.html#4500" class="Bound">a</a> <a id="4502" class="Symbol">:</a> <a id="4504" href="univalent-foundations.truncations.html#4075" class="Bound">A</a><a id="4505" class="Symbol">)</a> <a id="4507" class="Symbol">→</a> <a id="4509" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="4529" class="Symbol">(</a><a id="4530" href="univalent-foundations.truncations.html#4399" class="Bound">X</a> <a id="4532" class="Symbol">(</a><a id="4533" href="univalent-foundations.truncations.html#4456" class="Bound">h</a> <a id="4535" href="univalent-foundations.truncations.html#4500" class="Bound">a</a><a id="4536" class="Symbol">)))</a>
        <a id="4548" class="Symbol">(</a> <a id="4550" class="Symbol">λ</a> <a id="4552" class="Symbol">(</a><a id="4553" href="univalent-foundations.truncations.html#4553" class="Bound">g</a> <a id="4555" class="Symbol">:</a> <a id="4557" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="4577" href="univalent-foundations.truncations.html#4087" class="Bound">B</a> <a id="4579" class="Symbol">→</a> <a id="4581" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="4601" href="univalent-foundations.truncations.html#4087" class="Bound">B</a><a id="4602" class="Symbol">)</a> <a id="4604" class="Symbol">→</a> <a id="4606" href="univalent-foundations.truncations.html#4553" class="Bound">g</a> <a id="4608" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="4610" href="univalent-foundations.truncations.html#4118" class="Bound">f</a><a id="4611" class="Symbol">)</a>
        <a id="4621" class="Symbol">(</a> <a id="4623" class="Symbol">λ</a> <a id="4625" href="univalent-foundations.truncations.html#4625" class="Bound">g</a> <a id="4627" class="Symbol">(</a><a id="4628" href="univalent-foundations.truncations.html#4628" class="Bound">s</a> <a id="4630" class="Symbol">:</a> <a id="4632" class="Symbol">(</a><a id="4633" href="univalent-foundations.truncations.html#4633" class="Bound">b</a> <a id="4635" class="Symbol">:</a> <a id="4637" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="4657" href="univalent-foundations.truncations.html#4087" class="Bound">B</a><a id="4658" class="Symbol">)</a> <a id="4660" class="Symbol">→</a>
          <a id="4672" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="4692" class="Symbol">(</a><a id="4693" href="univalent-foundations.truncations.html#4399" class="Bound">X</a> <a id="4695" class="Symbol">(</a><a id="4696" href="univalent-foundations.truncations.html#4625" class="Bound">g</a> <a id="4698" href="univalent-foundations.truncations.html#4633" class="Bound">b</a><a id="4699" class="Symbol">)))</a> <a id="4703" class="Symbol">(</a><a id="4704" href="univalent-foundations.truncations.html#4704" class="Bound">a</a> <a id="4706" class="Symbol">:</a> <a id="4708" href="univalent-foundations.truncations.html#4075" class="Bound">A</a><a id="4709" class="Symbol">)</a> <a id="4711" class="Symbol">→</a> <a id="4713" href="univalent-foundations.truncations.html#4628" class="Bound">s</a> <a id="4715" class="Symbol">(</a><a id="4716" href="univalent-foundations.truncations.html#4118" class="Bound">f</a> <a id="4718" href="univalent-foundations.truncations.html#4704" class="Bound">a</a><a id="4719" class="Symbol">))</a>
        <a id="4730" class="Symbol">(</a> <a id="4732" href="univalent-foundations.truncations.html#4397" class="Bound">H</a> <a id="4734" href="univalent-foundations.truncations.html#4087" class="Bound">B</a><a id="4735" class="Symbol">)</a>
        <a id="4745" class="Symbol">(</a> <a id="4747" href="foundation-core.equivalences.html#12773" class="Function">is-equiv-equiv</a>
          <a id="4772" class="Symbol">(</a> <a id="4774" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#5106" class="Function">inv-distributive-Π-Σ</a><a id="4794" class="Symbol">)</a>
          <a id="4806" class="Symbol">(</a> <a id="4808" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#5106" class="Function">inv-distributive-Π-Σ</a><a id="4828" class="Symbol">)</a>
          <a id="4840" class="Symbol">(</a> <a id="4842" href="foundation-core.dependent-pair-types.html#687" class="Function">ind-Σ</a> <a id="4848" class="Symbol">(λ</a> <a id="4851" href="univalent-foundations.truncations.html#4851" class="Bound">g</a> <a id="4853" href="univalent-foundations.truncations.html#4853" class="Bound">s</a> <a id="4855" class="Symbol">→</a> <a id="4857" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="4861" class="Symbol">))</a>
          <a id="4874" class="Symbol">(</a> <a id="4876" href="univalent-foundations.truncations.html#4397" class="Bound">H</a> <a id="4878" class="Symbol">(</a><a id="4879" href="foundation-core.truncated-types.html#6052" class="Function">Σ-Truncated-Type</a> <a id="4896" href="univalent-foundations.truncations.html#4087" class="Bound">B</a> <a id="4898" href="univalent-foundations.truncations.html#4399" class="Bound">X</a><a id="4899" class="Symbol">)))</a>
        <a id="4911" class="Symbol">(</a> <a id="4913" href="foundation-core.functions.html#309" class="Function">id</a><a id="4915" class="Symbol">)</a>

  <a id="4920" class="Keyword">abstract</a>
    <a id="4933" href="univalent-foundations.truncations.html#4933" class="Function">is-truncation-dependent-universal-property-truncation</a> <a id="4987" class="Symbol">:</a>
      <a id="4995" class="Symbol">({</a><a id="4997" href="univalent-foundations.truncations.html#4997" class="Bound">l</a> <a id="4999" class="Symbol">:</a> <a id="5001" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5006" class="Symbol">}</a> <a id="5008" class="Symbol">→</a> <a id="5010" href="univalent-foundations.truncations.html#3709" class="Function">dependent-universal-property-truncation</a> <a id="5050" href="univalent-foundations.truncations.html#4997" class="Bound">l</a> <a id="5052" href="univalent-foundations.truncations.html#4087" class="Bound">B</a> <a id="5054" href="univalent-foundations.truncations.html#4118" class="Bound">f</a><a id="5055" class="Symbol">)</a> <a id="5057" class="Symbol">→</a>
      <a id="5065" class="Symbol">{</a><a id="5066" href="univalent-foundations.truncations.html#5066" class="Bound">l</a> <a id="5068" class="Symbol">:</a> <a id="5070" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5075" class="Symbol">}</a> <a id="5077" class="Symbol">→</a> <a id="5079" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="5093" href="univalent-foundations.truncations.html#5066" class="Bound">l</a> <a id="5095" href="univalent-foundations.truncations.html#4087" class="Bound">B</a> <a id="5097" href="univalent-foundations.truncations.html#4118" class="Bound">f</a>
    <a id="5103" href="univalent-foundations.truncations.html#4933" class="Function">is-truncation-dependent-universal-property-truncation</a> <a id="5157" href="univalent-foundations.truncations.html#5157" class="Bound">H</a> <a id="5159" href="univalent-foundations.truncations.html#5159" class="Bound">X</a> <a id="5161" class="Symbol">=</a>
      <a id="5169" href="univalent-foundations.truncations.html#5157" class="Bound">H</a> <a id="5171" class="Symbol">(λ</a> <a id="5174" href="univalent-foundations.truncations.html#5174" class="Bound">b</a> <a id="5176" class="Symbol">→</a> <a id="5178" href="univalent-foundations.truncations.html#5159" class="Bound">X</a><a id="5179" class="Symbol">)</a>

  <a id="5184" href="univalent-foundations.truncations.html#5184" class="Function">sec-is-truncation</a> <a id="5202" class="Symbol">:</a>
    <a id="5208" class="Symbol">({</a><a id="5210" href="univalent-foundations.truncations.html#5210" class="Bound">l</a> <a id="5212" class="Symbol">:</a> <a id="5214" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5219" class="Symbol">}</a> <a id="5221" class="Symbol">→</a> <a id="5223" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="5237" href="univalent-foundations.truncations.html#5210" class="Bound">l</a> <a id="5239" href="univalent-foundations.truncations.html#4087" class="Bound">B</a> <a id="5241" href="univalent-foundations.truncations.html#4118" class="Bound">f</a><a id="5242" class="Symbol">)</a> <a id="5244" class="Symbol">→</a>
    <a id="5250" class="Symbol">{</a><a id="5251" href="univalent-foundations.truncations.html#5251" class="Bound">l3</a> <a id="5254" class="Symbol">:</a> <a id="5256" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5261" class="Symbol">}</a> <a id="5263" class="Symbol">(</a><a id="5264" href="univalent-foundations.truncations.html#5264" class="Bound">C</a> <a id="5266" class="Symbol">:</a> <a id="5268" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="5286" href="univalent-foundations.truncations.html#5251" class="Bound">l3</a> <a id="5289" href="univalent-foundations.truncations.html#4067" class="Bound">k</a><a id="5290" class="Symbol">)</a>
    <a id="5296" class="Symbol">(</a><a id="5297" href="univalent-foundations.truncations.html#5297" class="Bound">h</a> <a id="5299" class="Symbol">:</a> <a id="5301" href="univalent-foundations.truncations.html#4075" class="Bound">A</a> <a id="5303" class="Symbol">→</a> <a id="5305" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="5325" href="univalent-foundations.truncations.html#5264" class="Bound">C</a><a id="5326" class="Symbol">)</a> <a id="5328" class="Symbol">(</a><a id="5329" href="univalent-foundations.truncations.html#5329" class="Bound">g</a> <a id="5331" class="Symbol">:</a> <a id="5333" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="5357" href="univalent-foundations.truncations.html#4067" class="Bound">k</a> <a id="5359" href="univalent-foundations.truncations.html#5264" class="Bound">C</a> <a id="5361" href="univalent-foundations.truncations.html#4087" class="Bound">B</a><a id="5362" class="Symbol">)</a> <a id="5364" class="Symbol">→</a>
    <a id="5370" href="univalent-foundations.truncations.html#4118" class="Bound">f</a> <a id="5372" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="5374" class="Symbol">(</a><a id="5375" href="univalent-foundations.truncations.html#5329" class="Bound">g</a> <a id="5377" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="5379" href="univalent-foundations.truncations.html#5297" class="Bound">h</a><a id="5380" class="Symbol">)</a> <a id="5382" class="Symbol">→</a> <a id="5384" href="foundation-core.sections.html#521" class="Function">sec</a> <a id="5388" href="univalent-foundations.truncations.html#5329" class="Bound">g</a>
  <a id="5392" href="univalent-foundations.truncations.html#5184" class="Function">sec-is-truncation</a> <a id="5410" href="univalent-foundations.truncations.html#5410" class="Bound">H</a> <a id="5412" href="univalent-foundations.truncations.html#5412" class="Bound">C</a> <a id="5414" href="univalent-foundations.truncations.html#5414" class="Bound">h</a> <a id="5416" href="univalent-foundations.truncations.html#5416" class="Bound">g</a> <a id="5418" href="univalent-foundations.truncations.html#5418" class="Bound">K</a> <a id="5420" class="Symbol">=</a>
    <a id="5426" href="foundation.distributivity-of-dependent-functions-over-dependent-pairs.html#2808" class="Function">map-distributive-Π-Σ</a>
      <a id="5453" class="Symbol">(</a> <a id="5455" href="foundation-core.equivalences.html#4173" class="Function">map-inv-is-equiv</a>
        <a id="5480" class="Symbol">(</a> <a id="5482" href="univalent-foundations.truncations.html#4173" class="Function">dependent-universal-property-truncation-is-truncation</a> <a id="5536" href="univalent-foundations.truncations.html#5410" class="Bound">H</a>
          <a id="5548" class="Symbol">(</a> <a id="5550" href="foundation-core.truncated-types.html#6435" class="Function">fib-Truncated-Type</a> <a id="5569" href="univalent-foundations.truncations.html#5412" class="Bound">C</a> <a id="5571" href="univalent-foundations.truncations.html#4087" class="Bound">B</a> <a id="5573" href="univalent-foundations.truncations.html#5416" class="Bound">g</a><a id="5574" class="Symbol">))</a>
        <a id="5585" class="Symbol">(</a> <a id="5587" class="Symbol">λ</a> <a id="5589" href="univalent-foundations.truncations.html#5589" class="Bound">a</a> <a id="5591" class="Symbol">→</a> <a id="5593" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="5598" class="Symbol">(</a><a id="5599" href="univalent-foundations.truncations.html#5414" class="Bound">h</a> <a id="5601" href="univalent-foundations.truncations.html#5589" class="Bound">a</a><a id="5602" class="Symbol">)</a> <a id="5604" class="Symbol">(</a><a id="5605" href="foundation-core.identity-types.html#1552" class="Function">inv</a> <a id="5609" class="Symbol">(</a><a id="5610" href="univalent-foundations.truncations.html#5418" class="Bound">K</a> <a id="5612" href="univalent-foundations.truncations.html#5589" class="Bound">a</a><a id="5613" class="Symbol">))))</a>
</pre>
## Uniqueness of truncations

<pre class="Agda"><a id="5661" class="Keyword">module</a> <a id="5668" href="univalent-foundations.truncations.html#5668" class="Module">_</a>
  <a id="5672" class="Symbol">{</a><a id="5673" href="univalent-foundations.truncations.html#5673" class="Bound">l1</a> <a id="5676" href="univalent-foundations.truncations.html#5676" class="Bound">l2</a> <a id="5679" href="univalent-foundations.truncations.html#5679" class="Bound">l3</a> <a id="5682" class="Symbol">:</a> <a id="5684" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5689" class="Symbol">}</a> <a id="5691" class="Symbol">(</a><a id="5692" href="univalent-foundations.truncations.html#5692" class="Bound">k</a> <a id="5694" class="Symbol">:</a> <a id="5696" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a><a id="5697" class="Symbol">)</a> <a id="5699" class="Symbol">{</a><a id="5700" href="univalent-foundations.truncations.html#5700" class="Bound">A</a> <a id="5702" class="Symbol">:</a> <a id="5704" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="5707" href="univalent-foundations.truncations.html#5673" class="Bound">l1</a><a id="5709" class="Symbol">}</a>
  <a id="5713" class="Symbol">(</a><a id="5714" href="univalent-foundations.truncations.html#5714" class="Bound">B</a> <a id="5716" class="Symbol">:</a> <a id="5718" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="5736" href="univalent-foundations.truncations.html#5676" class="Bound">l2</a> <a id="5739" href="univalent-foundations.truncations.html#5692" class="Bound">k</a><a id="5740" class="Symbol">)</a> <a id="5742" class="Symbol">(</a><a id="5743" href="univalent-foundations.truncations.html#5743" class="Bound">f</a> <a id="5745" class="Symbol">:</a> <a id="5747" href="univalent-foundations.truncations.html#5700" class="Bound">A</a> <a id="5749" class="Symbol">→</a> <a id="5751" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="5771" href="univalent-foundations.truncations.html#5714" class="Bound">B</a><a id="5772" class="Symbol">)</a>
  <a id="5776" class="Symbol">(</a><a id="5777" href="univalent-foundations.truncations.html#5777" class="Bound">C</a> <a id="5779" class="Symbol">:</a> <a id="5781" href="foundation-core.truncated-types.html#1651" class="Function">UU-Truncated-Type</a> <a id="5799" href="univalent-foundations.truncations.html#5679" class="Bound">l3</a> <a id="5802" href="univalent-foundations.truncations.html#5692" class="Bound">k</a><a id="5803" class="Symbol">)</a> <a id="5805" class="Symbol">(</a><a id="5806" href="univalent-foundations.truncations.html#5806" class="Bound">g</a> <a id="5808" class="Symbol">:</a> <a id="5810" href="univalent-foundations.truncations.html#5700" class="Bound">A</a> <a id="5812" class="Symbol">→</a> <a id="5814" href="foundation-core.truncated-types.html#1792" class="Function">type-Truncated-Type</a> <a id="5834" href="univalent-foundations.truncations.html#5777" class="Bound">C</a><a id="5835" class="Symbol">)</a>
  <a id="5839" class="Symbol">{</a><a id="5840" href="univalent-foundations.truncations.html#5840" class="Bound">h</a> <a id="5842" class="Symbol">:</a> <a id="5844" href="foundation.truncated-types.html#3516" class="Function">type-hom-Truncated-Type</a> <a id="5868" href="univalent-foundations.truncations.html#5692" class="Bound">k</a> <a id="5870" href="univalent-foundations.truncations.html#5714" class="Bound">B</a> <a id="5872" href="univalent-foundations.truncations.html#5777" class="Bound">C</a><a id="5873" class="Symbol">}</a> <a id="5875" class="Symbol">(</a><a id="5876" href="univalent-foundations.truncations.html#5876" class="Bound">H</a> <a id="5878" class="Symbol">:</a> <a id="5880" class="Symbol">(</a><a id="5881" href="univalent-foundations.truncations.html#5840" class="Bound">h</a> <a id="5883" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="5885" href="univalent-foundations.truncations.html#5743" class="Bound">f</a><a id="5886" class="Symbol">)</a> <a id="5888" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="5890" href="univalent-foundations.truncations.html#5806" class="Bound">g</a><a id="5891" class="Symbol">)</a>
  <a id="5895" class="Keyword">where</a>

  <a id="5904" class="Keyword">abstract</a>
    <a id="5917" href="univalent-foundations.truncations.html#5917" class="Function">is-equiv-is-truncation-is-truncation</a> <a id="5954" class="Symbol">:</a>
      <a id="5962" class="Symbol">({</a><a id="5964" href="univalent-foundations.truncations.html#5964" class="Bound">l</a> <a id="5966" class="Symbol">:</a> <a id="5968" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="5973" class="Symbol">}</a> <a id="5975" class="Symbol">→</a> <a id="5977" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="5991" href="univalent-foundations.truncations.html#5964" class="Bound">l</a> <a id="5993" href="univalent-foundations.truncations.html#5714" class="Bound">B</a> <a id="5995" href="univalent-foundations.truncations.html#5743" class="Bound">f</a><a id="5996" class="Symbol">)</a> <a id="5998" class="Symbol">→</a>
      <a id="6006" class="Symbol">({</a><a id="6008" href="univalent-foundations.truncations.html#6008" class="Bound">l</a> <a id="6010" class="Symbol">:</a> <a id="6012" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="6017" class="Symbol">}</a> <a id="6019" class="Symbol">→</a> <a id="6021" href="univalent-foundations.truncations.html#608" class="Function">is-truncation</a> <a id="6035" href="univalent-foundations.truncations.html#6008" class="Bound">l</a> <a id="6037" href="univalent-foundations.truncations.html#5777" class="Bound">C</a> <a id="6039" href="univalent-foundations.truncations.html#5806" class="Bound">g</a><a id="6040" class="Symbol">)</a> <a id="6042" class="Symbol">→</a>
      <a id="6050" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a> <a id="6059" href="univalent-foundations.truncations.html#5840" class="Bound">h</a>
    <a id="6065" href="univalent-foundations.truncations.html#5917" class="Function">is-equiv-is-truncation-is-truncation</a> <a id="6102" href="univalent-foundations.truncations.html#6102" class="Bound">H</a> <a id="6104" href="univalent-foundations.truncations.html#6104" class="Bound">K</a> <a id="6106" class="Symbol">=</a>
      <a id="6114" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
        <a id="6127" class="Hole">{! sec-is-truncation!}</a>
        <a id="6158" class="Hole">{!!}</a>

<a id="6164" class="Comment">{-
      is-equiv-has-inverse 
        ( pr1 (center K))
        ( htpy-eq
          ( is-injective-is-equiv
            ( Ug C)
            { h ∘ k}
            { id}
            ( ( precomp-comp-Set-Quotient R C g B k C h) ∙
              ( ( ap (λ t → precomp-Set-Quotient R B t C h) α) ∙
                ( ( eq-htpy-reflecting-map-Eq-Rel R C
                    ( precomp-Set-Quotient R B f C h) g H) ∙
                  ( inv (precomp-id-Set-Quotient R C g)))))))
        ( htpy-eq
          ( is-injective-is-equiv
            ( Uf B)
            { k ∘ h}
            { id}
            ( ( precomp-comp-Set-Quotient R B f C h B k) ∙
              ( ( ap
                  ( λ t → precomp-Set-Quotient R C t B k)
                  ( eq-htpy-reflecting-map-Eq-Rel R C
                    ( precomp-Set-Quotient R B f C h) g H)) ∙
                ( ( α) ∙
                  ( inv (precomp-id-Set-Quotient R B f)))))))
      where
      K : is-contr
            ( Σ ( type-hom-Set C B)
                ( λ h →
                  ( h ∘ map-reflecting-map-Eq-Rel R g) ~
                  ( map-reflecting-map-Eq-Rel R f)))
      K = universal-property-set-quotient-is-set-quotient R C g Ug B f
      k : type-Set C → type-Set B
      k = pr1 (center K)
      α : Id (precomp-Set-Quotient R C g B k) f
      α = eq-htpy-reflecting-map-Eq-Rel R B
            ( precomp-Set-Quotient R C g B k)
            ( f)
            ( pr2 (center K))
            -}</a>

  
<a id="7620" class="Comment">{-
-- Uniqueness of set truncations

module _
  {l1 l2 l3 : Level} {A : UU l1} (B : UU-Set l2) (f : A → type-Set B)
  (C : UU-Set l3) (g : A → type-Set C) {h : type-hom-Set B C}
  (H : (h ∘ f) ~ g)
  where

  abstract
    is-equiv-is-set-truncation-is-set-truncation :
      ({l : Level} → is-set-truncation l B f) →
      ({l : Level} → is-set-truncation l C g) →
      is-equiv h
    is-equiv-is-set-truncation-is-set-truncation Sf Sg =
      is-equiv-is-set-quotient-is-set-quotient
        ( mere-eq-Eq-Rel A)
        ( B)
        ( reflecting-map-mere-eq B f)
        ( C)
        ( reflecting-map-mere-eq C g)
        ( H)
        ( λ {l} → is-set-quotient-is-set-truncation B f Sf)
        ( λ {l} → is-set-quotient-is-set-truncation C g Sg)

  abstract
    is-set-truncation-is-equiv-is-set-truncation :
      ({l : Level} → is-set-truncation l C g) → is-equiv h → 
      {l : Level} → is-set-truncation l B f
    is-set-truncation-is-equiv-is-set-truncation Sg Eh =
      is-set-truncation-is-set-quotient B f
        ( is-set-quotient-is-equiv-is-set-quotient
          ( mere-eq-Eq-Rel A)
          ( B)
          ( reflecting-map-mere-eq B f)
          ( C)
          ( reflecting-map-mere-eq C g)
          ( H)
          ( is-set-quotient-is-set-truncation C g Sg)
          ( Eh))

  abstract
    is-set-truncation-is-set-truncation-is-equiv :
      is-equiv h → ({l : Level} → is-set-truncation l B f) →
      {l : Level} → is-set-truncation l C g
    is-set-truncation-is-set-truncation-is-equiv Eh Sf =
      is-set-truncation-is-set-quotient C g
        ( is-set-quotient-is-set-quotient-is-equiv
          ( mere-eq-Eq-Rel A)
          ( B)
          ( reflecting-map-mere-eq B f)
          ( C)
          ( reflecting-map-mere-eq C g)
          ( H)
          ( Eh)
          ( is-set-quotient-is-set-truncation B f Sf))

module _
  {l1 l2 l3 : Level} {A : UU l1} (B : UU-Set l2) (f : A → type-Set B)
  (C : UU-Set l3) (g : A → type-Set C)
  (Sf : {l : Level} → is-set-truncation l B f)
  (Sg : {l : Level} → is-set-truncation l C g)
  where

  abstract
    uniqueness-set-truncation :
      is-contr (Σ (type-Set B ≃ type-Set C) (λ e → (map-equiv e ∘ f) ~ g))
    uniqueness-set-truncation =
      uniqueness-set-quotient
        ( mere-eq-Eq-Rel A)
        ( B)
        ( reflecting-map-mere-eq B f)
        ( is-set-quotient-is-set-truncation B f Sf)
        ( C)
        ( reflecting-map-mere-eq C g)
        ( is-set-quotient-is-set-truncation C g Sg)
  
  equiv-uniqueness-set-truncation : type-Set B ≃ type-Set C
  equiv-uniqueness-set-truncation =
    pr1 (center uniqueness-set-truncation)

  map-equiv-uniqueness-set-truncation : type-Set B → type-Set C
  map-equiv-uniqueness-set-truncation =
    map-equiv equiv-uniqueness-set-truncation

  triangle-uniqueness-set-truncation :
    (map-equiv-uniqueness-set-truncation ∘ f) ~ g
  triangle-uniqueness-set-truncation =
    pr2 (center uniqueness-set-truncation)

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