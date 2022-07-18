---
title: Quotient groups of concrete groups
---

<pre class="Agda"><a id="60" class="Keyword">module</a> <a id="67" href="group-theory.quotient-groups-concrete-groups.html" class="Module">group-theory.quotient-groups-concrete-groups</a> <a id="112" class="Keyword">where</a>

<a id="119" class="Keyword">open</a> <a id="124" class="Keyword">import</a> <a id="131" href="foundation.0-images-of-maps.html" class="Module">foundation.0-images-of-maps</a>
<a id="159" class="Keyword">open</a> <a id="164" class="Keyword">import</a> <a id="171" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="203" class="Keyword">open</a> <a id="208" class="Keyword">import</a> <a id="215" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="241" class="Keyword">open</a> <a id="246" class="Keyword">import</a> <a id="253" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="280" class="Keyword">open</a> <a id="285" class="Keyword">import</a> <a id="292" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="308" class="Keyword">open</a> <a id="313" class="Keyword">import</a> <a id="320" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="348" class="Keyword">open</a> <a id="353" class="Keyword">import</a> <a id="360" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="396" class="Keyword">open</a> <a id="401" class="Keyword">import</a> <a id="408" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="437" class="Keyword">open</a> <a id="442" class="Keyword">import</a> <a id="449" href="group-theory.mere-equivalences-concrete-group-actions.html" class="Module">group-theory.mere-equivalences-concrete-group-actions</a>
<a id="503" class="Keyword">open</a> <a id="508" class="Keyword">import</a> <a id="515" href="group-theory.normal-subgroups-concrete-groups.html" class="Module">group-theory.normal-subgroups-concrete-groups</a>

<a id="562" class="Keyword">open</a> <a id="567" class="Keyword">import</a> <a id="574" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
</pre>
## Idea

Given a normal subgroup `N` of a concrete group `G`, the quotient group `G/N` is a concrete group that satisfies the universal property that for any concrete group homomorphism `f : G → H` such that the kernel of `f` is contained in `N`, then `f` extends uniquely to a group homomorphism `G/N → H`.

The quotient `G/N` can be constructed in several ways.

1. We can construct `G/N` as the type of `G`-sets merely equivalent to the coset action of `N`. Since this construction is reminiscent of the torsor construction of BG, we call this the **transitive construction** of `G/N`.
2. We can construct `G/N` as the 0-image of the coset action `N : BG → U`. We call this the **0-image construction** of `G/N`. 

## Definitions

### The transitive construction of `G/N`

