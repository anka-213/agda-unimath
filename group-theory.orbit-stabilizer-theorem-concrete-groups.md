---
title: The orbit-stabilizer theorem for concrete groups
---

<pre class="Agda"><a id="74" class="Symbol">{-#</a> <a id="78" class="Keyword">OPTIONS</a> <a id="86" class="Pragma">--without-K</a> <a id="98" class="Pragma">--exact-split</a> <a id="112" class="Symbol">#-}</a>

<a id="117" class="Keyword">module</a> <a id="124" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html" class="Module">group-theory.orbit-stabilizer-theorem-concrete-groups</a> <a id="178" class="Keyword">where</a>

<a id="185" class="Keyword">open</a> <a id="190" class="Keyword">import</a> <a id="197" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="229" class="Keyword">open</a> <a id="234" class="Keyword">import</a> <a id="241" href="foundation.mere-equality.html" class="Module">foundation.mere-equality</a>
<a id="266" class="Keyword">open</a> <a id="271" class="Keyword">import</a> <a id="278" href="foundation.subtypes.html" class="Module">foundation.subtypes</a>
<a id="298" class="Keyword">open</a> <a id="303" class="Keyword">import</a> <a id="310" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="338" class="Keyword">open</a> <a id="343" class="Keyword">import</a> <a id="350" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="386" class="Keyword">open</a> <a id="391" class="Keyword">import</a> <a id="398" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
</pre>
## Idea

The orbit stabilizer theorem for concrete groups asserts that the type `Orbit(x)` of orbits of an element `x : X *` is deloopable and fits in a fiber sequence

```md
  BG_x ----> BG ----> B(Orbit(x))
```

To see that this is indeed a formulation of the orbit-stabilizer theorem, note that the delooping of `Orbit(x)` gives `Orbit(x)` the structure of a group. Furthermore, this fiber sequence induces a short exact sequence

```md
  G_x ----> G ----> Orbit(x),
```

which induces a bijection from the cosets of the stabilizer subgroup `G_x` of `G` to the type `Orbit(x)`.

## Definitions

<pre class="Agda"><a id="coset-stabilizer-action-Concrete-Group"></a><a id="1038" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1038" class="Function">coset-stabilizer-action-Concrete-Group</a> <a id="1077" class="Symbol">:</a>
  <a id="1081" class="Symbol">{</a><a id="1082" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1082" class="Bound">l1</a> <a id="1085" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1085" class="Bound">l2</a> <a id="1088" class="Symbol">:</a> <a id="1090" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1095" class="Symbol">}</a> <a id="1097" class="Symbol">(</a><a id="1098" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1098" class="Bound">G</a> <a id="1100" class="Symbol">:</a> <a id="1102" href="group-theory.concrete-groups.html#2028" class="Function">Concrete-Group</a> <a id="1117" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1082" class="Bound">l1</a><a id="1119" class="Symbol">)</a> <a id="1121" class="Symbol">(</a><a id="1122" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1122" class="Bound">X</a> <a id="1124" class="Symbol">:</a> <a id="1126" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="1148" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1085" class="Bound">l2</a> <a id="1151" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1098" class="Bound">G</a><a id="1152" class="Symbol">)</a> <a id="1154" class="Symbol">→</a>
  <a id="1158" href="group-theory.concrete-group-actions.html#1115" class="Function">type-action-Concrete-Group</a> <a id="1185" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1098" class="Bound">G</a> <a id="1187" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1122" class="Bound">X</a> <a id="1189" class="Symbol">→</a> <a id="1191" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="1213" class="Symbol">(</a><a id="1214" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1082" class="Bound">l1</a> <a id="1217" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1219" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1085" class="Bound">l2</a><a id="1221" class="Symbol">)</a> <a id="1223" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1098" class="Bound">G</a>
<a id="1225" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1038" class="Function">coset-stabilizer-action-Concrete-Group</a> <a id="1264" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1264" class="Bound">G</a> <a id="1266" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1266" class="Bound">X</a> <a id="1268" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1268" class="Bound">x</a> <a id="1270" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1270" class="Bound">u</a> <a id="1272" class="Symbol">=</a>
  <a id="1276" href="foundation-core.subtypes.html#5615" class="Function">subset-Set</a>
    <a id="1291" class="Symbol">(</a> <a id="1293" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1266" class="Bound">X</a> <a id="1295" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1270" class="Bound">u</a><a id="1296" class="Symbol">)</a>
    <a id="1302" class="Symbol">(</a> <a id="1304" class="Symbol">λ</a> <a id="1306" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1306" class="Bound">y</a> <a id="1308" class="Symbol">→</a> <a id="1310" href="foundation.mere-equality.html#1010" class="Function">mere-eq-Prop</a> <a id="1323" class="Symbol">(</a><a id="1324" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a> <a id="1329" class="Symbol">(</a><a id="1330" href="group-theory.concrete-groups.html#2559" class="Function">shape-Concrete-Group</a> <a id="1351" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1264" class="Bound">G</a><a id="1352" class="Symbol">)</a> <a id="1354" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1268" class="Bound">x</a><a id="1355" class="Symbol">)</a> <a id="1357" class="Symbol">(</a><a id="1358" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a> <a id="1363" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1270" class="Bound">u</a> <a id="1365" href="group-theory.orbit-stabilizer-theorem-concrete-groups.html#1306" class="Bound">y</a><a id="1366" class="Symbol">))</a>
</pre>