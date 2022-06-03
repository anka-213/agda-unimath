---
title: Uncountable sets
___

<pre class="Agda"><a id="42" class="Symbol">{-#</a> <a id="46" class="Keyword">OPTIONS</a> <a id="54" class="Pragma">--without-K</a> <a id="66" class="Pragma">--exact-split</a> <a id="80" class="Symbol">#-}</a>

<a id="85" class="Keyword">module</a> <a id="92" href="set-theory.uncountable-sets.html" class="Module">set-theory.uncountable-sets</a> <a id="120" class="Keyword">where</a>

<a id="127" class="Keyword">open</a> <a id="132" class="Keyword">import</a> <a id="139" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="159" class="Keyword">open</a> <a id="164" class="Keyword">import</a> <a id="171" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="195" class="Keyword">open</a> <a id="200" class="Keyword">import</a> <a id="207" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="235" class="Keyword">open</a> <a id="240" class="Keyword">import</a> <a id="247" href="set-theory.countable-sets.html" class="Module">set-theory.countable-sets</a>
</pre>
## Definition

<pre class="Agda"><a id="is-uncountable-Prop"></a><a id="301" href="set-theory.uncountable-sets.html#301" class="Function">is-uncountable-Prop</a> <a id="321" class="Symbol">:</a> <a id="323" class="Symbol">{</a><a id="324" href="set-theory.uncountable-sets.html#324" class="Bound">l</a> <a id="326" class="Symbol">:</a> <a id="328" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="333" class="Symbol">}</a> <a id="335" class="Symbol">→</a> <a id="337" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="340" href="set-theory.uncountable-sets.html#324" class="Bound">l</a> <a id="342" class="Symbol">→</a> <a id="344" href="foundation-core.propositions.html#1380" class="Function">UU-Prop</a> <a id="352" href="set-theory.uncountable-sets.html#324" class="Bound">l</a>
<a id="354" href="set-theory.uncountable-sets.html#301" class="Function">is-uncountable-Prop</a> <a id="374" href="set-theory.uncountable-sets.html#374" class="Bound">X</a> <a id="376" class="Symbol">=</a> <a id="378" href="foundation.negation.html#1157" class="Function">neg-Prop</a> <a id="387" class="Symbol">(</a><a id="388" href="set-theory.countable-sets.html#383" class="Function">is-countable-Prop</a> <a id="406" href="set-theory.uncountable-sets.html#374" class="Bound">X</a><a id="407" class="Symbol">)</a>

<a id="is-uncountable"></a><a id="410" href="set-theory.uncountable-sets.html#410" class="Function">is-uncountable</a> <a id="425" class="Symbol">:</a> <a id="427" class="Symbol">{</a><a id="428" href="set-theory.uncountable-sets.html#428" class="Bound">l</a> <a id="430" class="Symbol">:</a> <a id="432" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="437" class="Symbol">}</a> <a id="439" class="Symbol">→</a> <a id="441" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="444" href="set-theory.uncountable-sets.html#428" class="Bound">l</a> <a id="446" class="Symbol">→</a> <a id="448" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="451" href="set-theory.uncountable-sets.html#428" class="Bound">l</a>
<a id="453" href="set-theory.uncountable-sets.html#410" class="Function">is-uncountable</a> <a id="468" href="set-theory.uncountable-sets.html#468" class="Bound">X</a> <a id="470" class="Symbol">=</a> <a id="472" href="foundation-core.propositions.html#1482" class="Function">type-Prop</a> <a id="482" class="Symbol">(</a><a id="483" href="set-theory.uncountable-sets.html#301" class="Function">is-uncountable-Prop</a> <a id="503" href="set-theory.uncountable-sets.html#468" class="Bound">X</a><a id="504" class="Symbol">)</a>

<a id="is-prop-is-uncountable"></a><a id="507" href="set-theory.uncountable-sets.html#507" class="Function">is-prop-is-uncountable</a> <a id="530" class="Symbol">:</a> <a id="532" class="Symbol">{</a><a id="533" href="set-theory.uncountable-sets.html#533" class="Bound">l</a> <a id="535" class="Symbol">:</a> <a id="537" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="542" class="Symbol">}</a> <a id="544" class="Symbol">(</a><a id="545" href="set-theory.uncountable-sets.html#545" class="Bound">X</a> <a id="547" class="Symbol">:</a> <a id="549" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="552" href="set-theory.uncountable-sets.html#533" class="Bound">l</a><a id="553" class="Symbol">)</a> <a id="555" class="Symbol">→</a> <a id="557" href="foundation-core.propositions.html#1295" class="Function">is-prop</a> <a id="565" class="Symbol">(</a><a id="566" href="set-theory.uncountable-sets.html#410" class="Function">is-uncountable</a> <a id="581" href="set-theory.uncountable-sets.html#545" class="Bound">X</a><a id="582" class="Symbol">)</a>
<a id="584" href="set-theory.uncountable-sets.html#507" class="Function">is-prop-is-uncountable</a> <a id="607" href="set-theory.uncountable-sets.html#607" class="Bound">X</a> <a id="609" class="Symbol">=</a> <a id="611" href="foundation-core.propositions.html#1549" class="Function">is-prop-type-Prop</a> <a id="629" class="Symbol">(</a><a id="630" href="set-theory.uncountable-sets.html#301" class="Function">is-uncountable-Prop</a> <a id="650" href="set-theory.uncountable-sets.html#607" class="Bound">X</a><a id="651" class="Symbol">)</a>
</pre>