<pre class="Agda"><a id="1394" class="Keyword">module</a> <a id="1401" href="group-theory.quotient-groups-concrete-groups.html#1401" class="Module">_</a>
  <a id="1405" class="Symbol">{</a> <a id="1407" href="group-theory.quotient-groups-concrete-groups.html#1407" class="Bound">l1</a> <a id="1410" href="group-theory.quotient-groups-concrete-groups.html#1410" class="Bound">l2</a> <a id="1413" class="Symbol">:</a> <a id="1415" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1420" class="Symbol">}</a> <a id="1422" class="Symbol">(</a><a id="1423" href="group-theory.quotient-groups-concrete-groups.html#1423" class="Bound">G</a> <a id="1425" class="Symbol">:</a> <a id="1427" href="group-theory.concrete-groups.html#2024" class="Function">Concrete-Group</a> <a id="1442" href="group-theory.quotient-groups-concrete-groups.html#1407" class="Bound">l1</a><a id="1444" class="Symbol">)</a>
  <a id="1448" class="Symbol">(</a> <a id="1450" href="group-theory.quotient-groups-concrete-groups.html#1450" class="Bound">N</a> <a id="1452" class="Symbol">:</a> <a id="1454" href="group-theory.normal-subgroups-concrete-groups.html#479" class="Function">normal-subgroup-Concrete-Group</a> <a id="1485" href="group-theory.quotient-groups-concrete-groups.html#1410" class="Bound">l2</a> <a id="1488" href="group-theory.quotient-groups-concrete-groups.html#1423" class="Bound">G</a><a id="1489" class="Symbol">)</a>
  <a id="1493" class="Keyword">where</a>

  <a id="1502" href="group-theory.quotient-groups-concrete-groups.html#1502" class="Function">classifying-type-transitive-quotient-Concrete-Group</a> <a id="1554" class="Symbol">:</a> <a id="1556" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1559" class="Symbol">(</a><a id="1560" href="group-theory.quotient-groups-concrete-groups.html#1407" class="Bound">l1</a> <a id="1563" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1565" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1570" href="group-theory.quotient-groups-concrete-groups.html#1410" class="Bound">l2</a><a id="1572" class="Symbol">)</a>
  <a id="1576" href="group-theory.quotient-groups-concrete-groups.html#1502" class="Function">classifying-type-transitive-quotient-Concrete-Group</a> <a id="1628" class="Symbol">=</a>
    <a id="1634" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1636" class="Symbol">(</a> <a id="1638" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="1660" href="group-theory.quotient-groups-concrete-groups.html#1410" class="Bound">l2</a> <a id="1663" href="group-theory.quotient-groups-concrete-groups.html#1423" class="Bound">G</a><a id="1664" class="Symbol">)</a>
      <a id="1672" class="Symbol">(</a> <a id="1674" href="group-theory.mere-equivalences-concrete-group-actions.html#708" class="Function">mere-equiv-action-Concrete-Group</a> <a id="1707" href="group-theory.quotient-groups-concrete-groups.html#1423" class="Bound">G</a>
        <a id="1717" class="Symbol">(</a> <a id="1719" href="group-theory.normal-subgroups-concrete-groups.html#958" class="Function">action-normal-subgroup-Concrete-Group</a> <a id="1757" href="group-theory.quotient-groups-concrete-groups.html#1423" class="Bound">G</a> <a id="1759" href="group-theory.quotient-groups-concrete-groups.html#1450" class="Bound">N</a><a id="1760" class="Symbol">))</a>

  <a id="1766" href="group-theory.quotient-groups-concrete-groups.html#1766" class="Function">shape-transitive-quotient-Concrete-Group</a> <a id="1807" class="Symbol">:</a>
    <a id="1813" href="group-theory.quotient-groups-concrete-groups.html#1502" class="Function">classifying-type-transitive-quotient-Concrete-Group</a>
  <a id="1867" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1871" href="group-theory.quotient-groups-concrete-groups.html#1766" class="Function">shape-transitive-quotient-Concrete-Group</a> <a id="1912" class="Symbol">=</a>
    <a id="1918" href="group-theory.normal-subgroups-concrete-groups.html#958" class="Function">action-normal-subgroup-Concrete-Group</a> <a id="1956" href="group-theory.quotient-groups-concrete-groups.html#1423" class="Bound">G</a> <a id="1958" href="group-theory.quotient-groups-concrete-groups.html#1450" class="Bound">N</a>
  <a id="1962" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="1966" href="group-theory.quotient-groups-concrete-groups.html#1766" class="Function">shape-transitive-quotient-Concrete-Group</a> <a id="2007" class="Symbol">=</a>
    <a id="2013" href="group-theory.mere-equivalences-concrete-group-actions.html#1293" class="Function">refl-mere-equiv-action-Concrete-Group</a> <a id="2051" href="group-theory.quotient-groups-concrete-groups.html#1423" class="Bound">G</a>
      <a id="2059" class="Symbol">(</a> <a id="2061" href="group-theory.normal-subgroups-concrete-groups.html#958" class="Function">action-normal-subgroup-Concrete-Group</a> <a id="2099" href="group-theory.quotient-groups-concrete-groups.html#1423" class="Bound">G</a> <a id="2101" href="group-theory.quotient-groups-concrete-groups.html#1450" class="Bound">N</a><a id="2102" class="Symbol">)</a>

  <a id="2107" href="group-theory.quotient-groups-concrete-groups.html#2107" class="Function">classifying-pointed-type-transitive-quotient-Concrete-Group</a> <a id="2167" class="Symbol">:</a>
    <a id="2173" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="2186" class="Symbol">(</a><a id="2187" href="group-theory.quotient-groups-concrete-groups.html#1407" class="Bound">l1</a> <a id="2190" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2192" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="2197" href="group-theory.quotient-groups-concrete-groups.html#1410" class="Bound">l2</a><a id="2199" class="Symbol">)</a>
  <a id="2203" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="2207" href="group-theory.quotient-groups-concrete-groups.html#2107" class="Function">classifying-pointed-type-transitive-quotient-Concrete-Group</a> <a id="2267" class="Symbol">=</a>
    <a id="2273" href="group-theory.quotient-groups-concrete-groups.html#1502" class="Function">classifying-type-transitive-quotient-Concrete-Group</a>
  <a id="2327" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="2331" href="group-theory.quotient-groups-concrete-groups.html#2107" class="Function">classifying-pointed-type-transitive-quotient-Concrete-Group</a> <a id="2391" class="Symbol">=</a>
    <a id="2397" href="group-theory.quotient-groups-concrete-groups.html#1766" class="Function">shape-transitive-quotient-Concrete-Group</a>
</pre>
### The 0-image construction of `G/N`

<pre class="Agda"><a id="2490" class="Keyword">module</a> <a id="2497" href="group-theory.quotient-groups-concrete-groups.html#2497" class="Module">_</a>
  <a id="2501" class="Symbol">{</a> <a id="2503" href="group-theory.quotient-groups-concrete-groups.html#2503" class="Bound">l1</a> <a id="2506" href="group-theory.quotient-groups-concrete-groups.html#2506" class="Bound">l2</a> <a id="2509" class="Symbol">:</a> <a id="2511" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="2516" class="Symbol">}</a> <a id="2518" class="Symbol">(</a><a id="2519" href="group-theory.quotient-groups-concrete-groups.html#2519" class="Bound">G</a> <a id="2521" class="Symbol">:</a> <a id="2523" href="group-theory.concrete-groups.html#2024" class="Function">Concrete-Group</a> <a id="2538" href="group-theory.quotient-groups-concrete-groups.html#2503" class="Bound">l1</a><a id="2540" class="Symbol">)</a>
  <a id="2544" class="Symbol">(</a> <a id="2546" href="group-theory.quotient-groups-concrete-groups.html#2546" class="Bound">N</a> <a id="2548" class="Symbol">:</a> <a id="2550" href="group-theory.normal-subgroups-concrete-groups.html#479" class="Function">normal-subgroup-Concrete-Group</a> <a id="2581" href="group-theory.quotient-groups-concrete-groups.html#2506" class="Bound">l2</a> <a id="2584" href="group-theory.quotient-groups-concrete-groups.html#2519" class="Bound">G</a><a id="2585" class="Symbol">)</a>
  <a id="2589" class="Keyword">where</a>

  <a id="2598" href="group-theory.quotient-groups-concrete-groups.html#2598" class="Function">classifying-type-0-image-quotient-Concrete-Group</a> <a id="2647" class="Symbol">:</a> <a id="2649" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="2652" class="Symbol">(</a><a id="2653" href="group-theory.quotient-groups-concrete-groups.html#2503" class="Bound">l1</a> <a id="2656" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="2658" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="2663" href="group-theory.quotient-groups-concrete-groups.html#2506" class="Bound">l2</a><a id="2665" class="Symbol">)</a>
  <a id="2669" href="group-theory.quotient-groups-concrete-groups.html#2598" class="Function">classifying-type-0-image-quotient-Concrete-Group</a> <a id="2718" class="Symbol">=</a>
    <a id="2724" href="foundation.0-images-of-maps.html#569" class="Function">0-im</a> <a id="2729" class="Symbol">(</a><a id="2730" href="group-theory.normal-subgroups-concrete-groups.html#958" class="Function">action-normal-subgroup-Concrete-Group</a> <a id="2768" href="group-theory.quotient-groups-concrete-groups.html#2519" class="Bound">G</a> <a id="2770" href="group-theory.quotient-groups-concrete-groups.html#2546" class="Bound">N</a><a id="2771" class="Symbol">)</a>

  <a id="2776" href="group-theory.quotient-groups-concrete-groups.html#2776" class="Function">shape-0-image-quotient-Concrete-Group</a> <a id="2814" class="Symbol">:</a>
    <a id="2820" href="group-theory.quotient-groups-concrete-groups.html#2598" class="Function">classifying-type-0-image-quotient-Concrete-Group</a>
  <a id="2871" href="group-theory.quotient-groups-concrete-groups.html#2776" class="Function">shape-0-image-quotient-Concrete-Group</a> <a id="2909" class="Symbol">=</a>
    <a id="2915" href="foundation.0-images-of-maps.html#638" class="Function">unit-0-im</a>
      <a id="2931" class="Symbol">(</a> <a id="2933" href="group-theory.normal-subgroups-concrete-groups.html#958" class="Function">action-normal-subgroup-Concrete-Group</a> <a id="2971" href="group-theory.quotient-groups-concrete-groups.html#2519" class="Bound">G</a> <a id="2973" href="group-theory.quotient-groups-concrete-groups.html#2546" class="Bound">N</a><a id="2974" class="Symbol">)</a>
      <a id="2982" class="Symbol">(</a> <a id="2984" href="group-theory.concrete-groups.html#2555" class="Function">shape-Concrete-Group</a> <a id="3005" href="group-theory.quotient-groups-concrete-groups.html#2519" class="Bound">G</a><a id="3006" class="Symbol">)</a>

  <a id="3011" href="group-theory.quotient-groups-concrete-groups.html#3011" class="Function">classifying-pointed-type-0-image-quotient-Concrete-Group</a> <a id="3068" class="Symbol">:</a>
    <a id="3074" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="3087" class="Symbol">(</a><a id="3088" href="group-theory.quotient-groups-concrete-groups.html#2503" class="Bound">l1</a> <a id="3091" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="3093" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="3098" href="group-theory.quotient-groups-concrete-groups.html#2506" class="Bound">l2</a><a id="3100" class="Symbol">)</a>
  <a id="3104" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="3108" href="group-theory.quotient-groups-concrete-groups.html#3011" class="Function">classifying-pointed-type-0-image-quotient-Concrete-Group</a> <a id="3165" class="Symbol">=</a>
    <a id="3171" href="group-theory.quotient-groups-concrete-groups.html#2598" class="Function">classifying-type-0-image-quotient-Concrete-Group</a>
  <a id="3222" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="3226" href="group-theory.quotient-groups-concrete-groups.html#3011" class="Function">classifying-pointed-type-0-image-quotient-Concrete-Group</a> <a id="3283" class="Symbol">=</a>
    <a id="3289" href="group-theory.quotient-groups-concrete-groups.html#2776" class="Function">shape-0-image-quotient-Concrete-Group</a>
</pre>