---
title: The order of an element in a group
---

<pre class="Agda"><a id="60" class="Keyword">module</a> <a id="67" href="group-theory.orders-of-elements-groups.html" class="Module">group-theory.orders-of-elements-groups</a> <a id="106" class="Keyword">where</a>

<a id="113" class="Keyword">open</a> <a id="118" class="Keyword">import</a> <a id="125" href="elementary-number-theory.group-of-integers.html" class="Module">elementary-number-theory.group-of-integers</a>

<a id="169" class="Keyword">open</a> <a id="174" class="Keyword">import</a> <a id="181" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="209" class="Keyword">open</a> <a id="214" class="Keyword">import</a> <a id="221" href="group-theory.free-groups-with-one-generator.html" class="Module">group-theory.free-groups-with-one-generator</a>
<a id="265" class="Keyword">open</a> <a id="270" class="Keyword">import</a> <a id="277" href="group-theory.groups.html" class="Module">group-theory.groups</a>
<a id="297" class="Keyword">open</a> <a id="302" class="Keyword">import</a> <a id="309" href="group-theory.kernels.html" class="Module">group-theory.kernels</a>
<a id="330" class="Keyword">open</a> <a id="335" class="Keyword">import</a> <a id="342" href="group-theory.normal-subgroups.html" class="Module">group-theory.normal-subgroups</a>
</pre>
## Idea

For each element `g : G` of a group `G` we have a unique group homomorphism `f : ℤ → G` such that `f 1 = g`. The order of `g` is defined to be the kernel of this group homomorphism `f`. Since kernels are ordered by inclusion, it follows that the orders of elements of a group are ordered by reversed inclusion.

If the group `G` has decidable equality, then we can reduce the order of `g` to a natural number. In this case, the orders of elements of `G` are ordered by divisibility.

If the unique group homomorphism `f : ℤ → G` such that `f 1 = g` is injective, and `G` has decidable equality, then the order of `g` is set to be `0`, which is a consequence of the point of view that orders are normal subgroups of `ℤ`.

## Definitions

### The type of orders of elements in groups

<pre class="Agda"><a id="order-Group"></a><a id="1177" href="group-theory.orders-of-elements-groups.html#1177" class="Function">order-Group</a> <a id="1189" class="Symbol">:</a> <a id="1191" class="Symbol">(</a><a id="1192" href="group-theory.orders-of-elements-groups.html#1192" class="Bound">l</a> <a id="1194" class="Symbol">:</a> <a id="1196" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1201" class="Symbol">)</a> <a id="1203" class="Symbol">→</a> <a id="1205" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1208" class="Symbol">(</a><a id="1209" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1214" href="group-theory.orders-of-elements-groups.html#1192" class="Bound">l</a><a id="1215" class="Symbol">)</a>
<a id="1217" href="group-theory.orders-of-elements-groups.html#1177" class="Function">order-Group</a> <a id="1229" href="group-theory.orders-of-elements-groups.html#1229" class="Bound">l</a> <a id="1231" class="Symbol">=</a> <a id="1233" href="group-theory.normal-subgroups.html#1463" class="Function">Normal-Subgroup</a> <a id="1249" href="group-theory.orders-of-elements-groups.html#1229" class="Bound">l</a> <a id="1251" href="elementary-number-theory.group-of-integers.html#658" class="Function">ℤ-Group</a>
</pre>
### The order of an element in a group

<pre class="Agda"><a id="1312" class="Keyword">module</a> <a id="1319" href="group-theory.orders-of-elements-groups.html#1319" class="Module">_</a>
  <a id="1323" class="Symbol">{</a><a id="1324" href="group-theory.orders-of-elements-groups.html#1324" class="Bound">l</a> <a id="1326" class="Symbol">:</a> <a id="1328" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1333" class="Symbol">}</a> <a id="1335" class="Symbol">(</a><a id="1336" href="group-theory.orders-of-elements-groups.html#1336" class="Bound">G</a> <a id="1338" class="Symbol">:</a> <a id="1340" href="group-theory.groups.html#2650" class="Function">Group</a> <a id="1346" href="group-theory.orders-of-elements-groups.html#1324" class="Bound">l</a><a id="1347" class="Symbol">)</a>
  <a id="1351" class="Keyword">where</a>

  <a id="1360" href="group-theory.orders-of-elements-groups.html#1360" class="Function">order-element-Group</a> <a id="1380" class="Symbol">:</a> <a id="1382" href="group-theory.groups.html#2893" class="Function">type-Group</a> <a id="1393" href="group-theory.orders-of-elements-groups.html#1336" class="Bound">G</a> <a id="1395" class="Symbol">→</a> <a id="1397" href="group-theory.orders-of-elements-groups.html#1177" class="Function">order-Group</a> <a id="1409" href="group-theory.orders-of-elements-groups.html#1324" class="Bound">l</a>
  <a id="1413" href="group-theory.orders-of-elements-groups.html#1360" class="Function">order-element-Group</a> <a id="1433" href="group-theory.orders-of-elements-groups.html#1433" class="Bound">g</a> <a id="1435" class="Symbol">=</a>
    <a id="1441" href="group-theory.kernels.html#3934" class="Function">kernel-hom-Group</a> <a id="1458" href="elementary-number-theory.group-of-integers.html#658" class="Function">ℤ-Group</a> <a id="1466" href="group-theory.orders-of-elements-groups.html#1336" class="Bound">G</a> <a id="1468" class="Symbol">(</a><a id="1469" href="group-theory.free-groups-with-one-generator.html#4565" class="Function">hom-free-group-with-one-generator-ℤ</a> <a id="1505" href="group-theory.orders-of-elements-groups.html#1336" class="Bound">G</a> <a id="1507" href="group-theory.orders-of-elements-groups.html#1433" class="Bound">g</a><a id="1508" class="Symbol">)</a>
</pre>