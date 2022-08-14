---
title: Eulerian circuits in undirected graphs
---

<pre class="Agda"><a id="64" class="Symbol">{-#</a> <a id="68" class="Keyword">OPTIONS</a> <a id="76" class="Pragma">--without-K</a> <a id="88" class="Pragma">--exact-split</a> <a id="102" class="Symbol">#-}</a>

<a id="107" class="Keyword">module</a> <a id="114" href="graph-theory.eulerian-circuits-undirected-graphs.html" class="Module">graph-theory.eulerian-circuits-undirected-graphs</a> <a id="163" class="Keyword">where</a>

<a id="170" class="Keyword">open</a> <a id="175" class="Keyword">import</a> <a id="182" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="224" class="Keyword">open</a> <a id="229" class="Keyword">import</a> <a id="236" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="268" class="Keyword">open</a> <a id="273" class="Keyword">import</a> <a id="280" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="304" class="Keyword">open</a> <a id="309" class="Keyword">import</a> <a id="316" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="362" class="Keyword">open</a> <a id="367" class="Keyword">import</a> <a id="374" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="402" class="Keyword">open</a> <a id="407" class="Keyword">import</a> <a id="414" href="graph-theory.morphisms-undirected-graphs.html" class="Module">graph-theory.morphisms-undirected-graphs</a>
<a id="455" class="Keyword">open</a> <a id="460" class="Keyword">import</a> <a id="467" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>
<a id="489" class="Keyword">open</a> <a id="494" class="Keyword">import</a> <a id="501" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a>
</pre>
## Idea

An Eulerian cicuit in an undirected graph `G` consists of a cicuit `T` in `G` such that every edge in `G` is in the image of `T`. In other words, an Eulerian circuit `T` consists of `k`-gon `H` equipped with a graph homomorphism `f : H → G` that induces an equivalence

```md
  Σ (unordered-pair-vertices-Polygon k H) (edge-Polygon k H) ≃
  Σ (unordered-pair-vertices-Undirected-Graph G) (edge-Undirected-Graph G)
```

## Definition

<pre class="Agda"><a id="988" class="Keyword">module</a> <a id="995" href="graph-theory.eulerian-circuits-undirected-graphs.html#995" class="Module">_</a>
  <a id="999" class="Symbol">{</a><a id="1000" href="graph-theory.eulerian-circuits-undirected-graphs.html#1000" class="Bound">l1</a> <a id="1003" href="graph-theory.eulerian-circuits-undirected-graphs.html#1003" class="Bound">l2</a> <a id="1006" class="Symbol">:</a> <a id="1008" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1013" class="Symbol">}</a> <a id="1015" class="Symbol">(</a><a id="1016" href="graph-theory.eulerian-circuits-undirected-graphs.html#1016" class="Bound">G</a> <a id="1018" class="Symbol">:</a> <a id="1020" href="graph-theory.undirected-graphs.html#1060" class="Function">Undirected-Graph</a> <a id="1037" href="graph-theory.eulerian-circuits-undirected-graphs.html#1000" class="Bound">l1</a> <a id="1040" href="graph-theory.eulerian-circuits-undirected-graphs.html#1003" class="Bound">l2</a><a id="1042" class="Symbol">)</a>
  <a id="1046" class="Keyword">where</a>

  <a id="1055" href="graph-theory.eulerian-circuits-undirected-graphs.html#1055" class="Function">eulerian-circuit-Undirected-Graph</a> <a id="1089" class="Symbol">:</a> <a id="1091" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1094" class="Symbol">(</a><a id="1095" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1100" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="1106" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1108" href="graph-theory.eulerian-circuits-undirected-graphs.html#1000" class="Bound">l1</a> <a id="1111" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1113" href="graph-theory.eulerian-circuits-undirected-graphs.html#1003" class="Bound">l2</a><a id="1115" class="Symbol">)</a>
  <a id="1119" href="graph-theory.eulerian-circuits-undirected-graphs.html#1055" class="Function">eulerian-circuit-Undirected-Graph</a> <a id="1153" class="Symbol">=</a>
    <a id="1159" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1161" class="Symbol">(</a> <a id="1163" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="1164" class="Symbol">)</a>
      <a id="1172" class="Symbol">(</a> <a id="1174" class="Symbol">λ</a> <a id="1176" href="graph-theory.eulerian-circuits-undirected-graphs.html#1176" class="Bound">k</a> <a id="1178" class="Symbol">→</a>
        <a id="1188" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1190" class="Symbol">(</a> <a id="1192" href="graph-theory.polygons.html#2934" class="Function">Polygon</a> <a id="1200" href="graph-theory.eulerian-circuits-undirected-graphs.html#1176" class="Bound">k</a><a id="1201" class="Symbol">)</a>
          <a id="1213" class="Symbol">(</a> <a id="1215" class="Symbol">λ</a> <a id="1217" href="graph-theory.eulerian-circuits-undirected-graphs.html#1217" class="Bound">H</a> <a id="1219" class="Symbol">→</a>
            <a id="1233" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1235" class="Symbol">(</a> <a id="1237" href="graph-theory.morphisms-undirected-graphs.html#1538" class="Function">hom-Undirected-Graph</a> <a id="1258" class="Symbol">(</a><a id="1259" href="graph-theory.polygons.html#3134" class="Function">undirected-graph-Polygon</a> <a id="1284" href="graph-theory.eulerian-circuits-undirected-graphs.html#1176" class="Bound">k</a> <a id="1286" href="graph-theory.eulerian-circuits-undirected-graphs.html#1217" class="Bound">H</a><a id="1287" class="Symbol">)</a> <a id="1289" href="graph-theory.eulerian-circuits-undirected-graphs.html#1016" class="Bound">G</a><a id="1290" class="Symbol">)</a>
              <a id="1306" class="Symbol">(</a> <a id="1308" class="Symbol">λ</a> <a id="1310" href="graph-theory.eulerian-circuits-undirected-graphs.html#1310" class="Bound">f</a> <a id="1312" class="Symbol">→</a>
                <a id="1330" href="foundation-core.equivalences.html#1556" class="Function">is-equiv</a>
                  <a id="1357" class="Symbol">(</a> <a id="1359" href="foundation-core.functoriality-dependent-pair-types.html#1913" class="Function">tot</a>
                    <a id="1383" class="Symbol">(</a> <a id="1385" href="graph-theory.morphisms-undirected-graphs.html#2289" class="Function">edge-hom-Undirected-Graph</a>
                      <a id="1433" class="Symbol">(</a> <a id="1435" href="graph-theory.polygons.html#3134" class="Function">undirected-graph-Polygon</a> <a id="1460" href="graph-theory.eulerian-circuits-undirected-graphs.html#1176" class="Bound">k</a> <a id="1462" href="graph-theory.eulerian-circuits-undirected-graphs.html#1217" class="Bound">H</a><a id="1463" class="Symbol">)</a>
                      <a id="1487" class="Symbol">(</a> <a id="1489" href="graph-theory.eulerian-circuits-undirected-graphs.html#1016" class="Bound">G</a><a id="1490" class="Symbol">)</a>
                      <a id="1514" class="Symbol">(</a> <a id="1516" href="graph-theory.eulerian-circuits-undirected-graphs.html#1310" class="Bound">f</a><a id="1517" class="Symbol">))))))</a>
</pre>