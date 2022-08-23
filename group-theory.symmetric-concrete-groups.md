---
title: Symmetric concrete groups
---

<pre class="Agda"><a id="51" class="Keyword">module</a> <a id="58" href="group-theory.symmetric-concrete-groups.html" class="Module">group-theory.symmetric-concrete-groups</a> <a id="97" class="Keyword">where</a>

<a id="104" class="Keyword">open</a> <a id="109" class="Keyword">import</a> <a id="116" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="132" class="Keyword">open</a> <a id="137" class="Keyword">import</a> <a id="144" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="172" class="Keyword">open</a> <a id="177" class="Keyword">import</a> <a id="184" href="group-theory.automorphism-groups.html" class="Module">group-theory.automorphism-groups</a>
<a id="217" class="Keyword">open</a> <a id="222" class="Keyword">import</a> <a id="229" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
</pre>
## Idea

The symmetric concrete group of a set `X` is the connected component of the universe of sets at `X`.

## Definition

<pre class="Agda"><a id="397" class="Keyword">module</a> <a id="404" href="group-theory.symmetric-concrete-groups.html#404" class="Module">_</a>
  <a id="408" class="Symbol">{</a><a id="409" href="group-theory.symmetric-concrete-groups.html#409" class="Bound">l</a> <a id="411" class="Symbol">:</a> <a id="413" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="418" class="Symbol">}</a> <a id="420" class="Symbol">(</a><a id="421" href="group-theory.symmetric-concrete-groups.html#421" class="Bound">X</a> <a id="423" class="Symbol">:</a> <a id="425" href="foundation-core.sets.html#1190" class="Function">UU-Set</a> <a id="432" href="group-theory.symmetric-concrete-groups.html#409" class="Bound">l</a><a id="433" class="Symbol">)</a>
  <a id="437" class="Keyword">where</a>

  <a id="446" href="group-theory.symmetric-concrete-groups.html#446" class="Function">symmetric-Concrete-Group</a> <a id="471" class="Symbol">:</a> <a id="473" href="group-theory.concrete-groups.html#2030" class="Function">Concrete-Group</a> <a id="488" class="Symbol">(</a><a id="489" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="494" href="group-theory.symmetric-concrete-groups.html#409" class="Bound">l</a><a id="495" class="Symbol">)</a>
  <a id="499" href="group-theory.symmetric-concrete-groups.html#446" class="Function">symmetric-Concrete-Group</a> <a id="524" class="Symbol">=</a> <a id="526" href="group-theory.automorphism-groups.html#1165" class="Function">Automorphism-Group</a> <a id="545" class="Symbol">(</a><a id="546" href="foundation-core.sets.html#1190" class="Function">UU-Set</a> <a id="553" href="group-theory.symmetric-concrete-groups.html#409" class="Bound">l</a><a id="554" class="Symbol">)</a> <a id="556" href="group-theory.symmetric-concrete-groups.html#421" class="Bound">X</a> <a id="558" href="foundation.sets.html#1357" class="Function">is-1-type-UU-Set</a>
</pre>