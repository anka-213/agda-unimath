---
title: Univalent type families
---

<pre class="Agda"><a id="49" class="Symbol">{-#</a> <a id="53" class="Keyword">OPTIONS</a> <a id="61" class="Pragma">--without-K</a> <a id="73" class="Pragma">--exact-split</a> <a id="87" class="Symbol">#-}</a>

<a id="92" class="Keyword">module</a> <a id="99" href="foundation.univalent-type-families.html" class="Module">foundation.univalent-type-families</a> <a id="134" class="Keyword">where</a>

<a id="141" class="Keyword">open</a> <a id="146" class="Keyword">import</a> <a id="153" href="foundation.equivalences.html" class="Module">foundation.equivalences</a> <a id="177" class="Keyword">using</a> <a id="183" class="Symbol">(</a><a id="184" href="foundation-core.equivalences.html#1556" class="Function">is-equiv</a><a id="192" class="Symbol">)</a>
<a id="194" class="Keyword">open</a> <a id="199" class="Keyword">import</a> <a id="206" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="232" class="Keyword">using</a> <a id="238" class="Symbol">(</a><a id="239" href="foundation-core.identity-types.html#1865" class="Function Operator">_＝_</a><a id="242" class="Symbol">;</a> <a id="244" href="foundation.identity-types.html#3838" class="Function">equiv-tr</a><a id="252" class="Symbol">)</a>
<a id="254" class="Keyword">open</a> <a id="259" class="Keyword">import</a> <a id="266" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="293" class="Keyword">using</a> <a id="299" class="Symbol">(</a><a id="300" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="305" class="Symbol">;</a> <a id="307" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a><a id="309" class="Symbol">;</a> <a id="311" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="314" class="Symbol">)</a>
</pre>
## Idea

A type family `B` over `A` is said to be univalent if the map

```md
  equiv-tr : (Id x y) → (B x ≃ B y)
```

is an equivalence for every `x y : A`.

## Definition

<pre class="Agda"><a id="is-univalent"></a><a id="503" href="foundation.univalent-type-families.html#503" class="Function">is-univalent</a> <a id="516" class="Symbol">:</a>
  <a id="520" class="Symbol">{</a><a id="521" href="foundation.univalent-type-families.html#521" class="Bound">l1</a> <a id="524" href="foundation.univalent-type-families.html#524" class="Bound">l2</a> <a id="527" class="Symbol">:</a> <a id="529" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="534" class="Symbol">}</a> <a id="536" class="Symbol">{</a><a id="537" href="foundation.univalent-type-families.html#537" class="Bound">A</a> <a id="539" class="Symbol">:</a> <a id="541" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="544" href="foundation.univalent-type-families.html#521" class="Bound">l1</a><a id="546" class="Symbol">}</a> <a id="548" class="Symbol">→</a> <a id="550" class="Symbol">(</a><a id="551" href="foundation.univalent-type-families.html#537" class="Bound">A</a> <a id="553" class="Symbol">→</a> <a id="555" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="558" href="foundation.univalent-type-families.html#524" class="Bound">l2</a><a id="560" class="Symbol">)</a> <a id="562" class="Symbol">→</a> <a id="564" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="567" class="Symbol">(</a><a id="568" href="foundation.univalent-type-families.html#521" class="Bound">l1</a> <a id="571" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="573" href="foundation.univalent-type-families.html#524" class="Bound">l2</a><a id="575" class="Symbol">)</a>
<a id="577" href="foundation.univalent-type-families.html#503" class="Function">is-univalent</a> <a id="590" class="Symbol">{</a><a id="591" class="Argument">A</a> <a id="593" class="Symbol">=</a> <a id="595" href="foundation.univalent-type-families.html#595" class="Bound">A</a><a id="596" class="Symbol">}</a> <a id="598" href="foundation.univalent-type-families.html#598" class="Bound">B</a> <a id="600" class="Symbol">=</a> <a id="602" class="Symbol">(</a><a id="603" href="foundation.univalent-type-families.html#603" class="Bound">x</a> <a id="605" href="foundation.univalent-type-families.html#605" class="Bound">y</a> <a id="607" class="Symbol">:</a> <a id="609" href="foundation.univalent-type-families.html#595" class="Bound">A</a><a id="610" class="Symbol">)</a> <a id="612" class="Symbol">→</a> <a id="614" href="foundation-core.equivalences.html#1556" class="Function">is-equiv</a> <a id="623" class="Symbol">(λ</a> <a id="626" class="Symbol">(</a><a id="627" href="foundation.univalent-type-families.html#627" class="Bound">p</a> <a id="629" class="Symbol">:</a> <a id="631" href="foundation.univalent-type-families.html#603" class="Bound">x</a> <a id="633" href="foundation-core.identity-types.html#1865" class="Function Operator">＝</a> <a id="635" href="foundation.univalent-type-families.html#605" class="Bound">y</a><a id="636" class="Symbol">)</a> <a id="638" class="Symbol">→</a> <a id="640" href="foundation.identity-types.html#3838" class="Function">equiv-tr</a> <a id="649" href="foundation.univalent-type-families.html#598" class="Bound">B</a> <a id="651" href="foundation.univalent-type-families.html#627" class="Bound">p</a><a id="652" class="Symbol">)</a>
</pre>