---
title: 0-Images of maps
---

<pre class="Agda"><a id="42" class="Keyword">module</a> <a id="49" href="foundation.0-images-of-maps.html" class="Module">foundation.0-images-of-maps</a> <a id="77" class="Keyword">where</a>

<a id="84" class="Keyword">open</a> <a id="89" class="Keyword">import</a> <a id="96" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="128" class="Keyword">open</a> <a id="133" class="Keyword">import</a> <a id="140" href="foundation.fibers-of-maps.html" class="Module">foundation.fibers-of-maps</a>
<a id="166" class="Keyword">open</a> <a id="171" class="Keyword">import</a> <a id="178" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="204" class="Keyword">open</a> <a id="209" class="Keyword">import</a> <a id="216" href="foundation.images.html" class="Module">foundation.images</a>
<a id="234" class="Keyword">open</a> <a id="239" class="Keyword">import</a> <a id="246" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="283" class="Keyword">open</a> <a id="288" class="Keyword">import</a> <a id="295" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="322" class="Keyword">open</a> <a id="327" class="Keyword">import</a> <a id="334" href="foundation.truncation-images-of-maps.html" class="Module">foundation.truncation-images-of-maps</a>
<a id="371" class="Keyword">open</a> <a id="376" class="Keyword">import</a> <a id="383" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a>
<a id="412" class="Keyword">open</a> <a id="417" class="Keyword">import</a> <a id="424" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
</pre>
## Idea

The 0-image of a map `f : A → B` is the type `0-im f := Σ (b : B), type-trunc-Set (fib f b)`. The map `A → 0-im f` is 0-connected and the map `0-im f → B` is `0`-truncated.

## Definition

<pre class="Agda"><a id="662" class="Keyword">module</a> <a id="669" href="foundation.0-images-of-maps.html#669" class="Module">_</a>
  <a id="673" class="Symbol">{</a><a id="674" href="foundation.0-images-of-maps.html#674" class="Bound">l1</a> <a id="677" href="foundation.0-images-of-maps.html#677" class="Bound">l2</a> <a id="680" class="Symbol">:</a> <a id="682" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="687" class="Symbol">}</a> <a id="689" class="Symbol">{</a><a id="690" href="foundation.0-images-of-maps.html#690" class="Bound">A</a> <a id="692" class="Symbol">:</a> <a id="694" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="697" href="foundation.0-images-of-maps.html#674" class="Bound">l1</a><a id="699" class="Symbol">}</a> <a id="701" class="Symbol">{</a><a id="702" href="foundation.0-images-of-maps.html#702" class="Bound">B</a> <a id="704" class="Symbol">:</a> <a id="706" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="709" href="foundation.0-images-of-maps.html#677" class="Bound">l2</a><a id="711" class="Symbol">}</a> <a id="713" class="Symbol">(</a><a id="714" href="foundation.0-images-of-maps.html#714" class="Bound">f</a> <a id="716" class="Symbol">:</a> <a id="718" href="foundation.0-images-of-maps.html#690" class="Bound">A</a> <a id="720" class="Symbol">→</a> <a id="722" href="foundation.0-images-of-maps.html#702" class="Bound">B</a><a id="723" class="Symbol">)</a>
  <a id="727" class="Keyword">where</a>
  
  <a id="738" href="foundation.0-images-of-maps.html#738" class="Function">0-im</a> <a id="743" class="Symbol">:</a> <a id="745" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="748" class="Symbol">(</a><a id="749" href="foundation.0-images-of-maps.html#674" class="Bound">l1</a> <a id="752" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="754" href="foundation.0-images-of-maps.html#677" class="Bound">l2</a><a id="756" class="Symbol">)</a>
  <a id="760" href="foundation.0-images-of-maps.html#738" class="Function">0-im</a> <a id="765" class="Symbol">=</a> <a id="767" href="foundation.truncation-images-of-maps.html#841" class="Function">trunc-im</a> <a id="776" href="foundation-core.truncation-levels.html#492" class="Function">zero-𝕋</a> <a id="783" href="foundation.0-images-of-maps.html#714" class="Bound">f</a>

  <a id="788" href="foundation.0-images-of-maps.html#788" class="Function">unit-0-im</a> <a id="798" class="Symbol">:</a> <a id="800" href="foundation.0-images-of-maps.html#690" class="Bound">A</a> <a id="802" class="Symbol">→</a> <a id="804" href="foundation.0-images-of-maps.html#738" class="Function">0-im</a>
  <a id="811" href="foundation.0-images-of-maps.html#788" class="Function">unit-0-im</a> <a id="821" class="Symbol">=</a> <a id="823" href="foundation.truncation-images-of-maps.html#916" class="Function">unit-trunc-im</a> <a id="837" href="foundation-core.truncation-levels.html#492" class="Function">zero-𝕋</a> <a id="844" href="foundation.0-images-of-maps.html#714" class="Bound">f</a>

  <a id="849" href="foundation.0-images-of-maps.html#849" class="Function">projection-0-im</a> <a id="865" class="Symbol">:</a> <a id="867" href="foundation.0-images-of-maps.html#738" class="Function">0-im</a> <a id="872" class="Symbol">→</a> <a id="874" href="foundation.0-images-of-maps.html#702" class="Bound">B</a>
  <a id="878" href="foundation.0-images-of-maps.html#849" class="Function">projection-0-im</a> <a id="894" class="Symbol">=</a> <a id="896" href="foundation.truncation-images-of-maps.html#1029" class="Function">projection-trunc-im</a> <a id="916" href="foundation-core.truncation-levels.html#492" class="Function">zero-𝕋</a> <a id="923" href="foundation.0-images-of-maps.html#714" class="Bound">f</a>
