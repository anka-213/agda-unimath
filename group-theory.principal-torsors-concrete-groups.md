---
title: Principal torsors of concrete groups
---

<pre class="Agda"><a id="62" class="Symbol">{-#</a> <a id="66" class="Keyword">OPTIONS</a> <a id="74" class="Pragma">--without-K</a> <a id="86" class="Pragma">--exact-split</a> <a id="100" class="Symbol">#-}</a>

<a id="105" class="Keyword">module</a> <a id="112" href="group-theory.principal-torsors-concrete-groups.html" class="Module">group-theory.principal-torsors-concrete-groups</a> <a id="159" class="Keyword">where</a>

<a id="166" class="Keyword">open</a> <a id="171" class="Keyword">import</a> <a id="178" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="206" class="Keyword">open</a> <a id="211" class="Keyword">import</a> <a id="218" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="254" class="Keyword">open</a> <a id="259" class="Keyword">import</a> <a id="266" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
</pre>
## Idea

The principal torsor of a concrete group `G` is the identity type of `BG`.

## Definition

<pre class="Agda"><a id="408" class="Keyword">module</a> <a id="415" href="group-theory.principal-torsors-concrete-groups.html#415" class="Module">_</a>
  <a id="419" class="Symbol">{</a><a id="420" href="group-theory.principal-torsors-concrete-groups.html#420" class="Bound">l1</a> <a id="423" class="Symbol">:</a> <a id="425" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="430" class="Symbol">}</a> <a id="432" class="Symbol">(</a><a id="433" href="group-theory.principal-torsors-concrete-groups.html#433" class="Bound">G</a> <a id="435" class="Symbol">:</a> <a id="437" href="group-theory.concrete-groups.html#1988" class="Function">Concrete-Group</a> <a id="452" href="group-theory.principal-torsors-concrete-groups.html#420" class="Bound">l1</a><a id="454" class="Symbol">)</a>
  <a id="458" class="Keyword">where</a> 

  <a id="468" href="group-theory.principal-torsors-concrete-groups.html#468" class="Function">principal-torsor-Concrete-Group</a> <a id="500" class="Symbol">:</a>
    <a id="506" href="group-theory.concrete-groups.html#2389" class="Function">classifying-type-Concrete-Group</a> <a id="538" href="group-theory.principal-torsors-concrete-groups.html#433" class="Bound">G</a> <a id="540" class="Symbol">→</a> <a id="542" href="group-theory.concrete-group-actions.html#794" class="Function">action-Concrete-Group</a> <a id="564" href="group-theory.principal-torsors-concrete-groups.html#420" class="Bound">l1</a> <a id="567" href="group-theory.principal-torsors-concrete-groups.html#433" class="Bound">G</a>
  <a id="571" href="group-theory.principal-torsors-concrete-groups.html#468" class="Function">principal-torsor-Concrete-Group</a> <a id="603" class="Symbol">=</a> <a id="605" href="group-theory.concrete-groups.html#4446" class="Function">Id-BG-Set</a> <a id="615" href="group-theory.principal-torsors-concrete-groups.html#433" class="Bound">G</a>
</pre>