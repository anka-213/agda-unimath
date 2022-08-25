---
title: Quotients of finite types
---

<pre class="Agda"><a id="51" class="Keyword">module</a> <a id="58" href="univalent-combinatorics.quotients-finite-types.html" class="Module">univalent-combinatorics.quotients-finite-types</a> <a id="105" class="Keyword">where</a>

<a id="112" class="Keyword">open</a> <a id="117" class="Keyword">import</a> <a id="124" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="156" class="Keyword">open</a> <a id="161" class="Keyword">import</a> <a id="168" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a>
<a id="202" class="Keyword">open</a> <a id="207" class="Keyword">import</a> <a id="214" href="foundation.equivalence-classes.html" class="Module">foundation.equivalence-classes</a>
<a id="245" class="Keyword">open</a> <a id="250" class="Keyword">import</a> <a id="257" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="285" class="Keyword">open</a> <a id="290" class="Keyword">import</a> <a id="297" href="univalent-combinatorics.decidable-equivalence-relations.html" class="Module">univalent-combinatorics.decidable-equivalence-relations</a>
<a id="353" class="Keyword">open</a> <a id="358" class="Keyword">import</a> <a id="365" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a>
<a id="408" class="Keyword">open</a> <a id="413" class="Keyword">import</a> <a id="420" href="univalent-combinatorics.function-types.html" class="Module">univalent-combinatorics.function-types</a>
<a id="459" class="Keyword">open</a> <a id="464" class="Keyword">import</a> <a id="471" href="univalent-combinatorics.equality-finite-types.html" class="Module">univalent-combinatorics.equality-finite-types</a>
<a id="517" class="Keyword">open</a> <a id="522" class="Keyword">import</a> <a id="529" href="univalent-combinatorics.image-of-maps.html" class="Module">univalent-combinatorics.image-of-maps</a>
<a id="567" class="Keyword">open</a> <a id="572" class="Keyword">import</a> <a id="579" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
</pre>
## Idea

The quotient of a finite type by a decidable equivalence relation is again a finite type. In this file we set up some infrastructure for such quotients.

## Definition

