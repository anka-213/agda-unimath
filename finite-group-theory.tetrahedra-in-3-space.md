---
title: Tetrahedra in 3-dimensional space
---

<pre class="Agda"><a id="59" class="Symbol">{-#</a> <a id="63" class="Keyword">OPTIONS</a> <a id="71" class="Pragma">--without-K</a> <a id="83" class="Pragma">--exact-split</a> <a id="97" class="Symbol">#-}</a>

<a id="102" class="Keyword">module</a> <a id="109" href="finite-group-theory.tetrahedra-in-3-space.html" class="Module">finite-group-theory.tetrahedra-in-3-space</a> <a id="151" class="Keyword">where</a>

<a id="158" class="Keyword">open</a> <a id="163" class="Keyword">import</a> <a id="170" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="202" class="Keyword">open</a> <a id="207" class="Keyword">import</a> <a id="214" href="foundation.empty-types.html" class="Module">foundation.empty-types</a>
<a id="237" class="Keyword">open</a> <a id="242" class="Keyword">import</a> <a id="249" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="277" class="Keyword">open</a> <a id="282" class="Keyword">import</a> <a id="289" href="univalent-combinatorics.2-element-decidable-subtypes.html" class="Module">univalent-combinatorics.2-element-decidable-subtypes</a>
<a id="342" class="Keyword">open</a> <a id="347" class="Keyword">import</a> <a id="354" href="univalent-combinatorics.cyclic-types.html" class="Module">univalent-combinatorics.cyclic-types</a>
<a id="391" class="Keyword">open</a> <a id="396" class="Keyword">import</a> <a id="403" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
</pre>
## Idea

The type of tetrahedra in 3-dimensional space is a type of tetrahedra that can be rotated, but not reflected. In other words, the symmetry group of the tetrahedra in 3-dimensional space is the alternating group `A₄`.

Note that any rotation of a tetrahedron in 3-space induces a rotation on the set of opposing pairs of edges. There are three such pairs of edges.

## Definition

<pre class="Agda"><a id="tetrahedron-in-3-space"></a><a id="842" href="finite-group-theory.tetrahedra-in-3-space.html#842" class="Function">tetrahedron-in-3-space</a> <a id="865" class="Symbol">:</a> <a id="867" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="870" class="Symbol">(</a><a id="871" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="876" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="881" class="Symbol">)</a>
<a id="883" href="finite-group-theory.tetrahedra-in-3-space.html#842" class="Function">tetrahedron-in-3-space</a> <a id="906" class="Symbol">=</a>
  <a id="910" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="912" class="Symbol">(</a> <a id="914" href="univalent-combinatorics.finite-types.html#5852" class="Function">UU-Fin</a> <a id="921" class="Number">4</a><a id="922" class="Symbol">)</a>
    <a id="928" class="Symbol">(</a> <a id="930" class="Symbol">λ</a> <a id="932" href="finite-group-theory.tetrahedra-in-3-space.html#932" class="Bound">X</a> <a id="934" class="Symbol">→</a>
      <a id="942" href="univalent-combinatorics.cyclic-types.html#5274" class="Function">cyclic-structure</a> <a id="959" class="Number">3</a>
        <a id="969" class="Symbol">(</a> <a id="971" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="973" class="Symbol">(</a> <a id="975" href="univalent-combinatorics.2-element-decidable-subtypes.html#4845" class="Function">2-Element-Decidable-Subtype</a> <a id="1003" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
              <a id="1023" class="Symbol">(</a> <a id="1025" href="univalent-combinatorics.2-element-decidable-subtypes.html#4845" class="Function">2-Element-Decidable-Subtype</a> <a id="1053" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
                <a id="1075" class="Symbol">(</a> <a id="1077" href="univalent-combinatorics.finite-types.html#5914" class="Function">type-UU-Fin</a> <a id="1089" class="Number">4</a> <a id="1091" href="finite-group-theory.tetrahedra-in-3-space.html#932" class="Bound">X</a><a id="1092" class="Symbol">)))</a>
            <a id="1108" class="Symbol">(</a> <a id="1110" class="Symbol">λ</a> <a id="1112" href="finite-group-theory.tetrahedra-in-3-space.html#1112" class="Bound">Q</a> <a id="1114" class="Symbol">→</a>
              <a id="1130" class="Symbol">(</a><a id="1131" href="finite-group-theory.tetrahedra-in-3-space.html#1131" class="Bound">x</a> <a id="1133" class="Symbol">:</a> <a id="1135" href="univalent-combinatorics.finite-types.html#5914" class="Function">type-UU-Fin</a> <a id="1147" class="Number">4</a> <a id="1149" href="finite-group-theory.tetrahedra-in-3-space.html#932" class="Bound">X</a><a id="1150" class="Symbol">)</a> <a id="1152" class="Symbol">→</a>
              <a id="1168" href="foundation-core.empty-types.html#1228" class="Function">is-empty</a>
                <a id="1193" class="Symbol">(</a> <a id="1195" class="Symbol">(</a><a id="1196" href="finite-group-theory.tetrahedra-in-3-space.html#1196" class="Bound">P</a> <a id="1198" class="Symbol">:</a> <a id="1200" href="univalent-combinatorics.2-element-decidable-subtypes.html#6347" class="Function">type-2-Element-Decidable-Subtype</a> <a id="1233" href="finite-group-theory.tetrahedra-in-3-space.html#1112" class="Bound">Q</a><a id="1234" class="Symbol">)</a> <a id="1236" class="Symbol">→</a>
                  <a id="1256" href="univalent-combinatorics.2-element-decidable-subtypes.html#5726" class="Function">is-in-2-Element-Decidable-Subtype</a>
                    <a id="1310" class="Symbol">(</a><a id="1311" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1315" href="finite-group-theory.tetrahedra-in-3-space.html#1196" class="Bound">P</a><a id="1316" class="Symbol">)</a>
                    <a id="1338" class="Symbol">(</a> <a id="1340" href="finite-group-theory.tetrahedra-in-3-space.html#1131" class="Bound">x</a><a id="1341" class="Symbol">)))))</a>

<a id="1348" class="Keyword">module</a> <a id="1355" href="finite-group-theory.tetrahedra-in-3-space.html#1355" class="Module">_</a>
  <a id="1359" class="Symbol">(</a><a id="1360" href="finite-group-theory.tetrahedra-in-3-space.html#1360" class="Bound">T</a> <a id="1362" class="Symbol">:</a> <a id="1364" href="finite-group-theory.tetrahedra-in-3-space.html#842" class="Function">tetrahedron-in-3-space</a><a id="1386" class="Symbol">)</a>
  <a id="1390" class="Keyword">where</a>

  <a id="1399" href="finite-group-theory.tetrahedra-in-3-space.html#1399" class="Function">vertex-tetrahedron-in-3-space</a> <a id="1429" class="Symbol">:</a> <a id="1431" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1434" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
  <a id="1442" href="finite-group-theory.tetrahedra-in-3-space.html#1399" class="Function">vertex-tetrahedron-in-3-space</a> <a id="1472" class="Symbol">=</a> <a id="1474" href="univalent-combinatorics.finite-types.html#5914" class="Function">type-UU-Fin</a> <a id="1486" class="Number">4</a> <a id="1488" class="Symbol">(</a><a id="1489" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1493" href="finite-group-theory.tetrahedra-in-3-space.html#1360" class="Bound">T</a><a id="1494" class="Symbol">)</a>

  <a id="1499" href="finite-group-theory.tetrahedra-in-3-space.html#1499" class="Function">cyclic-structure-tetrahedron-in-3-space</a> <a id="1539" class="Symbol">:</a>
    <a id="1545" href="univalent-combinatorics.cyclic-types.html#5274" class="Function">cyclic-structure</a> <a id="1562" class="Number">3</a>
      <a id="1570" class="Symbol">(</a> <a id="1572" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1574" class="Symbol">(</a> <a id="1576" href="univalent-combinatorics.2-element-decidable-subtypes.html#4845" class="Function">2-Element-Decidable-Subtype</a> <a id="1604" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
            <a id="1622" class="Symbol">(</a> <a id="1624" href="univalent-combinatorics.2-element-decidable-subtypes.html#4845" class="Function">2-Element-Decidable-Subtype</a> <a id="1652" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
              <a id="1672" class="Symbol">(</a> <a id="1674" href="finite-group-theory.tetrahedra-in-3-space.html#1399" class="Function">vertex-tetrahedron-in-3-space</a><a id="1703" class="Symbol">)))</a>
          <a id="1717" class="Symbol">(</a> <a id="1719" class="Symbol">λ</a> <a id="1721" href="finite-group-theory.tetrahedra-in-3-space.html#1721" class="Bound">Q</a> <a id="1723" class="Symbol">→</a>
            <a id="1737" class="Symbol">(</a><a id="1738" href="finite-group-theory.tetrahedra-in-3-space.html#1738" class="Bound">x</a> <a id="1740" class="Symbol">:</a> <a id="1742" href="finite-group-theory.tetrahedra-in-3-space.html#1399" class="Function">vertex-tetrahedron-in-3-space</a><a id="1771" class="Symbol">)</a> <a id="1773" class="Symbol">→</a>
            <a id="1787" href="foundation-core.empty-types.html#1228" class="Function">is-empty</a>
              <a id="1810" class="Symbol">(</a> <a id="1812" class="Symbol">(</a><a id="1813" href="finite-group-theory.tetrahedra-in-3-space.html#1813" class="Bound">P</a> <a id="1815" class="Symbol">:</a> <a id="1817" href="univalent-combinatorics.2-element-decidable-subtypes.html#6347" class="Function">type-2-Element-Decidable-Subtype</a> <a id="1850" href="finite-group-theory.tetrahedra-in-3-space.html#1721" class="Bound">Q</a><a id="1851" class="Symbol">)</a> <a id="1853" class="Symbol">→</a>
                <a id="1871" href="univalent-combinatorics.2-element-decidable-subtypes.html#5726" class="Function">is-in-2-Element-Decidable-Subtype</a>
                  <a id="1923" class="Symbol">(</a><a id="1924" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1928" href="finite-group-theory.tetrahedra-in-3-space.html#1813" class="Bound">P</a><a id="1929" class="Symbol">)</a>
                  <a id="1949" class="Symbol">(</a> <a id="1951" href="finite-group-theory.tetrahedra-in-3-space.html#1738" class="Bound">x</a><a id="1952" class="Symbol">))))</a>
  <a id="1959" href="finite-group-theory.tetrahedra-in-3-space.html#1499" class="Function">cyclic-structure-tetrahedron-in-3-space</a> <a id="1999" class="Symbol">=</a> <a id="2001" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="2005" href="finite-group-theory.tetrahedra-in-3-space.html#1360" class="Bound">T</a>
</pre>