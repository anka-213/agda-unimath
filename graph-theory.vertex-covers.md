# Vertex covers

<pre class="Agda"><a id="26" class="Symbol">{-#</a> <a id="30" class="Keyword">OPTIONS</a> <a id="38" class="Pragma">--without-K</a> <a id="50" class="Pragma">--exact-split</a> <a id="64" class="Symbol">#-}</a>

<a id="69" class="Keyword">module</a> <a id="76" href="graph-theory.vertex-covers.html" class="Module">graph-theory.vertex-covers</a> <a id="103" class="Keyword">where</a>

<a id="110" class="Keyword">open</a> <a id="115" class="Keyword">import</a> <a id="122" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a> <a id="157" class="Keyword">using</a> <a id="163" class="Symbol">(</a><a id="164" href="foundation-core.cartesian-product-types.html#590" class="Function Operator">_×_</a><a id="167" class="Symbol">)</a>
<a id="169" class="Keyword">open</a> <a id="174" class="Keyword">import</a> <a id="181" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a> <a id="208" class="Keyword">using</a> <a id="214" class="Symbol">(</a><a id="215" href="foundation.coproduct-types.html#1276" class="InductiveConstructor">inr</a><a id="218" class="Symbol">)</a>
<a id="220" class="Keyword">open</a> <a id="225" class="Keyword">import</a> <a id="232" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="264" class="Keyword">using</a> <a id="270" class="Symbol">(</a><a id="271" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a><a id="272" class="Symbol">;</a> <a id="274" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a><a id="278" class="Symbol">;</a> <a id="280" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a><a id="283" class="Symbol">;</a> <a id="285" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a><a id="288" class="Symbol">)</a>
<a id="290" class="Keyword">open</a> <a id="295" class="Keyword">import</a> <a id="302" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="328" class="Keyword">using</a> <a id="334" class="Symbol">(</a><a id="335" href="foundation-core.identity-types.html#1767" class="Datatype">Id</a><a id="337" class="Symbol">)</a>
<a id="339" class="Keyword">open</a> <a id="344" class="Keyword">import</a> <a id="351" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a> <a id="388" class="Keyword">using</a> <a id="394" class="Symbol">(</a><a id="395" href="foundation.propositional-truncations.html#2048" class="Function">type-trunc-Prop</a><a id="410" class="Symbol">)</a>
<a id="412" class="Keyword">open</a> <a id="417" class="Keyword">import</a> <a id="424" href="foundation.propositions.html" class="Module">foundation.propositions</a> <a id="448" class="Keyword">using</a> <a id="454" class="Symbol">(</a><a id="455" href="foundation-core.propositions.html#1309" class="Function">is-prop</a><a id="462" class="Symbol">)</a>
<a id="464" class="Keyword">open</a> <a id="469" class="Keyword">import</a> <a id="476" href="foundation.unit-type.html" class="Module">foundation.unit-type</a> <a id="497" class="Keyword">using</a> <a id="503" class="Symbol">(</a><a id="504" href="foundation.unit-type.html#1108" class="InductiveConstructor">star</a><a id="508" class="Symbol">)</a>
<a id="510" class="Keyword">open</a> <a id="515" class="Keyword">import</a> <a id="522" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="549" class="Keyword">using</a> <a id="555" class="Symbol">(</a><a id="556" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="561" class="Symbol">;</a> <a id="563" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a><a id="565" class="Symbol">;</a> <a id="567" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="570" class="Symbol">;</a> <a id="572" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="576" class="Symbol">;</a> <a id="578" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="583" class="Symbol">)</a>
<a id="585" class="Keyword">open</a> <a id="590" class="Keyword">import</a> <a id="597" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a> <a id="624" class="Keyword">using</a> <a id="630" class="Symbol">(</a><a id="631" href="foundation.unordered-pairs.html#3819" class="Function">is-in-unordered-pair</a><a id="651" class="Symbol">)</a>

<a id="654" class="Keyword">open</a> <a id="659" class="Keyword">import</a> <a id="666" href="graph-theory.edge-coloured-undirected-graphs.html" class="Module">graph-theory.edge-coloured-undirected-graphs</a> <a id="711" class="Keyword">using</a>
  <a id="719" class="Symbol">(</a> <a id="721" href="graph-theory.edge-coloured-undirected-graphs.html#1116" class="Function">incidence-edge-colouring-Undirected-Graph</a><a id="762" class="Symbol">)</a>
<a id="764" class="Keyword">open</a> <a id="769" class="Keyword">import</a> <a id="776" href="graph-theory.incidence-undirected-graphs.html" class="Module">graph-theory.incidence-undirected-graphs</a> <a id="817" class="Keyword">using</a>
  <a id="825" class="Symbol">(</a> <a id="827" href="graph-theory.incidence-undirected-graphs.html#695" class="Function">incidence-Undirected-Graph</a><a id="853" class="Symbol">)</a>
<a id="855" class="Keyword">open</a> <a id="860" class="Keyword">import</a> <a id="867" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a> <a id="898" class="Keyword">using</a>
  <a id="906" class="Symbol">(</a> <a id="908" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a><a id="924" class="Symbol">;</a> <a id="926" href="graph-theory.undirected-graphs.html#1050" class="Function">unordered-pair-vertices-Undirected-Graph</a><a id="966" class="Symbol">;</a>
    <a id="972" href="graph-theory.undirected-graphs.html#981" class="Function">vertex-Undirected-Graph</a><a id="995" class="Symbol">;</a> <a id="997" href="graph-theory.undirected-graphs.html#1651" class="Function">edge-Undirected-Graph</a><a id="1018" class="Symbol">)</a>

<a id="1021" class="Keyword">open</a> <a id="1026" class="Keyword">import</a> <a id="1033" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a> <a id="1079" class="Keyword">using</a> <a id="1085" class="Symbol">(</a><a id="1086" href="univalent-combinatorics.standard-finite-types.html#2149" class="Function">Fin</a><a id="1089" class="Symbol">)</a>
</pre>
## Idea

A vertex cover on a undirect graph is a set of vertices that includes at least one extremity of each edge of the graph

## Definitions

<pre class="Agda"><a id="vertex-cover"></a><a id="1249" href="graph-theory.vertex-covers.html#1249" class="Function">vertex-cover</a> <a id="1262" class="Symbol">:</a> <a id="1264" class="Symbol">{</a><a id="1265" href="graph-theory.vertex-covers.html#1265" class="Bound">l1</a> <a id="1268" href="graph-theory.vertex-covers.html#1268" class="Bound">l2</a> <a id="1271" class="Symbol">:</a> <a id="1273" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1278" class="Symbol">}</a> <a id="1280" class="Symbol">→</a> <a id="1282" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a> <a id="1299" href="graph-theory.vertex-covers.html#1265" class="Bound">l1</a> <a id="1302" href="graph-theory.vertex-covers.html#1268" class="Bound">l2</a> <a id="1305" class="Symbol">→</a>
  <a id="1309" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1312" class="Symbol">(</a><a id="1313" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1318" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="1324" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1326" href="graph-theory.vertex-covers.html#1265" class="Bound">l1</a> <a id="1329" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1331" href="graph-theory.vertex-covers.html#1268" class="Bound">l2</a><a id="1333" class="Symbol">)</a>
<a id="1335" href="graph-theory.vertex-covers.html#1249" class="Function">vertex-cover</a> <a id="1348" href="graph-theory.vertex-covers.html#1348" class="Bound">G</a> <a id="1350" class="Symbol">=</a> 
  <a id="1355" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1357" class="Symbol">(</a> <a id="1359" href="graph-theory.undirected-graphs.html#981" class="Function">vertex-Undirected-Graph</a> <a id="1383" href="graph-theory.vertex-covers.html#1348" class="Bound">G</a> <a id="1385" class="Symbol">→</a> <a id="1387" href="univalent-combinatorics.standard-finite-types.html#2149" class="Function">Fin</a> <a id="1391" class="Number">2</a><a id="1392" class="Symbol">)</a>
    <a id="1398" class="Symbol">(</a> <a id="1400" class="Symbol">λ</a> <a id="1402" href="graph-theory.vertex-covers.html#1402" class="Bound">c</a> <a id="1404" class="Symbol">→</a>
      <a id="1412" class="Symbol">(</a> <a id="1414" href="graph-theory.vertex-covers.html#1414" class="Bound">p</a> <a id="1416" class="Symbol">:</a> <a id="1418" href="graph-theory.undirected-graphs.html#1050" class="Function">unordered-pair-vertices-Undirected-Graph</a> <a id="1459" href="graph-theory.vertex-covers.html#1348" class="Bound">G</a><a id="1460" class="Symbol">)</a> <a id="1462" class="Symbol">→</a> <a id="1464" href="graph-theory.undirected-graphs.html#1651" class="Function">edge-Undirected-Graph</a> <a id="1486" href="graph-theory.vertex-covers.html#1348" class="Bound">G</a> <a id="1488" href="graph-theory.vertex-covers.html#1414" class="Bound">p</a> <a id="1490" class="Symbol">→</a>
        <a id="1500" href="foundation.propositional-truncations.html#2048" class="Function">type-trunc-Prop</a>
          <a id="1526" class="Symbol">(</a> <a id="1528" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1530" class="Symbol">(</a><a id="1531" href="graph-theory.undirected-graphs.html#981" class="Function">vertex-Undirected-Graph</a> <a id="1555" href="graph-theory.vertex-covers.html#1348" class="Bound">G</a><a id="1556" class="Symbol">)</a>
            <a id="1570" class="Symbol">(</a> <a id="1572" class="Symbol">λ</a> <a id="1574" href="graph-theory.vertex-covers.html#1574" class="Bound">x</a> <a id="1576" class="Symbol">→</a> <a id="1578" href="foundation.unordered-pairs.html#3819" class="Function">is-in-unordered-pair</a> <a id="1599" href="graph-theory.vertex-covers.html#1414" class="Bound">p</a> <a id="1601" href="graph-theory.vertex-covers.html#1574" class="Bound">x</a> <a id="1603" href="foundation-core.cartesian-product-types.html#590" class="Function Operator">×</a> <a id="1605" href="foundation-core.identity-types.html#1767" class="Datatype">Id</a> <a id="1608" class="Symbol">(</a><a id="1609" href="graph-theory.vertex-covers.html#1402" class="Bound">c</a> <a id="1611" href="graph-theory.vertex-covers.html#1574" class="Bound">x</a><a id="1612" class="Symbol">)</a> <a id="1614" class="Symbol">(</a><a id="1615" href="foundation.coproduct-types.html#1276" class="InductiveConstructor">inr</a> <a id="1619" href="foundation.unit-type.html#1108" class="InductiveConstructor">star</a><a id="1623" class="Symbol">))))</a>
</pre>