<pre class="Agda"><a id="807" class="Keyword">module</a> <a id="814" href="univalent-combinatorics.quotients-finite-types.html#814" class="Module">_</a>
  <a id="818" class="Symbol">{</a><a id="819" href="univalent-combinatorics.quotients-finite-types.html#819" class="Bound">l1</a> <a id="822" href="univalent-combinatorics.quotients-finite-types.html#822" class="Bound">l2</a> <a id="825" class="Symbol">:</a> <a id="827" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="832" class="Symbol">}</a> <a id="834" class="Symbol">(</a><a id="835" href="univalent-combinatorics.quotients-finite-types.html#835" class="Bound">X</a> <a id="837" class="Symbol">:</a> <a id="839" href="univalent-combinatorics.finite-types.html#4550" class="Function">𝔽</a> <a id="841" href="univalent-combinatorics.quotients-finite-types.html#819" class="Bound">l1</a><a id="843" class="Symbol">)</a> <a id="845" class="Symbol">(</a><a id="846" href="univalent-combinatorics.quotients-finite-types.html#846" class="Bound">R</a> <a id="848" class="Symbol">:</a> <a id="850" href="univalent-combinatorics.decidable-equivalence-relations.html#663" class="Function">Decidable-Equivalence-Relation-𝔽</a> <a id="883" href="univalent-combinatorics.quotients-finite-types.html#822" class="Bound">l2</a> <a id="886" href="univalent-combinatorics.quotients-finite-types.html#835" class="Bound">X</a><a id="887" class="Symbol">)</a>
  <a id="891" class="Keyword">where</a>

  <a id="900" href="univalent-combinatorics.quotients-finite-types.html#900" class="Function">equivalence-class-Decidable-Equivalence-Relation-𝔽</a> <a id="951" class="Symbol">:</a> <a id="953" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="956" class="Symbol">(</a><a id="957" href="univalent-combinatorics.quotients-finite-types.html#819" class="Bound">l1</a> <a id="960" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="962" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="967" href="univalent-combinatorics.quotients-finite-types.html#822" class="Bound">l2</a><a id="969" class="Symbol">)</a>
  <a id="973" href="univalent-combinatorics.quotients-finite-types.html#900" class="Function">equivalence-class-Decidable-Equivalence-Relation-𝔽</a> <a id="1024" class="Symbol">=</a>
    <a id="1030" href="foundation.images.html#2169" class="Function">im</a> <a id="1033" class="Symbol">(</a><a id="1034" href="univalent-combinatorics.decidable-equivalence-relations.html#938" class="Function">decidable-relation-Decidable-Equivalence-Relation-𝔽</a> <a id="1086" href="univalent-combinatorics.quotients-finite-types.html#835" class="Bound">X</a> <a id="1088" href="univalent-combinatorics.quotients-finite-types.html#846" class="Bound">R</a><a id="1089" class="Symbol">)</a>

  <a id="1094" href="univalent-combinatorics.quotients-finite-types.html#1094" class="Function">is-finite-equivalence-class-Decidable-Equivalence-Relation-𝔽&#39;</a> <a id="1156" class="Symbol">:</a>
    <a id="1162" href="univalent-combinatorics.finite-types.html#4139" class="Function">is-finite</a> <a id="1172" href="univalent-combinatorics.quotients-finite-types.html#900" class="Function">equivalence-class-Decidable-Equivalence-Relation-𝔽</a>
  <a id="1225" href="univalent-combinatorics.quotients-finite-types.html#1094" class="Function">is-finite-equivalence-class-Decidable-Equivalence-Relation-𝔽&#39;</a> <a id="1287" class="Symbol">=</a>
    <a id="1293" href="univalent-combinatorics.image-of-maps.html#1502" class="Function">is-finite-im</a>
      <a id="1312" class="Symbol">(</a> <a id="1314" href="univalent-combinatorics.finite-types.html#4658" class="Function">is-finite-type-𝔽</a> <a id="1331" href="univalent-combinatorics.quotients-finite-types.html#835" class="Bound">X</a><a id="1332" class="Symbol">)</a>
      <a id="1340" class="Symbol">(</a> <a id="1342" href="univalent-combinatorics.decidable-subtypes.html#2796" class="Function">has-decidable-equality-Subset-𝔽</a> <a id="1374" href="univalent-combinatorics.quotients-finite-types.html#835" class="Bound">X</a><a id="1375" class="Symbol">)</a>

  <a id="1380" href="univalent-combinatorics.quotients-finite-types.html#1380" class="Function">quotient-𝔽</a> <a id="1391" class="Symbol">:</a> <a id="1393" href="univalent-combinatorics.finite-types.html#4550" class="Function">𝔽</a> <a id="1395" class="Symbol">(</a><a id="1396" href="univalent-combinatorics.quotients-finite-types.html#819" class="Bound">l1</a> <a id="1399" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1401" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1406" href="univalent-combinatorics.quotients-finite-types.html#822" class="Bound">l2</a><a id="1408" class="Symbol">)</a>
  <a id="1412" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1416" href="univalent-combinatorics.quotients-finite-types.html#1380" class="Function">quotient-𝔽</a> <a id="1427" class="Symbol">=</a> <a id="1429" href="univalent-combinatorics.quotients-finite-types.html#900" class="Function">equivalence-class-Decidable-Equivalence-Relation-𝔽</a>
  <a id="1482" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="1486" href="univalent-combinatorics.quotients-finite-types.html#1380" class="Function">quotient-𝔽</a> <a id="1497" class="Symbol">=</a> <a id="1499" href="univalent-combinatorics.quotients-finite-types.html#1094" class="Function">is-finite-equivalence-class-Decidable-Equivalence-Relation-𝔽&#39;</a>
</pre>