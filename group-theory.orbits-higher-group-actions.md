---
title: Orbits of higher group actions
---

<pre class="Agda"><a id="56" class="Symbol">{-#</a> <a id="60" class="Keyword">OPTIONS</a> <a id="68" class="Pragma">--without-K</a> <a id="80" class="Pragma">--exact-split</a> <a id="94" class="Symbol">#-}</a>

<a id="99" class="Keyword">module</a> <a id="106" href="group-theory.orbits-higher-group-actions.html" class="Module">group-theory.orbits-higher-group-actions</a> <a id="147" class="Keyword">where</a>

<a id="154" class="Keyword">open</a> <a id="159" class="Keyword">import</a> <a id="166" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="198" class="Keyword">open</a> <a id="203" class="Keyword">import</a> <a id="210" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="238" class="Keyword">open</a> <a id="243" class="Keyword">import</a> <a id="250" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="284" class="Keyword">open</a> <a id="289" class="Keyword">import</a> <a id="296" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
</pre>
## Idea

The type of orbits of a higher group action `X` acted upon by `G` is the total space of `X`.

## Definition

<pre class="Agda"><a id="orbit-action-∞-Group"></a><a id="454" href="group-theory.orbits-higher-group-actions.html#454" class="Function">orbit-action-∞-Group</a> <a id="475" class="Symbol">:</a>
  <a id="479" class="Symbol">{</a><a id="480" href="group-theory.orbits-higher-group-actions.html#480" class="Bound">l1</a> <a id="483" href="group-theory.orbits-higher-group-actions.html#483" class="Bound">l2</a> <a id="486" class="Symbol">:</a> <a id="488" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="493" class="Symbol">}</a> <a id="495" class="Symbol">(</a><a id="496" href="group-theory.orbits-higher-group-actions.html#496" class="Bound">G</a> <a id="498" class="Symbol">:</a> <a id="500" href="group-theory.higher-groups.html#1626" class="Function">∞-Group</a> <a id="508" href="group-theory.orbits-higher-group-actions.html#480" class="Bound">l1</a><a id="510" class="Symbol">)</a> <a id="512" class="Symbol">(</a><a id="513" href="group-theory.orbits-higher-group-actions.html#513" class="Bound">X</a> <a id="515" class="Symbol">:</a> <a id="517" href="group-theory.higher-group-actions.html#367" class="Function">action-∞-Group</a> <a id="532" href="group-theory.orbits-higher-group-actions.html#483" class="Bound">l2</a> <a id="535" href="group-theory.orbits-higher-group-actions.html#496" class="Bound">G</a><a id="536" class="Symbol">)</a> <a id="538" class="Symbol">→</a> <a id="540" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="543" class="Symbol">(</a><a id="544" href="group-theory.orbits-higher-group-actions.html#480" class="Bound">l1</a> <a id="547" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="549" href="group-theory.orbits-higher-group-actions.html#483" class="Bound">l2</a><a id="551" class="Symbol">)</a>
<a id="553" href="group-theory.orbits-higher-group-actions.html#454" class="Function">orbit-action-∞-Group</a> <a id="574" href="group-theory.orbits-higher-group-actions.html#574" class="Bound">G</a> <a id="576" href="group-theory.orbits-higher-group-actions.html#576" class="Bound">X</a> <a id="578" class="Symbol">=</a> <a id="580" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="582" class="Symbol">(</a><a id="583" href="group-theory.higher-groups.html#1885" class="Function">classifying-type-∞-Group</a> <a id="608" href="group-theory.orbits-higher-group-actions.html#574" class="Bound">G</a><a id="609" class="Symbol">)</a> <a id="611" href="group-theory.orbits-higher-group-actions.html#576" class="Bound">X</a>
</pre>