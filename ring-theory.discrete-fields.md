# Discrete fields

<pre class="Agda"><a id="28" class="Symbol">{-#</a> <a id="32" class="Keyword">OPTIONS</a> <a id="40" class="Pragma">--without-K</a> <a id="52" class="Pragma">--exact-split</a> <a id="66" class="Symbol">#-}</a>

<a id="71" class="Keyword">module</a> <a id="78" href="ring-theory.discrete-fields.html" class="Module">ring-theory.discrete-fields</a> <a id="106" class="Keyword">where</a>

<a id="113" class="Keyword">open</a> <a id="118" class="Keyword">import</a> <a id="125" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="152" class="Keyword">using</a> <a id="158" class="Symbol">(</a><a id="159" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="164" class="Symbol">;</a> <a id="166" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="168" class="Symbol">)</a>

<a id="171" class="Keyword">open</a> <a id="176" class="Keyword">import</a> <a id="183" href="ring-theory.commutative-rings.html" class="Module">ring-theory.commutative-rings</a> <a id="213" class="Keyword">using</a> <a id="219" class="Symbol">(</a><a id="220" href="ring-theory.commutative-rings.html#991" class="Function">Comm-Ring</a><a id="229" class="Symbol">;</a> <a id="231" href="ring-theory.commutative-rings.html#1078" class="Function">ring-Comm-Ring</a><a id="245" class="Symbol">)</a>
<a id="247" class="Keyword">open</a> <a id="252" class="Keyword">import</a> <a id="259" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a> <a id="286" class="Keyword">using</a> <a id="292" class="Symbol">(</a><a id="293" href="ring-theory.division-rings.html#649" class="Function">is-division-Ring</a><a id="309" class="Symbol">)</a>
</pre>
## Idea

A discrete field is a commutative division ring. They are called discrete, because only nonzero elements are assumed to be invertible.

## Definition

<pre class="Agda"><a id="is-discrete-field-Comm-Ring"></a><a id="484" href="ring-theory.discrete-fields.html#484" class="Function">is-discrete-field-Comm-Ring</a> <a id="512" class="Symbol">:</a>
  <a id="516" class="Symbol">{</a> <a id="518" href="ring-theory.discrete-fields.html#518" class="Bound">l</a> <a id="520" class="Symbol">:</a> <a id="522" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="527" class="Symbol">}</a> <a id="529" class="Symbol">→</a> <a id="531" href="ring-theory.commutative-rings.html#991" class="Function">Comm-Ring</a> <a id="541" href="ring-theory.discrete-fields.html#518" class="Bound">l</a> <a id="543" class="Symbol">→</a> <a id="545" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="548" href="ring-theory.discrete-fields.html#518" class="Bound">l</a>
<a id="550" href="ring-theory.discrete-fields.html#484" class="Function">is-discrete-field-Comm-Ring</a> <a id="578" href="ring-theory.discrete-fields.html#578" class="Bound">R</a> <a id="580" class="Symbol">=</a> <a id="582" href="ring-theory.division-rings.html#649" class="Function">is-division-Ring</a> <a id="599" class="Symbol">(</a><a id="600" href="ring-theory.commutative-rings.html#1078" class="Function">ring-Comm-Ring</a> <a id="615" href="ring-theory.discrete-fields.html#578" class="Bound">R</a><a id="616" class="Symbol">)</a>
</pre>