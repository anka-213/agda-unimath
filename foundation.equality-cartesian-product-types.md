# Equality of cartesian product types

<pre class="Agda"><a id="48" class="Symbol">{-#</a> <a id="52" class="Keyword">OPTIONS</a> <a id="60" class="Pragma">--without-K</a> <a id="72" class="Pragma">--exact-split</a> <a id="86" class="Symbol">#-}</a>

<a id="91" class="Keyword">module</a> <a id="98" href="foundation.equality-cartesian-product-types.html" class="Module">foundation.equality-cartesian-product-types</a> <a id="142" class="Keyword">where</a>

<a id="149" class="Keyword">open</a> <a id="154" class="Keyword">import</a> <a id="161" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a> <a id="196" class="Keyword">using</a> <a id="202" class="Symbol">(</a><a id="203" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">_×_</a><a id="206" class="Symbol">)</a>
<a id="208" class="Keyword">open</a> <a id="213" class="Keyword">import</a> <a id="220" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="252" class="Keyword">using</a> <a id="258" class="Symbol">(</a><a id="259" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="263" class="Symbol">;</a> <a id="265" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="268" class="Symbol">;</a> <a id="270" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="273" class="Symbol">)</a>
<a id="275" class="Keyword">open</a> <a id="280" class="Keyword">import</a> <a id="287" href="foundation.equivalences.html" class="Module">foundation.equivalences</a> <a id="311" class="Keyword">using</a> <a id="317" class="Symbol">(</a><a id="318" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a><a id="326" class="Symbol">;</a> <a id="328" href="foundation-core.equivalences.html#1607" class="Function Operator">_≃_</a><a id="331" class="Symbol">;</a> <a id="333" href="foundation-core.equivalences.html#2999" class="Function">is-equiv-has-inverse</a><a id="353" class="Symbol">)</a>
<a id="355" class="Keyword">open</a> <a id="360" class="Keyword">import</a> <a id="367" href="foundation.functions.html" class="Module">foundation.functions</a> <a id="388" class="Keyword">using</a> <a id="394" class="Symbol">(</a><a id="395" href="foundation-core.functions.html#309" class="Function">id</a><a id="397" class="Symbol">;</a> <a id="399" href="foundation-core.functions.html#407" class="Function Operator">_∘_</a><a id="402" class="Symbol">)</a>
<a id="404" class="Keyword">open</a> <a id="409" class="Keyword">import</a> <a id="416" href="foundation.homotopies.html" class="Module">foundation.homotopies</a> <a id="438" class="Keyword">using</a> <a id="444" class="Symbol">(</a><a id="445" href="foundation-core.homotopies.html#467" class="Function Operator">_~_</a><a id="448" class="Symbol">)</a>
<a id="450" class="Keyword">open</a> <a id="455" class="Keyword">import</a> <a id="462" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="488" class="Keyword">using</a> <a id="494" class="Symbol">(</a><a id="495" href="foundation-core.identity-types.html#641" class="Datatype">Id</a><a id="497" class="Symbol">;</a> <a id="499" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="503" class="Symbol">;</a> <a id="505" href="foundation-core.identity-types.html#2853" class="Function">ap</a><a id="507" class="Symbol">)</a>
<a id="509" class="Keyword">open</a> <a id="514" class="Keyword">import</a> <a id="521" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="548" class="Keyword">using</a> <a id="554" class="Symbol">(</a><a id="555" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="557" class="Symbol">;</a> <a id="559" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="564" class="Symbol">;</a> <a id="566" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="569" class="Symbol">)</a>
</pre>
## Idea

Identifications `Id (pair x y) (pair x' y')` in a cartesian product are equivalently described as pairs of identifications `Id x x'` and `Id y y'`. This provides us with a characterization of the identity type of cartesian product types.

## Definition

<pre class="Agda"><a id="847" class="Keyword">module</a> <a id="854" href="foundation.equality-cartesian-product-types.html#854" class="Module">_</a>
  <a id="858" class="Symbol">{</a><a id="859" href="foundation.equality-cartesian-product-types.html#859" class="Bound">l1</a> <a id="862" href="foundation.equality-cartesian-product-types.html#862" class="Bound">l2</a> <a id="865" class="Symbol">:</a> <a id="867" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="872" class="Symbol">}</a> <a id="874" class="Symbol">{</a><a id="875" href="foundation.equality-cartesian-product-types.html#875" class="Bound">A</a> <a id="877" class="Symbol">:</a> <a id="879" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="882" href="foundation.equality-cartesian-product-types.html#859" class="Bound">l1</a><a id="884" class="Symbol">}</a> <a id="886" class="Symbol">{</a><a id="887" href="foundation.equality-cartesian-product-types.html#887" class="Bound">B</a> <a id="889" class="Symbol">:</a> <a id="891" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="894" href="foundation.equality-cartesian-product-types.html#862" class="Bound">l2</a><a id="896" class="Symbol">}</a>
  <a id="900" class="Keyword">where</a>
  
  <a id="911" href="foundation.equality-cartesian-product-types.html#911" class="Function">Eq-prod</a> <a id="919" class="Symbol">:</a> <a id="921" class="Symbol">(</a><a id="922" href="foundation.equality-cartesian-product-types.html#922" class="Bound">s</a> <a id="924" href="foundation.equality-cartesian-product-types.html#924" class="Bound">t</a> <a id="926" class="Symbol">:</a> <a id="928" href="foundation.equality-cartesian-product-types.html#875" class="Bound">A</a> <a id="930" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="932" href="foundation.equality-cartesian-product-types.html#887" class="Bound">B</a><a id="933" class="Symbol">)</a> <a id="935" class="Symbol">→</a> <a id="937" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="940" class="Symbol">(</a><a id="941" href="foundation.equality-cartesian-product-types.html#859" class="Bound">l1</a> <a id="944" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="946" href="foundation.equality-cartesian-product-types.html#862" class="Bound">l2</a><a id="948" class="Symbol">)</a>
  <a id="952" href="foundation.equality-cartesian-product-types.html#911" class="Function">Eq-prod</a> <a id="960" href="foundation.equality-cartesian-product-types.html#960" class="Bound">s</a> <a id="962" href="foundation.equality-cartesian-product-types.html#962" class="Bound">t</a> <a id="964" class="Symbol">=</a> <a id="966" class="Symbol">(</a><a id="967" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="970" class="Symbol">(</a><a id="971" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="975" href="foundation.equality-cartesian-product-types.html#960" class="Bound">s</a><a id="976" class="Symbol">)</a> <a id="978" class="Symbol">(</a><a id="979" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="983" href="foundation.equality-cartesian-product-types.html#962" class="Bound">t</a><a id="984" class="Symbol">))</a> <a id="987" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="989" class="Symbol">(</a><a id="990" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="993" class="Symbol">(</a><a id="994" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="998" href="foundation.equality-cartesian-product-types.html#960" class="Bound">s</a><a id="999" class="Symbol">)</a> <a id="1001" class="Symbol">(</a><a id="1002" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1006" href="foundation.equality-cartesian-product-types.html#962" class="Bound">t</a><a id="1007" class="Symbol">))</a>
</pre>
## Properties

### The type `Eq-prod s t` is equivalent to `Id s t`.

<pre class="Agda"><a id="1093" class="Keyword">module</a> <a id="1100" href="foundation.equality-cartesian-product-types.html#1100" class="Module">_</a>
  <a id="1104" class="Symbol">{</a><a id="1105" href="foundation.equality-cartesian-product-types.html#1105" class="Bound">l1</a> <a id="1108" href="foundation.equality-cartesian-product-types.html#1108" class="Bound">l2</a> <a id="1111" class="Symbol">:</a> <a id="1113" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1118" class="Symbol">}</a> <a id="1120" class="Symbol">{</a><a id="1121" href="foundation.equality-cartesian-product-types.html#1121" class="Bound">A</a> <a id="1123" class="Symbol">:</a> <a id="1125" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1128" href="foundation.equality-cartesian-product-types.html#1105" class="Bound">l1</a><a id="1130" class="Symbol">}</a> <a id="1132" class="Symbol">{</a><a id="1133" href="foundation.equality-cartesian-product-types.html#1133" class="Bound">B</a> <a id="1135" class="Symbol">:</a> <a id="1137" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="1140" href="foundation.equality-cartesian-product-types.html#1108" class="Bound">l2</a><a id="1142" class="Symbol">}</a>
  <a id="1146" class="Keyword">where</a>
  
  <a id="1157" href="foundation.equality-cartesian-product-types.html#1157" class="Function">eq-pair&#39;</a> <a id="1166" class="Symbol">:</a> <a id="1168" class="Symbol">{</a><a id="1169" href="foundation.equality-cartesian-product-types.html#1169" class="Bound">s</a> <a id="1171" href="foundation.equality-cartesian-product-types.html#1171" class="Bound">t</a> <a id="1173" class="Symbol">:</a> <a id="1175" href="foundation.equality-cartesian-product-types.html#1121" class="Bound">A</a> <a id="1177" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="1179" href="foundation.equality-cartesian-product-types.html#1133" class="Bound">B</a><a id="1180" class="Symbol">}</a> <a id="1182" class="Symbol">→</a> <a id="1184" href="foundation.equality-cartesian-product-types.html#911" class="Function">Eq-prod</a> <a id="1192" href="foundation.equality-cartesian-product-types.html#1169" class="Bound">s</a> <a id="1194" href="foundation.equality-cartesian-product-types.html#1171" class="Bound">t</a> <a id="1196" class="Symbol">→</a> <a id="1198" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="1201" href="foundation.equality-cartesian-product-types.html#1169" class="Bound">s</a> <a id="1203" href="foundation.equality-cartesian-product-types.html#1171" class="Bound">t</a>
  <a id="1207" href="foundation.equality-cartesian-product-types.html#1157" class="Function">eq-pair&#39;</a> <a id="1216" class="Symbol">{</a><a id="1217" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1222" href="foundation.equality-cartesian-product-types.html#1222" class="Bound">x</a> <a id="1224" href="foundation.equality-cartesian-product-types.html#1224" class="Bound">y</a><a id="1225" class="Symbol">}</a> <a id="1227" class="Symbol">{</a><a id="1228" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1233" class="DottedPattern Symbol">.</a><a id="1234" href="foundation.equality-cartesian-product-types.html#1222" class="DottedPattern Bound">x</a> <a id="1236" class="DottedPattern Symbol">.</a><a id="1237" href="foundation.equality-cartesian-product-types.html#1224" class="DottedPattern Bound">y</a><a id="1238" class="Symbol">}</a> <a id="1240" class="Symbol">(</a><a id="1241" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1246" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a> <a id="1251" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="1255" class="Symbol">)</a> <a id="1257" class="Symbol">=</a> <a id="1259" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a>

  <a id="1267" href="foundation.equality-cartesian-product-types.html#1267" class="Function">eq-pair</a> <a id="1275" class="Symbol">:</a>
    <a id="1281" class="Symbol">{</a><a id="1282" href="foundation.equality-cartesian-product-types.html#1282" class="Bound">s</a> <a id="1284" href="foundation.equality-cartesian-product-types.html#1284" class="Bound">t</a> <a id="1286" class="Symbol">:</a> <a id="1288" href="foundation.equality-cartesian-product-types.html#1121" class="Bound">A</a> <a id="1290" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="1292" href="foundation.equality-cartesian-product-types.html#1133" class="Bound">B</a><a id="1293" class="Symbol">}</a> <a id="1295" class="Symbol">→</a> <a id="1297" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="1300" class="Symbol">(</a><a id="1301" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1305" href="foundation.equality-cartesian-product-types.html#1282" class="Bound">s</a><a id="1306" class="Symbol">)</a> <a id="1308" class="Symbol">(</a><a id="1309" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1313" href="foundation.equality-cartesian-product-types.html#1284" class="Bound">t</a><a id="1314" class="Symbol">)</a> <a id="1316" class="Symbol">→</a> <a id="1318" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="1321" class="Symbol">(</a><a id="1322" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1326" href="foundation.equality-cartesian-product-types.html#1282" class="Bound">s</a><a id="1327" class="Symbol">)</a> <a id="1329" class="Symbol">(</a><a id="1330" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1334" href="foundation.equality-cartesian-product-types.html#1284" class="Bound">t</a><a id="1335" class="Symbol">)</a> <a id="1337" class="Symbol">→</a> <a id="1339" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="1342" href="foundation.equality-cartesian-product-types.html#1282" class="Bound">s</a> <a id="1344" href="foundation.equality-cartesian-product-types.html#1284" class="Bound">t</a>
  <a id="1348" href="foundation.equality-cartesian-product-types.html#1267" class="Function">eq-pair</a> <a id="1356" href="foundation.equality-cartesian-product-types.html#1356" class="Bound">p</a> <a id="1358" href="foundation.equality-cartesian-product-types.html#1358" class="Bound">q</a> <a id="1360" class="Symbol">=</a> <a id="1362" href="foundation.equality-cartesian-product-types.html#1157" class="Function">eq-pair&#39;</a> <a id="1371" class="Symbol">(</a><a id="1372" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1377" href="foundation.equality-cartesian-product-types.html#1356" class="Bound">p</a> <a id="1379" href="foundation.equality-cartesian-product-types.html#1358" class="Bound">q</a><a id="1380" class="Symbol">)</a>

  <a id="1385" href="foundation.equality-cartesian-product-types.html#1385" class="Function">pair-eq</a> <a id="1393" class="Symbol">:</a> <a id="1395" class="Symbol">{</a><a id="1396" href="foundation.equality-cartesian-product-types.html#1396" class="Bound">s</a> <a id="1398" href="foundation.equality-cartesian-product-types.html#1398" class="Bound">t</a> <a id="1400" class="Symbol">:</a> <a id="1402" href="foundation.equality-cartesian-product-types.html#1121" class="Bound">A</a> <a id="1404" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="1406" href="foundation.equality-cartesian-product-types.html#1133" class="Bound">B</a><a id="1407" class="Symbol">}</a> <a id="1409" class="Symbol">→</a> <a id="1411" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="1414" href="foundation.equality-cartesian-product-types.html#1396" class="Bound">s</a> <a id="1416" href="foundation.equality-cartesian-product-types.html#1398" class="Bound">t</a> <a id="1418" class="Symbol">→</a> <a id="1420" href="foundation.equality-cartesian-product-types.html#911" class="Function">Eq-prod</a> <a id="1428" href="foundation.equality-cartesian-product-types.html#1396" class="Bound">s</a> <a id="1430" href="foundation.equality-cartesian-product-types.html#1398" class="Bound">t</a>
  <a id="1434" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1438" class="Symbol">(</a><a id="1439" href="foundation.equality-cartesian-product-types.html#1385" class="Function">pair-eq</a> <a id="1447" href="foundation.equality-cartesian-product-types.html#1447" class="Bound">α</a><a id="1448" class="Symbol">)</a> <a id="1450" class="Symbol">=</a> <a id="1452" href="foundation-core.identity-types.html#2853" class="Function">ap</a> <a id="1455" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="1459" href="foundation.equality-cartesian-product-types.html#1447" class="Bound">α</a>
  <a id="1463" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1467" class="Symbol">(</a><a id="1468" href="foundation.equality-cartesian-product-types.html#1385" class="Function">pair-eq</a> <a id="1476" href="foundation.equality-cartesian-product-types.html#1476" class="Bound">α</a><a id="1477" class="Symbol">)</a> <a id="1479" class="Symbol">=</a> <a id="1481" href="foundation-core.identity-types.html#2853" class="Function">ap</a> <a id="1484" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="1488" href="foundation.equality-cartesian-product-types.html#1476" class="Bound">α</a>

  <a id="1493" href="foundation.equality-cartesian-product-types.html#1493" class="Function">isretr-pair-eq</a> <a id="1508" class="Symbol">:</a>
    <a id="1514" class="Symbol">{</a><a id="1515" href="foundation.equality-cartesian-product-types.html#1515" class="Bound">s</a> <a id="1517" href="foundation.equality-cartesian-product-types.html#1517" class="Bound">t</a> <a id="1519" class="Symbol">:</a> <a id="1521" href="foundation.equality-cartesian-product-types.html#1121" class="Bound">A</a> <a id="1523" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="1525" href="foundation.equality-cartesian-product-types.html#1133" class="Bound">B</a><a id="1526" class="Symbol">}</a> <a id="1528" class="Symbol">→</a> <a id="1530" class="Symbol">((</a><a id="1532" href="foundation.equality-cartesian-product-types.html#1385" class="Function">pair-eq</a> <a id="1540" class="Symbol">{</a><a id="1541" href="foundation.equality-cartesian-product-types.html#1515" class="Bound">s</a><a id="1542" class="Symbol">}</a> <a id="1544" class="Symbol">{</a><a id="1545" href="foundation.equality-cartesian-product-types.html#1517" class="Bound">t</a><a id="1546" class="Symbol">})</a> <a id="1549" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="1551" class="Symbol">(</a><a id="1552" href="foundation.equality-cartesian-product-types.html#1157" class="Function">eq-pair&#39;</a> <a id="1561" class="Symbol">{</a><a id="1562" href="foundation.equality-cartesian-product-types.html#1515" class="Bound">s</a><a id="1563" class="Symbol">}</a> <a id="1565" class="Symbol">{</a><a id="1566" href="foundation.equality-cartesian-product-types.html#1517" class="Bound">t</a><a id="1567" class="Symbol">}))</a> <a id="1571" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="1573" href="foundation-core.functions.html#309" class="Function">id</a>
  <a id="1578" href="foundation.equality-cartesian-product-types.html#1493" class="Function">isretr-pair-eq</a> <a id="1593" class="Symbol">{</a><a id="1594" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1599" href="foundation.equality-cartesian-product-types.html#1599" class="Bound">x</a> <a id="1601" href="foundation.equality-cartesian-product-types.html#1601" class="Bound">y</a><a id="1602" class="Symbol">}</a> <a id="1604" class="Symbol">{</a><a id="1605" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1610" class="DottedPattern Symbol">.</a><a id="1611" href="foundation.equality-cartesian-product-types.html#1599" class="DottedPattern Bound">x</a> <a id="1613" class="DottedPattern Symbol">.</a><a id="1614" href="foundation.equality-cartesian-product-types.html#1601" class="DottedPattern Bound">y</a><a id="1615" class="Symbol">}</a> <a id="1617" class="Symbol">(</a><a id="1618" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1623" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a> <a id="1628" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="1632" class="Symbol">)</a> <a id="1634" class="Symbol">=</a> <a id="1636" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a>

  <a id="1644" href="foundation.equality-cartesian-product-types.html#1644" class="Function">issec-pair-eq</a> <a id="1658" class="Symbol">:</a>
    <a id="1664" class="Symbol">{</a><a id="1665" href="foundation.equality-cartesian-product-types.html#1665" class="Bound">s</a> <a id="1667" href="foundation.equality-cartesian-product-types.html#1667" class="Bound">t</a> <a id="1669" class="Symbol">:</a> <a id="1671" href="foundation.equality-cartesian-product-types.html#1121" class="Bound">A</a> <a id="1673" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="1675" href="foundation.equality-cartesian-product-types.html#1133" class="Bound">B</a><a id="1676" class="Symbol">}</a> <a id="1678" class="Symbol">→</a> <a id="1680" class="Symbol">((</a><a id="1682" href="foundation.equality-cartesian-product-types.html#1157" class="Function">eq-pair&#39;</a> <a id="1691" class="Symbol">{</a><a id="1692" href="foundation.equality-cartesian-product-types.html#1665" class="Bound">s</a><a id="1693" class="Symbol">}</a> <a id="1695" class="Symbol">{</a><a id="1696" href="foundation.equality-cartesian-product-types.html#1667" class="Bound">t</a><a id="1697" class="Symbol">})</a> <a id="1700" href="foundation-core.functions.html#407" class="Function Operator">∘</a> <a id="1702" class="Symbol">(</a><a id="1703" href="foundation.equality-cartesian-product-types.html#1385" class="Function">pair-eq</a> <a id="1711" class="Symbol">{</a><a id="1712" href="foundation.equality-cartesian-product-types.html#1665" class="Bound">s</a><a id="1713" class="Symbol">}</a> <a id="1715" class="Symbol">{</a><a id="1716" href="foundation.equality-cartesian-product-types.html#1667" class="Bound">t</a><a id="1717" class="Symbol">}))</a> <a id="1721" href="foundation-core.homotopies.html#467" class="Function Operator">~</a> <a id="1723" href="foundation-core.functions.html#309" class="Function">id</a>
  <a id="1728" href="foundation.equality-cartesian-product-types.html#1644" class="Function">issec-pair-eq</a> <a id="1742" class="Symbol">{</a><a id="1743" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1748" href="foundation.equality-cartesian-product-types.html#1748" class="Bound">x</a> <a id="1750" href="foundation.equality-cartesian-product-types.html#1750" class="Bound">y</a><a id="1751" class="Symbol">}</a> <a id="1753" class="Symbol">{</a><a id="1754" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="1759" class="DottedPattern Symbol">.</a><a id="1760" href="foundation.equality-cartesian-product-types.html#1748" class="DottedPattern Bound">x</a> <a id="1762" class="DottedPattern Symbol">.</a><a id="1763" href="foundation.equality-cartesian-product-types.html#1750" class="DottedPattern Bound">y</a><a id="1764" class="Symbol">}</a> <a id="1766" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a> <a id="1771" class="Symbol">=</a> <a id="1773" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a>

  <a id="1781" class="Keyword">abstract</a>
    <a id="1794" href="foundation.equality-cartesian-product-types.html#1794" class="Function">is-equiv-eq-pair</a> <a id="1811" class="Symbol">:</a>
      <a id="1819" class="Symbol">(</a><a id="1820" href="foundation.equality-cartesian-product-types.html#1820" class="Bound">s</a> <a id="1822" href="foundation.equality-cartesian-product-types.html#1822" class="Bound">t</a> <a id="1824" class="Symbol">:</a> <a id="1826" href="foundation.equality-cartesian-product-types.html#1121" class="Bound">A</a> <a id="1828" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="1830" href="foundation.equality-cartesian-product-types.html#1133" class="Bound">B</a><a id="1831" class="Symbol">)</a> <a id="1833" class="Symbol">→</a> <a id="1835" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a> <a id="1844" class="Symbol">(</a><a id="1845" href="foundation.equality-cartesian-product-types.html#1157" class="Function">eq-pair&#39;</a> <a id="1854" class="Symbol">{</a><a id="1855" href="foundation.equality-cartesian-product-types.html#1820" class="Bound">s</a><a id="1856" class="Symbol">}</a> <a id="1858" class="Symbol">{</a><a id="1859" href="foundation.equality-cartesian-product-types.html#1822" class="Bound">t</a><a id="1860" class="Symbol">})</a>
    <a id="1867" href="foundation.equality-cartesian-product-types.html#1794" class="Function">is-equiv-eq-pair</a> <a id="1884" href="foundation.equality-cartesian-product-types.html#1884" class="Bound">s</a> <a id="1886" href="foundation.equality-cartesian-product-types.html#1886" class="Bound">t</a> <a id="1888" class="Symbol">=</a>
      <a id="1896" href="foundation-core.equivalences.html#2999" class="Function">is-equiv-has-inverse</a> <a id="1917" href="foundation.equality-cartesian-product-types.html#1385" class="Function">pair-eq</a> <a id="1925" href="foundation.equality-cartesian-product-types.html#1644" class="Function">issec-pair-eq</a> <a id="1939" href="foundation.equality-cartesian-product-types.html#1493" class="Function">isretr-pair-eq</a>

  <a id="1957" href="foundation.equality-cartesian-product-types.html#1957" class="Function">equiv-eq-pair</a> <a id="1971" class="Symbol">:</a>
    <a id="1977" class="Symbol">(</a><a id="1978" href="foundation.equality-cartesian-product-types.html#1978" class="Bound">s</a> <a id="1980" href="foundation.equality-cartesian-product-types.html#1980" class="Bound">t</a> <a id="1982" class="Symbol">:</a> <a id="1984" href="foundation.equality-cartesian-product-types.html#1121" class="Bound">A</a> <a id="1986" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="1988" href="foundation.equality-cartesian-product-types.html#1133" class="Bound">B</a><a id="1989" class="Symbol">)</a> <a id="1991" class="Symbol">→</a> <a id="1993" href="foundation.equality-cartesian-product-types.html#911" class="Function">Eq-prod</a> <a id="2001" href="foundation.equality-cartesian-product-types.html#1978" class="Bound">s</a> <a id="2003" href="foundation.equality-cartesian-product-types.html#1980" class="Bound">t</a> <a id="2005" href="foundation-core.equivalences.html#1607" class="Function Operator">≃</a> <a id="2007" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="2010" href="foundation.equality-cartesian-product-types.html#1978" class="Bound">s</a> <a id="2012" href="foundation.equality-cartesian-product-types.html#1980" class="Bound">t</a>
  <a id="2016" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2020" class="Symbol">(</a><a id="2021" href="foundation.equality-cartesian-product-types.html#1957" class="Function">equiv-eq-pair</a> <a id="2035" href="foundation.equality-cartesian-product-types.html#2035" class="Bound">s</a> <a id="2037" href="foundation.equality-cartesian-product-types.html#2037" class="Bound">t</a><a id="2038" class="Symbol">)</a> <a id="2040" class="Symbol">=</a> <a id="2042" href="foundation.equality-cartesian-product-types.html#1157" class="Function">eq-pair&#39;</a>
  <a id="2053" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2057" class="Symbol">(</a><a id="2058" href="foundation.equality-cartesian-product-types.html#1957" class="Function">equiv-eq-pair</a> <a id="2072" href="foundation.equality-cartesian-product-types.html#2072" class="Bound">s</a> <a id="2074" href="foundation.equality-cartesian-product-types.html#2074" class="Bound">t</a><a id="2075" class="Symbol">)</a> <a id="2077" class="Symbol">=</a> <a id="2079" href="foundation.equality-cartesian-product-types.html#1794" class="Function">is-equiv-eq-pair</a> <a id="2096" href="foundation.equality-cartesian-product-types.html#2072" class="Bound">s</a> <a id="2098" href="foundation.equality-cartesian-product-types.html#2074" class="Bound">t</a>

  <a id="2103" class="Keyword">abstract</a>
    <a id="2116" href="foundation.equality-cartesian-product-types.html#2116" class="Function">is-equiv-pair-eq</a> <a id="2133" class="Symbol">:</a>
      <a id="2141" class="Symbol">(</a><a id="2142" href="foundation.equality-cartesian-product-types.html#2142" class="Bound">s</a> <a id="2144" href="foundation.equality-cartesian-product-types.html#2144" class="Bound">t</a> <a id="2146" class="Symbol">:</a> <a id="2148" href="foundation.equality-cartesian-product-types.html#1121" class="Bound">A</a> <a id="2150" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="2152" href="foundation.equality-cartesian-product-types.html#1133" class="Bound">B</a><a id="2153" class="Symbol">)</a> <a id="2155" class="Symbol">→</a> <a id="2157" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a> <a id="2166" class="Symbol">(</a><a id="2167" href="foundation.equality-cartesian-product-types.html#1385" class="Function">pair-eq</a> <a id="2175" class="Symbol">{</a><a id="2176" href="foundation.equality-cartesian-product-types.html#2142" class="Bound">s</a><a id="2177" class="Symbol">}</a> <a id="2179" class="Symbol">{</a><a id="2180" href="foundation.equality-cartesian-product-types.html#2144" class="Bound">t</a><a id="2181" class="Symbol">})</a>
    <a id="2188" href="foundation.equality-cartesian-product-types.html#2116" class="Function">is-equiv-pair-eq</a> <a id="2205" href="foundation.equality-cartesian-product-types.html#2205" class="Bound">s</a> <a id="2207" href="foundation.equality-cartesian-product-types.html#2207" class="Bound">t</a> <a id="2209" class="Symbol">=</a>
      <a id="2217" href="foundation-core.equivalences.html#2999" class="Function">is-equiv-has-inverse</a> <a id="2238" href="foundation.equality-cartesian-product-types.html#1157" class="Function">eq-pair&#39;</a> <a id="2247" href="foundation.equality-cartesian-product-types.html#1493" class="Function">isretr-pair-eq</a> <a id="2262" href="foundation.equality-cartesian-product-types.html#1644" class="Function">issec-pair-eq</a>

  <a id="2279" href="foundation.equality-cartesian-product-types.html#2279" class="Function">equiv-pair-eq</a> <a id="2293" class="Symbol">:</a>
    <a id="2299" class="Symbol">(</a><a id="2300" href="foundation.equality-cartesian-product-types.html#2300" class="Bound">s</a> <a id="2302" href="foundation.equality-cartesian-product-types.html#2302" class="Bound">t</a> <a id="2304" class="Symbol">:</a> <a id="2306" href="foundation.equality-cartesian-product-types.html#1121" class="Bound">A</a> <a id="2308" href="foundation-core.cartesian-product-types.html#577" class="Function Operator">×</a> <a id="2310" href="foundation.equality-cartesian-product-types.html#1133" class="Bound">B</a><a id="2311" class="Symbol">)</a> <a id="2313" class="Symbol">→</a> <a id="2315" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="2318" href="foundation.equality-cartesian-product-types.html#2300" class="Bound">s</a> <a id="2320" href="foundation.equality-cartesian-product-types.html#2302" class="Bound">t</a> <a id="2322" href="foundation-core.equivalences.html#1607" class="Function Operator">≃</a> <a id="2324" href="foundation.equality-cartesian-product-types.html#911" class="Function">Eq-prod</a> <a id="2332" href="foundation.equality-cartesian-product-types.html#2300" class="Bound">s</a> <a id="2334" href="foundation.equality-cartesian-product-types.html#2302" class="Bound">t</a>
  <a id="2338" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="2342" class="Symbol">(</a><a id="2343" href="foundation.equality-cartesian-product-types.html#2279" class="Function">equiv-pair-eq</a> <a id="2357" href="foundation.equality-cartesian-product-types.html#2357" class="Bound">s</a> <a id="2359" href="foundation.equality-cartesian-product-types.html#2359" class="Bound">t</a><a id="2360" class="Symbol">)</a> <a id="2362" class="Symbol">=</a> <a id="2364" href="foundation.equality-cartesian-product-types.html#1385" class="Function">pair-eq</a>
  <a id="2374" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="2378" class="Symbol">(</a><a id="2379" href="foundation.equality-cartesian-product-types.html#2279" class="Function">equiv-pair-eq</a> <a id="2393" href="foundation.equality-cartesian-product-types.html#2393" class="Bound">s</a> <a id="2395" href="foundation.equality-cartesian-product-types.html#2395" class="Bound">t</a><a id="2396" class="Symbol">)</a> <a id="2398" class="Symbol">=</a> <a id="2400" href="foundation.equality-cartesian-product-types.html#2116" class="Function">is-equiv-pair-eq</a> <a id="2417" href="foundation.equality-cartesian-product-types.html#2393" class="Bound">s</a> <a id="2419" href="foundation.equality-cartesian-product-types.html#2395" class="Bound">t</a>
</pre>