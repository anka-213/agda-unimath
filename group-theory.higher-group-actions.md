---
title: Higher group actions
---

<pre class="Agda"><a id="46" class="Symbol">{-#</a> <a id="50" class="Keyword">OPTIONS</a> <a id="58" class="Pragma">--without-K</a> <a id="70" class="Pragma">--exact-split</a> <a id="84" class="Symbol">#-}</a>

<a id="89" class="Keyword">module</a> <a id="96" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a> <a id="130" class="Keyword">where</a>

<a id="137" class="Keyword">open</a> <a id="142" class="Keyword">import</a> <a id="149" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="177" class="Keyword">open</a> <a id="182" class="Keyword">import</a> <a id="189" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
</pre>
## Idea

An action of a higher group `G` on a type is just a type family over `BG`.

## Definition

<pre class="Agda"><a id="action-∞-Group"></a><a id="329" href="group-theory.higher-group-actions.html#329" class="Function">action-∞-Group</a> <a id="344" class="Symbol">:</a>
  <a id="348" class="Symbol">{</a><a id="349" href="group-theory.higher-group-actions.html#349" class="Bound">l1</a> <a id="352" class="Symbol">:</a> <a id="354" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="359" class="Symbol">}</a> <a id="361" class="Symbol">(</a><a id="362" href="group-theory.higher-group-actions.html#362" class="Bound">l2</a> <a id="365" class="Symbol">:</a> <a id="367" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="372" class="Symbol">)</a> <a id="374" class="Symbol">(</a><a id="375" href="group-theory.higher-group-actions.html#375" class="Bound">G</a> <a id="377" class="Symbol">:</a> <a id="379" href="group-theory.higher-groups.html#1633" class="Function">∞-Group</a> <a id="387" href="group-theory.higher-group-actions.html#349" class="Bound">l1</a><a id="389" class="Symbol">)</a> <a id="391" class="Symbol">→</a> <a id="393" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="396" class="Symbol">(</a><a id="397" href="group-theory.higher-group-actions.html#349" class="Bound">l1</a> <a id="400" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="402" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="407" href="group-theory.higher-group-actions.html#362" class="Bound">l2</a><a id="409" class="Symbol">)</a>
<a id="411" href="group-theory.higher-group-actions.html#329" class="Function">action-∞-Group</a> <a id="426" href="group-theory.higher-group-actions.html#426" class="Bound">l2</a> <a id="429" href="group-theory.higher-group-actions.html#429" class="Bound">G</a> <a id="431" class="Symbol">=</a> <a id="433" href="group-theory.higher-groups.html#1895" class="Function">classifying-type-∞-Group</a> <a id="458" href="group-theory.higher-group-actions.html#429" class="Bound">G</a> <a id="460" class="Symbol">→</a> <a id="462" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="465" href="group-theory.higher-group-actions.html#426" class="Bound">l2</a>
</pre>