---
title: Symmetric higher groups
---

<pre class="Agda"><a id="49" class="Symbol">{-#</a> <a id="53" class="Keyword">OPTIONS</a> <a id="61" class="Pragma">--without-K</a> <a id="73" class="Pragma">--exact-split</a> <a id="87" class="Symbol">#-}</a>

<a id="92" class="Keyword">module</a> <a id="99" href="group-theory.symmetric-higher-groups.html" class="Module">group-theory.symmetric-higher-groups</a> <a id="136" class="Keyword">where</a>

<a id="143" class="Keyword">open</a> <a id="148" class="Keyword">import</a> <a id="155" href="foundation.0-connected-types.html" class="Module">foundation.0-connected-types</a>
<a id="184" class="Keyword">open</a> <a id="189" class="Keyword">import</a> <a id="196" href="foundation.connected-components-universes.html" class="Module">foundation.connected-components-universes</a>
<a id="238" class="Keyword">open</a> <a id="243" class="Keyword">import</a> <a id="250" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="282" class="Keyword">open</a> <a id="287" class="Keyword">import</a> <a id="294" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="323" class="Keyword">open</a> <a id="328" class="Keyword">import</a> <a id="335" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="363" class="Keyword">open</a> <a id="368" class="Keyword">import</a> <a id="375" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>

<a id="403" class="Keyword">open</a> <a id="408" class="Keyword">import</a> <a id="415" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
</pre>
## Idea

The symmetric higher group of a type `X` is the connected component of the universe at `X`.

## Definition

<pre class="Agda"><a id="576" class="Keyword">module</a> <a id="583" href="group-theory.symmetric-higher-groups.html#583" class="Module">_</a>
  <a id="587" class="Symbol">{</a><a id="588" href="group-theory.symmetric-higher-groups.html#588" class="Bound">l</a> <a id="590" class="Symbol">:</a> <a id="592" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="597" class="Symbol">}</a> <a id="599" class="Symbol">(</a><a id="600" href="group-theory.symmetric-higher-groups.html#600" class="Bound">X</a> <a id="602" class="Symbol">:</a> <a id="604" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="607" href="group-theory.symmetric-higher-groups.html#588" class="Bound">l</a><a id="608" class="Symbol">)</a>
  <a id="612" class="Keyword">where</a>

  <a id="621" href="group-theory.symmetric-higher-groups.html#621" class="Function">classifying-type-symmetric-∞-Group</a> <a id="656" class="Symbol">:</a> <a id="658" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="661" class="Symbol">(</a><a id="662" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="667" href="group-theory.symmetric-higher-groups.html#588" class="Bound">l</a><a id="668" class="Symbol">)</a>
  <a id="672" href="group-theory.symmetric-higher-groups.html#621" class="Function">classifying-type-symmetric-∞-Group</a> <a id="707" class="Symbol">=</a> <a id="709" href="foundation.connected-components-universes.html#2316" class="Function">component-UU</a> <a id="722" href="group-theory.symmetric-higher-groups.html#600" class="Bound">X</a>

  <a id="727" href="group-theory.symmetric-higher-groups.html#727" class="Function">shape-symmetric-∞-Group</a> <a id="751" class="Symbol">:</a> <a id="753" href="group-theory.symmetric-higher-groups.html#621" class="Function">classifying-type-symmetric-∞-Group</a>
  <a id="790" href="group-theory.symmetric-higher-groups.html#727" class="Function">shape-symmetric-∞-Group</a> <a id="814" class="Symbol">=</a>
    <a id="820" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a> <a id="825" href="group-theory.symmetric-higher-groups.html#600" class="Bound">X</a> <a id="827" class="Symbol">(</a><a id="828" href="foundation.mere-equivalences.html#1771" class="Function">refl-mere-equiv</a> <a id="844" href="group-theory.symmetric-higher-groups.html#600" class="Bound">X</a><a id="845" class="Symbol">)</a>

  <a id="850" href="group-theory.symmetric-higher-groups.html#850" class="Function">classifying-pointed-type-symmetric-∞-Group</a> <a id="893" class="Symbol">:</a> <a id="895" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="908" class="Symbol">(</a><a id="909" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="914" href="group-theory.symmetric-higher-groups.html#588" class="Bound">l</a><a id="915" class="Symbol">)</a>
  <a id="919" href="group-theory.symmetric-higher-groups.html#850" class="Function">classifying-pointed-type-symmetric-∞-Group</a> <a id="962" class="Symbol">=</a>
    <a id="968" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a>
      <a id="979" href="group-theory.symmetric-higher-groups.html#621" class="Function">classifying-type-symmetric-∞-Group</a>
      <a id="1020" href="group-theory.symmetric-higher-groups.html#727" class="Function">shape-symmetric-∞-Group</a>

  <a id="1047" href="group-theory.symmetric-higher-groups.html#1047" class="Function">is-0-connected-classifying-type-symmetric-∞-Group</a> <a id="1097" class="Symbol">:</a>
    <a id="1103" href="foundation.0-connected-types.html#1858" class="Function">is-0-connected</a> <a id="1118" href="group-theory.symmetric-higher-groups.html#621" class="Function">classifying-type-symmetric-∞-Group</a>
  <a id="1155" href="group-theory.symmetric-higher-groups.html#1047" class="Function">is-0-connected-classifying-type-symmetric-∞-Group</a> <a id="1205" class="Symbol">=</a>
    <a id="1211" href="foundation.connected-components-universes.html#6341" class="Function">is-0-connected-component-UU</a> <a id="1239" href="group-theory.symmetric-higher-groups.html#600" class="Bound">X</a>
  
  <a id="1246" href="group-theory.symmetric-higher-groups.html#1246" class="Function">symmetric-∞-Group</a> <a id="1264" class="Symbol">:</a> <a id="1266" href="group-theory.higher-groups.html#1626" class="Function">∞-Group</a> <a id="1274" class="Symbol">(</a><a id="1275" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1280" href="group-theory.symmetric-higher-groups.html#588" class="Bound">l</a><a id="1281" class="Symbol">)</a>
  <a id="1285" href="group-theory.symmetric-higher-groups.html#1246" class="Function">symmetric-∞-Group</a> <a id="1303" class="Symbol">=</a>
    <a id="1309" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a>
      <a id="1320" href="group-theory.symmetric-higher-groups.html#850" class="Function">classifying-pointed-type-symmetric-∞-Group</a>
      <a id="1369" href="group-theory.symmetric-higher-groups.html#1047" class="Function">is-0-connected-classifying-type-symmetric-∞-Group</a>
</pre>