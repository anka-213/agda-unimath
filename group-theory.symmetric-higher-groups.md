---
title: Symmetric higher groups
---

<pre class="Agda"><a id="49" class="Symbol">{-#</a> <a id="53" class="Keyword">OPTIONS</a> <a id="61" class="Pragma">--without-K</a> <a id="73" class="Pragma">--exact-split</a> <a id="87" class="Symbol">#-}</a>

<a id="92" class="Keyword">module</a> <a id="99" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a> <a id="136" class="Keyword">where</a>

<a id="143" class="Keyword">open</a> <a id="148" class="Keyword">import</a> <a id="155" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="187" class="Keyword">open</a> <a id="192" class="Keyword">import</a> <a id="199" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="241" class="Keyword">open</a> <a id="246" class="Keyword">import</a> <a id="253" href="foundation.connected-types.html" class="Module">foundation.connected-types</a>
<a id="280" class="Keyword">open</a> <a id="285" class="Keyword">import</a> <a id="292" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="321" class="Keyword">open</a> <a id="326" class="Keyword">import</a> <a id="333" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="361" class="Keyword">open</a> <a id="366" class="Keyword">import</a> <a id="373" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>

<a id="401" class="Keyword">open</a> <a id="406" class="Keyword">import</a> <a id="413" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
</pre>
## Idea

The symmetric higher group of a type `X` is the connected component of the universe at `X`.

## Definition

<pre class="Agda"><a id="574" class="Keyword">module</a> <a id="581" href="group-theory.symmetric-higher-groups.html#581" class="Module">_</a>
  <a id="585" class="Symbol">{</a><a id="586" href="group-theory.symmetric-higher-groups.html#586" class="Bound">l</a> <a id="588" class="Symbol">:</a> <a id="590" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="595" class="Symbol">}</a> <a id="597" class="Symbol">(</a><a id="598" href="group-theory.symmetric-higher-groups.html#598" class="Bound">X</a> <a id="600" class="Symbol">:</a> <a id="602" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="605" href="group-theory.symmetric-higher-groups.html#586" class="Bound">l</a><a id="606" class="Symbol">)</a>
  <a id="610" class="Keyword">where</a>

  <a id="619" href="group-theory.symmetric-higher-groups.html#619" class="Function">classifying-type-symmetric-∞-Group</a> <a id="654" class="Symbol">:</a> <a id="656" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="659" class="Symbol">(</a><a id="660" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="665" href="group-theory.symmetric-higher-groups.html#586" class="Bound">l</a><a id="666" class="Symbol">)</a>
  <a id="670" href="group-theory.symmetric-higher-groups.html#619" class="Function">classifying-type-symmetric-∞-Group</a> <a id="705" class="Symbol">=</a> <a id="707" href="foundation.connected-components-universes.html#2320" class="Function">component-UU</a> <a id="720" href="group-theory.symmetric-higher-groups.html#598" class="Bound">X</a>

  <a id="725" href="group-theory.symmetric-higher-groups.html#725" class="Function">shape-symmetric-∞-Group</a> <a id="749" class="Symbol">:</a> <a id="751" href="group-theory.symmetric-higher-groups.html#619" class="Function">classifying-type-symmetric-∞-Group</a>
  <a id="788" href="group-theory.symmetric-higher-groups.html#725" class="Function">shape-symmetric-∞-Group</a> <a id="812" class="Symbol">=</a>
    <a id="818" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a> <a id="823" href="group-theory.symmetric-higher-groups.html#598" class="Bound">X</a> <a id="825" class="Symbol">(</a><a id="826" href="foundation.mere-equivalences.html#1771" class="Function">refl-mere-equiv</a> <a id="842" href="group-theory.symmetric-higher-groups.html#598" class="Bound">X</a><a id="843" class="Symbol">)</a>

  <a id="848" href="group-theory.symmetric-higher-groups.html#848" class="Function">classifying-pointed-type-symmetric-∞-Group</a> <a id="891" class="Symbol">:</a> <a id="893" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="906" class="Symbol">(</a><a id="907" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="912" href="group-theory.symmetric-higher-groups.html#586" class="Bound">l</a><a id="913" class="Symbol">)</a>
  <a id="917" href="group-theory.symmetric-higher-groups.html#848" class="Function">classifying-pointed-type-symmetric-∞-Group</a> <a id="960" class="Symbol">=</a>
    <a id="966" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a>
      <a id="977" href="group-theory.symmetric-higher-groups.html#619" class="Function">classifying-type-symmetric-∞-Group</a>
      <a id="1018" href="group-theory.symmetric-higher-groups.html#725" class="Function">shape-symmetric-∞-Group</a>

  <a id="1045" href="group-theory.symmetric-higher-groups.html#1045" class="Function">is-path-connected-classifying-type-symmetric-∞-Group</a> <a id="1098" class="Symbol">:</a>
    <a id="1104" href="foundation.connected-types.html#1757" class="Function">is-path-connected</a> <a id="1122" href="group-theory.symmetric-higher-groups.html#619" class="Function">classifying-type-symmetric-∞-Group</a>
  <a id="1159" href="group-theory.symmetric-higher-groups.html#1045" class="Function">is-path-connected-classifying-type-symmetric-∞-Group</a> <a id="1212" class="Symbol">=</a>
    <a id="1218" href="foundation.connected-components-universes.html#6389" class="Function">is-path-connected-component-UU</a> <a id="1249" href="group-theory.symmetric-higher-groups.html#598" class="Bound">X</a>
  
  <a id="1256" href="group-theory.symmetric-higher-groups.html#1256" class="Function">symmetric-∞-Group</a> <a id="1274" class="Symbol">:</a> <a id="1276" href="group-theory.higher-groups.html#1633" class="Function">∞-Group</a> <a id="1284" class="Symbol">(</a><a id="1285" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1290" href="group-theory.symmetric-higher-groups.html#586" class="Bound">l</a><a id="1291" class="Symbol">)</a>
  <a id="1295" href="group-theory.symmetric-higher-groups.html#1256" class="Function">symmetric-∞-Group</a> <a id="1313" class="Symbol">=</a>
    <a id="1319" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a>
      <a id="1330" href="group-theory.symmetric-higher-groups.html#848" class="Function">classifying-pointed-type-symmetric-∞-Group</a>
      <a id="1379" href="group-theory.symmetric-higher-groups.html#1045" class="Function">is-path-connected-classifying-type-symmetric-∞-Group</a>
</pre>