</pre>
## Properties

### Characterization of the identity type of `0-im f`

<pre class="Agda"><a id="1008" class="Keyword">module</a> <a id="1015" href="foundation.0-images-of-maps.html#1015" class="Module">_</a>
  <a id="1019" class="Symbol">{</a><a id="1020" href="foundation.0-images-of-maps.html#1020" class="Bound">l1</a> <a id="1023" href="foundation.0-images-of-maps.html#1023" class="Bound">l2</a> <a id="1026" class="Symbol">:</a> <a id="1028" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1033" class="Symbol">}</a> <a id="1035" class="Symbol">{</a><a id="1036" href="foundation.0-images-of-maps.html#1036" class="Bound">A</a> <a id="1038" class="Symbol">:</a> <a id="1040" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1043" href="foundation.0-images-of-maps.html#1020" class="Bound">l1</a><a id="1045" class="Symbol">}</a> <a id="1047" class="Symbol">{</a><a id="1048" href="foundation.0-images-of-maps.html#1048" class="Bound">B</a> <a id="1050" class="Symbol">:</a> <a id="1052" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1055" href="foundation.0-images-of-maps.html#1023" class="Bound">l2</a><a id="1057" class="Symbol">}</a> <a id="1059" class="Symbol">(</a><a id="1060" href="foundation.0-images-of-maps.html#1060" class="Bound">f</a> <a id="1062" class="Symbol">:</a> <a id="1064" href="foundation.0-images-of-maps.html#1036" class="Bound">A</a> <a id="1066" class="Symbol">→</a> <a id="1068" href="foundation.0-images-of-maps.html#1048" class="Bound">B</a><a id="1069" class="Symbol">)</a>
  <a id="1073" class="Keyword">where</a>

  <a id="1082" href="foundation.0-images-of-maps.html#1082" class="Function">Eq-unit-0-im</a> <a id="1095" class="Symbol">:</a> <a id="1097" href="foundation.0-images-of-maps.html#1036" class="Bound">A</a> <a id="1099" class="Symbol">→</a> <a id="1101" href="foundation.0-images-of-maps.html#1036" class="Bound">A</a> <a id="1103" class="Symbol">→</a> <a id="1105" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1108" class="Symbol">(</a><a id="1109" href="foundation.0-images-of-maps.html#1020" class="Bound">l1</a> <a id="1112" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1114" href="foundation.0-images-of-maps.html#1023" class="Bound">l2</a><a id="1116" class="Symbol">)</a>
  <a id="1120" href="foundation.0-images-of-maps.html#1082" class="Function">Eq-unit-0-im</a> <a id="1133" class="Symbol">=</a> <a id="1135" href="foundation.truncation-images-of-maps.html#1273" class="Function">Eq-unit-trunc-im</a> <a id="1152" href="foundation-core.truncation-levels.html#448" class="Function">neg-one-𝕋</a> <a id="1162" href="foundation.0-images-of-maps.html#1060" class="Bound">f</a>
</pre>