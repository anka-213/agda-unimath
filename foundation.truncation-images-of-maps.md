---
title: Truncation images of maps
---

<pre class="Agda"><a id="51" class="Keyword">module</a> <a id="58" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a> <a id="95" class="Keyword">where</a>

<a id="102" class="Keyword">open</a> <a id="107" class="Keyword">import</a> <a id="114" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="146" class="Keyword">open</a> <a id="151" class="Keyword">import</a> <a id="158" href="foundation.equality-dependent-pair-types.html" class="Module">foundation.equality-dependent-pair-types</a>
<a id="199" class="Keyword">open</a> <a id="204" class="Keyword">import</a> <a id="211" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="235" class="Keyword">open</a> <a id="240" class="Keyword">import</a> <a id="247" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="273" class="Keyword">open</a> <a id="278" class="Keyword">import</a> <a id="285" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a>
<a id="331" class="Keyword">open</a> <a id="336" class="Keyword">import</a> <a id="343" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="369" class="Keyword">open</a> <a id="374" class="Keyword">import</a> <a id="381" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="410" class="Keyword">open</a> <a id="415" class="Keyword">import</a> <a id="422" href="foundation.truncations.html" class="Module">foundation.truncations</a>
<a id="445" class="Keyword">open</a> <a id="450" class="Keyword">import</a> <a id="457" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

The **`k`-truncation image** of a map `f : A → B` is the type `trunc-im k f` that fits in the (`k`-connected,`k`-truncated) factorization of `f`. It is defined as the type

```md
  trunc-im k f := Σ (y : B), type-trunc k (fib f y)
```

## Definition

