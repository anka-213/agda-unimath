---
title: Propositional resizing
---

<pre class="Agda"><a id="48" class="Symbol">{-#</a> <a id="52" class="Keyword">OPTIONS</a> <a id="60" class="Pragma">--without-K</a> <a id="72" class="Pragma">--exact-split</a> <a id="86" class="Symbol">#-}</a>

<a id="91" class="Keyword">module</a> <a id="98" href="foundation.propositional-resizing.html" class="Module">foundation.propositional-resizing</a> <a id="132" class="Keyword">where</a>

<a id="139" class="Keyword">open</a> <a id="144" class="Keyword">import</a> <a id="151" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="183" class="Keyword">open</a> <a id="188" class="Keyword">import</a> <a id="195" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="219" class="Keyword">open</a> <a id="224" class="Keyword">import</a> <a id="231" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="255" class="Keyword">open</a> <a id="260" class="Keyword">import</a> <a id="267" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

We say that there is propositional resizing for propositions of universe levels `l1` and `l2` if there is an equivalence `e : UU-Prop l1 ≃ UU-Prop l2` such that for any proposition `P : UU-Prop l1` we have `P ↔ e P`.

## Definition

<pre class="Agda"><a id="propositional-resizing"></a><a id="549" href="foundation.propositional-resizing.html#549" class="Function">propositional-resizing</a> <a id="572" class="Symbol">:</a> <a id="574" class="Symbol">(</a><a id="575" href="foundation.propositional-resizing.html#575" class="Bound">l1</a> <a id="578" href="foundation.propositional-resizing.html#578" class="Bound">l2</a> <a id="581" class="Symbol">:</a> <a id="583" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="588" class="Symbol">)</a> <a id="590" class="Symbol">→</a> <a id="592" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="595" class="Symbol">(</a><a id="596" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="601" href="foundation.propositional-resizing.html#575" class="Bound">l1</a> <a id="604" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="606" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="611" href="foundation.propositional-resizing.html#578" class="Bound">l2</a><a id="613" class="Symbol">)</a>
<a id="615" href="foundation.propositional-resizing.html#549" class="Function">propositional-resizing</a> <a id="638" href="foundation.propositional-resizing.html#638" class="Bound">l1</a> <a id="641" href="foundation.propositional-resizing.html#641" class="Bound">l2</a> <a id="644" class="Symbol">=</a>
  <a id="648" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="650" class="Symbol">(</a> <a id="652" href="foundation-core.propositions.html#1380" class="Function">UU-Prop</a> <a id="660" href="foundation.propositional-resizing.html#638" class="Bound">l1</a> <a id="663" href="foundation-core.equivalences.html#1607" class="Function Operator">≃</a> <a id="665" href="foundation-core.propositions.html#1380" class="Function">UU-Prop</a> <a id="673" href="foundation.propositional-resizing.html#641" class="Bound">l2</a><a id="675" class="Symbol">)</a>
    <a id="681" class="Symbol">(</a> <a id="683" class="Symbol">λ</a> <a id="685" href="foundation.propositional-resizing.html#685" class="Bound">e</a> <a id="687" class="Symbol">→</a> <a id="689" class="Symbol">(</a><a id="690" href="foundation.propositional-resizing.html#690" class="Bound">P</a> <a id="692" class="Symbol">:</a> <a id="694" href="foundation-core.propositions.html#1380" class="Function">UU-Prop</a> <a id="702" href="foundation.propositional-resizing.html#638" class="Bound">l1</a><a id="704" class="Symbol">)</a> <a id="706" class="Symbol">→</a> <a id="708" href="foundation-core.propositions.html#1482" class="Function">type-Prop</a> <a id="718" href="foundation.propositional-resizing.html#690" class="Bound">P</a> <a id="720" href="foundation-core.equivalences.html#1607" class="Function Operator">≃</a> <a id="722" href="foundation-core.propositions.html#1482" class="Function">type-Prop</a> <a id="732" class="Symbol">(</a><a id="733" href="foundation-core.equivalences.html#1807" class="Function">map-equiv</a> <a id="743" href="foundation.propositional-resizing.html#685" class="Bound">e</a> <a id="745" href="foundation.propositional-resizing.html#690" class="Bound">P</a><a id="746" class="Symbol">))</a>
</pre>