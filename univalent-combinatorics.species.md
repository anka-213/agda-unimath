# Species

<pre class="Agda"><a id="20" class="Symbol">{-#</a> <a id="24" class="Keyword">OPTIONS</a> <a id="32" class="Pragma">--without-K</a> <a id="44" class="Pragma">--exact-split</a> <a id="58" class="Symbol">#-}</a>

<a id="63" class="Keyword">module</a> <a id="70" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a> <a id="102" class="Keyword">where</a>

<a id="109" class="Keyword">open</a> <a id="114" class="Keyword">import</a> <a id="121" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="148" class="Keyword">using</a> <a id="154" class="Symbol">(</a><a id="155" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="160" class="Symbol">;</a> <a id="162" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="164" class="Symbol">;</a> <a id="166" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="170" class="Symbol">)</a>

<a id="173" class="Keyword">open</a> <a id="178" class="Keyword">import</a> <a id="185" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a> <a id="222" class="Keyword">using</a> <a id="228" class="Symbol">(</a><a id="229" href="univalent-combinatorics.finite-types.html#4042" class="Function">𝔽</a><a id="230" class="Symbol">)</a>
</pre>
## Definition

<pre class="Agda"><a id="species"></a><a id="260" href="univalent-combinatorics.species.html#260" class="Function">species</a> <a id="268" class="Symbol">:</a> <a id="270" class="Symbol">(</a><a id="271" href="univalent-combinatorics.species.html#271" class="Bound">l</a> <a id="273" class="Symbol">:</a> <a id="275" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="280" class="Symbol">)</a> <a id="282" class="Symbol">→</a> <a id="284" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="287" class="Symbol">(</a><a id="288" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="293" href="univalent-combinatorics.species.html#271" class="Bound">l</a><a id="294" class="Symbol">)</a>
<a id="296" href="univalent-combinatorics.species.html#260" class="Function">species</a> <a id="304" href="univalent-combinatorics.species.html#304" class="Bound">l</a> <a id="306" class="Symbol">=</a> <a id="308" href="univalent-combinatorics.finite-types.html#4042" class="Function">𝔽</a> <a id="310" class="Symbol">→</a> <a id="312" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="315" href="univalent-combinatorics.species.html#304" class="Bound">l</a>
</pre>