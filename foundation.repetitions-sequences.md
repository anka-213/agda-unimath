---
title: Repetitions in sequences
---

<pre class="Agda"><a id="50" class="Symbol">{-#</a> <a id="54" class="Keyword">OPTIONS</a> <a id="62" class="Pragma">--without-K</a> <a id="74" class="Pragma">--exact-split</a> <a id="88" class="Symbol">#-}</a>

<a id="93" class="Keyword">module</a> <a id="100" href="foundation.repetitions-sequences.html" class="Module">foundation.repetitions-sequences</a> <a id="133" class="Keyword">where</a>

<a id="140" class="Keyword">open</a> <a id="145" class="Keyword">import</a> <a id="152" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="194" class="Keyword">open</a> <a id="199" class="Keyword">import</a> <a id="206" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="238" class="Keyword">open</a> <a id="243" class="Keyword">import</a> <a id="250" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="276" class="Keyword">open</a> <a id="281" class="Keyword">import</a> <a id="288" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="308" class="Keyword">open</a> <a id="313" class="Keyword">import</a> <a id="320" href="foundation.pairs-of-distinct-elements.html" class="Module">foundation.pairs-of-distinct-elements</a>
<a id="358" class="Keyword">open</a> <a id="363" class="Keyword">import</a> <a id="370" href="foundation.repetitions.html" class="Module">foundation.repetitions</a>
<a id="393" class="Keyword">open</a> <a id="398" class="Keyword">import</a> <a id="405" href="foundation.sequences.html" class="Module">foundation.sequences</a>
<a id="426" class="Keyword">open</a> <a id="431" class="Keyword">import</a> <a id="438" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

A repetition in a sequence `a : ℕ → A` consists of a pair of distinct natural numbers `m` and `n` such that `a m = a n`.

## Definition

<pre class="Agda"><a id="is-repetition-pair-of-distinct-elements-sequence"></a><a id="624" href="foundation.repetitions-sequences.html#624" class="Function">is-repetition-pair-of-distinct-elements-sequence</a> <a id="673" class="Symbol">:</a>
  <a id="677" class="Symbol">{</a><a id="678" href="foundation.repetitions-sequences.html#678" class="Bound">l</a> <a id="680" class="Symbol">:</a> <a id="682" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="687" class="Symbol">}</a> <a id="689" class="Symbol">{</a><a id="690" href="foundation.repetitions-sequences.html#690" class="Bound">A</a> <a id="692" class="Symbol">:</a> <a id="694" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="697" href="foundation.repetitions-sequences.html#678" class="Bound">l</a><a id="698" class="Symbol">}</a> <a id="700" class="Symbol">(</a><a id="701" href="foundation.repetitions-sequences.html#701" class="Bound">a</a> <a id="703" class="Symbol">:</a> <a id="705" href="foundation.sequences.html#369" class="Function">sequence</a> <a id="714" href="foundation.repetitions-sequences.html#690" class="Bound">A</a><a id="715" class="Symbol">)</a> <a id="717" class="Symbol">(</a><a id="718" href="foundation.repetitions-sequences.html#718" class="Bound">p</a> <a id="720" class="Symbol">:</a> <a id="722" href="foundation.pairs-of-distinct-elements.html#1376" class="Function">pair-of-distinct-elements</a> <a id="748" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="749" class="Symbol">)</a> <a id="751" class="Symbol">→</a>
  <a id="755" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="758" href="foundation.repetitions-sequences.html#678" class="Bound">l</a>
<a id="760" href="foundation.repetitions-sequences.html#624" class="Function">is-repetition-pair-of-distinct-elements-sequence</a> <a id="809" href="foundation.repetitions-sequences.html#809" class="Bound">a</a> <a id="811" href="foundation.repetitions-sequences.html#811" class="Bound">p</a> <a id="813" class="Symbol">=</a>
  <a id="817" href="foundation.repetitions.html#843" class="Function">is-repetition-pair-of-distinct-elements</a> <a id="857" href="foundation.repetitions-sequences.html#809" class="Bound">a</a> <a id="859" href="foundation.repetitions-sequences.html#811" class="Bound">p</a>

<a id="repetition-sequence"></a><a id="862" href="foundation.repetitions-sequences.html#862" class="Function">repetition-sequence</a> <a id="882" class="Symbol">:</a>
  <a id="886" class="Symbol">{</a><a id="887" href="foundation.repetitions-sequences.html#887" class="Bound">l</a> <a id="889" class="Symbol">:</a> <a id="891" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="896" class="Symbol">}</a> <a id="898" class="Symbol">{</a><a id="899" href="foundation.repetitions-sequences.html#899" class="Bound">A</a> <a id="901" class="Symbol">:</a> <a id="903" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="906" href="foundation.repetitions-sequences.html#887" class="Bound">l</a><a id="907" class="Symbol">}</a> <a id="909" class="Symbol">→</a> <a id="911" href="foundation.sequences.html#369" class="Function">sequence</a> <a id="920" href="foundation.repetitions-sequences.html#899" class="Bound">A</a> <a id="922" class="Symbol">→</a> <a id="924" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="927" href="foundation.repetitions-sequences.html#887" class="Bound">l</a>
<a id="929" href="foundation.repetitions-sequences.html#862" class="Function">repetition-sequence</a> <a id="949" href="foundation.repetitions-sequences.html#949" class="Bound">a</a> <a id="951" class="Symbol">=</a>
  <a id="955" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="957" class="Symbol">(</a><a id="958" href="foundation.pairs-of-distinct-elements.html#1376" class="Function">pair-of-distinct-elements</a> <a id="984" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="985" class="Symbol">)</a> <a id="987" class="Symbol">(</a><a id="988" href="foundation.repetitions.html#843" class="Function">is-repetition-pair-of-distinct-elements</a> <a id="1028" href="foundation.repetitions-sequences.html#949" class="Bound">a</a><a id="1029" class="Symbol">)</a>

<a id="1032" class="Keyword">module</a> <a id="1039" href="foundation.repetitions-sequences.html#1039" class="Module">_</a>
  <a id="1043" class="Symbol">{</a><a id="1044" href="foundation.repetitions-sequences.html#1044" class="Bound">l</a> <a id="1046" class="Symbol">:</a> <a id="1048" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1053" class="Symbol">}</a> <a id="1055" class="Symbol">{</a><a id="1056" href="foundation.repetitions-sequences.html#1056" class="Bound">A</a> <a id="1058" class="Symbol">:</a> <a id="1060" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1063" href="foundation.repetitions-sequences.html#1044" class="Bound">l</a><a id="1064" class="Symbol">}</a> <a id="1066" class="Symbol">(</a><a id="1067" href="foundation.repetitions-sequences.html#1067" class="Bound">a</a> <a id="1069" class="Symbol">:</a> <a id="1071" href="foundation.sequences.html#369" class="Function">sequence</a> <a id="1080" href="foundation.repetitions-sequences.html#1056" class="Bound">A</a><a id="1081" class="Symbol">)</a> <a id="1083" class="Symbol">(</a><a id="1084" href="foundation.repetitions-sequences.html#1084" class="Bound">r</a> <a id="1086" class="Symbol">:</a> <a id="1088" href="foundation.repetitions-sequences.html#862" class="Function">repetition-sequence</a> <a id="1108" href="foundation.repetitions-sequences.html#1067" class="Bound">a</a><a id="1109" class="Symbol">)</a>
  <a id="1113" class="Keyword">where</a>

  <a id="1122" href="foundation.repetitions-sequences.html#1122" class="Function">pair-of-distinct-elements-repetition-sequence</a> <a id="1168" class="Symbol">:</a>
    <a id="1174" href="foundation.pairs-of-distinct-elements.html#1376" class="Function">pair-of-distinct-elements</a> <a id="1200" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a>
  <a id="1204" href="foundation.repetitions-sequences.html#1122" class="Function">pair-of-distinct-elements-repetition-sequence</a> <a id="1250" class="Symbol">=</a> <a id="1252" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1256" href="foundation.repetitions-sequences.html#1084" class="Bound">r</a>

  <a id="1261" href="foundation.repetitions-sequences.html#1261" class="Function">fst-repetition-sequence</a> <a id="1285" class="Symbol">:</a> <a id="1287" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a>
  <a id="1291" href="foundation.repetitions-sequences.html#1261" class="Function">fst-repetition-sequence</a> <a id="1315" class="Symbol">=</a>
    <a id="1321" href="foundation.pairs-of-distinct-elements.html#1578" class="Function">fst-pair-of-distinct-elements</a> <a id="1351" href="foundation.repetitions-sequences.html#1122" class="Function">pair-of-distinct-elements-repetition-sequence</a>

  <a id="1400" href="foundation.repetitions-sequences.html#1400" class="Function">snd-repetition-sequence</a> <a id="1424" class="Symbol">:</a> <a id="1426" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a>
  <a id="1430" href="foundation.repetitions-sequences.html#1400" class="Function">snd-repetition-sequence</a> <a id="1454" class="Symbol">=</a>
    <a id="1460" href="foundation.pairs-of-distinct-elements.html#1655" class="Function">snd-pair-of-distinct-elements</a> <a id="1490" href="foundation.repetitions-sequences.html#1122" class="Function">pair-of-distinct-elements-repetition-sequence</a>

  <a id="1539" href="foundation.repetitions-sequences.html#1539" class="Function">distinction-repetition-sequence</a> <a id="1571" class="Symbol">:</a>
    <a id="1577" href="foundation-core.negation.html#465" class="Function">¬</a> <a id="1579" class="Symbol">(</a><a id="1580" href="foundation.repetitions-sequences.html#1261" class="Function">fst-repetition-sequence</a> <a id="1604" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="1606" href="foundation.repetitions-sequences.html#1400" class="Function">snd-repetition-sequence</a><a id="1629" class="Symbol">)</a>
  <a id="1633" href="foundation.repetitions-sequences.html#1539" class="Function">distinction-repetition-sequence</a> <a id="1665" class="Symbol">=</a>
    <a id="1671" href="foundation.pairs-of-distinct-elements.html#1738" class="Function">distinction-pair-of-distinct-elements</a>
      <a id="1715" href="foundation.repetitions-sequences.html#1122" class="Function">pair-of-distinct-elements-repetition-sequence</a>

  <a id="1764" href="foundation.repetitions-sequences.html#1764" class="Function">is-repetition-pair-of-distinct-elements-repetition-sequence</a> <a id="1824" class="Symbol">:</a>
    <a id="1830" href="foundation.repetitions.html#843" class="Function">is-repetition-pair-of-distinct-elements</a> <a id="1870" href="foundation.repetitions-sequences.html#1067" class="Bound">a</a>
      <a id="1878" href="foundation.repetitions-sequences.html#1122" class="Function">pair-of-distinct-elements-repetition-sequence</a>
  <a id="1926" href="foundation.repetitions-sequences.html#1764" class="Function">is-repetition-pair-of-distinct-elements-repetition-sequence</a> <a id="1986" class="Symbol">=</a> <a id="1988" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="1992" href="foundation.repetitions-sequences.html#1084" class="Bound">r</a>
</pre>