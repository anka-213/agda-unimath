---
title: Fixed points of higher group actions
---

<pre class="Agda"><a id="62" class="Symbol">{-#</a> <a id="66" class="Keyword">OPTIONS</a> <a id="74" class="Pragma">--without-K</a> <a id="86" class="Pragma">--exact-split</a> <a id="100" class="Symbol">#-}</a>

<a id="105" class="Keyword">module</a> <a id="112" href="group-theory.fixed-points-higher-group-actions.html" class="Module">group-theory.fixed-points-higher-group-actions</a> <a id="159" class="Keyword">where</a>

<a id="166" class="Keyword">open</a> <a id="171" class="Keyword">import</a> <a id="178" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="206" class="Keyword">open</a> <a id="211" class="Keyword">import</a> <a id="218" href="group-theory.higher-group-actions.html" class="Module">group-theory.higher-group-actions</a>
<a id="252" class="Keyword">open</a> <a id="257" class="Keyword">import</a> <a id="264" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
</pre>
## Idea

The type of fixed points of a higher group action `X : BG → UU` is the type of sections `(u : BG) → X u`.

## Definition

<pre class="Agda"><a id="fixed-point-action-∞-Group"></a><a id="435" href="group-theory.fixed-points-higher-group-actions.html#435" class="Function">fixed-point-action-∞-Group</a> <a id="462" class="Symbol">:</a>
  <a id="466" class="Symbol">{</a><a id="467" href="group-theory.fixed-points-higher-group-actions.html#467" class="Bound">l1</a> <a id="470" href="group-theory.fixed-points-higher-group-actions.html#470" class="Bound">l2</a> <a id="473" class="Symbol">:</a> <a id="475" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="480" class="Symbol">}</a> <a id="482" class="Symbol">(</a><a id="483" href="group-theory.fixed-points-higher-group-actions.html#483" class="Bound">G</a> <a id="485" class="Symbol">:</a> <a id="487" href="group-theory.higher-groups.html#1633" class="Function">∞-Group</a> <a id="495" href="group-theory.fixed-points-higher-group-actions.html#467" class="Bound">l1</a><a id="497" class="Symbol">)</a> <a id="499" class="Symbol">(</a><a id="500" href="group-theory.fixed-points-higher-group-actions.html#500" class="Bound">X</a> <a id="502" class="Symbol">:</a> <a id="504" href="group-theory.higher-group-actions.html#367" class="Function">action-∞-Group</a> <a id="519" href="group-theory.fixed-points-higher-group-actions.html#470" class="Bound">l2</a> <a id="522" href="group-theory.fixed-points-higher-group-actions.html#483" class="Bound">G</a><a id="523" class="Symbol">)</a> <a id="525" class="Symbol">→</a> <a id="527" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="530" class="Symbol">(</a><a id="531" href="group-theory.fixed-points-higher-group-actions.html#467" class="Bound">l1</a> <a id="534" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="536" href="group-theory.fixed-points-higher-group-actions.html#470" class="Bound">l2</a><a id="538" class="Symbol">)</a>
<a id="540" href="group-theory.fixed-points-higher-group-actions.html#435" class="Function">fixed-point-action-∞-Group</a> <a id="567" href="group-theory.fixed-points-higher-group-actions.html#567" class="Bound">G</a> <a id="569" href="group-theory.fixed-points-higher-group-actions.html#569" class="Bound">X</a> <a id="571" class="Symbol">=</a> <a id="573" class="Symbol">(</a><a id="574" href="group-theory.fixed-points-higher-group-actions.html#574" class="Bound">u</a> <a id="576" class="Symbol">:</a> <a id="578" href="group-theory.higher-groups.html#1895" class="Function">classifying-type-∞-Group</a> <a id="603" href="group-theory.fixed-points-higher-group-actions.html#567" class="Bound">G</a><a id="604" class="Symbol">)</a> <a id="606" class="Symbol">→</a> <a id="608" href="group-theory.fixed-points-higher-group-actions.html#569" class="Bound">X</a> <a id="610" href="group-theory.fixed-points-higher-group-actions.html#574" class="Bound">u</a>
</pre>