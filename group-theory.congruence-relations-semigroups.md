---
title: Congruence relations on semigroups
---

<pre class="Agda"><a id="60" class="Keyword">module</a> <a id="67" href="group-theory.congruence-relations-semigroups.html" class="Module">group-theory.congruence-relations-semigroups</a> <a id="112" class="Keyword">where</a>

<a id="119" class="Keyword">open</a> <a id="124" class="Keyword">import</a> <a id="131" href="foundation.binary-relations.html" class="Module">foundation.binary-relations</a>
<a id="159" class="Keyword">open</a> <a id="164" class="Keyword">import</a> <a id="171" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="203" class="Keyword">open</a> <a id="208" class="Keyword">import</a> <a id="215" href="foundation.equivalence-relations.html" class="Module">foundation.equivalence-relations</a>
<a id="248" class="Keyword">open</a> <a id="253" class="Keyword">import</a> <a id="260" href="foundation.equivalences.html" class="Module">foundation.equivalences</a>
<a id="284" class="Keyword">open</a> <a id="289" class="Keyword">import</a> <a id="296" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="320" class="Keyword">open</a> <a id="325" class="Keyword">import</a> <a id="332" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="360" class="Keyword">open</a> <a id="365" class="Keyword">import</a> <a id="372" href="group-theory.semigroups.html" class="Module">group-theory.semigroups</a>
</pre>
## Idea

A congruence relation on a semigroup `G` is an equivalence relation `≡` on `G` such that for every `x1 x2 y1 y2 : G` such that `x1 ≡ x2` and `y1 ≡ y2` we have `x1 · y1 ≡ x2 · y2`.

## Definition

<pre class="Agda"><a id="is-congruence-Eq-Rel-Semigroup"></a><a id="614" href="group-theory.congruence-relations-semigroups.html#614" class="Function">is-congruence-Eq-Rel-Semigroup</a> <a id="645" class="Symbol">:</a>
  <a id="649" class="Symbol">{</a><a id="650" href="group-theory.congruence-relations-semigroups.html#650" class="Bound">l1</a> <a id="653" href="group-theory.congruence-relations-semigroups.html#653" class="Bound">l2</a> <a id="656" class="Symbol">:</a> <a id="658" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="663" class="Symbol">}</a> <a id="665" class="Symbol">(</a><a id="666" href="group-theory.congruence-relations-semigroups.html#666" class="Bound">G</a> <a id="668" class="Symbol">:</a> <a id="670" href="group-theory.semigroups.html#750" class="Function">Semigroup</a> <a id="680" href="group-theory.congruence-relations-semigroups.html#650" class="Bound">l1</a><a id="682" class="Symbol">)</a> <a id="684" class="Symbol">→</a> <a id="686" href="foundation.equivalence-relations.html#996" class="Function">Eq-Rel</a> <a id="693" href="group-theory.congruence-relations-semigroups.html#653" class="Bound">l2</a> <a id="696" class="Symbol">(</a><a id="697" href="group-theory.semigroups.html#946" class="Function">type-Semigroup</a> <a id="712" href="group-theory.congruence-relations-semigroups.html#666" class="Bound">G</a><a id="713" class="Symbol">)</a> <a id="715" class="Symbol">→</a> <a id="717" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="720" class="Symbol">(</a><a id="721" href="group-theory.congruence-relations-semigroups.html#650" class="Bound">l1</a> <a id="724" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="726" href="group-theory.congruence-relations-semigroups.html#653" class="Bound">l2</a><a id="728" class="Symbol">)</a>