<pre class="Agda"><a id="757" class="Keyword">module</a> <a id="764" href="foundation.truncation-images-of-maps.html#764" class="Module">_</a>
  <a id="768" class="Symbol">{</a><a id="769" href="foundation.truncation-images-of-maps.html#769" class="Bound">l1</a> <a id="772" href="foundation.truncation-images-of-maps.html#772" class="Bound">l2</a> <a id="775" class="Symbol">:</a> <a id="777" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="782" class="Symbol">}</a> <a id="784" class="Symbol">(</a><a id="785" href="foundation.truncation-images-of-maps.html#785" class="Bound">k</a> <a id="787" class="Symbol">:</a> <a id="789" href="foundation-core.truncation-levels.html#395" class="Datatype">𝕋</a><a id="790" class="Symbol">)</a> <a id="792" class="Symbol">{</a><a id="793" href="foundation.truncation-images-of-maps.html#793" class="Bound">A</a> <a id="795" class="Symbol">:</a> <a id="797" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="800" href="foundation.truncation-images-of-maps.html#769" class="Bound">l1</a><a id="802" class="Symbol">}</a> <a id="804" class="Symbol">{</a><a id="805" href="foundation.truncation-images-of-maps.html#805" class="Bound">B</a> <a id="807" class="Symbol">:</a> <a id="809" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="812" href="foundation.truncation-images-of-maps.html#772" class="Bound">l2</a><a id="814" class="Symbol">}</a> <a id="816" class="Symbol">(</a><a id="817" href="foundation.truncation-images-of-maps.html#817" class="Bound">f</a> <a id="819" class="Symbol">:</a> <a id="821" href="foundation.truncation-images-of-maps.html#793" class="Bound">A</a> <a id="823" class="Symbol">→</a> <a id="825" href="foundation.truncation-images-of-maps.html#805" class="Bound">B</a><a id="826" class="Symbol">)</a>
  <a id="830" class="Keyword">where</a>
  
  <a id="841" href="foundation.truncation-images-of-maps.html#841" class="Function">trunc-im</a> <a id="850" class="Symbol">:</a> <a id="852" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="855" class="Symbol">(</a><a id="856" href="foundation.truncation-images-of-maps.html#769" class="Bound">l1</a> <a id="859" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="861" href="foundation.truncation-images-of-maps.html#772" class="Bound">l2</a><a id="863" class="Symbol">)</a>
  <a id="867" href="foundation.truncation-images-of-maps.html#841" class="Function">trunc-im</a> <a id="876" class="Symbol">=</a> <a id="878" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="880" href="foundation.truncation-images-of-maps.html#805" class="Bound">B</a> <a id="882" class="Symbol">(λ</a> <a id="885" href="foundation.truncation-images-of-maps.html#885" class="Bound">y</a> <a id="887" class="Symbol">→</a> <a id="889" href="foundation.truncations.html#2077" class="Postulate">type-trunc</a> <a id="900" href="foundation.truncation-images-of-maps.html#785" class="Bound">k</a> <a id="902" class="Symbol">(</a><a id="903" href="foundation-core.fibers-of-maps.html#942" class="Function">fib</a> <a id="907" href="foundation.truncation-images-of-maps.html#817" class="Bound">f</a> <a id="909" href="foundation.truncation-images-of-maps.html#885" class="Bound">y</a><a id="910" class="Symbol">))</a>

  <a id="916" href="foundation.truncation-images-of-maps.html#916" class="Function">unit-trunc-im</a> <a id="930" class="Symbol">:</a> <a id="932" href="foundation.truncation-images-of-maps.html#793" class="Bound">A</a> <a id="934" class="Symbol">→</a> <a id="936" href="foundation.truncation-images-of-maps.html#841" class="Function">trunc-im</a>
  <a id="947" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="951" class="Symbol">(</a><a id="952" href="foundation.truncation-images-of-maps.html#916" class="Function">unit-trunc-im</a> <a id="966" href="foundation.truncation-images-of-maps.html#966" class="Bound">x</a><a id="967" class="Symbol">)</a> <a id="969" class="Symbol">=</a> <a id="971" href="foundation.truncation-images-of-maps.html#817" class="Bound">f</a> <a id="973" href="foundation.truncation-images-of-maps.html#966" class="Bound">x</a>
  <a id="977" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="981" class="Symbol">(</a><a id="982" href="foundation.truncation-images-of-maps.html#916" class="Function">unit-trunc-im</a> <a id="996" href="foundation.truncation-images-of-maps.html#996" class="Bound">x</a><a id="997" class="Symbol">)</a> <a id="999" class="Symbol">=</a> <a id="1001" href="foundation.truncations.html#2365" class="Postulate">unit-trunc</a> <a id="1012" class="Symbol">(</a><a id="1013" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a> <a id="1018" href="foundation.truncation-images-of-maps.html#996" class="Bound">x</a> <a id="1020" href="foundation-core.identity-types.html#1820" class="InductiveConstructor">refl</a><a id="1024" class="Symbol">)</a>

  <a id="1029" href="foundation.truncation-images-of-maps.html#1029" class="Function">projection-trunc-im</a> <a id="1049" class="Symbol">:</a> <a id="1051" href="foundation.truncation-images-of-maps.html#841" class="Function">trunc-im</a> <a id="1060" class="Symbol">→</a> <a id="1062" href="foundation.truncation-images-of-maps.html#805" class="Bound">B</a>
  <a id="1066" href="foundation.truncation-images-of-maps.html#1029" class="Function">projection-trunc-im</a> <a id="1086" class="Symbol">=</a> <a id="1088" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a>
</pre>
## Properties

### Characterization of the identity types of `k+1`-truncation images

