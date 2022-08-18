---
title: The weak limited principle of omniscience
---

<pre class="Agda"><a id="67" class="Keyword">module</a> <a id="74" href="foundation.weak-limited-principle-of-omniscience.html" class="Module">foundation.weak-limited-principle-of-omniscience</a> <a id="123" class="Keyword">where</a>

<a id="130" class="Keyword">open</a> <a id="135" class="Keyword">import</a> <a id="142" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="184" class="Keyword">open</a> <a id="189" class="Keyword">import</a> <a id="196" href="foundation.disjunction.html" class="Module">foundation.disjunction</a>
<a id="219" class="Keyword">open</a> <a id="224" class="Keyword">import</a> <a id="231" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="257" class="Keyword">open</a> <a id="262" class="Keyword">import</a> <a id="269" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="289" class="Keyword">open</a> <a id="294" class="Keyword">import</a> <a id="301" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="325" class="Keyword">open</a> <a id="330" class="Keyword">import</a> <a id="337" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="353" class="Keyword">open</a> <a id="358" class="Keyword">import</a> <a id="365" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="393" class="Keyword">open</a> <a id="398" class="Keyword">import</a> <a id="405" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
</pre>
## Idea

The **Weak Limited Principle of Omniscience** asserts that for any sequence `f : ℕ → Fin 2` either `f n ＝ 0` for all `n : ℕ` or not. In particular, it is a restricted form of the law of excluded middle.

## Definition

<pre class="Agda"><a id="WLPO"></a><a id="692" href="foundation.weak-limited-principle-of-omniscience.html#692" class="Function">WLPO</a> <a id="697" class="Symbol">:</a> <a id="699" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="702" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="708" href="foundation.weak-limited-principle-of-omniscience.html#692" class="Function">WLPO</a> <a id="713" class="Symbol">=</a>
  <a id="717" class="Symbol">(</a><a id="718" href="foundation.weak-limited-principle-of-omniscience.html#718" class="Bound">f</a> <a id="720" class="Symbol">:</a> <a id="722" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="724" class="Symbol">→</a> <a id="726" href="univalent-combinatorics.standard-finite-types.html#2392" class="Function">Fin</a> <a id="730" class="Number">2</a><a id="731" class="Symbol">)</a> <a id="733" class="Symbol">→</a>
  <a id="737" href="foundation.disjunction.html#1277" class="Function">type-disj-Prop</a>
    <a id="756" class="Symbol">(</a> <a id="758" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a> <a id="765" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="767" class="Symbol">(λ</a> <a id="770" href="foundation.weak-limited-principle-of-omniscience.html#770" class="Bound">n</a> <a id="772" class="Symbol">→</a> <a id="774" href="foundation-core.sets.html#1420" class="Function">Id-Prop</a> <a id="782" class="Symbol">(</a><a id="783" href="univalent-combinatorics.standard-finite-types.html#2284" class="Function">Fin-Set</a> <a id="791" class="Number">2</a><a id="792" class="Symbol">)</a> <a id="794" class="Symbol">(</a><a id="795" href="foundation.weak-limited-principle-of-omniscience.html#718" class="Bound">f</a> <a id="797" href="foundation.weak-limited-principle-of-omniscience.html#770" class="Bound">n</a><a id="798" class="Symbol">)</a> <a id="800" class="Symbol">(</a><a id="801" href="univalent-combinatorics.standard-finite-types.html#6791" class="Function">zero-Fin</a> <a id="810" class="Number">1</a><a id="811" class="Symbol">)))</a>
    <a id="819" class="Symbol">(</a> <a id="821" href="foundation.negation.html#1170" class="Function">neg-Prop</a> <a id="830" class="Symbol">(</a><a id="831" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a> <a id="838" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="840" class="Symbol">(λ</a> <a id="843" href="foundation.weak-limited-principle-of-omniscience.html#843" class="Bound">n</a> <a id="845" class="Symbol">→</a> <a id="847" href="foundation-core.sets.html#1420" class="Function">Id-Prop</a> <a id="855" class="Symbol">(</a><a id="856" href="univalent-combinatorics.standard-finite-types.html#2284" class="Function">Fin-Set</a> <a id="864" class="Number">2</a><a id="865" class="Symbol">)</a> <a id="867" class="Symbol">(</a><a id="868" href="foundation.weak-limited-principle-of-omniscience.html#718" class="Bound">f</a> <a id="870" href="foundation.weak-limited-principle-of-omniscience.html#843" class="Bound">n</a><a id="871" class="Symbol">)</a> <a id="873" class="Symbol">(</a><a id="874" href="univalent-combinatorics.standard-finite-types.html#6791" class="Function">zero-Fin</a> <a id="883" class="Number">1</a><a id="884" class="Symbol">))))</a>
</pre>