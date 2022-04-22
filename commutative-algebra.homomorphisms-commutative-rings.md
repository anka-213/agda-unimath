---
title: Homomorphisms of commutative rings
---

<pre class="Agda"><a id="60" class="Symbol">{-#</a> <a id="64" class="Keyword">OPTIONS</a> <a id="72" class="Pragma">--without-K</a> <a id="84" class="Pragma">--exact-split</a> <a id="98" class="Symbol">#-}</a>

<a id="103" class="Keyword">module</a> <a id="110" href="commutative-algebra.homomorphisms-commutative-rings.html" class="Module">commutative-algebra.homomorphisms-commutative-rings</a> <a id="162" class="Keyword">where</a>

<a id="169" class="Keyword">open</a> <a id="174" class="Keyword">import</a> <a id="181" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a> <a id="219" class="Keyword">using</a>
  <a id="227" class="Symbol">(</a> <a id="229" href="commutative-algebra.commutative-rings.html#1043" class="Function">Comm-Ring</a><a id="238" class="Symbol">;</a> <a id="240" href="commutative-algebra.commutative-rings.html#1184" class="Function">ring-Comm-Ring</a><a id="254" class="Symbol">)</a>

<a id="257" class="Keyword">open</a> <a id="262" class="Keyword">import</a> <a id="269" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="296" class="Keyword">using</a> <a id="302" class="Symbol">(</a><a id="303" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="308" class="Symbol">;</a> <a id="310" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="312" class="Symbol">;</a> <a id="314" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="317" class="Symbol">)</a>

<a id="320" class="Keyword">open</a> <a id="325" class="Keyword">import</a> <a id="332" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a> <a id="364" class="Keyword">using</a> <a id="370" class="Symbol">(</a><a id="371" href="ring-theory.homomorphisms-rings.html#3835" class="Function">type-hom-Ring</a><a id="384" class="Symbol">)</a>
</pre>
## Idea

A morphism of commutative rings is just a morphism between their underlying rings.

## Definition

<pre class="Agda"><a id="type-hom-Comm-Ring"></a><a id="507" href="commutative-algebra.homomorphisms-commutative-rings.html#507" class="Function">type-hom-Comm-Ring</a> <a id="526" class="Symbol">:</a>
  <a id="530" class="Symbol">{</a> <a id="532" href="commutative-algebra.homomorphisms-commutative-rings.html#532" class="Bound">l1</a> <a id="535" href="commutative-algebra.homomorphisms-commutative-rings.html#535" class="Bound">l2</a> <a id="538" class="Symbol">:</a> <a id="540" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="545" class="Symbol">}</a> <a id="547" class="Symbol">→</a> <a id="549" href="commutative-algebra.commutative-rings.html#1043" class="Function">Comm-Ring</a> <a id="559" href="commutative-algebra.homomorphisms-commutative-rings.html#532" class="Bound">l1</a> <a id="562" class="Symbol">→</a> <a id="564" href="commutative-algebra.commutative-rings.html#1043" class="Function">Comm-Ring</a> <a id="574" href="commutative-algebra.homomorphisms-commutative-rings.html#535" class="Bound">l2</a> <a id="577" class="Symbol">→</a> <a id="579" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="582" class="Symbol">(</a><a id="583" href="commutative-algebra.homomorphisms-commutative-rings.html#532" class="Bound">l1</a> <a id="586" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="588" href="commutative-algebra.homomorphisms-commutative-rings.html#535" class="Bound">l2</a><a id="590" class="Symbol">)</a>
<a id="592" href="commutative-algebra.homomorphisms-commutative-rings.html#507" class="Function">type-hom-Comm-Ring</a> <a id="611" href="commutative-algebra.homomorphisms-commutative-rings.html#611" class="Bound">R1</a> <a id="614" href="commutative-algebra.homomorphisms-commutative-rings.html#614" class="Bound">R2</a> <a id="617" class="Symbol">=</a> <a id="619" href="ring-theory.homomorphisms-rings.html#3835" class="Function">type-hom-Ring</a> <a id="633" class="Symbol">(</a><a id="634" href="commutative-algebra.commutative-rings.html#1184" class="Function">ring-Comm-Ring</a> <a id="649" href="commutative-algebra.homomorphisms-commutative-rings.html#611" class="Bound">R1</a><a id="651" class="Symbol">)</a> <a id="653" class="Symbol">(</a><a id="654" href="commutative-algebra.commutative-rings.html#1184" class="Function">ring-Comm-Ring</a> <a id="669" href="commutative-algebra.homomorphisms-commutative-rings.html#614" class="Bound">R2</a><a id="671" class="Symbol">)</a>
</pre>