<pre class="Agda"><a id="1191" class="Keyword">module</a> <a id="1198" href="foundation.truncation-images-of-maps.html#1198" class="Module">_</a>
  <a id="1202" class="Symbol">{</a><a id="1203" href="foundation.truncation-images-of-maps.html#1203" class="Bound">l1</a> <a id="1206" href="foundation.truncation-images-of-maps.html#1206" class="Bound">l2</a> <a id="1209" class="Symbol">:</a> <a id="1211" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1216" class="Symbol">}</a> <a id="1218" class="Symbol">(</a><a id="1219" href="foundation.truncation-images-of-maps.html#1219" class="Bound">k</a> <a id="1221" class="Symbol">:</a> <a id="1223" href="foundation-core.truncation-levels.html#395" class="Datatype">𝕋</a><a id="1224" class="Symbol">)</a> <a id="1226" class="Symbol">{</a><a id="1227" href="foundation.truncation-images-of-maps.html#1227" class="Bound">A</a> <a id="1229" class="Symbol">:</a> <a id="1231" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1234" href="foundation.truncation-images-of-maps.html#1203" class="Bound">l1</a><a id="1236" class="Symbol">}</a> <a id="1238" class="Symbol">{</a><a id="1239" href="foundation.truncation-images-of-maps.html#1239" class="Bound">B</a> <a id="1241" class="Symbol">:</a> <a id="1243" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1246" href="foundation.truncation-images-of-maps.html#1206" class="Bound">l2</a><a id="1248" class="Symbol">}</a> <a id="1250" class="Symbol">(</a><a id="1251" href="foundation.truncation-images-of-maps.html#1251" class="Bound">f</a> <a id="1253" class="Symbol">:</a> <a id="1255" href="foundation.truncation-images-of-maps.html#1227" class="Bound">A</a> <a id="1257" class="Symbol">→</a> <a id="1259" href="foundation.truncation-images-of-maps.html#1239" class="Bound">B</a><a id="1260" class="Symbol">)</a>
  <a id="1264" class="Keyword">where</a>

  <a id="1273" href="foundation.truncation-images-of-maps.html#1273" class="Function">Eq-unit-trunc-im</a> <a id="1290" class="Symbol">:</a> <a id="1292" href="foundation.truncation-images-of-maps.html#1227" class="Bound">A</a> <a id="1294" class="Symbol">→</a> <a id="1296" href="foundation.truncation-images-of-maps.html#1227" class="Bound">A</a> <a id="1298" class="Symbol">→</a> <a id="1300" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1303" class="Symbol">(</a><a id="1304" href="foundation.truncation-images-of-maps.html#1203" class="Bound">l1</a> <a id="1307" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1309" href="foundation.truncation-images-of-maps.html#1206" class="Bound">l2</a><a id="1311" class="Symbol">)</a>
  <a id="1315" href="foundation.truncation-images-of-maps.html#1273" class="Function">Eq-unit-trunc-im</a> <a id="1332" href="foundation.truncation-images-of-maps.html#1332" class="Bound">x</a> <a id="1334" href="foundation.truncation-images-of-maps.html#1334" class="Bound">y</a> <a id="1336" class="Symbol">=</a> <a id="1338" href="foundation.truncation-images-of-maps.html#841" class="Function">trunc-im</a> <a id="1347" href="foundation.truncation-images-of-maps.html#1219" class="Bound">k</a> <a id="1349" class="Symbol">(</a><a id="1350" href="foundation-core.identity-types.html#4003" class="Function">ap</a> <a id="1353" href="foundation.truncation-images-of-maps.html#1251" class="Bound">f</a> <a id="1355" class="Symbol">{</a><a id="1356" href="foundation.truncation-images-of-maps.html#1332" class="Bound">x</a><a id="1357" class="Symbol">}</a> <a id="1359" class="Symbol">{</a><a id="1360" href="foundation.truncation-images-of-maps.html#1334" class="Bound">y</a><a id="1361" class="Symbol">})</a>

<a id="1365" class="Comment">{-
  extensionality-trunc-im :
    (x y : A) →
    ( unit-trunc-im (succ-𝕋 k) f x ＝ unit-trunc-im (succ-𝕋 k) f y) ≃
    ( Eq-unit-trunc-im x y)
  extensionality-trunc-im x y =
    ( equiv-tot
      ( λ q →
        {!!})) ∘e
    ( equiv-pair-eq-Σ
      ( unit-trunc-im (succ-𝕋 k) f x)
      ( unit-trunc-im (succ-𝕋 k) f y))
-}</a>
</pre>