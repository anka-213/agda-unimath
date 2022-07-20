---
title: Totally faithful morphisms of undirected graphs
---

<pre class="Agda"><a id="73" class="Symbol">{-#</a> <a id="77" class="Keyword">OPTIONS</a> <a id="85" class="Pragma">--without-K</a> <a id="97" class="Pragma">--exact-split</a> <a id="111" class="Symbol">#-}</a>

<a id="116" class="Keyword">module</a> <a id="123" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html" class="Module">graph-theory.totally-faithful-morphisms-undirected-graphs</a> <a id="181" class="Keyword">where</a>

<a id="188" class="Keyword">open</a> <a id="193" class="Keyword">import</a> <a id="200" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="232" class="Keyword">open</a> <a id="237" class="Keyword">import</a> <a id="244" href="foundation.embeddings.html" class="Module">foundation.embeddings</a>
<a id="266" class="Keyword">open</a> <a id="271" class="Keyword">import</a> <a id="278" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="324" class="Keyword">open</a> <a id="329" class="Keyword">import</a> <a id="336" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="364" class="Keyword">open</a> <a id="369" class="Keyword">import</a> <a id="376" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="417" class="Keyword">open</a> <a id="422" class="Keyword">import</a> <a id="429" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Idea

A totally faithful morphism of undirected graphs is a morphism `f : G → H` of undirected graphs such that for edge `e` in `H` there is at most one edge in `G` that `f` maps to `e`.

## Definition

<pre class="Agda"><a id="679" class="Keyword">module</a> <a id="686" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#686" class="Module">_</a>
  <a id="690" class="Symbol">{</a><a id="691" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#691" class="Bound">l1</a> <a id="694" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#694" class="Bound">l2</a> <a id="697" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#697" class="Bound">l3</a> <a id="700" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#700" class="Bound">l4</a> <a id="703" class="Symbol">:</a> <a id="705" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="710" class="Symbol">}</a>
  <a id="714" class="Symbol">(</a><a id="715" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#715" class="Bound">G</a> <a id="717" class="Symbol">:</a> <a id="719" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a> <a id="736" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#691" class="Bound">l1</a> <a id="739" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#694" class="Bound">l2</a><a id="741" class="Symbol">)</a> <a id="743" class="Symbol">(</a><a id="744" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#744" class="Bound">H</a> <a id="746" class="Symbol">:</a> <a id="748" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a> <a id="765" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#697" class="Bound">l3</a> <a id="768" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#700" class="Bound">l4</a><a id="770" class="Symbol">)</a>
  <a id="774" class="Keyword">where</a>
  
  <a id="785" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#785" class="Function">is-totally-faithful-hom-Undirected-Graph</a> <a id="826" class="Symbol">:</a>
    <a id="832" href="graph-theory.morphisms-undirected-graphs.html#1538" class="Function">hom-Undirected-Graph</a> <a id="853" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#715" class="Bound">G</a> <a id="855" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#744" class="Bound">H</a> <a id="857" class="Symbol">→</a> <a id="859" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="862" class="Symbol">(</a><a id="863" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="868" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="874" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="876" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#691" class="Bound">l1</a> <a id="879" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="881" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#694" class="Bound">l2</a> <a id="884" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="886" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#700" class="Bound">l4</a><a id="888" class="Symbol">)</a>
  <a id="892" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#785" class="Function">is-totally-faithful-hom-Undirected-Graph</a> <a id="933" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#933" class="Bound">f</a> <a id="935" class="Symbol">=</a>
    <a id="941" href="foundation-core.embeddings.html#992" class="Function">is-emb</a> <a id="948" class="Symbol">(</a><a id="949" href="foundation-core.functoriality-dependent-pair-types.html#1894" class="Function">tot</a> <a id="953" class="Symbol">(</a><a id="954" href="graph-theory.morphisms-undirected-graphs.html#2289" class="Function">edge-hom-Undirected-Graph</a> <a id="980" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#715" class="Bound">G</a> <a id="982" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#744" class="Bound">H</a> <a id="984" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#933" class="Bound">f</a><a id="985" class="Symbol">))</a>

  <a id="991" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#991" class="Function">totally-faithful-hom-Undirected-Graph</a> <a id="1029" class="Symbol">:</a> <a id="1031" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1034" class="Symbol">(</a><a id="1035" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1040" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="1046" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1048" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#691" class="Bound">l1</a> <a id="1051" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1053" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#694" class="Bound">l2</a> <a id="1056" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1058" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#697" class="Bound">l3</a> <a id="1061" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1063" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#700" class="Bound">l4</a><a id="1065" class="Symbol">)</a>
  <a id="1069" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#991" class="Function">totally-faithful-hom-Undirected-Graph</a> <a id="1107" class="Symbol">=</a>
    <a id="1113" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1115" class="Symbol">(</a><a id="1116" href="graph-theory.morphisms-undirected-graphs.html#1538" class="Function">hom-Undirected-Graph</a> <a id="1137" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#715" class="Bound">G</a> <a id="1139" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#744" class="Bound">H</a><a id="1140" class="Symbol">)</a> <a id="1142" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#785" class="Function">is-totally-faithful-hom-Undirected-Graph</a>

<a id="1184" class="Keyword">module</a> <a id="1191" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1191" class="Module">_</a>
  <a id="1195" class="Symbol">{</a><a id="1196" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1196" class="Bound">l1</a> <a id="1199" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1199" class="Bound">l2</a> <a id="1202" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1202" class="Bound">l3</a> <a id="1205" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1205" class="Bound">l4</a> <a id="1208" class="Symbol">:</a> <a id="1210" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1215" class="Symbol">}</a>
  <a id="1219" class="Symbol">(</a><a id="1220" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a> <a id="1222" class="Symbol">:</a> <a id="1224" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a> <a id="1241" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1196" class="Bound">l1</a> <a id="1244" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1199" class="Bound">l2</a><a id="1246" class="Symbol">)</a> <a id="1248" class="Symbol">(</a><a id="1249" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1249" class="Bound">H</a> <a id="1251" class="Symbol">:</a> <a id="1253" href="graph-theory.undirected-graphs.html#785" class="Function">Undirected-Graph</a> <a id="1270" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1202" class="Bound">l3</a> <a id="1273" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1205" class="Bound">l4</a><a id="1275" class="Symbol">)</a>
  <a id="1279" class="Symbol">(</a><a id="1280" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1280" class="Bound">f</a> <a id="1282" class="Symbol">:</a> <a id="1284" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#991" class="Function">totally-faithful-hom-Undirected-Graph</a> <a id="1322" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a> <a id="1324" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1249" class="Bound">H</a><a id="1325" class="Symbol">)</a>
  <a id="1329" class="Keyword">where</a>

  <a id="1338" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1338" class="Function">hom-totally-faithful-hom-Undirected-Graph</a> <a id="1380" class="Symbol">:</a> <a id="1382" href="graph-theory.morphisms-undirected-graphs.html#1538" class="Function">hom-Undirected-Graph</a> <a id="1403" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a> <a id="1405" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1249" class="Bound">H</a>
  <a id="1409" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1338" class="Function">hom-totally-faithful-hom-Undirected-Graph</a> <a id="1451" class="Symbol">=</a> <a id="1453" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1457" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1280" class="Bound">f</a>

  <a id="1462" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1462" class="Function">vertex-totally-faithful-hom-Undirected-Graph</a> <a id="1507" class="Symbol">:</a>
    <a id="1513" href="graph-theory.undirected-graphs.html#981" class="Function">vertex-Undirected-Graph</a> <a id="1537" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a> <a id="1539" class="Symbol">→</a> <a id="1541" href="graph-theory.undirected-graphs.html#981" class="Function">vertex-Undirected-Graph</a> <a id="1565" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1249" class="Bound">H</a>
  <a id="1569" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1462" class="Function">vertex-totally-faithful-hom-Undirected-Graph</a> <a id="1614" class="Symbol">=</a>
    <a id="1620" href="graph-theory.morphisms-undirected-graphs.html#1856" class="Function">vertex-hom-Undirected-Graph</a> <a id="1648" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a> <a id="1650" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1249" class="Bound">H</a> <a id="1652" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1338" class="Function">hom-totally-faithful-hom-Undirected-Graph</a>

  <a id="1697" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1697" class="Function">unordered-pair-vertices-totally-faithful-hom-Undirected-Graph</a> <a id="1759" class="Symbol">:</a>
    <a id="1765" href="graph-theory.undirected-graphs.html#1050" class="Function">unordered-pair-vertices-Undirected-Graph</a> <a id="1806" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a> <a id="1808" class="Symbol">→</a>
    <a id="1814" href="graph-theory.undirected-graphs.html#1050" class="Function">unordered-pair-vertices-Undirected-Graph</a> <a id="1855" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1249" class="Bound">H</a>
  <a id="1859" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1697" class="Function">unordered-pair-vertices-totally-faithful-hom-Undirected-Graph</a> <a id="1921" class="Symbol">=</a>
    <a id="1927" href="graph-theory.morphisms-undirected-graphs.html#2010" class="Function">unordered-pair-vertices-hom-Undirected-Graph</a> <a id="1972" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a> <a id="1974" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1249" class="Bound">H</a>
      <a id="1982" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1338" class="Function">hom-totally-faithful-hom-Undirected-Graph</a>

  <a id="2027" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#2027" class="Function">edge-totally-faithful-hom-Undirected-Graph</a> <a id="2070" class="Symbol">:</a>
    <a id="2076" class="Symbol">(</a><a id="2077" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#2077" class="Bound">p</a> <a id="2079" class="Symbol">:</a> <a id="2081" href="graph-theory.undirected-graphs.html#1050" class="Function">unordered-pair-vertices-Undirected-Graph</a> <a id="2122" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a><a id="2123" class="Symbol">)</a> <a id="2125" class="Symbol">→</a>
    <a id="2131" href="graph-theory.undirected-graphs.html#1651" class="Function">edge-Undirected-Graph</a> <a id="2153" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a> <a id="2155" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#2077" class="Bound">p</a> <a id="2157" class="Symbol">→</a>
    <a id="2163" href="graph-theory.undirected-graphs.html#1651" class="Function">edge-Undirected-Graph</a> <a id="2185" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1249" class="Bound">H</a>
      <a id="2193" class="Symbol">(</a> <a id="2195" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1697" class="Function">unordered-pair-vertices-totally-faithful-hom-Undirected-Graph</a> <a id="2257" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#2077" class="Bound">p</a><a id="2258" class="Symbol">)</a>
  <a id="2262" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#2027" class="Function">edge-totally-faithful-hom-Undirected-Graph</a> <a id="2305" class="Symbol">=</a>
    <a id="2311" href="graph-theory.morphisms-undirected-graphs.html#2289" class="Function">edge-hom-Undirected-Graph</a> <a id="2337" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a> <a id="2339" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1249" class="Bound">H</a> <a id="2341" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1338" class="Function">hom-totally-faithful-hom-Undirected-Graph</a>

  <a id="2386" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#2386" class="Function">is-totally-faithful-totally-faithful-hom-Undirected-Graph</a> <a id="2444" class="Symbol">:</a>
    <a id="2450" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#785" class="Function">is-totally-faithful-hom-Undirected-Graph</a> <a id="2491" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1220" class="Bound">G</a> <a id="2493" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1249" class="Bound">H</a>
      <a id="2501" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1338" class="Function">hom-totally-faithful-hom-Undirected-Graph</a>
  <a id="2545" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#2386" class="Function">is-totally-faithful-totally-faithful-hom-Undirected-Graph</a> <a id="2603" class="Symbol">=</a> <a id="2605" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="2609" href="graph-theory.totally-faithful-morphisms-undirected-graphs.html#1280" class="Bound">f</a>
</pre>
## See also

- Embeddings of undirected graphs
- Faithful morphisms of undirected graphs