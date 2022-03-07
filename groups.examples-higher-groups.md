---
title: Formalisation of the Symmetry Book
---

<pre class="Agda"><a id="60" class="Symbol">{-#</a> <a id="64" class="Keyword">OPTIONS</a> <a id="72" class="Pragma">--without-K</a> <a id="84" class="Pragma">--exact-split</a> <a id="98" class="Symbol">#-}</a>

<a id="103" class="Keyword">module</a> <a id="110" href="groups.examples-higher-groups.html" class="Module">groups.examples-higher-groups</a> <a id="140" class="Keyword">where</a>

<a id="147" class="Keyword">open</a> <a id="152" class="Keyword">import</a> <a id="159" href="groups.higher-groups.html" class="Module">groups.higher-groups</a> <a id="180" class="Keyword">public</a>
<a id="187" class="Keyword">open</a> <a id="192" class="Keyword">import</a> <a id="199" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a> <a id="232" class="Keyword">public</a>

<a id="240" class="Keyword">open</a> <a id="245" class="Keyword">import</a> <a id="252" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a>

<a id="293" class="Keyword">module</a> <a id="300" href="groups.examples-higher-groups.html#300" class="Module">_</a>
  <a id="304" class="Keyword">where</a>

  <a id="313" href="groups.examples-higher-groups.html#313" class="Function">classifying-type-ℤ-∞-Group</a> <a id="340" class="Symbol">:</a> <a id="342" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="345" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
  <a id="353" href="groups.examples-higher-groups.html#313" class="Function">classifying-type-ℤ-∞-Group</a> <a id="380" class="Symbol">=</a> <a id="382" href="synthetic-homotopy-theory.circle.html#11476" class="Postulate">𝕊¹</a>

  <a id="388" href="groups.examples-higher-groups.html#388" class="Function">shape-ℤ-∞-Group</a> <a id="404" class="Symbol">:</a> <a id="406" href="synthetic-homotopy-theory.circle.html#11476" class="Postulate">𝕊¹</a>
  <a id="411" href="groups.examples-higher-groups.html#388" class="Function">shape-ℤ-∞-Group</a> <a id="427" class="Symbol">=</a> <a id="429" href="synthetic-homotopy-theory.circle.html#11501" class="Postulate">base-𝕊¹</a>

  <a id="440" href="groups.examples-higher-groups.html#440" class="Function">classifying-pointed-type-ℤ-∞-Group</a> <a id="475" class="Symbol">:</a> <a id="477" href="synthetic-homotopy-theory.pointed-types.html#392" class="Function">Pointed-Type</a> <a id="490" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
  <a id="498" href="groups.examples-higher-groups.html#440" class="Function">classifying-pointed-type-ℤ-∞-Group</a> <a id="533" class="Symbol">=</a>
    <a id="539" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
      <a id="550" href="groups.examples-higher-groups.html#313" class="Function">classifying-type-ℤ-∞-Group</a>
      <a id="583" href="groups.examples-higher-groups.html#388" class="Function">shape-ℤ-∞-Group</a>

  <a id="602" href="groups.examples-higher-groups.html#602" class="Function">ℤ-∞-Group</a> <a id="612" class="Symbol">:</a> <a id="614" href="groups.higher-groups.html#1485" class="Function">∞-Group</a> <a id="622" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
  <a id="630" href="groups.examples-higher-groups.html#602" class="Function">ℤ-∞-Group</a> <a id="640" class="Symbol">=</a>
    <a id="646" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
      <a id="657" href="groups.examples-higher-groups.html#440" class="Function">classifying-pointed-type-ℤ-∞-Group</a>
      <a id="698" href="synthetic-homotopy-theory.circle.html#18994" class="Function">is-path-connected-𝕊¹</a>

<a id="720" class="Keyword">module</a> <a id="727" href="groups.examples-higher-groups.html#727" class="Module">_</a>
  <a id="731" class="Symbol">{</a><a id="732" href="groups.examples-higher-groups.html#732" class="Bound">l</a> <a id="734" class="Symbol">:</a> <a id="736" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="741" class="Symbol">}</a> <a id="743" class="Symbol">(</a><a id="744" href="groups.examples-higher-groups.html#744" class="Bound">X</a> <a id="746" class="Symbol">:</a> <a id="748" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="751" href="groups.examples-higher-groups.html#732" class="Bound">l</a><a id="752" class="Symbol">)</a>
  <a id="756" class="Keyword">where</a>

  <a id="765" href="groups.examples-higher-groups.html#765" class="Function">classifying-type-symmetric-∞-Group</a> <a id="800" class="Symbol">:</a> <a id="802" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="805" class="Symbol">(</a><a id="806" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="811" href="groups.examples-higher-groups.html#732" class="Bound">l</a><a id="812" class="Symbol">)</a>
  <a id="816" href="groups.examples-higher-groups.html#765" class="Function">classifying-type-symmetric-∞-Group</a> <a id="851" class="Symbol">=</a> <a id="853" href="foundation.connected-components-universes.html#2310" class="Function">component-UU</a> <a id="866" href="groups.examples-higher-groups.html#744" class="Bound">X</a>

  <a id="871" href="groups.examples-higher-groups.html#871" class="Function">shape-symmetric-∞-Group</a> <a id="895" class="Symbol">:</a> <a id="897" href="groups.examples-higher-groups.html#765" class="Function">classifying-type-symmetric-∞-Group</a>
  <a id="934" href="groups.examples-higher-groups.html#871" class="Function">shape-symmetric-∞-Group</a> <a id="958" class="Symbol">=</a>
    <a id="964" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a> <a id="969" href="groups.examples-higher-groups.html#744" class="Bound">X</a> <a id="971" class="Symbol">(</a><a id="972" href="foundation.mere-equivalences.html#1762" class="Function">refl-mere-equiv</a> <a id="988" href="groups.examples-higher-groups.html#744" class="Bound">X</a><a id="989" class="Symbol">)</a>

  <a id="994" href="groups.examples-higher-groups.html#994" class="Function">classifying-pointed-type-symmetric-∞-Group</a> <a id="1037" class="Symbol">:</a> <a id="1039" href="synthetic-homotopy-theory.pointed-types.html#392" class="Function">Pointed-Type</a> <a id="1052" class="Symbol">(</a><a id="1053" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1058" href="groups.examples-higher-groups.html#732" class="Bound">l</a><a id="1059" class="Symbol">)</a>
  <a id="1063" href="groups.examples-higher-groups.html#994" class="Function">classifying-pointed-type-symmetric-∞-Group</a> <a id="1106" class="Symbol">=</a>
    <a id="1112" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
      <a id="1123" href="groups.examples-higher-groups.html#765" class="Function">classifying-type-symmetric-∞-Group</a>
      <a id="1164" href="groups.examples-higher-groups.html#871" class="Function">shape-symmetric-∞-Group</a>

  <a id="1191" href="groups.examples-higher-groups.html#1191" class="Function">is-path-connected-classifying-type-symmetric-∞-Group</a> <a id="1244" class="Symbol">:</a>
    <a id="1250" href="foundation.connected-types.html#1682" class="Function">is-path-connected</a> <a id="1268" href="groups.examples-higher-groups.html#765" class="Function">classifying-type-symmetric-∞-Group</a>
  <a id="1305" href="groups.examples-higher-groups.html#1191" class="Function">is-path-connected-classifying-type-symmetric-∞-Group</a> <a id="1358" class="Symbol">=</a>
    <a id="1364" href="foundation.connected-components-universes.html#6383" class="Function">is-path-connected-component-UU</a> <a id="1395" href="groups.examples-higher-groups.html#744" class="Bound">X</a>
  
  <a id="1402" href="groups.examples-higher-groups.html#1402" class="Function">symmetric-∞-Group</a> <a id="1420" class="Symbol">:</a> <a id="1422" href="groups.higher-groups.html#1485" class="Function">∞-Group</a> <a id="1430" class="Symbol">(</a><a id="1431" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1436" href="groups.examples-higher-groups.html#732" class="Bound">l</a><a id="1437" class="Symbol">)</a>
  <a id="1441" href="groups.examples-higher-groups.html#1402" class="Function">symmetric-∞-Group</a> <a id="1459" class="Symbol">=</a>
    <a id="1465" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a>
      <a id="1476" href="groups.examples-higher-groups.html#994" class="Function">classifying-pointed-type-symmetric-∞-Group</a>
      <a id="1525" href="groups.examples-higher-groups.html#1191" class="Function">is-path-connected-classifying-type-symmetric-∞-Group</a>
</pre>