<a id="730" href="group-theory.congruence-relations-semigroups.html#614" class="Function">is-congruence-Eq-Rel-Semigroup</a> <a id="761" href="group-theory.congruence-relations-semigroups.html#761" class="Bound">G</a> <a id="763" href="group-theory.congruence-relations-semigroups.html#763" class="Bound">R</a> <a id="765" class="Symbol">=</a>
  <a id="769" class="Symbol">{</a><a id="770" href="group-theory.congruence-relations-semigroups.html#770" class="Bound">x1</a> <a id="773" href="group-theory.congruence-relations-semigroups.html#773" class="Bound">x2</a> <a id="776" href="group-theory.congruence-relations-semigroups.html#776" class="Bound">y1</a> <a id="779" href="group-theory.congruence-relations-semigroups.html#779" class="Bound">y2</a> <a id="782" class="Symbol">:</a> <a id="784" href="group-theory.semigroups.html#946" class="Function">type-Semigroup</a> <a id="799" href="group-theory.congruence-relations-semigroups.html#761" class="Bound">G</a><a id="800" class="Symbol">}</a> <a id="802" class="Symbol">→</a> <a id="804" href="foundation.equivalence-relations.html#1213" class="Function">sim-Eq-Rel</a> <a id="815" href="group-theory.congruence-relations-semigroups.html#763" class="Bound">R</a> <a id="817" href="group-theory.congruence-relations-semigroups.html#770" class="Bound">x1</a> <a id="820" href="group-theory.congruence-relations-semigroups.html#773" class="Bound">x2</a> <a id="823" class="Symbol">→</a> <a id="825" href="foundation.equivalence-relations.html#1213" class="Function">sim-Eq-Rel</a> <a id="836" href="group-theory.congruence-relations-semigroups.html#763" class="Bound">R</a> <a id="838" href="group-theory.congruence-relations-semigroups.html#776" class="Bound">y1</a> <a id="841" href="group-theory.congruence-relations-semigroups.html#779" class="Bound">y2</a> <a id="844" class="Symbol">→</a>
  <a id="848" href="foundation.equivalence-relations.html#1213" class="Function">sim-Eq-Rel</a> <a id="859" href="group-theory.congruence-relations-semigroups.html#763" class="Bound">R</a> <a id="861" class="Symbol">(</a><a id="862" href="group-theory.semigroups.html#1228" class="Function">mul-Semigroup</a> <a id="876" href="group-theory.congruence-relations-semigroups.html#761" class="Bound">G</a> <a id="878" href="group-theory.congruence-relations-semigroups.html#770" class="Bound">x1</a> <a id="881" href="group-theory.congruence-relations-semigroups.html#776" class="Bound">y1</a><a id="883" class="Symbol">)</a> <a id="885" class="Symbol">(</a><a id="886" href="group-theory.semigroups.html#1228" class="Function">mul-Semigroup</a> <a id="900" href="group-theory.congruence-relations-semigroups.html#761" class="Bound">G</a> <a id="902" href="group-theory.congruence-relations-semigroups.html#773" class="Bound">x2</a> <a id="905" href="group-theory.congruence-relations-semigroups.html#779" class="Bound">y2</a><a id="907" class="Symbol">)</a>

<a id="congruence-Semigroup"></a><a id="910" href="group-theory.congruence-relations-semigroups.html#910" class="Function">congruence-Semigroup</a> <a id="931" class="Symbol">:</a> <a id="933" class="Symbol">{</a><a id="934" href="group-theory.congruence-relations-semigroups.html#934" class="Bound">l</a> <a id="936" class="Symbol">:</a> <a id="938" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="943" class="Symbol">}</a> <a id="945" class="Symbol">(</a><a id="946" href="group-theory.congruence-relations-semigroups.html#946" class="Bound">l2</a> <a id="949" class="Symbol">:</a> <a id="951" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="956" class="Symbol">)</a> <a id="958" class="Symbol">(</a><a id="959" href="group-theory.congruence-relations-semigroups.html#959" class="Bound">G</a> <a id="961" class="Symbol">:</a> <a id="963" href="group-theory.semigroups.html#750" class="Function">Semigroup</a> <a id="973" href="group-theory.congruence-relations-semigroups.html#934" class="Bound">l</a><a id="974" class="Symbol">)</a> <a id="976" class="Symbol">→</a> <a id="978" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="981" class="Symbol">(</a><a id="982" href="group-theory.congruence-relations-semigroups.html#934" class="Bound">l</a> <a id="984" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="986" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="991" href="group-theory.congruence-relations-semigroups.html#946" class="Bound">l2</a><a id="993" class="Symbol">)</a>
<a id="995" href="group-theory.congruence-relations-semigroups.html#910" class="Function">congruence-Semigroup</a> <a id="1016" href="group-theory.congruence-relations-semigroups.html#1016" class="Bound">l2</a> <a id="1019" href="group-theory.congruence-relations-semigroups.html#1019" class="Bound">G</a> <a id="1021" class="Symbol">=</a>
  <a id="1025" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1027" class="Symbol">(</a><a id="1028" href="foundation.equivalence-relations.html#996" class="Function">Eq-Rel</a> <a id="1035" href="group-theory.congruence-relations-semigroups.html#1016" class="Bound">l2</a> <a id="1038" class="Symbol">(</a><a id="1039" href="group-theory.semigroups.html#946" class="Function">type-Semigroup</a> <a id="1054" href="group-theory.congruence-relations-semigroups.html#1019" class="Bound">G</a><a id="1055" class="Symbol">))</a> <a id="1058" class="Symbol">(</a><a id="1059" href="group-theory.congruence-relations-semigroups.html#614" class="Function">is-congruence-Eq-Rel-Semigroup</a> <a id="1090" href="group-theory.congruence-relations-semigroups.html#1019" class="Bound">G</a><a id="1091" class="Symbol">)</a>

