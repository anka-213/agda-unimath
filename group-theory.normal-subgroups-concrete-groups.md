---
title: Normal subgroups of concrete groups
---

<pre class="Agda"><a id="61" class="Symbol">{-#</a> <a id="65" class="Keyword">OPTIONS</a> <a id="73" class="Pragma">--without-K</a> <a id="85" class="Pragma">--exact-split</a> <a id="99" class="Symbol">#-}</a>

<a id="104" class="Keyword">module</a> <a id="111" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a> <a id="157" class="Keyword">where</a>

<a id="164" class="Keyword">open</a> <a id="169" class="Keyword">import</a> <a id="176" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="204" class="Keyword">open</a> <a id="209" class="Keyword">import</a> <a id="216" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="252" class="Keyword">open</a> <a id="257" class="Keyword">import</a> <a id="264" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="293" class="Keyword">open</a> <a id="298" class="Keyword">import</a> <a id="305" href="group-theory.subgroups-concrete-groups.html" class="Module">group-theory.subgroups-concrete-groups</a>
</pre>
## Idea

A normal subgroup is a fixed point of the conjugation action on the (large) set of all subgroups

## Definition

<pre class="Agda"><a id="normal-subgroup-Concrete-Group"></a><a id="479" href="group-theory.normal-subgroups-concrete-groups.html#479" class="Function">normal-subgroup-Concrete-Group</a> <a id="510" class="Symbol">:</a>
  <a id="514" class="Symbol">{</a><a id="515" href="group-theory.normal-subgroups-concrete-groups.html#515" class="Bound">l1</a> <a id="518" class="Symbol">:</a> <a id="520" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="525" class="Symbol">}</a> <a id="527" class="Symbol">(</a><a id="528" href="group-theory.normal-subgroups-concrete-groups.html#528" class="Bound">l2</a> <a id="531" class="Symbol">:</a> <a id="533" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="538" class="Symbol">)</a> <a id="540" class="Symbol">(</a><a id="541" href="group-theory.normal-subgroups-concrete-groups.html#541" class="Bound">G</a> <a id="543" class="Symbol">:</a> <a id="545" href="group-theory.concrete-groups.html#2024" class="Function">Concrete-Group</a> <a id="560" href="group-theory.normal-subgroups-concrete-groups.html#515" class="Bound">l1</a><a id="562" class="Symbol">)</a> <a id="564" class="Symbol">→</a> <a id="566" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="569" class="Symbol">(</a><a id="570" href="group-theory.normal-subgroups-concrete-groups.html#515" class="Bound">l1</a> <a id="573" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="575" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="580" href="group-theory.normal-subgroups-concrete-groups.html#528" class="Bound">l2</a><a id="582" class="Symbol">)</a>
<a id="584" href="group-theory.normal-subgroups-concrete-groups.html#479" class="Function">normal-subgroup-Concrete-Group</a> <a id="615" href="group-theory.normal-subgroups-concrete-groups.html#615" class="Bound">l2</a> <a id="618" href="group-theory.normal-subgroups-concrete-groups.html#618" class="Bound">G</a> <a id="620" class="Symbol">=</a>
  <a id="624" class="Symbol">(</a><a id="625" href="group-theory.normal-subgroups-concrete-groups.html#625" class="Bound">u</a> <a id="627" class="Symbol">:</a> <a id="629" href="group-theory.concrete-groups.html#2425" class="Function">classifying-type-Concrete-Group</a> <a id="661" href="group-theory.normal-subgroups-concrete-groups.html#618" class="Bound">G</a><a id="662" class="Symbol">)</a> <a id="664" class="Symbol">→</a>
  <a id="668" href="group-theory.subgroups-concrete-groups.html#1185" class="Function">subgroup-action-Concrete-Group</a> <a id="699" href="group-theory.normal-subgroups-concrete-groups.html#615" class="Bound">l2</a> <a id="702" href="group-theory.normal-subgroups-concrete-groups.html#618" class="Bound">G</a> <a id="704" href="group-theory.normal-subgroups-concrete-groups.html#625" class="Bound">u</a>

<a id="707" class="Keyword">module</a> <a id="714" href="group-theory.normal-subgroups-concrete-groups.html#714" class="Module">_</a>
  <a id="718" class="Symbol">{</a><a id="719" href="group-theory.normal-subgroups-concrete-groups.html#719" class="Bound">l1</a> <a id="722" href="group-theory.normal-subgroups-concrete-groups.html#722" class="Bound">l2</a> <a id="725" class="Symbol">:</a> <a id="727" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="732" class="Symbol">}</a> <a id="734" class="Symbol">(</a><a id="735" href="group-theory.normal-subgroups-concrete-groups.html#735" class="Bound">G</a> <a id="737" class="Symbol">:</a> <a id="739" href="group-theory.concrete-groups.html#2024" class="Function">Concrete-Group</a> <a id="754" href="group-theory.normal-subgroups-concrete-groups.html#719" class="Bound">l1</a><a id="756" class="Symbol">)</a>
  <a id="760" class="Symbol">(</a><a id="761" href="group-theory.normal-subgroups-concrete-groups.html#761" class="Bound">H</a> <a id="763" class="Symbol">:</a> <a id="765" href="group-theory.normal-subgroups-concrete-groups.html#479" class="Function">normal-subgroup-Concrete-Group</a> <a id="796" href="group-theory.normal-subgroups-concrete-groups.html#722" class="Bound">l2</a> <a id="799" href="group-theory.normal-subgroups-concrete-groups.html#735" class="Bound">G</a><a id="800" class="Symbol">)</a>
  <a id="804" class="Keyword">where</a>

  <a id="813" href="group-theory.normal-subgroups-concrete-groups.html#813" class="Function">subgroup-normal-subgroup-Concrete-Group</a> <a id="853" class="Symbol">:</a> <a id="855" href="group-theory.subgroups-concrete-groups.html#1484" class="Function">subgroup-Concrete-Group</a> <a id="879" href="group-theory.normal-subgroups-concrete-groups.html#722" class="Bound">l2</a> <a id="882" href="group-theory.normal-subgroups-concrete-groups.html#735" class="Bound">G</a>
  <a id="886" href="group-theory.normal-subgroups-concrete-groups.html#813" class="Function">subgroup-normal-subgroup-Concrete-Group</a> <a id="926" class="Symbol">=</a> <a id="928" href="group-theory.normal-subgroups-concrete-groups.html#761" class="Bound">H</a> <a id="930" class="Symbol">(</a><a id="931" href="group-theory.concrete-groups.html#2555" class="Function">shape-Concrete-Group</a> <a id="952" href="group-theory.normal-subgroups-concrete-groups.html#735" class="Bound">G</a><a id="953" class="Symbol">)</a>

  <a id="958" href="group-theory.normal-subgroups-concrete-groups.html#958" class="Function">action-normal-subgroup-Concrete-Group</a> <a id="996" class="Symbol">:</a> <a id="998" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="1020" href="group-theory.normal-subgroups-concrete-groups.html#722" class="Bound">l2</a> <a id="1023" href="group-theory.normal-subgroups-concrete-groups.html#735" class="Bound">G</a>
  <a id="1027" href="group-theory.normal-subgroups-concrete-groups.html#958" class="Function">action-normal-subgroup-Concrete-Group</a> <a id="1065" class="Symbol">=</a>
    <a id="1071" href="group-theory.subgroups-concrete-groups.html#1915" class="Function">action-subgroup-Concrete-Group</a> <a id="1102" href="group-theory.normal-subgroups-concrete-groups.html#735" class="Bound">G</a> <a id="1104" href="group-theory.normal-subgroups-concrete-groups.html#813" class="Function">subgroup-normal-subgroup-Concrete-Group</a>
</pre>
