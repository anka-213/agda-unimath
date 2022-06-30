---
title : Voltage graphs
--- 

<pre class="Agda"><a id="42" class="Symbol">{-#</a> <a id="46" class="Keyword">OPTIONS</a> <a id="54" class="Pragma">--without-K</a> <a id="66" class="Pragma">--exact-split</a> <a id="80" class="Symbol">#-}</a>

<a id="85" class="Keyword">module</a> <a id="92" href="graph-theory.voltage-graphs.html" class="Module">graph-theory.voltage-graphs</a> <a id="120" class="Keyword">where</a>

<a id="127" class="Keyword">open</a> <a id="132" class="Keyword">import</a> <a id="139" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="171" class="Keyword">open</a> <a id="176" class="Keyword">import</a> <a id="183" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="211" class="Keyword">open</a> <a id="216" class="Keyword">import</a> <a id="223" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a>

<a id="253" class="Keyword">open</a> <a id="258" class="Keyword">import</a> <a id="265" href="group-theory.groups.html" class="Module">group-theory.groups</a>
</pre>
## Idea

A voltage graph is a directed graph `G` equipped with a group `Π` (the voltage group) and a labelling of the edges of `G` by elements of `Π`.

## Definition

<pre class="Agda"><a id="Voltage-Graph"></a><a id="465" href="graph-theory.voltage-graphs.html#465" class="Function">Voltage-Graph</a> <a id="479" class="Symbol">:</a>
  <a id="483" class="Symbol">{</a><a id="484" href="graph-theory.voltage-graphs.html#484" class="Bound">l1</a> <a id="487" class="Symbol">:</a> <a id="489" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="494" class="Symbol">}</a> <a id="496" class="Symbol">(</a><a id="497" href="graph-theory.voltage-graphs.html#497" class="Bound">l2</a> <a id="500" href="graph-theory.voltage-graphs.html#500" class="Bound">l3</a> <a id="503" class="Symbol">:</a> <a id="505" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="510" class="Symbol">)</a> <a id="512" class="Symbol">(</a><a id="513" href="graph-theory.voltage-graphs.html#513" class="Bound">Π</a> <a id="515" class="Symbol">:</a> <a id="517" href="group-theory.groups.html#2468" class="Function">Group</a> <a id="523" href="graph-theory.voltage-graphs.html#484" class="Bound">l1</a><a id="525" class="Symbol">)</a> <a id="527" class="Symbol">→</a> <a id="529" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="532" class="Symbol">(</a><a id="533" href="graph-theory.voltage-graphs.html#484" class="Bound">l1</a> <a id="536" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="538" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="543" href="graph-theory.voltage-graphs.html#497" class="Bound">l2</a> <a id="546" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="548" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="553" href="graph-theory.voltage-graphs.html#500" class="Bound">l3</a><a id="555" class="Symbol">)</a>
<a id="557" href="graph-theory.voltage-graphs.html#465" class="Function">Voltage-Graph</a> <a id="571" href="graph-theory.voltage-graphs.html#571" class="Bound">l2</a> <a id="574" href="graph-theory.voltage-graphs.html#574" class="Bound">l3</a> <a id="577" href="graph-theory.voltage-graphs.html#577" class="Bound">Π</a> <a id="579" class="Symbol">=</a>
  <a id="583" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="585" class="Symbol">(</a> <a id="587" href="graph-theory.directed-graphs.html#483" class="Function">Graph</a> <a id="593" href="graph-theory.voltage-graphs.html#571" class="Bound">l2</a> <a id="596" href="graph-theory.voltage-graphs.html#574" class="Bound">l3</a><a id="598" class="Symbol">)</a>
    <a id="604" class="Symbol">(</a> <a id="606" class="Symbol">λ</a> <a id="608" href="graph-theory.voltage-graphs.html#608" class="Bound">G</a> <a id="610" class="Symbol">→</a> <a id="612" class="Symbol">{</a><a id="613" href="graph-theory.voltage-graphs.html#613" class="Bound">x</a> <a id="615" href="graph-theory.voltage-graphs.html#615" class="Bound">y</a> <a id="617" class="Symbol">:</a> <a id="619" href="graph-theory.directed-graphs.html#635" class="Function">vertex-Graph</a> <a id="632" href="graph-theory.voltage-graphs.html#608" class="Bound">G</a><a id="633" class="Symbol">}</a> <a id="635" class="Symbol">→</a> <a id="637" href="graph-theory.directed-graphs.html#682" class="Function">edge-Graph</a> <a id="648" href="graph-theory.voltage-graphs.html#608" class="Bound">G</a> <a id="650" href="graph-theory.voltage-graphs.html#613" class="Bound">x</a> <a id="652" href="graph-theory.voltage-graphs.html#615" class="Bound">y</a> <a id="654" class="Symbol">→</a> <a id="656" href="group-theory.groups.html#2711" class="Function">type-Group</a> <a id="667" href="graph-theory.voltage-graphs.html#577" class="Bound">Π</a><a id="668" class="Symbol">)</a>

<a id="671" class="Keyword">module</a> <a id="678" href="graph-theory.voltage-graphs.html#678" class="Module">_</a>
  <a id="682" class="Symbol">{</a><a id="683" href="graph-theory.voltage-graphs.html#683" class="Bound">l1</a> <a id="686" href="graph-theory.voltage-graphs.html#686" class="Bound">l2</a> <a id="689" href="graph-theory.voltage-graphs.html#689" class="Bound">l3</a> <a id="692" class="Symbol">:</a> <a id="694" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="699" class="Symbol">}</a> <a id="701" class="Symbol">(</a><a id="702" href="graph-theory.voltage-graphs.html#702" class="Bound">Π</a> <a id="704" class="Symbol">:</a> <a id="706" href="group-theory.groups.html#2468" class="Function">Group</a> <a id="712" href="graph-theory.voltage-graphs.html#683" class="Bound">l1</a><a id="714" class="Symbol">)</a> <a id="716" class="Symbol">(</a><a id="717" href="graph-theory.voltage-graphs.html#717" class="Bound">G</a> <a id="719" class="Symbol">:</a> <a id="721" href="graph-theory.voltage-graphs.html#465" class="Function">Voltage-Graph</a> <a id="735" href="graph-theory.voltage-graphs.html#686" class="Bound">l2</a> <a id="738" href="graph-theory.voltage-graphs.html#689" class="Bound">l3</a> <a id="741" href="graph-theory.voltage-graphs.html#702" class="Bound">Π</a><a id="742" class="Symbol">)</a>
  <a id="746" class="Keyword">where</a>

  <a id="755" href="graph-theory.voltage-graphs.html#755" class="Function">graph-Voltage-Graph</a> <a id="775" class="Symbol">:</a> <a id="777" href="graph-theory.directed-graphs.html#483" class="Function">Graph</a> <a id="783" href="graph-theory.voltage-graphs.html#686" class="Bound">l2</a> <a id="786" href="graph-theory.voltage-graphs.html#689" class="Bound">l3</a>
  <a id="791" href="graph-theory.voltage-graphs.html#755" class="Function">graph-Voltage-Graph</a> <a id="811" class="Symbol">=</a> <a id="813" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="817" href="graph-theory.voltage-graphs.html#717" class="Bound">G</a>

  <a id="822" href="graph-theory.voltage-graphs.html#822" class="Function">vertex-Voltage-Graph</a> <a id="843" class="Symbol">:</a> <a id="845" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="848" href="graph-theory.voltage-graphs.html#686" class="Bound">l2</a>
  <a id="853" href="graph-theory.voltage-graphs.html#822" class="Function">vertex-Voltage-Graph</a> <a id="874" class="Symbol">=</a> <a id="876" href="graph-theory.directed-graphs.html#635" class="Function">vertex-Graph</a> <a id="889" href="graph-theory.voltage-graphs.html#755" class="Function">graph-Voltage-Graph</a>

  <a id="912" href="graph-theory.voltage-graphs.html#912" class="Function">edge-Voltage-Graph</a> <a id="931" class="Symbol">:</a> <a id="933" class="Symbol">(</a><a id="934" href="graph-theory.voltage-graphs.html#934" class="Bound">x</a> <a id="936" href="graph-theory.voltage-graphs.html#936" class="Bound">y</a> <a id="938" class="Symbol">:</a> <a id="940" href="graph-theory.voltage-graphs.html#822" class="Function">vertex-Voltage-Graph</a><a id="960" class="Symbol">)</a> <a id="962" class="Symbol">→</a> <a id="964" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="967" href="graph-theory.voltage-graphs.html#689" class="Bound">l3</a>
  <a id="972" href="graph-theory.voltage-graphs.html#912" class="Function">edge-Voltage-Graph</a> <a id="991" class="Symbol">=</a> <a id="993" href="graph-theory.directed-graphs.html#682" class="Function">edge-Graph</a> <a id="1004" href="graph-theory.voltage-graphs.html#755" class="Function">graph-Voltage-Graph</a>

  <a id="1027" href="graph-theory.voltage-graphs.html#1027" class="Function">voltage-Voltage-Graph</a> <a id="1049" class="Symbol">:</a>
    <a id="1055" class="Symbol">{</a><a id="1056" href="graph-theory.voltage-graphs.html#1056" class="Bound">x</a> <a id="1058" href="graph-theory.voltage-graphs.html#1058" class="Bound">y</a> <a id="1060" class="Symbol">:</a> <a id="1062" href="graph-theory.voltage-graphs.html#822" class="Function">vertex-Voltage-Graph</a><a id="1082" class="Symbol">}</a> <a id="1084" class="Symbol">→</a> <a id="1086" href="graph-theory.voltage-graphs.html#912" class="Function">edge-Voltage-Graph</a> <a id="1105" href="graph-theory.voltage-graphs.html#1056" class="Bound">x</a> <a id="1107" href="graph-theory.voltage-graphs.html#1058" class="Bound">y</a> <a id="1109" class="Symbol">→</a> <a id="1111" href="group-theory.groups.html#2711" class="Function">type-Group</a> <a id="1122" href="graph-theory.voltage-graphs.html#702" class="Bound">Π</a>
  <a id="1126" href="graph-theory.voltage-graphs.html#1027" class="Function">voltage-Voltage-Graph</a> <a id="1148" class="Symbol">=</a> <a id="1150" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="1154" href="graph-theory.voltage-graphs.html#717" class="Bound">G</a>
</pre>