---
title: Alcohols
---

<pre class="Agda"><a id="34" class="Symbol">{-#</a> <a id="38" class="Keyword">OPTIONS</a> <a id="46" class="Pragma">--without-K</a> <a id="58" class="Pragma">--exact-split</a> <a id="72" class="Symbol">#-}</a>

<a id="77" class="Keyword">module</a> <a id="84" href="organic-chemistry.alcohols.html" class="Module">organic-chemistry.alcohols</a> <a id="111" class="Keyword">where</a>

<a id="118" class="Keyword">open</a> <a id="123" class="Keyword">import</a> <a id="130" href="foundation.cartesian-product-types.html" class="Module">foundation.cartesian-product-types</a>
<a id="165" class="Keyword">open</a> <a id="170" class="Keyword">import</a> <a id="177" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a>
<a id="207" class="Keyword">open</a> <a id="212" class="Keyword">import</a> <a id="219" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="251" class="Keyword">open</a> <a id="256" class="Keyword">import</a> <a id="263" href="foundation.negation.html" class="Module">foundation.negation</a>
<a id="283" class="Keyword">open</a> <a id="288" class="Keyword">import</a> <a id="295" href="foundation.propositional-truncations.html" class="Module">foundation.propositional-truncations</a>
<a id="332" class="Keyword">open</a> <a id="337" class="Keyword">import</a> <a id="344" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>
<a id="371" class="Keyword">open</a> <a id="376" class="Keyword">import</a> <a id="383" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>

<a id="411" class="Keyword">open</a> <a id="416" class="Keyword">import</a> <a id="423" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
<a id="459" class="Keyword">open</a> <a id="464" class="Keyword">import</a> <a id="471" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
</pre>
## Idea

An alcohol is a hydrocarbon with at least one `-OH` group. The type of alcohols can therefore be defined as the type of hydrocarbons equipped with a distinguished subset of the available (unbonded) electrons of the carbon atoms.

## Definition

<pre class="Agda"><a id="alcohol"></a><a id="769" href="organic-chemistry.alcohols.html#769" class="Function">alcohol</a> <a id="777" class="Symbol">:</a> <a id="779" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="782" class="Symbol">(</a><a id="783" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="788" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="793" class="Symbol">)</a>
<a id="795" href="organic-chemistry.alcohols.html#769" class="Function">alcohol</a> <a id="803" class="Symbol">=</a>
  <a id="807" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="809" class="Symbol">(</a> <a id="811" href="organic-chemistry.hydrocarbons.html#1564" class="Function">hydrocarbon</a><a id="822" class="Symbol">)</a>
    <a id="828" class="Symbol">(</a> <a id="830" class="Symbol">λ</a> <a id="832" href="organic-chemistry.alcohols.html#832" class="Bound">X</a> <a id="834" class="Symbol">→</a>
      <a id="842" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="844" class="Symbol">(</a> <a id="846" class="Symbol">(</a><a id="847" href="organic-chemistry.alcohols.html#847" class="Bound">c</a> <a id="849" class="Symbol">:</a> <a id="851" href="organic-chemistry.hydrocarbons.html#2659" class="Function">vertex-hydrocarbon</a> <a id="870" href="organic-chemistry.alcohols.html#832" class="Bound">X</a><a id="871" class="Symbol">)</a> <a id="873" class="Symbol">→</a>
          <a id="885" href="foundation.decidable-subtypes.html#1803" class="Function">decidable-subtype</a> <a id="903" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="909" class="Symbol">(</a><a id="910" href="organic-chemistry.hydrocarbons.html#3636" class="Function">electron-carbon-atom-hydrocarbon</a> <a id="943" href="organic-chemistry.alcohols.html#832" class="Bound">X</a> <a id="945" href="organic-chemistry.alcohols.html#847" class="Bound">c</a><a id="946" class="Symbol">))</a>
        <a id="957" class="Symbol">(</a> <a id="959" class="Symbol">λ</a> <a id="961" href="organic-chemistry.alcohols.html#961" class="Bound">OH</a> <a id="964" class="Symbol">→</a>
          <a id="976" class="Symbol">(</a> <a id="978" class="Symbol">(</a> <a id="980" href="organic-chemistry.alcohols.html#980" class="Bound">c</a> <a id="982" href="organic-chemistry.alcohols.html#982" class="Bound">c&#39;</a> <a id="985" class="Symbol">:</a> <a id="987" href="organic-chemistry.hydrocarbons.html#2659" class="Function">vertex-hydrocarbon</a> <a id="1006" href="organic-chemistry.alcohols.html#832" class="Bound">X</a><a id="1007" class="Symbol">)</a> <a id="1009" class="Symbol">→</a>
            <a id="1023" class="Symbol">(</a> <a id="1025" href="organic-chemistry.alcohols.html#1025" class="Bound">b</a> <a id="1027" class="Symbol">:</a> <a id="1029" href="organic-chemistry.hydrocarbons.html#3175" class="Function">edge-hydrocarbon</a> <a id="1046" href="organic-chemistry.alcohols.html#832" class="Bound">X</a> <a id="1048" class="Symbol">(</a><a id="1049" href="foundation.unordered-pairs.html#4717" class="Function">standard-unordered-pair</a> <a id="1073" href="organic-chemistry.alcohols.html#980" class="Bound">c</a> <a id="1075" href="organic-chemistry.alcohols.html#982" class="Bound">c&#39;</a><a id="1077" class="Symbol">))</a> <a id="1080" class="Symbol">→</a>
            <a id="1094" href="foundation-core.negation.html#465" class="Function">¬</a> <a id="1096" class="Symbol">(</a><a id="1097" href="foundation.decidable-subtypes.html#2370" class="Function">is-in-decidable-subtype</a> <a id="1121" class="Symbol">(</a><a id="1122" href="organic-chemistry.alcohols.html#961" class="Bound">OH</a> <a id="1125" href="organic-chemistry.alcohols.html#980" class="Bound">c</a><a id="1126" class="Symbol">)</a> <a id="1128" class="Symbol">(</a><a id="1129" href="organic-chemistry.hydrocarbons.html#4051" class="Function">bonding-hydrocarbon</a> <a id="1149" href="organic-chemistry.alcohols.html#832" class="Bound">X</a> <a id="1151" href="organic-chemistry.alcohols.html#1025" class="Bound">b</a><a id="1152" class="Symbol">)))</a> <a id="1156" href="foundation-core.cartesian-product-types.html#590" class="Function Operator">×</a>
          <a id="1168" class="Symbol">(</a> <a id="1170" class="Symbol">(</a> <a id="1172" href="foundation.propositional-truncations.html#2209" class="Function">type-trunc-Prop</a>
            <a id="1200" class="Symbol">(</a> <a id="1202" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1204" class="Symbol">(</a> <a id="1206" href="organic-chemistry.hydrocarbons.html#2659" class="Function">vertex-hydrocarbon</a> <a id="1225" href="organic-chemistry.alcohols.html#832" class="Bound">X</a><a id="1226" class="Symbol">)</a>
                <a id="1244" class="Symbol">(</a> <a id="1246" class="Symbol">λ</a> <a id="1248" href="organic-chemistry.alcohols.html#1248" class="Bound">c</a> <a id="1250" class="Symbol">→</a> <a id="1252" href="foundation.decidable-subtypes.html#2791" class="Function">type-decidable-subtype</a> <a id="1275" class="Symbol">(</a><a id="1276" href="organic-chemistry.alcohols.html#961" class="Bound">OH</a> <a id="1279" href="organic-chemistry.alcohols.html#1248" class="Bound">c</a><a id="1280" class="Symbol">))))</a> <a id="1285" href="foundation-core.cartesian-product-types.html#590" class="Function Operator">×</a>
            <a id="1299" class="Symbol">(</a> <a id="1301" class="Symbol">(</a> <a id="1303" href="organic-chemistry.alcohols.html#1303" class="Bound">c</a> <a id="1305" class="Symbol">:</a> <a id="1307" href="organic-chemistry.hydrocarbons.html#2659" class="Function">vertex-hydrocarbon</a> <a id="1326" href="organic-chemistry.alcohols.html#832" class="Bound">X</a><a id="1327" class="Symbol">)</a> <a id="1329" class="Symbol">→</a>
              <a id="1345" href="foundation.decidable-subtypes.html#2791" class="Function">type-decidable-subtype</a> <a id="1368" class="Symbol">(</a><a id="1369" href="organic-chemistry.alcohols.html#961" class="Bound">OH</a> <a id="1372" href="organic-chemistry.alcohols.html#1303" class="Bound">c</a><a id="1373" class="Symbol">)</a> <a id="1375" class="Symbol">→</a>
              <a id="1391" href="organic-chemistry.saturated-carbons.html#823" class="Function">is-saturated-carbon-hydrocarbon</a> <a id="1423" href="organic-chemistry.alcohols.html#832" class="Bound">X</a> <a id="1425" href="organic-chemistry.alcohols.html#1303" class="Bound">c</a>
              <a id="1441" class="Symbol">))))</a>
</pre>
More explicitly, an alcohol is a hydrocarbon equipped with, for each of its carbons, a subset of its electrons, where membership in that subset indicates whether or not a hydroxyl group is bonded to that specific electron. We require the following conditions:

- The electron shared between a carbon atom and a hydroxyl group can not also be shared between that carbon atom and a different carbon.
- There must be at least one hydroxyl group.
- Atoms to which hydroxyl groups are bonded must be saturated.