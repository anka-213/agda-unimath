---
title: Species
---

<pre class="Agda"><a id="33" class="Symbol">{-#</a> <a id="37" class="Keyword">OPTIONS</a> <a id="45" class="Pragma">--without-K</a> <a id="57" class="Pragma">--exact-split</a> <a id="71" class="Symbol">#-}</a>

<a id="76" class="Keyword">module</a> <a id="83" href="univalent-combinatorics.species.html" class="Module">univalent-combinatorics.species</a> <a id="115" class="Keyword">where</a>

<a id="122" class="Keyword">open</a> <a id="127" class="Keyword">import</a> <a id="134" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="158" class="Keyword">open</a> <a id="163" class="Keyword">import</a> <a id="170" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="196" class="Keyword">open</a> <a id="201" class="Keyword">import</a> <a id="208" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="236" class="Keyword">open</a> <a id="241" class="Keyword">import</a> <a id="248" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
</pre>
### Idea

In this file, we define the type of species. A species is just a
map from 𝔽 to a universe.

## Definitions

### Species

<pre class="Agda"><a id="species"></a><a id="429" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="437" class="Symbol">:</a> <a id="439" class="Symbol">(</a><a id="440" href="univalent-combinatorics.species.html#440" class="Bound">l</a> <a id="442" class="Symbol">:</a> <a id="444" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="449" class="Symbol">)</a> <a id="451" class="Symbol">→</a> <a id="453" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="456" class="Symbol">(</a><a id="457" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="462" href="univalent-combinatorics.species.html#440" class="Bound">l</a><a id="463" class="Symbol">)</a>
<a id="465" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="473" href="univalent-combinatorics.species.html#473" class="Bound">l</a> <a id="475" class="Symbol">=</a> <a id="477" href="univalent-combinatorics.finite-types.html#4639" class="Function">𝔽</a> <a id="479" class="Symbol">→</a> <a id="481" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="484" href="univalent-combinatorics.species.html#473" class="Bound">l</a>
</pre>
### Transport in species

<pre class="Agda"><a id="tr-species"></a><a id="525" href="univalent-combinatorics.species.html#525" class="Function">tr-species</a> <a id="536" class="Symbol">:</a>
  <a id="540" class="Symbol">{</a><a id="541" href="univalent-combinatorics.species.html#541" class="Bound">l</a> <a id="543" class="Symbol">:</a> <a id="545" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="550" class="Symbol">}</a> <a id="552" class="Symbol">(</a><a id="553" href="univalent-combinatorics.species.html#553" class="Bound">F</a> <a id="555" class="Symbol">:</a> <a id="557" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="565" href="univalent-combinatorics.species.html#541" class="Bound">l</a><a id="566" class="Symbol">)</a> <a id="568" class="Symbol">(</a><a id="569" href="univalent-combinatorics.species.html#569" class="Bound">X</a> <a id="571" href="univalent-combinatorics.species.html#571" class="Bound">Y</a> <a id="573" class="Symbol">:</a> <a id="575" href="univalent-combinatorics.finite-types.html#4639" class="Function">𝔽</a><a id="576" class="Symbol">)</a> <a id="578" class="Symbol">→</a> <a id="580" href="univalent-combinatorics.finite-types.html#4687" class="Function">type-𝔽</a> <a id="587" href="univalent-combinatorics.species.html#569" class="Bound">X</a> <a id="589" href="foundation-core.equivalences.html#1607" class="Function Operator">≃</a> <a id="591" href="univalent-combinatorics.finite-types.html#4687" class="Function">type-𝔽</a> <a id="598" href="univalent-combinatorics.species.html#571" class="Bound">Y</a> <a id="600" class="Symbol">→</a> <a id="602" href="univalent-combinatorics.species.html#553" class="Bound">F</a> <a id="604" href="univalent-combinatorics.species.html#569" class="Bound">X</a> <a id="606" class="Symbol">→</a> <a id="608" href="univalent-combinatorics.species.html#553" class="Bound">F</a> <a id="610" href="univalent-combinatorics.species.html#571" class="Bound">Y</a>
<a id="612" href="univalent-combinatorics.species.html#525" class="Function">tr-species</a> <a id="623" href="univalent-combinatorics.species.html#623" class="Bound">F</a> <a id="625" href="univalent-combinatorics.species.html#625" class="Bound">X</a> <a id="627" href="univalent-combinatorics.species.html#627" class="Bound">Y</a> <a id="629" href="univalent-combinatorics.species.html#629" class="Bound">e</a> <a id="631" class="Symbol">=</a> <a id="633" href="foundation-core.identity-types.html#5689" class="Function">tr</a> <a id="636" href="univalent-combinatorics.species.html#623" class="Bound">F</a> <a id="638" class="Symbol">(</a><a id="639" href="univalent-combinatorics.finite-types.html#19315" class="Function">eq-equiv-𝔽</a> <a id="650" href="univalent-combinatorics.species.html#625" class="Bound">X</a> <a id="652" href="univalent-combinatorics.species.html#627" class="Bound">Y</a> <a id="654" href="univalent-combinatorics.species.html#629" class="Bound">e</a><a id="655" class="Symbol">)</a>
</pre>