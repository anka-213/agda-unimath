---
title: Concrete group actions
---

<pre class="Agda"><a id="48" class="Symbol">{-#</a> <a id="52" class="Keyword">OPTIONS</a> <a id="60" class="Pragma">--without-K</a> <a id="72" class="Pragma">--exact-split</a> <a id="86" class="Symbol">#-}</a>

<a id="91" class="Keyword">module</a> <a id="98" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a> <a id="134" class="Keyword">where</a>

<a id="141" class="Keyword">open</a> <a id="146" class="Keyword">import</a> <a id="153" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="188" class="Keyword">open</a> <a id="193" class="Keyword">import</a> <a id="200" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="232" class="Keyword">open</a> <a id="237" class="Keyword">import</a> <a id="244" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="265" class="Keyword">open</a> <a id="270" class="Keyword">import</a> <a id="277" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="303" class="Keyword">open</a> <a id="308" class="Keyword">import</a> <a id="315" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="331" class="Keyword">open</a> <a id="336" class="Keyword">import</a> <a id="343" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="371" class="Keyword">open</a> <a id="376" class="Keyword">import</a> <a id="383" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>

<a id="413" class="Keyword">open</a> <a id="418" class="Keyword">import</a> <a id="425" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
</pre>
## Idea

Given a concrete group `G`, a concrete action of `G` on a type is defined to be a type family over `BG`. Given a type family `X` over `BG`, the type being acted on is the type `X *`, and the action of `G` on `X *` is given by transport.

## Definition

<pre class="Agda"><a id="733" class="Keyword">module</a> <a id="740" href="group-theory.concrete-group-actions.html#740" class="Module">_</a>
  <a id="744" class="Symbol">{</a><a id="745" href="group-theory.concrete-group-actions.html#745" class="Bound">l1</a> <a id="748" class="Symbol">:</a> <a id="750" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="755" class="Symbol">}</a> <a id="757" class="Symbol">(</a><a id="758" href="group-theory.concrete-group-actions.html#758" class="Bound">l2</a> <a id="761" class="Symbol">:</a> <a id="763" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="768" class="Symbol">)</a> <a id="770" class="Symbol">(</a><a id="771" href="group-theory.concrete-group-actions.html#771" class="Bound">G</a> <a id="773" class="Symbol">:</a> <a id="775" href="group-theory.concrete-groups.html#1969" class="Function">Concrete-Group</a> <a id="790" href="group-theory.concrete-group-actions.html#745" class="Bound">l1</a><a id="792" class="Symbol">)</a>
  <a id="796" class="Keyword">where</a>
  
  <a id="807" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="829" class="Symbol">:</a> <a id="831" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="834" class="Symbol">(</a><a id="835" href="group-theory.concrete-group-actions.html#745" class="Bound">l1</a> <a id="838" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="840" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="845" href="group-theory.concrete-group-actions.html#758" class="Bound">l2</a><a id="847" class="Symbol">)</a>
  <a id="851" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="873" class="Symbol">=</a> <a id="875" href="group-theory.concrete-groups.html#2370" class="Function">classifying-type-Concrete-Group</a> <a id="907" href="group-theory.concrete-group-actions.html#771" class="Bound">G</a> <a id="909" class="Symbol">→</a> <a id="911" href="foundation-core.sets.html#1190" class="Function">UU-Set</a> <a id="918" href="group-theory.concrete-group-actions.html#758" class="Bound">l2</a>

<a id="922" class="Keyword">module</a> <a id="929" href="group-theory.concrete-group-actions.html#929" class="Module">_</a>
  <a id="933" class="Symbol">{</a><a id="934" href="group-theory.concrete-group-actions.html#934" class="Bound">l1</a> <a id="937" href="group-theory.concrete-group-actions.html#937" class="Bound">l2</a> <a id="940" class="Symbol">:</a> <a id="942" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="947" class="Symbol">}</a> <a id="949" class="Symbol">(</a><a id="950" href="group-theory.concrete-group-actions.html#950" class="Bound">G</a> <a id="952" class="Symbol">:</a> <a id="954" href="group-theory.concrete-groups.html#1969" class="Function">Concrete-Group</a> <a id="969" href="group-theory.concrete-group-actions.html#934" class="Bound">l1</a><a id="971" class="Symbol">)</a> <a id="973" class="Symbol">(</a><a id="974" href="group-theory.concrete-group-actions.html#974" class="Bound">X</a> <a id="976" class="Symbol">:</a> <a id="978" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="1000" href="group-theory.concrete-group-actions.html#937" class="Bound">l2</a> <a id="1003" href="group-theory.concrete-group-actions.html#950" class="Bound">G</a><a id="1004" class="Symbol">)</a>
  <a id="1008" class="Keyword">where</a>

  <a id="1017" href="group-theory.concrete-group-actions.html#1017" class="Function">set-action-Concrete-Group</a> <a id="1043" class="Symbol">:</a> <a id="1045" href="foundation-core.sets.html#1190" class="Function">UU-Set</a> <a id="1052" href="group-theory.concrete-group-actions.html#937" class="Bound">l2</a>
  <a id="1057" href="group-theory.concrete-group-actions.html#1017" class="Function">set-action-Concrete-Group</a> <a id="1083" class="Symbol">=</a> <a id="1085" href="group-theory.concrete-group-actions.html#974" class="Bound">X</a> <a id="1087" class="Symbol">(</a><a id="1088" href="group-theory.concrete-groups.html#2500" class="Function">shape-Concrete-Group</a> <a id="1109" href="group-theory.concrete-group-actions.html#950" class="Bound">G</a><a id="1110" class="Symbol">)</a>

  <a id="1115" href="group-theory.concrete-group-actions.html#1115" class="Function">type-action-Concrete-Group</a> <a id="1142" class="Symbol">:</a> <a id="1144" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1147" href="group-theory.concrete-group-actions.html#937" class="Bound">l2</a>
  <a id="1152" href="group-theory.concrete-group-actions.html#1115" class="Function">type-action-Concrete-Group</a> <a id="1179" class="Symbol">=</a> <a id="1181" href="foundation-core.sets.html#1304" class="Function">type-Set</a> <a id="1190" href="group-theory.concrete-group-actions.html#1017" class="Function">set-action-Concrete-Group</a>

  <a id="1219" href="group-theory.concrete-group-actions.html#1219" class="Function">is-set-type-action-Concrete-Group</a> <a id="1253" class="Symbol">:</a> <a id="1255" href="foundation-core.sets.html#1113" class="Function">is-set</a> <a id="1262" href="group-theory.concrete-group-actions.html#1115" class="Function">type-action-Concrete-Group</a>
  <a id="1291" href="group-theory.concrete-group-actions.html#1219" class="Function">is-set-type-action-Concrete-Group</a> <a id="1325" class="Symbol">=</a> <a id="1327" href="foundation-core.sets.html#1355" class="Function">is-set-type-Set</a> <a id="1343" href="group-theory.concrete-group-actions.html#1017" class="Function">set-action-Concrete-Group</a>

  <a id="1372" href="group-theory.concrete-group-actions.html#1372" class="Function">mul-action-Concrete-Group</a> <a id="1398" class="Symbol">:</a>
    <a id="1404" href="group-theory.concrete-groups.html#3392" class="Function">type-Concrete-Group</a> <a id="1424" href="group-theory.concrete-group-actions.html#950" class="Bound">G</a> <a id="1426" class="Symbol">→</a>
    <a id="1432" href="group-theory.concrete-group-actions.html#1115" class="Function">type-action-Concrete-Group</a> <a id="1459" class="Symbol">→</a> <a id="1461" href="group-theory.concrete-group-actions.html#1115" class="Function">type-action-Concrete-Group</a>
  <a id="1490" href="group-theory.concrete-group-actions.html#1372" class="Function">mul-action-Concrete-Group</a> <a id="1516" href="group-theory.concrete-group-actions.html#1516" class="Bound">g</a> <a id="1518" href="group-theory.concrete-group-actions.html#1518" class="Bound">x</a> <a id="1520" class="Symbol">=</a> <a id="1522" href="foundation-core.identity-types.html#5702" class="Function">tr</a> <a id="1525" class="Symbol">(</a><a id="1526" href="foundation-core.sets.html#1304" class="Function">type-Set</a> <a id="1535" href="foundation-core.functions.html#420" class="Function Operator">∘</a> <a id="1537" href="group-theory.concrete-group-actions.html#974" class="Bound">X</a><a id="1538" class="Symbol">)</a> <a id="1540" href="group-theory.concrete-group-actions.html#1516" class="Bound">g</a> <a id="1542" href="group-theory.concrete-group-actions.html#1518" class="Bound">x</a>
</pre>