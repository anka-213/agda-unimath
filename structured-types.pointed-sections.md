---
title: Pointed sections of pointed maps
---

<pre class="Agda"><a id="58" class="Keyword">module</a> <a id="65" href="structured-types.pointed-sections.html" class="Module">structured-types.pointed-sections</a> <a id="99" class="Keyword">where</a>

<a id="106" class="Keyword">open</a> <a id="111" class="Keyword">import</a> <a id="118" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="150" class="Keyword">open</a> <a id="155" class="Keyword">import</a> <a id="162" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="190" class="Keyword">open</a> <a id="195" class="Keyword">import</a> <a id="202" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a>
<a id="238" class="Keyword">open</a> <a id="243" class="Keyword">import</a> <a id="250" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a>
<a id="280" class="Keyword">open</a> <a id="285" class="Keyword">import</a> <a id="292" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
</pre>
## Idea

A **pointed section** of a pointed map `f : A →* B` consists of a pointed map `g : B →* A` equipped with a pointed homotopy `H : (f ∘* g) ~* id`.

<pre class="Agda"><a id="pointed-section-Pointed-Type"></a><a id="492" href="structured-types.pointed-sections.html#492" class="Function">pointed-section-Pointed-Type</a> <a id="521" class="Symbol">:</a>
  <a id="525" class="Symbol">{</a><a id="526" href="structured-types.pointed-sections.html#526" class="Bound">l1</a> <a id="529" href="structured-types.pointed-sections.html#529" class="Bound">l2</a> <a id="532" class="Symbol">:</a> <a id="534" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="539" class="Symbol">}</a> <a id="541" class="Symbol">(</a><a id="542" href="structured-types.pointed-sections.html#542" class="Bound">A</a> <a id="544" class="Symbol">:</a> <a id="546" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="559" href="structured-types.pointed-sections.html#526" class="Bound">l1</a><a id="561" class="Symbol">)</a> <a id="563" class="Symbol">(</a><a id="564" href="structured-types.pointed-sections.html#564" class="Bound">B</a> <a id="566" class="Symbol">:</a> <a id="568" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="581" href="structured-types.pointed-sections.html#529" class="Bound">l2</a><a id="583" class="Symbol">)</a> <a id="585" class="Symbol">→</a>
  <a id="589" class="Symbol">(</a><a id="590" href="structured-types.pointed-sections.html#542" class="Bound">A</a> <a id="592" href="structured-types.pointed-maps.html#1015" class="Function Operator">→*</a> <a id="595" href="structured-types.pointed-sections.html#564" class="Bound">B</a><a id="596" class="Symbol">)</a> <a id="598" class="Symbol">→</a> <a id="600" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="603" class="Symbol">(</a><a id="604" href="structured-types.pointed-sections.html#526" class="Bound">l1</a> <a id="607" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="609" href="structured-types.pointed-sections.html#529" class="Bound">l2</a><a id="611" class="Symbol">)</a>
<a id="613" href="structured-types.pointed-sections.html#492" class="Function">pointed-section-Pointed-Type</a> <a id="642" href="structured-types.pointed-sections.html#642" class="Bound">A</a> <a id="644" href="structured-types.pointed-sections.html#644" class="Bound">B</a> <a id="646" href="structured-types.pointed-sections.html#646" class="Bound">f</a> <a id="648" class="Symbol">=</a>
  <a id="652" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="654" class="Symbol">(</a> <a id="656" href="structured-types.pointed-sections.html#644" class="Bound">B</a> <a id="658" href="structured-types.pointed-maps.html#1015" class="Function Operator">→*</a> <a id="661" href="structured-types.pointed-sections.html#642" class="Bound">A</a><a id="662" class="Symbol">)</a>
    <a id="668" class="Symbol">(</a> <a id="670" class="Symbol">λ</a> <a id="672" href="structured-types.pointed-sections.html#672" class="Bound">g</a> <a id="674" class="Symbol">→</a> <a id="676" href="structured-types.pointed-homotopies.html#2941" class="Function">htpy-pointed-map</a> <a id="693" href="structured-types.pointed-sections.html#644" class="Bound">B</a> <a id="695" href="structured-types.pointed-sections.html#644" class="Bound">B</a> <a id="697" class="Symbol">(</a><a id="698" href="structured-types.pointed-maps.html#3342" class="Function">comp-pointed-map</a> <a id="715" href="structured-types.pointed-sections.html#644" class="Bound">B</a> <a id="717" href="structured-types.pointed-sections.html#642" class="Bound">A</a> <a id="719" href="structured-types.pointed-sections.html#644" class="Bound">B</a> <a id="721" href="structured-types.pointed-sections.html#646" class="Bound">f</a> <a id="723" href="structured-types.pointed-sections.html#672" class="Bound">g</a><a id="724" class="Symbol">)</a> <a id="726" href="structured-types.pointed-maps.html#3709" class="Function">id-pointed-map</a><a id="740" class="Symbol">)</a>
</pre>