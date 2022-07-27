---
title: The higher group of integers
---

<pre class="Agda"><a id="54" class="Symbol">{-#</a> <a id="58" class="Keyword">OPTIONS</a> <a id="66" class="Pragma">--without-K</a> <a id="78" class="Pragma">--exact-split</a> <a id="92" class="Symbol">#-}</a>

<a id="97" class="Keyword">module</a> <a id="104" href="group-theory.integers-higher-group.html" class="Module">group-theory.integers-higher-group</a> <a id="139" class="Keyword">where</a>

<a id="146" class="Keyword">open</a> <a id="151" class="Keyword">import</a> <a id="158" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="190" class="Keyword">open</a> <a id="195" class="Keyword">import</a> <a id="202" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="230" class="Keyword">open</a> <a id="235" class="Keyword">import</a> <a id="242" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>

<a id="270" class="Keyword">open</a> <a id="275" class="Keyword">import</a> <a id="282" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>

<a id="314" class="Keyword">open</a> <a id="319" class="Keyword">import</a> <a id="326" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a>
</pre>
## Idea

The higher group of integers is defined to be the circle. The loop space of the circle is ℤ.

## Definition

<pre class="Agda"><a id="490" class="Keyword">module</a> <a id="497" href="group-theory.integers-higher-group.html#497" class="Module">_</a>
  <a id="501" class="Keyword">where</a>

  <a id="510" href="group-theory.integers-higher-group.html#510" class="Function">classifying-type-ℤ-∞-Group</a> <a id="537" class="Symbol">:</a> <a id="539" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="542" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
  <a id="550" href="group-theory.integers-higher-group.html#510" class="Function">classifying-type-ℤ-∞-Group</a> <a id="577" class="Symbol">=</a> <a id="579" href="synthetic-homotopy-theory.circle.html#12074" class="Postulate">𝕊¹</a>

  <a id="585" href="group-theory.integers-higher-group.html#585" class="Function">shape-ℤ-∞-Group</a> <a id="601" class="Symbol">:</a> <a id="603" href="synthetic-homotopy-theory.circle.html#12074" class="Postulate">𝕊¹</a>
  <a id="608" href="group-theory.integers-higher-group.html#585" class="Function">shape-ℤ-∞-Group</a> <a id="624" class="Symbol">=</a> <a id="626" href="synthetic-homotopy-theory.circle.html#12099" class="Postulate">base-𝕊¹</a>

  <a id="637" href="group-theory.integers-higher-group.html#637" class="Function">classifying-pointed-type-ℤ-∞-Group</a> <a id="672" class="Symbol">:</a> <a id="674" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="687" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
  <a id="695" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="699" href="group-theory.integers-higher-group.html#637" class="Function">classifying-pointed-type-ℤ-∞-Group</a> <a id="734" class="Symbol">=</a> <a id="736" href="group-theory.integers-higher-group.html#510" class="Function">classifying-type-ℤ-∞-Group</a>
  <a id="765" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="769" href="group-theory.integers-higher-group.html#637" class="Function">classifying-pointed-type-ℤ-∞-Group</a> <a id="804" class="Symbol">=</a> <a id="806" href="group-theory.integers-higher-group.html#585" class="Function">shape-ℤ-∞-Group</a>

  <a id="825" href="group-theory.integers-higher-group.html#825" class="Function">ℤ-∞-Group</a> <a id="835" class="Symbol">:</a> <a id="837" href="group-theory.higher-groups.html#1626" class="Function">∞-Group</a> <a id="845" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
  <a id="853" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="857" href="group-theory.integers-higher-group.html#825" class="Function">ℤ-∞-Group</a> <a id="867" class="Symbol">=</a> <a id="869" href="group-theory.integers-higher-group.html#637" class="Function">classifying-pointed-type-ℤ-∞-Group</a>
  <a id="906" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="910" href="group-theory.integers-higher-group.html#825" class="Function">ℤ-∞-Group</a> <a id="920" class="Symbol">=</a> <a id="922" href="synthetic-homotopy-theory.circle.html#16858" class="Function">is-0-connected-𝕊¹</a>
</pre>