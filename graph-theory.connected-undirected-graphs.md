# Connected graphs

<pre class="Agda"><a id="29" class="Symbol">{-#</a> <a id="33" class="Keyword">OPTIONS</a> <a id="41" class="Pragma">--without-K</a> <a id="53" class="Pragma">--exact-split</a> <a id="67" class="Symbol">#-}</a>

<a id="72" class="Keyword">module</a> <a id="79" href="graph-theory.connected-undirected-graphs.html" class="Module">graph-theory.connected-undirected-graphs</a> <a id="120" class="Keyword">where</a>

<a id="127" class="Keyword">open</a> <a id="132" class="Keyword">import</a> <a id="139" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a> <a id="176" class="Keyword">using</a> <a id="182" class="Symbol">(</a><a id="183" href="foundation.propositional-truncations.html#2209" class="Function">type-trunc-Prop</a><a id="198" class="Symbol">;</a> <a id="200" href="foundation.propositional-truncations.html#2388" class="Function">is-prop-type-trunc-Prop</a><a id="223" class="Symbol">)</a>
<a id="225" class="Keyword">open</a> <a id="230" class="Keyword">import</a> <a id="237" href="foundation.propositions.html" class="Module">foundation.propositions</a> <a id="261" class="Keyword">using</a>
  <a id="269" class="Symbol">(</a> <a id="271" href="foundation-core.propositions.html#1309" class="Function">is-prop</a><a id="278" class="Symbol">;</a> <a id="280" href="foundation-core.propositions.html#6158" class="Function">is-prop-Π</a> <a id="290" class="Symbol">)</a>
<a id="292" class="Keyword">open</a> <a id="297" class="Keyword">import</a> <a id="304" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="331" class="Keyword">using</a> <a id="337" class="Symbol">(</a><a id="338" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="343" class="Symbol">;</a> <a id="345" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a><a id="347" class="Symbol">;</a> <a id="349" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="352" class="Symbol">;</a> <a id="354" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="358" class="Symbol">;</a> <a id="360" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="365" class="Symbol">)</a>

<a id="368" class="Keyword">open</a> <a id="373" class="Keyword">import</a> <a id="380" href="graph-theory.undirected-graphs.html" class="Module">graph-theory.undirected-graphs</a> <a id="411" class="Keyword">using</a>
  <a id="419" class="Symbol">(</a> <a id="421" href="graph-theory.undirected-graphs.html#1060" class="Function">Undirected-Graph</a><a id="437" class="Symbol">;</a> <a id="439" href="graph-theory.undirected-graphs.html#1256" class="Function">vertex-Undirected-Graph</a><a id="462" class="Symbol">)</a>
<a id="464" class="Keyword">open</a> <a id="469" class="Keyword">import</a> <a id="476" href="graph-theory.walks-undirected-graphs.html" class="Module">graph-theory.walks-undirected-graphs</a> <a id="513" class="Keyword">using</a>
  <a id="521" class="Symbol">(</a> <a id="523" href="graph-theory.walks-undirected-graphs.html#1356" class="Datatype">walk-Undirected-Graph</a><a id="544" class="Symbol">)</a>
</pre>
## Idea

A graph is said to be connected if any point can be reached from any point by a walk.

## Definition

<pre class="Agda"><a id="670" class="Keyword">module</a> <a id="677" href="graph-theory.connected-undirected-graphs.html#677" class="Module">_</a>
  <a id="681" class="Symbol">{</a><a id="682" href="graph-theory.connected-undirected-graphs.html#682" class="Bound">l1</a> <a id="685" href="graph-theory.connected-undirected-graphs.html#685" class="Bound">l2</a> <a id="688" class="Symbol">:</a> <a id="690" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="695" class="Symbol">}</a> <a id="697" class="Symbol">(</a><a id="698" href="graph-theory.connected-undirected-graphs.html#698" class="Bound">G</a> <a id="700" class="Symbol">:</a> <a id="702" href="graph-theory.undirected-graphs.html#1060" class="Function">Undirected-Graph</a> <a id="719" href="graph-theory.connected-undirected-graphs.html#682" class="Bound">l1</a> <a id="722" href="graph-theory.connected-undirected-graphs.html#685" class="Bound">l2</a><a id="724" class="Symbol">)</a>
  <a id="728" class="Keyword">where</a>

  <a id="737" href="graph-theory.connected-undirected-graphs.html#737" class="Function">is-connected-Undirected-Graph</a> <a id="767" class="Symbol">:</a> <a id="769" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="772" class="Symbol">(</a><a id="773" href="graph-theory.connected-undirected-graphs.html#682" class="Bound">l1</a> <a id="776" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="778" href="graph-theory.connected-undirected-graphs.html#685" class="Bound">l2</a> <a id="781" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="783" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="788" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="793" class="Symbol">)</a>
  <a id="797" href="graph-theory.connected-undirected-graphs.html#737" class="Function">is-connected-Undirected-Graph</a> <a id="827" class="Symbol">=</a>
    <a id="833" class="Symbol">(</a><a id="834" href="graph-theory.connected-undirected-graphs.html#834" class="Bound">x</a> <a id="836" href="graph-theory.connected-undirected-graphs.html#836" class="Bound">y</a> <a id="838" class="Symbol">:</a> <a id="840" href="graph-theory.undirected-graphs.html#1256" class="Function">vertex-Undirected-Graph</a> <a id="864" href="graph-theory.connected-undirected-graphs.html#698" class="Bound">G</a><a id="865" class="Symbol">)</a> <a id="867" class="Symbol">→</a>
    <a id="873" href="foundation.propositional-truncations.html#2209" class="Function">type-trunc-Prop</a> <a id="889" class="Symbol">(</a><a id="890" href="graph-theory.walks-undirected-graphs.html#1356" class="Datatype">walk-Undirected-Graph</a> <a id="912" href="graph-theory.connected-undirected-graphs.html#698" class="Bound">G</a> <a id="914" href="graph-theory.connected-undirected-graphs.html#834" class="Bound">x</a> <a id="916" href="graph-theory.connected-undirected-graphs.html#836" class="Bound">y</a><a id="917" class="Symbol">)</a>
</pre>
## Properties

### The property of being connected for an undirected graph is a proposition

<pre class="Agda">  <a id="1027" href="graph-theory.connected-undirected-graphs.html#1027" class="Function">is-prop-is-connected-Undirected-Graph</a>
    <a id="1069" class="Symbol">:</a> <a id="1071" href="foundation-core.propositions.html#1309" class="Function">is-prop</a> <a id="1079" href="graph-theory.connected-undirected-graphs.html#737" class="Function">is-connected-Undirected-Graph</a>
  <a id="1111" href="graph-theory.connected-undirected-graphs.html#1027" class="Function">is-prop-is-connected-Undirected-Graph</a> <a id="1149" class="Symbol">=</a>
     <a id="1156" href="foundation-core.propositions.html#6158" class="Function">is-prop-Π</a> <a id="1166" class="Symbol">(λ</a> <a id="1169" href="graph-theory.connected-undirected-graphs.html#1169" class="Bound">_</a> <a id="1171" class="Symbol">→</a> <a id="1173" href="foundation-core.propositions.html#6158" class="Function">is-prop-Π</a> <a id="1183" class="Symbol">(λ</a> <a id="1186" href="graph-theory.connected-undirected-graphs.html#1186" class="Bound">_</a> <a id="1188" class="Symbol">→</a> <a id="1190" href="foundation.propositional-truncations.html#2388" class="Function">is-prop-type-trunc-Prop</a><a id="1213" class="Symbol">))</a>
</pre>