<a id="1094" class="Keyword">module</a> <a id="1101" href="group-theory.congruence-relations-semigroups.html#1101" class="Module">_</a>
  <a id="1105" class="Symbol">{</a><a id="1106" href="group-theory.congruence-relations-semigroups.html#1106" class="Bound">l1</a> <a id="1109" href="group-theory.congruence-relations-semigroups.html#1109" class="Bound">l2</a> <a id="1112" class="Symbol">:</a> <a id="1114" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1119" class="Symbol">}</a> <a id="1121" class="Symbol">(</a><a id="1122" href="group-theory.congruence-relations-semigroups.html#1122" class="Bound">G</a> <a id="1124" class="Symbol">:</a> <a id="1126" href="group-theory.semigroups.html#750" class="Function">Semigroup</a> <a id="1136" href="group-theory.congruence-relations-semigroups.html#1106" class="Bound">l1</a><a id="1138" class="Symbol">)</a> <a id="1140" class="Symbol">(</a><a id="1141" href="group-theory.congruence-relations-semigroups.html#1141" class="Bound">R</a> <a id="1143" class="Symbol">:</a> <a id="1145" href="group-theory.congruence-relations-semigroups.html#910" class="Function">congruence-Semigroup</a> <a id="1166" href="group-theory.congruence-relations-semigroups.html#1109" class="Bound">l2</a> <a id="1169" href="group-theory.congruence-relations-semigroups.html#1122" class="Bound">G</a><a id="1170" class="Symbol">)</a>
  <a id="1174" class="Keyword">where</a>

  <a id="1183" href="group-theory.congruence-relations-semigroups.html#1183" class="Function">eq-rel-congruence-Semigroup</a> <a id="1211" class="Symbol">:</a> <a id="1213" href="foundation.equivalence-relations.html#996" class="Function">Eq-Rel</a> <a id="1220" href="group-theory.congruence-relations-semigroups.html#1109" class="Bound">l2</a> <a id="1223" class="Symbol">(</a><a id="1224" href="group-theory.semigroups.html#946" class="Function">type-Semigroup</a> <a id="1239" href="group-theory.congruence-relations-semigroups.html#1122" class="Bound">G</a><a id="1240" class="Symbol">)</a>
  <a id="1244" href="group-theory.congruence-relations-semigroups.html#1183" class="Function">eq-rel-congruence-Semigroup</a> <a id="1272" class="Symbol">=</a> <a id="1274" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1278" href="group-theory.congruence-relations-semigroups.html#1141" class="Bound">R</a>

  <a id="1283" href="group-theory.congruence-relations-semigroups.html#1283" class="Function">prop-congruence-Semigroup</a> <a id="1309" class="Symbol">:</a> <a id="1311" href="foundation.binary-relations.html#768" class="Function">Rel-Prop</a> <a id="1320" href="group-theory.congruence-relations-semigroups.html#1109" class="Bound">l2</a> <a id="1323" class="Symbol">(</a><a id="1324" href="group-theory.semigroups.html#946" class="Function">type-Semigroup</a> <a id="1339" href="group-theory.congruence-relations-semigroups.html#1122" class="Bound">G</a><a id="1340" class="Symbol">)</a>
  <a id="1344" href="group-theory.congruence-relations-semigroups.html#1283" class="Function">prop-congruence-Semigroup</a> <a id="1370" class="Symbol">=</a> <a id="1372" href="foundation.equivalence-relations.html#1120" class="Function">prop-Eq-Rel</a> <a id="1384" href="group-theory.congruence-relations-semigroups.html#1183" class="Function">eq-rel-congruence-Semigroup</a>

  <a id="1415" href="group-theory.congruence-relations-semigroups.html#1415" class="Function">sim-congruence-Semigroup</a> <a id="1440" class="Symbol">:</a> <a id="1442" class="Symbol">(</a><a id="1443" href="group-theory.congruence-relations-semigroups.html#1443" class="Bound">x</a> <a id="1445" href="group-theory.congruence-relations-semigroups.html#1445" class="Bound">y</a> <a id="1447" class="Symbol">:</a> <a id="1449" href="group-theory.semigroups.html#946" class="Function">type-Semigroup</a> <a id="1464" href="group-theory.congruence-relations-semigroups.html#1122" class="Bound">G</a><a id="1465" class="Symbol">)</a> <a id="1467" class="Symbol">→</a> <a id="1469" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1472" href="group-theory.congruence-relations-semigroups.html#1109" class="Bound">l2</a>
  <a id="1477" href="group-theory.congruence-relations-semigroups.html#1415" class="Function">sim-congruence-Semigroup</a> <a id="1502" class="Symbol">=</a> <a id="1504" href="foundation.equivalence-relations.html#1213" class="Function">sim-Eq-Rel</a> <a id="1515" href="group-theory.congruence-relations-semigroups.html#1183" class="Function">eq-rel-congruence-Semigroup</a>

  <a id="1546" href="group-theory.congruence-relations-semigroups.html#1546" class="Function">is-prop-sim-congruence-Semigroup</a> <a id="1579" class="Symbol">:</a>
    <a id="1585" class="Symbol">(</a><a id="1586" href="group-theory.congruence-relations-semigroups.html#1586" class="Bound">x</a> <a id="1588" href="group-theory.congruence-relations-semigroups.html#1588" class="Bound">y</a> <a id="1590" class="Symbol">:</a> <a id="1592" href="group-theory.semigroups.html#946" class="Function">type-Semigroup</a> <a id="1607" href="group-theory.congruence-relations-semigroups.html#1122" class="Bound">G</a><a id="1608" class="Symbol">)</a> <a id="1610" class="Symbol">→</a> <a id="1612" href="foundation-core.propositions.html#1309" class="Function">is-prop</a> <a id="1620" class="Symbol">(</a><a id="1621" href="group-theory.congruence-relations-semigroups.html#1415" class="Function">sim-congruence-Semigroup</a> <a id="1646" href="group-theory.congruence-relations-semigroups.html#1586" class="Bound">x</a> <a id="1648" href="group-theory.congruence-relations-semigroups.html#1588" class="Bound">y</a><a id="1649" class="Symbol">)</a>
  <a id="1653" href="group-theory.congruence-relations-semigroups.html#1546" class="Function">is-prop-sim-congruence-Semigroup</a> <a id="1686" class="Symbol">=</a> <a id="1688" href="foundation.equivalence-relations.html#1343" class="Function">is-prop-sim-Eq-Rel</a> <a id="1707" href="group-theory.congruence-relations-semigroups.html#1183" class="Function">eq-rel-congruence-Semigroup</a>

  <a id="1738" href="group-theory.congruence-relations-semigroups.html#1738" class="Function">refl-congruence-Semigroup</a> <a id="1764" class="Symbol">:</a> <a id="1766" href="foundation.binary-relations.html#1614" class="Function">is-reflexive-Rel-Prop</a> <a id="1788" href="group-theory.congruence-relations-semigroups.html#1283" class="Function">prop-congruence-Semigroup</a>
  <a id="1816" href="group-theory.congruence-relations-semigroups.html#1738" class="Function">refl-congruence-Semigroup</a> <a id="1842" class="Symbol">=</a> <a id="1844" href="foundation.equivalence-relations.html#1698" class="Function">refl-Eq-Rel</a> <a id="1856" href="group-theory.congruence-relations-semigroups.html#1183" class="Function">eq-rel-congruence-Semigroup</a>

  <a id="1887" href="group-theory.congruence-relations-semigroups.html#1887" class="Function">symm-congruence-Semigroup</a> <a id="1913" class="Symbol">:</a> <a id="1915" href="foundation.binary-relations.html#1766" class="Function">is-symmetric-Rel-Prop</a> <a id="1937" href="group-theory.congruence-relations-semigroups.html#1283" class="Function">prop-congruence-Semigroup</a>
  <a id="1965" href="group-theory.congruence-relations-semigroups.html#1887" class="Function">symm-congruence-Semigroup</a> <a id="1991" class="Symbol">=</a> <a id="1993" href="foundation.equivalence-relations.html#1863" class="Function">symm-Eq-Rel</a> <a id="2005" href="group-theory.congruence-relations-semigroups.html#1183" class="Function">eq-rel-congruence-Semigroup</a>

  <a id="2036" href="group-theory.congruence-relations-semigroups.html#2036" class="Function">equiv-symm-congruence-Semigroup</a> <a id="2068" class="Symbol">:</a>
    <a id="2074" class="Symbol">(</a><a id="2075" href="group-theory.congruence-relations-semigroups.html#2075" class="Bound">x</a> <a id="2077" href="group-theory.congruence-relations-semigroups.html#2077" class="Bound">y</a> <a id="2079" class="Symbol">:</a> <a id="2081" href="group-theory.semigroups.html#946" class="Function">type-Semigroup</a> <a id="2096" href="group-theory.congruence-relations-semigroups.html#1122" class="Bound">G</a><a id="2097" class="Symbol">)</a> <a id="2099" class="Symbol">→</a> <a id="2101" href="group-theory.congruence-relations-semigroups.html#1415" class="Function">sim-congruence-Semigroup</a> <a id="2126" href="group-theory.congruence-relations-semigroups.html#2075" class="Bound">x</a> <a id="2128" href="group-theory.congruence-relations-semigroups.html#2077" class="Bound">y</a> <a id="2130" href="foundation-core.equivalences.html#1621" class="Function Operator">≃</a> <a id="2132" href="group-theory.congruence-relations-semigroups.html#1415" class="Function">sim-congruence-Semigroup</a> <a id="2157" href="group-theory.congruence-relations-semigroups.html#2077" class="Bound">y</a> <a id="2159" href="group-theory.congruence-relations-semigroups.html#2075" class="Bound">x</a>
  <a id="2163" href="group-theory.congruence-relations-semigroups.html#2036" class="Function">equiv-symm-congruence-Semigroup</a> <a id="2195" class="Symbol">=</a> <a id="2197" href="foundation.equivalence-relations.html#2034" class="Function">equiv-symm-Eq-Rel</a> <a id="2215" href="group-theory.congruence-relations-semigroups.html#1183" class="Function">eq-rel-congruence-Semigroup</a>

  <a id="2246" href="group-theory.congruence-relations-semigroups.html#2246" class="Function">trans-congruence-Semigroup</a> <a id="2273" class="Symbol">:</a> <a id="2275" href="foundation.binary-relations.html#1942" class="Function">is-transitive-Rel-Prop</a> <a id="2298" href="group-theory.congruence-relations-semigroups.html#1283" class="Function">prop-congruence-Semigroup</a>
  <a id="2326" href="group-theory.congruence-relations-semigroups.html#2246" class="Function">trans-congruence-Semigroup</a> <a id="2353" class="Symbol">=</a> <a id="2355" href="foundation.equivalence-relations.html#2298" class="Function">trans-Eq-Rel</a> <a id="2368" href="group-theory.congruence-relations-semigroups.html#1183" class="Function">eq-rel-congruence-Semigroup</a>

  <a id="2399" href="group-theory.congruence-relations-semigroups.html#2399" class="Function">mul-congruence-Semigroup</a> <a id="2424" class="Symbol">:</a> <a id="2426" href="group-theory.congruence-relations-semigroups.html#614" class="Function">is-congruence-Eq-Rel-Semigroup</a> <a id="2457" href="group-theory.congruence-relations-semigroups.html#1122" class="Bound">G</a> <a id="2459" href="group-theory.congruence-relations-semigroups.html#1183" class="Function">eq-rel-congruence-Semigroup</a>
  <a id="2489" href="group-theory.congruence-relations-semigroups.html#2399" class="Function">mul-congruence-Semigroup</a> <a id="2514" class="Symbol">=</a> <a id="2516" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="2520" href="group-theory.congruence-relations-semigroups.html#1141" class="Bound">R</a>
</pre>