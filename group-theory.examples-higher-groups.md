---
title: Formalisation of the Symmetry Book
---

<pre class="Agda"><a id="60" class="Symbol">{-#</a> <a id="64" class="Keyword">OPTIONS</a> <a id="72" class="Pragma">--without-K</a> <a id="84" class="Pragma">--exact-split</a> <a id="98" class="Symbol">#-}</a>

<a id="103" class="Keyword">module</a> <a id="110" href="group-theory.examples-higher-groups.html" class="Module">group-theory.examples-higher-groups</a> <a id="146" class="Keyword">where</a>

<a id="153" class="Keyword">open</a> <a id="158" class="Keyword">import</a> <a id="165" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a> <a id="192" class="Keyword">public</a>
<a id="199" class="Keyword">open</a> <a id="204" class="Keyword">import</a> <a id="211" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a> <a id="244" class="Keyword">public</a>

<a id="252" class="Keyword">open</a> <a id="257" class="Keyword">import</a> <a id="264" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>

<a id="305" class="Keyword">module</a> <a id="312" href="group-theory.examples-higher-groups.html#312" class="Module">_</a>
  <a id="316" class="Keyword">where</a>

  <a id="325" href="group-theory.examples-higher-groups.html#325" class="Function">classifying-type-ℤ-∞-Group</a> <a id="352" class="Symbol">:</a> <a id="354" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="357" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
  <a id="365" href="group-theory.examples-higher-groups.html#325" class="Function">classifying-type-ℤ-∞-Group</a> <a id="392" class="Symbol">=</a> <a id="394" href="synthetic-homotopy-theory.circle.html#11476" class="Postulate">𝕊¹</a>

  <a id="400" href="group-theory.examples-higher-groups.html#400" class="Function">shape-ℤ-∞-Group</a> <a id="416" class="Symbol">:</a> <a id="418" href="synthetic-homotopy-theory.circle.html#11476" class="Postulate">𝕊¹</a>
  <a id="423" href="group-theory.examples-higher-groups.html#400" class="Function">shape-ℤ-∞-Group</a> <a id="439" class="Symbol">=</a> <a id="441" href="synthetic-homotopy-theory.circle.html#11501" class="Postulate">base-𝕊¹</a>

  <a id="452" href="group-theory.examples-higher-groups.html#452" class="Function">classifying-pointed-type-ℤ-∞-Group</a> <a id="487" class="Symbol">:</a> <a id="489" href="synthetic-homotopy-theory.pointed-types.html#392" class="Function">Pointed-Type</a> <a id="502" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
  <a id="510" href="group-theory.examples-higher-groups.html#452" class="Function">classifying-pointed-type-ℤ-∞-Group</a> <a id="545" class="Symbol">=</a>
    <a id="551" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
      <a id="562" href="group-theory.examples-higher-groups.html#325" class="Function">classifying-type-ℤ-∞-Group</a>
      <a id="595" href="group-theory.examples-higher-groups.html#400" class="Function">shape-ℤ-∞-Group</a>

  <a id="614" href="group-theory.examples-higher-groups.html#614" class="Function">ℤ-∞-Group</a> <a id="624" class="Symbol">:</a> <a id="626" href="group-theory.higher-groups.html#1500" class="Function">∞-Group</a> <a id="634" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
  <a id="642" href="group-theory.examples-higher-groups.html#614" class="Function">ℤ-∞-Group</a> <a id="652" class="Symbol">=</a>
    <a id="658" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
      <a id="669" href="group-theory.examples-higher-groups.html#452" class="Function">classifying-pointed-type-ℤ-∞-Group</a>
      <a id="710" href="synthetic-homotopy-theory.circle.html#18994" class="Function">is-path-connected-𝕊¹</a>

<a id="732" class="Keyword">module</a> <a id="739" href="group-theory.examples-higher-groups.html#739" class="Module">_</a>
  <a id="743" class="Symbol">{</a><a id="744" href="group-theory.examples-higher-groups.html#744" class="Bound">l</a> <a id="746" class="Symbol">:</a> <a id="748" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="753" class="Symbol">}</a> <a id="755" class="Symbol">(</a><a id="756" href="group-theory.examples-higher-groups.html#756" class="Bound">X</a> <a id="758" class="Symbol">:</a> <a id="760" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="763" href="group-theory.examples-higher-groups.html#744" class="Bound">l</a><a id="764" class="Symbol">)</a>
  <a id="768" class="Keyword">where</a>

  <a id="777" href="group-theory.examples-higher-groups.html#777" class="Function">classifying-type-symmetric-∞-Group</a> <a id="812" class="Symbol">:</a> <a id="814" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="817" class="Symbol">(</a><a id="818" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="823" href="group-theory.examples-higher-groups.html#744" class="Bound">l</a><a id="824" class="Symbol">)</a>
  <a id="828" href="group-theory.examples-higher-groups.html#777" class="Function">classifying-type-symmetric-∞-Group</a> <a id="863" class="Symbol">=</a> <a id="865" href="foundation.connected-components-universes.html#2310" class="Function">component-UU</a> <a id="878" href="group-theory.examples-higher-groups.html#756" class="Bound">X</a>

  <a id="883" href="group-theory.examples-higher-groups.html#883" class="Function">shape-symmetric-∞-Group</a> <a id="907" class="Symbol">:</a> <a id="909" href="group-theory.examples-higher-groups.html#777" class="Function">classifying-type-symmetric-∞-Group</a>
  <a id="946" href="group-theory.examples-higher-groups.html#883" class="Function">shape-symmetric-∞-Group</a> <a id="970" class="Symbol">=</a>
    <a id="976" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="981" href="group-theory.examples-higher-groups.html#756" class="Bound">X</a> <a id="983" class="Symbol">(</a><a id="984" href="foundation.mere-equivalences.html#1762" class="Function">refl-mere-equiv</a> <a id="1000" href="group-theory.examples-higher-groups.html#756" class="Bound">X</a><a id="1001" class="Symbol">)</a>

  <a id="1006" href="group-theory.examples-higher-groups.html#1006" class="Function">classifying-pointed-type-symmetric-∞-Group</a> <a id="1049" class="Symbol">:</a> <a id="1051" href="synthetic-homotopy-theory.pointed-types.html#392" class="Function">Pointed-Type</a> <a id="1064" class="Symbol">(</a><a id="1065" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1070" href="group-theory.examples-higher-groups.html#744" class="Bound">l</a><a id="1071" class="Symbol">)</a>
  <a id="1075" href="group-theory.examples-higher-groups.html#1006" class="Function">classifying-pointed-type-symmetric-∞-Group</a> <a id="1118" class="Symbol">=</a>
    <a id="1124" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
      <a id="1135" href="group-theory.examples-higher-groups.html#777" class="Function">classifying-type-symmetric-∞-Group</a>
      <a id="1176" href="group-theory.examples-higher-groups.html#883" class="Function">shape-symmetric-∞-Group</a>

  <a id="1203" href="group-theory.examples-higher-groups.html#1203" class="Function">is-path-connected-classifying-type-symmetric-∞-Group</a> <a id="1256" class="Symbol">:</a>
    <a id="1262" href="foundation.connected-types.html#1682" class="Function">is-path-connected</a> <a id="1280" href="group-theory.examples-higher-groups.html#777" class="Function">classifying-type-symmetric-∞-Group</a>
  <a id="1317" href="group-theory.examples-higher-groups.html#1203" class="Function">is-path-connected-classifying-type-symmetric-∞-Group</a> <a id="1370" class="Symbol">=</a>
    <a id="1376" href="foundation.connected-components-universes.html#6383" class="Function">is-path-connected-component-UU</a> <a id="1407" href="group-theory.examples-higher-groups.html#756" class="Bound">X</a>
  
  <a id="1414" href="group-theory.examples-higher-groups.html#1414" class="Function">symmetric-∞-Group</a> <a id="1432" class="Symbol">:</a> <a id="1434" href="group-theory.higher-groups.html#1500" class="Function">∞-Group</a> <a id="1442" class="Symbol">(</a><a id="1443" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1448" href="group-theory.examples-higher-groups.html#744" class="Bound">l</a><a id="1449" class="Symbol">)</a>
  <a id="1453" href="group-theory.examples-higher-groups.html#1414" class="Function">symmetric-∞-Group</a> <a id="1471" class="Symbol">=</a>
    <a id="1477" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
      <a id="1488" href="group-theory.examples-higher-groups.html#1006" class="Function">classifying-pointed-type-symmetric-∞-Group</a>
      <a id="1537" href="group-theory.examples-higher-groups.html#1203" class="Function">is-path-connected-classifying-type-symmetric-∞-Group</a>
</pre>