---
title: Global choice
---

<pre class="Agda"><a id="39" class="Symbol">{-#</a> <a id="43" class="Keyword">OPTIONS</a> <a id="51" class="Pragma">--without-K</a> <a id="63" class="Pragma">--exact-split</a> <a id="77" class="Symbol">#-}</a>

<a id="82" class="Keyword">module</a> <a id="89" href="foundation.global-choice.html" class="Module">foundation.global-choice</a> <a id="114" class="Keyword">where</a>

<a id="121" class="Keyword">open</a> <a id="126" class="Keyword">import</a> <a id="133" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="165" class="Keyword">using</a> <a id="171" class="Symbol">(</a><a id="172" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a><a id="173" class="Symbol">;</a> <a id="175" href="foundation-core.dependent-pair-types.html#588" class="InductiveConstructor">pair</a><a id="179" class="Symbol">;</a> <a id="181" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a><a id="184" class="Symbol">;</a> <a id="186" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a><a id="189" class="Symbol">)</a>
<a id="191" class="Keyword">open</a> <a id="196" class="Keyword">import</a> <a id="203" href="foundation.equivalences.html" class="Module">foundation.equivalences</a> <a id="227" class="Keyword">using</a> <a id="233" class="Symbol">(</a><a id="234" href="foundation-core.equivalences.html#1821" class="Function">map-equiv</a><a id="243" class="Symbol">)</a>
<a id="245" class="Keyword">open</a> <a id="250" class="Keyword">import</a> <a id="257" href="foundation.functoriality-propositional-truncation.html" class="Module">foundation.functoriality-propositional-truncation</a> <a id="307" class="Keyword">using</a>
  <a id="315" class="Symbol">(</a> <a id="317" href="foundation.functoriality-propositional-truncation.html#1456" class="Function">map-trunc-Prop</a><a id="331" class="Symbol">)</a>
<a id="333" class="Keyword">open</a> <a id="338" class="Keyword">import</a> <a id="345" href="foundation.hilberts-epsilon-operators.html" class="Module">foundation.hilberts-epsilon-operators</a> <a id="383" class="Keyword">using</a>
  <a id="391" class="Symbol">(</a> <a id="393" href="foundation.hilberts-epsilon-operators.html#675" class="Function">ε-operator-Hilbert</a><a id="411" class="Symbol">)</a>
<a id="413" class="Keyword">open</a> <a id="418" class="Keyword">import</a> <a id="425" href="foundation.negation.html" class="Module">foundation.negation</a> <a id="445" class="Keyword">using</a> <a id="451" class="Symbol">(</a><a id="452" href="foundation-core.negation.html#465" class="Function">¬</a><a id="453" class="Symbol">)</a>
<a id="455" class="Keyword">open</a> <a id="460" class="Keyword">import</a> <a id="467" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a> <a id="504" class="Keyword">using</a>
  <a id="512" class="Symbol">(</a> <a id="514" href="foundation.propositional-truncations.html#2209" class="Function">type-trunc-Prop</a><a id="529" class="Symbol">;</a> <a id="531" href="foundation.propositional-truncations.html#5775" class="Function">apply-universal-property-trunc-Prop</a><a id="566" class="Symbol">)</a>
<a id="568" class="Keyword">open</a> <a id="573" class="Keyword">import</a> <a id="580" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="607" class="Keyword">using</a> <a id="613" class="Symbol">(</a><a id="614" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="619" class="Symbol">;</a> <a id="621" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a><a id="623" class="Symbol">;</a> <a id="625" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="629" class="Symbol">)</a>

<a id="632" class="Keyword">open</a> <a id="637" class="Keyword">import</a> <a id="644" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a> <a id="684" class="Keyword">using</a>
  <a id="692" class="Symbol">(</a> <a id="694" href="univalent-combinatorics.2-element-types.html#17855" class="Function">no-section-type-UU-Fin-two-ℕ</a><a id="722" class="Symbol">)</a>
<a id="724" class="Keyword">open</a> <a id="729" class="Keyword">import</a> <a id="736" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a> <a id="782" class="Keyword">using</a>
  <a id="790" class="Symbol">(</a> <a id="792" href="univalent-combinatorics.standard-finite-types.html#6791" class="Function">zero-Fin</a><a id="800" class="Symbol">)</a>
</pre>
## Idea

Global choice is the principle that there is a map from `type-trunc-Prop A` back into `A`, for any type `A`. Here, we say that a type `A` satisfies global choice if there is such a map.

## Definition

### The global choice principle

<pre class="Agda"><a id="Global-Choice"></a><a id="1059" href="foundation.global-choice.html#1059" class="Function">Global-Choice</a> <a id="1073" class="Symbol">:</a> <a id="1075" class="Symbol">(</a><a id="1076" href="foundation.global-choice.html#1076" class="Bound">l</a> <a id="1078" class="Symbol">:</a> <a id="1080" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1085" class="Symbol">)</a> <a id="1087" class="Symbol">→</a> <a id="1089" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1092" class="Symbol">(</a><a id="1093" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1098" href="foundation.global-choice.html#1076" class="Bound">l</a><a id="1099" class="Symbol">)</a>
<a id="1101" href="foundation.global-choice.html#1059" class="Function">Global-Choice</a> <a id="1115" href="foundation.global-choice.html#1115" class="Bound">l</a> <a id="1117" class="Symbol">=</a> <a id="1119" class="Symbol">(</a><a id="1120" href="foundation.global-choice.html#1120" class="Bound">A</a> <a id="1122" class="Symbol">:</a> <a id="1124" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1127" href="foundation.global-choice.html#1115" class="Bound">l</a><a id="1128" class="Symbol">)</a> <a id="1130" class="Symbol">→</a> <a id="1132" href="foundation.hilberts-epsilon-operators.html#675" class="Function">ε-operator-Hilbert</a> <a id="1151" href="foundation.global-choice.html#1120" class="Bound">A</a>
</pre>
## Properties

### The global choice principle is inconsistent in `agda-unimath`

<pre class="Agda"><a id="1248" class="Keyword">abstract</a>
  <a id="no-global-choice"></a><a id="1259" href="foundation.global-choice.html#1259" class="Function">no-global-choice</a> <a id="1276" class="Symbol">:</a>
    <a id="1282" class="Symbol">{</a><a id="1283" href="foundation.global-choice.html#1283" class="Bound">l</a> <a id="1285" class="Symbol">:</a> <a id="1287" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1292" class="Symbol">}</a> <a id="1294" class="Symbol">→</a> <a id="1296" href="foundation-core.negation.html#465" class="Function">¬</a> <a id="1298" class="Symbol">(</a><a id="1299" href="foundation.global-choice.html#1059" class="Function">Global-Choice</a> <a id="1313" href="foundation.global-choice.html#1283" class="Bound">l</a><a id="1314" class="Symbol">)</a>
  <a id="1318" href="foundation.global-choice.html#1259" class="Function">no-global-choice</a> <a id="1335" href="foundation.global-choice.html#1335" class="Bound">f</a> <a id="1337" class="Symbol">=</a>
    <a id="1343" href="univalent-combinatorics.2-element-types.html#17855" class="Function">no-section-type-UU-Fin-two-ℕ</a>
      <a id="1378" class="Symbol">(</a> <a id="1380" class="Symbol">λ</a> <a id="1382" href="foundation.global-choice.html#1382" class="Bound">X</a> <a id="1384" class="Symbol">→</a>
        <a id="1394" href="foundation.global-choice.html#1335" class="Bound">f</a> <a id="1396" class="Symbol">(</a><a id="1397" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1401" href="foundation.global-choice.html#1382" class="Bound">X</a><a id="1402" class="Symbol">)</a> <a id="1404" class="Symbol">(</a><a id="1405" href="foundation.functoriality-propositional-truncation.html#1456" class="Function">map-trunc-Prop</a> <a id="1420" class="Symbol">(λ</a> <a id="1423" href="foundation.global-choice.html#1423" class="Bound">e</a> <a id="1425" class="Symbol">→</a> <a id="1427" href="foundation-core.equivalences.html#1821" class="Function">map-equiv</a> <a id="1437" href="foundation.global-choice.html#1423" class="Bound">e</a> <a id="1439" class="Symbol">(</a><a id="1440" href="univalent-combinatorics.standard-finite-types.html#6791" class="Function">zero-Fin</a> <a id="1449" class="Number">1</a><a id="1450" class="Symbol">))</a> <a id="1453" class="Symbol">(</a><a id="1454" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="1458" href="foundation.global-choice.html#1382" class="Bound">X</a><a id="1459" class="Symbol">)))</a>
</pre>