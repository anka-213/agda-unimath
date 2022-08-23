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

<pre class="Agda"><a id="species"></a><a id="429" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="437" class="Symbol">:</a> <a id="439" class="Symbol">(</a><a id="440" href="univalent-combinatorics.species.html#440" class="Bound">l1</a> <a id="443" href="univalent-combinatorics.species.html#443" class="Bound">l2</a> <a id="446" class="Symbol">:</a> <a id="448" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="453" class="Symbol">)</a> <a id="455" class="Symbol">→</a> <a id="457" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="460" class="Symbol">(</a><a id="461" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="466" href="univalent-combinatorics.species.html#440" class="Bound">l1</a> <a id="469" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="471" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="476" href="univalent-combinatorics.species.html#443" class="Bound">l2</a><a id="478" class="Symbol">)</a>
<a id="480" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="488" href="univalent-combinatorics.species.html#488" class="Bound">l1</a> <a id="491" href="univalent-combinatorics.species.html#491" class="Bound">l2</a> <a id="494" class="Symbol">=</a> <a id="496" href="univalent-combinatorics.finite-types.html#4550" class="Function">𝔽</a> <a id="498" href="univalent-combinatorics.species.html#488" class="Bound">l1</a> <a id="501" class="Symbol">→</a> <a id="503" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="506" href="univalent-combinatorics.species.html#491" class="Bound">l2</a>
</pre>
### Transport in species

<pre class="Agda"><a id="tr-species"></a><a id="548" href="univalent-combinatorics.species.html#548" class="Function">tr-species</a> <a id="559" class="Symbol">:</a>
  <a id="563" class="Symbol">{</a><a id="564" href="univalent-combinatorics.species.html#564" class="Bound">l1</a> <a id="567" href="univalent-combinatorics.species.html#567" class="Bound">l2</a> <a id="570" class="Symbol">:</a> <a id="572" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="577" class="Symbol">}</a> <a id="579" class="Symbol">(</a><a id="580" href="univalent-combinatorics.species.html#580" class="Bound">F</a> <a id="582" class="Symbol">:</a> <a id="584" href="univalent-combinatorics.species.html#429" class="Function">species</a> <a id="592" href="univalent-combinatorics.species.html#564" class="Bound">l1</a> <a id="595" href="univalent-combinatorics.species.html#567" class="Bound">l2</a><a id="597" class="Symbol">)</a> <a id="599" class="Symbol">(</a><a id="600" href="univalent-combinatorics.species.html#600" class="Bound">X</a> <a id="602" href="univalent-combinatorics.species.html#602" class="Bound">Y</a> <a id="604" class="Symbol">:</a> <a id="606" href="univalent-combinatorics.finite-types.html#4550" class="Function">𝔽</a> <a id="608" href="univalent-combinatorics.species.html#564" class="Bound">l1</a><a id="610" class="Symbol">)</a> <a id="612" class="Symbol">→</a>
  <a id="616" href="univalent-combinatorics.finite-types.html#4606" class="Function">type-𝔽</a> <a id="623" href="univalent-combinatorics.species.html#600" class="Bound">X</a> <a id="625" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="627" href="univalent-combinatorics.finite-types.html#4606" class="Function">type-𝔽</a> <a id="634" href="univalent-combinatorics.species.html#602" class="Bound">Y</a> <a id="636" class="Symbol">→</a> <a id="638" href="univalent-combinatorics.species.html#580" class="Bound">F</a> <a id="640" href="univalent-combinatorics.species.html#600" class="Bound">X</a> <a id="642" class="Symbol">→</a> <a id="644" href="univalent-combinatorics.species.html#580" class="Bound">F</a> <a id="646" href="univalent-combinatorics.species.html#602" class="Bound">Y</a>
<a id="648" href="univalent-combinatorics.species.html#548" class="Function">tr-species</a> <a id="659" href="univalent-combinatorics.species.html#659" class="Bound">F</a> <a id="661" href="univalent-combinatorics.species.html#661" class="Bound">X</a> <a id="663" href="univalent-combinatorics.species.html#663" class="Bound">Y</a> <a id="665" href="univalent-combinatorics.species.html#665" class="Bound">e</a> <a id="667" class="Symbol">=</a> <a id="669" href="foundation-core.identity-types.html#5702" class="Function">tr</a> <a id="672" href="univalent-combinatorics.species.html#659" class="Bound">F</a> <a id="674" class="Symbol">(</a><a id="675" href="univalent-combinatorics.finite-types.html#18735" class="Function">eq-equiv-𝔽</a> <a id="686" href="univalent-combinatorics.species.html#661" class="Bound">X</a> <a id="688" href="univalent-combinatorics.species.html#663" class="Bound">Y</a> <a id="690" href="univalent-combinatorics.species.html#665" class="Bound">e</a><a id="691" class="Symbol">)</a>
</pre>