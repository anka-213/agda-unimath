# Concrete group actions

<pre class="Agda"><a id="35" class="Symbol">{-#</a> <a id="39" class="Keyword">OPTIONS</a> <a id="47" class="Pragma">--without-K</a> <a id="59" class="Pragma">--exact-split</a> <a id="73" class="Symbol">#-}</a>

<a id="78" class="Keyword">module</a> <a id="85" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a> <a id="121" class="Keyword">where</a>

<a id="128" class="Keyword">open</a> <a id="133" class="Keyword">import</a> <a id="140" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="175" class="Keyword">open</a> <a id="180" class="Keyword">import</a> <a id="187" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="219" class="Keyword">open</a> <a id="224" class="Keyword">import</a> <a id="231" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="252" class="Keyword">open</a> <a id="257" class="Keyword">import</a> <a id="264" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="290" class="Keyword">open</a> <a id="295" class="Keyword">import</a> <a id="302" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="318" class="Keyword">open</a> <a id="323" class="Keyword">import</a> <a id="330" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="358" class="Keyword">open</a> <a id="363" class="Keyword">import</a> <a id="370" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>

<a id="400" class="Keyword">open</a> <a id="405" class="Keyword">import</a> <a id="412" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
</pre>
## Idea

Given a concrete group `G`, a concrete action of `G` on a type is defined to be a type family over `BG`. Given a type family `X` over `BG`, the type being acted on is the type `X *`, and the action of `G` on `X *` is given by transport.

## Definition

<pre class="Agda"><a id="720" class="Keyword">module</a> <a id="727" href="group-theory.concrete-group-actions.html#727" class="Module">_</a>
  <a id="731" class="Symbol">{</a><a id="732" href="group-theory.concrete-group-actions.html#732" class="Bound">l1</a> <a id="735" class="Symbol">:</a> <a id="737" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="742" class="Symbol">}</a> <a id="744" class="Symbol">(</a><a id="745" href="group-theory.concrete-group-actions.html#745" class="Bound">l2</a> <a id="748" class="Symbol">:</a> <a id="750" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="755" class="Symbol">)</a> <a id="757" class="Symbol">(</a><a id="758" href="group-theory.concrete-group-actions.html#758" class="Bound">G</a> <a id="760" class="Symbol">:</a> <a id="762" href="group-theory.concrete-groups.html#1988" class="Function">Concrete-Group</a> <a id="777" href="group-theory.concrete-group-actions.html#732" class="Bound">l1</a><a id="779" class="Symbol">)</a>
  <a id="783" class="Keyword">where</a>
  
  <a id="794" href="group-theory.concrete-group-actions.html#794" class="Function">action-Concrete-Group</a> <a id="816" class="Symbol">:</a> <a id="818" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="821" class="Symbol">(</a><a id="822" href="group-theory.concrete-group-actions.html#732" class="Bound">l1</a> <a id="825" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="827" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="832" href="group-theory.concrete-group-actions.html#745" class="Bound">l2</a><a id="834" class="Symbol">)</a>
  <a id="838" href="group-theory.concrete-group-actions.html#794" class="Function">action-Concrete-Group</a> <a id="860" class="Symbol">=</a> <a id="862" href="group-theory.concrete-groups.html#2389" class="Function">classifying-type-Concrete-Group</a> <a id="894" href="group-theory.concrete-group-actions.html#758" class="Bound">G</a> <a id="896" class="Symbol">→</a> <a id="898" href="foundation-core.sets.html#1190" class="Function">UU-Set</a> <a id="905" href="group-theory.concrete-group-actions.html#745" class="Bound">l2</a>

<a id="909" class="Keyword">module</a> <a id="916" href="group-theory.concrete-group-actions.html#916" class="Module">_</a>
  <a id="920" class="Symbol">{</a><a id="921" href="group-theory.concrete-group-actions.html#921" class="Bound">l1</a> <a id="924" href="group-theory.concrete-group-actions.html#924" class="Bound">l2</a> <a id="927" class="Symbol">:</a> <a id="929" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="934" class="Symbol">}</a> <a id="936" class="Symbol">(</a><a id="937" href="group-theory.concrete-group-actions.html#937" class="Bound">G</a> <a id="939" class="Symbol">:</a> <a id="941" href="group-theory.concrete-groups.html#1988" class="Function">Concrete-Group</a> <a id="956" href="group-theory.concrete-group-actions.html#921" class="Bound">l1</a><a id="958" class="Symbol">)</a> <a id="960" class="Symbol">(</a><a id="961" href="group-theory.concrete-group-actions.html#961" class="Bound">X</a> <a id="963" class="Symbol">:</a> <a id="965" href="group-theory.concrete-group-actions.html#794" class="Function">action-Concrete-Group</a> <a id="987" href="group-theory.concrete-group-actions.html#924" class="Bound">l2</a> <a id="990" href="group-theory.concrete-group-actions.html#937" class="Bound">G</a><a id="991" class="Symbol">)</a>
  <a id="995" class="Keyword">where</a>

  <a id="1004" href="group-theory.concrete-group-actions.html#1004" class="Function">set-action-Concrete-Group</a> <a id="1030" class="Symbol">:</a> <a id="1032" href="foundation-core.sets.html#1190" class="Function">UU-Set</a> <a id="1039" href="group-theory.concrete-group-actions.html#924" class="Bound">l2</a>
  <a id="1044" href="group-theory.concrete-group-actions.html#1004" class="Function">set-action-Concrete-Group</a> <a id="1070" class="Symbol">=</a> <a id="1072" href="group-theory.concrete-group-actions.html#961" class="Bound">X</a> <a id="1074" class="Symbol">(</a><a id="1075" href="group-theory.concrete-groups.html#2519" class="Function">shape-Concrete-Group</a> <a id="1096" href="group-theory.concrete-group-actions.html#937" class="Bound">G</a><a id="1097" class="Symbol">)</a>

  <a id="1102" href="group-theory.concrete-group-actions.html#1102" class="Function">type-action-Concrete-Group</a> <a id="1129" class="Symbol">:</a> <a id="1131" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1134" href="group-theory.concrete-group-actions.html#924" class="Bound">l2</a>
  <a id="1139" href="group-theory.concrete-group-actions.html#1102" class="Function">type-action-Concrete-Group</a> <a id="1166" class="Symbol">=</a> <a id="1168" href="foundation-core.sets.html#1304" class="Function">type-Set</a> <a id="1177" href="group-theory.concrete-group-actions.html#1004" class="Function">set-action-Concrete-Group</a>

  <a id="1206" href="group-theory.concrete-group-actions.html#1206" class="Function">is-set-type-action-Concrete-Group</a> <a id="1240" class="Symbol">:</a> <a id="1242" href="foundation-core.sets.html#1113" class="Function">is-set</a> <a id="1249" href="group-theory.concrete-group-actions.html#1102" class="Function">type-action-Concrete-Group</a>
  <a id="1278" href="group-theory.concrete-group-actions.html#1206" class="Function">is-set-type-action-Concrete-Group</a> <a id="1312" class="Symbol">=</a> <a id="1314" href="foundation-core.sets.html#1355" class="Function">is-set-type-Set</a> <a id="1330" href="group-theory.concrete-group-actions.html#1004" class="Function">set-action-Concrete-Group</a>

  <a id="1359" href="group-theory.concrete-group-actions.html#1359" class="Function">mul-action-Concrete-Group</a> <a id="1385" class="Symbol">:</a>
    <a id="1391" href="group-theory.concrete-groups.html#3411" class="Function">type-Concrete-Group</a> <a id="1411" href="group-theory.concrete-group-actions.html#937" class="Bound">G</a> <a id="1413" class="Symbol">→</a>
    <a id="1419" href="group-theory.concrete-group-actions.html#1102" class="Function">type-action-Concrete-Group</a> <a id="1446" class="Symbol">→</a> <a id="1448" href="group-theory.concrete-group-actions.html#1102" class="Function">type-action-Concrete-Group</a>
  <a id="1477" href="group-theory.concrete-group-actions.html#1359" class="Function">mul-action-Concrete-Group</a> <a id="1503" href="group-theory.concrete-group-actions.html#1503" class="Bound">g</a> <a id="1505" href="group-theory.concrete-group-actions.html#1505" class="Bound">x</a> <a id="1507" class="Symbol">=</a> <a id="1509" href="foundation-core.identity-types.html#5702" class="Function">tr</a> <a id="1512" class="Symbol">(</a><a id="1513" href="foundation-core.sets.html#1304" class="Function">type-Set</a> <a id="1522" href="foundation-core.functions.html#420" class="Function Operator">∘</a> <a id="1524" href="group-theory.concrete-group-actions.html#961" class="Bound">X</a><a id="1525" class="Symbol">)</a> <a id="1527" href="group-theory.concrete-group-actions.html#1503" class="Bound">g</a> <a id="1529" href="group-theory.concrete-group-actions.html#1505" class="Bound">x</a>
</pre>