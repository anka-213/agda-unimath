---
title: The limited principle of omniscience (LPO)
---

<pre class="Agda"><a id="68" class="Keyword">module</a> <a id="75" href="foundation.limited-principle-of-omniscience.html" class="Module">foundation.limited-principle-of-omniscience</a> <a id="119" class="Keyword">where</a>

<a id="126" class="Keyword">open</a> <a id="131" class="Keyword">import</a> <a id="138" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="180" class="Keyword">open</a> <a id="185" class="Keyword">import</a> <a id="192" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="215" class="Keyword">open</a> <a id="220" class="Keyword">import</a> <a id="227" href="foundation.existential-quantification.html" class="Module">foundation.existential-quantification</a>
<a id="265" class="Keyword">open</a> <a id="270" class="Keyword">import</a> <a id="277" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="303" class="Keyword">open</a> <a id="308" class="Keyword">import</a> <a id="315" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="339" class="Keyword">open</a> <a id="344" class="Keyword">import</a> <a id="351" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="367" class="Keyword">open</a> <a id="372" class="Keyword">import</a> <a id="379" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="407" class="Keyword">open</a> <a id="412" class="Keyword">import</a> <a id="419" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
</pre>
## Idea

The **Limited Principle of Omniscience** asserts that for every sequence `f : ℕ → Fin 2` either there exists an `n` such that `f n ＝ 1` or for all `n` we have `f n ＝ 0`.

## Definition

<pre class="Agda"><a id="LPO"></a><a id="673" href="foundation.limited-principle-of-omniscience.html#673" class="Function">LPO</a> <a id="677" class="Symbol">:</a> <a id="679" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="682" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="688" href="foundation.limited-principle-of-omniscience.html#673" class="Function">LPO</a> <a id="692" class="Symbol">=</a>
  <a id="696" class="Symbol">(</a><a id="697" href="foundation.limited-principle-of-omniscience.html#697" class="Bound">f</a> <a id="699" class="Symbol">:</a> <a id="701" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="703" class="Symbol">→</a> <a id="705" href="univalent-combinatorics.standard-finite-types.html#2392" class="Function">Fin</a> <a id="709" class="Number">2</a><a id="710" class="Symbol">)</a> <a id="712" class="Symbol">→</a>
  <a id="716" href="foundation.disjunction.html#1277" class="Function">type-disj-Prop</a>
    <a id="735" class="Symbol">(</a> <a id="737" href="foundation.existential-quantification.html#1666" class="Function">∃-Prop</a> <a id="744" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="746" class="Symbol">(λ</a> <a id="749" href="foundation.limited-principle-of-omniscience.html#749" class="Bound">n</a> <a id="751" class="Symbol">→</a> <a id="753" href="foundation.limited-principle-of-omniscience.html#697" class="Bound">f</a> <a id="755" href="foundation.limited-principle-of-omniscience.html#749" class="Bound">n</a> <a id="757" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="759" href="univalent-combinatorics.standard-finite-types.html#8189" class="Function">one-Fin</a> <a id="767" class="Number">1</a><a id="768" class="Symbol">))</a>
    <a id="775" class="Symbol">(</a> <a id="777" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a> <a id="784" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="786" class="Symbol">(λ</a> <a id="789" href="foundation.limited-principle-of-omniscience.html#789" class="Bound">n</a> <a id="791" class="Symbol">→</a> <a id="793" href="foundation-core.sets.html#1420" class="Function">Id-Prop</a> <a id="801" class="Symbol">(</a><a id="802" href="univalent-combinatorics.standard-finite-types.html#2284" class="Function">Fin-Set</a> <a id="810" class="Number">2</a><a id="811" class="Symbol">)</a> <a id="813" class="Symbol">(</a><a id="814" href="foundation.limited-principle-of-omniscience.html#697" class="Bound">f</a> <a id="816" href="foundation.limited-principle-of-omniscience.html#789" class="Bound">n</a><a id="817" class="Symbol">)</a> <a id="819" class="Symbol">(</a><a id="820" href="univalent-combinatorics.standard-finite-types.html#6791" class="Function">zero-Fin</a> <a id="829" class="Number">1</a><a id="830" class="Symbol">)))</a>
</pre>