# Nontrivial rings

<pre class="Agda"><a id="29" class="Symbol">{-#</a> <a id="33" class="Keyword">OPTIONS</a> <a id="41" class="Pragma">--without-K</a> <a id="53" class="Pragma">--exact-split</a> <a id="67" class="Symbol">#-}</a>

<a id="72" class="Keyword">module</a> <a id="79" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a> <a id="108" class="Keyword">where</a>

<a id="115" class="Keyword">open</a> <a id="120" class="Keyword">import</a> <a id="127" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="153" class="Keyword">using</a> <a id="159" class="Symbol">(</a><a id="160" href="foundation-core.identity-types.html#641" class="Datatype">Id</a><a id="162" class="Symbol">)</a>
<a id="164" class="Keyword">open</a> <a id="169" class="Keyword">import</a> <a id="176" href="foundation.negation.html" class="Module">foundation.negation</a> <a id="196" class="Keyword">using</a> <a id="202" class="Symbol">(</a><a id="203" href="foundation-core.negation.html#452" class="Function">¬</a><a id="204" class="Symbol">)</a>
<a id="206" class="Keyword">open</a> <a id="211" class="Keyword">import</a> <a id="218" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="245" class="Keyword">using</a> <a id="251" class="Symbol">(</a><a id="252" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="257" class="Symbol">;</a> <a id="259" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="261" class="Symbol">)</a>

<a id="264" class="Keyword">open</a> <a id="269" class="Keyword">import</a> <a id="276" href="ring-theory.rings.html" class="Module">ring-theory.rings</a> <a id="294" class="Keyword">using</a> <a id="300" class="Symbol">(</a><a id="301" href="ring-theory.rings.html#1734" class="Function">Ring</a><a id="305" class="Symbol">;</a> <a id="307" href="ring-theory.rings.html#3110" class="Function">zero-Ring</a><a id="316" class="Symbol">;</a> <a id="318" href="ring-theory.rings.html#5263" class="Function">unit-Ring</a><a id="327" class="Symbol">)</a>
</pre>
## Idea

Nontrivial rings are rings in which `0 ≠ 1`.

## Definition

<pre class="Agda"><a id="is-nontrivial-Ring"></a><a id="412" href="ring-theory.nontrivial-rings.html#412" class="Function">is-nontrivial-Ring</a> <a id="431" class="Symbol">:</a>
  <a id="435" class="Symbol">{</a> <a id="437" href="ring-theory.nontrivial-rings.html#437" class="Bound">l</a> <a id="439" class="Symbol">:</a> <a id="441" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="446" class="Symbol">}</a> <a id="448" class="Symbol">→</a> <a id="450" href="ring-theory.rings.html#1734" class="Function">Ring</a> <a id="455" href="ring-theory.nontrivial-rings.html#437" class="Bound">l</a> <a id="457" class="Symbol">→</a> <a id="459" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="462" href="ring-theory.nontrivial-rings.html#437" class="Bound">l</a>
<a id="464" href="ring-theory.nontrivial-rings.html#412" class="Function">is-nontrivial-Ring</a> <a id="483" href="ring-theory.nontrivial-rings.html#483" class="Bound">R</a> <a id="485" class="Symbol">=</a> <a id="487" href="foundation-core.negation.html#452" class="Function">¬</a> <a id="489" class="Symbol">(</a><a id="490" href="foundation-core.identity-types.html#641" class="Datatype">Id</a> <a id="493" class="Symbol">(</a><a id="494" href="ring-theory.rings.html#3110" class="Function">zero-Ring</a> <a id="504" href="ring-theory.nontrivial-rings.html#483" class="Bound">R</a><a id="505" class="Symbol">)</a> <a id="507" class="Symbol">(</a><a id="508" href="ring-theory.rings.html#5263" class="Function">unit-Ring</a> <a id="518" href="ring-theory.nontrivial-rings.html#483" class="Bound">R</a><a id="519" class="Symbol">))</a>
</pre>