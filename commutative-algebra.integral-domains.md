---
title: Integral domains
---

<pre class="Agda"><a id="42" class="Symbol">{-#</a> <a id="46" class="Keyword">OPTIONS</a> <a id="54" class="Pragma">--without-K</a> <a id="66" class="Pragma">--exact-split</a> <a id="80" class="Symbol">#-}</a>

<a id="85" class="Keyword">module</a> <a id="92" href="commutative-algebra.integral-domains.html" class="Module">commutative-algebra.integral-domains</a> <a id="129" class="Keyword">where</a>

<a id="136" class="Keyword">open</a> <a id="141" class="Keyword">import</a> <a id="148" href="commutative-algebra.commutative-rings.html" class="Module">commutative-algebra.commutative-rings</a>

<a id="187" class="Keyword">open</a> <a id="192" class="Keyword">import</a> <a id="199" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="231" class="Keyword">open</a> <a id="236" class="Keyword">import</a> <a id="243" href="foundation.injective-maps.html" class="Module">foundation.injective-maps</a>
<a id="269" class="Keyword">open</a> <a id="274" class="Keyword">import</a> <a id="281" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="297" class="Keyword">open</a> <a id="302" class="Keyword">import</a> <a id="309" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="337" class="Keyword">open</a> <a id="342" class="Keyword">import</a> <a id="349" href="group-theory.abelian-groups.html" class="Module">group-theory.abelian-groups</a>

<a id="378" class="Keyword">open</a> <a id="383" class="Keyword">import</a> <a id="390" href="ring-theory.rings.html" class="Module">ring-theory.rings</a>
</pre>
## Idea

An integral domain is a commutative ring `R` such that the product of any two nonzero elements in `R` is nonzero. Equivalently, a commutative ring `R` is an integral domain if and only if multiplication by any nonzero element `a` satisfies the cancellation property: `ax = ay ⇒ x = y`.

## Definition

### The cancellation property for a commutative ring

<pre class="Agda"><a id="cancellation-property-Commutative-Ring"></a><a id="786" href="commutative-algebra.integral-domains.html#786" class="Function">cancellation-property-Commutative-Ring</a> <a id="825" class="Symbol">:</a>
  <a id="829" class="Symbol">{</a><a id="830" href="commutative-algebra.integral-domains.html#830" class="Bound">l</a> <a id="832" class="Symbol">:</a> <a id="834" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="839" class="Symbol">}</a> <a id="841" class="Symbol">(</a><a id="842" href="commutative-algebra.integral-domains.html#842" class="Bound">R</a> <a id="844" class="Symbol">:</a> <a id="846" href="commutative-algebra.commutative-rings.html#1514" class="Function">Commutative-Ring</a> <a id="863" href="commutative-algebra.integral-domains.html#830" class="Bound">l</a><a id="864" class="Symbol">)</a> <a id="866" class="Symbol">→</a> <a id="868" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="871" href="commutative-algebra.integral-domains.html#830" class="Bound">l</a>
<a id="873" href="commutative-algebra.integral-domains.html#786" class="Function">cancellation-property-Commutative-Ring</a> <a id="912" href="commutative-algebra.integral-domains.html#912" class="Bound">R</a> <a id="914" class="Symbol">=</a>
  <a id="918" class="Symbol">(</a><a id="919" href="commutative-algebra.integral-domains.html#919" class="Bound">x</a> <a id="921" class="Symbol">:</a> <a id="923" href="commutative-algebra.commutative-rings.html#1833" class="Function">type-Commutative-Ring</a> <a id="945" href="commutative-algebra.integral-domains.html#912" class="Bound">R</a><a id="946" class="Symbol">)</a> <a id="948" class="Symbol">→</a> <a id="950" href="commutative-algebra.commutative-rings.html#2288" class="Function">is-nonzero-Commutative-Ring</a> <a id="978" href="commutative-algebra.integral-domains.html#912" class="Bound">R</a> <a id="980" href="commutative-algebra.integral-domains.html#919" class="Bound">x</a> <a id="982" class="Symbol">→</a>
  <a id="986" href="foundation.injective-maps.html#1309" class="Function">is-injective</a> <a id="999" class="Symbol">(</a><a id="1000" href="commutative-algebra.commutative-rings.html#4124" class="Function">mul-Commutative-Ring</a> <a id="1021" href="commutative-algebra.integral-domains.html#912" class="Bound">R</a> <a id="1023" href="commutative-algebra.integral-domains.html#919" class="Bound">x</a><a id="1024" class="Symbol">)</a>
</pre>
### Integral domains

<pre class="Agda"><a id="Integral-Domain"></a><a id="1061" href="commutative-algebra.integral-domains.html#1061" class="Function">Integral-Domain</a> <a id="1077" class="Symbol">:</a> <a id="1079" class="Symbol">(</a><a id="1080" href="commutative-algebra.integral-domains.html#1080" class="Bound">l</a> <a id="1082" class="Symbol">:</a> <a id="1084" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1089" class="Symbol">)</a> <a id="1091" class="Symbol">→</a> <a id="1093" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1096" class="Symbol">(</a><a id="1097" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1102" href="commutative-algebra.integral-domains.html#1080" class="Bound">l</a><a id="1103" class="Symbol">)</a>
<a id="1105" href="commutative-algebra.integral-domains.html#1061" class="Function">Integral-Domain</a> <a id="1121" href="commutative-algebra.integral-domains.html#1121" class="Bound">l</a> <a id="1123" class="Symbol">=</a>
  <a id="1127" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1129" class="Symbol">(</a><a id="1130" href="commutative-algebra.commutative-rings.html#1514" class="Function">Commutative-Ring</a> <a id="1147" href="commutative-algebra.integral-domains.html#1121" class="Bound">l</a><a id="1148" class="Symbol">)</a> <a id="1150" href="commutative-algebra.integral-domains.html#786" class="Function">cancellation-property-Commutative-Ring</a>

<a id="1190" class="Keyword">module</a> <a id="1197" href="commutative-algebra.integral-domains.html#1197" class="Module">_</a>
  <a id="1201" class="Symbol">{</a><a id="1202" href="commutative-algebra.integral-domains.html#1202" class="Bound">l</a> <a id="1204" class="Symbol">:</a> <a id="1206" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1211" class="Symbol">}</a> <a id="1213" class="Symbol">(</a><a id="1214" href="commutative-algebra.integral-domains.html#1214" class="Bound">R</a> <a id="1216" class="Symbol">:</a> <a id="1218" href="commutative-algebra.integral-domains.html#1061" class="Function">Integral-Domain</a> <a id="1234" href="commutative-algebra.integral-domains.html#1202" class="Bound">l</a><a id="1235" class="Symbol">)</a>
  <a id="1239" class="Keyword">where</a>

  <a id="1248" href="commutative-algebra.integral-domains.html#1248" class="Function">commutative-ring-Integral-Domain</a> <a id="1281" class="Symbol">:</a> <a id="1283" href="commutative-algebra.commutative-rings.html#1514" class="Function">Commutative-Ring</a> <a id="1300" href="commutative-algebra.integral-domains.html#1202" class="Bound">l</a>
  <a id="1304" href="commutative-algebra.integral-domains.html#1248" class="Function">commutative-ring-Integral-Domain</a> <a id="1337" class="Symbol">=</a> <a id="1339" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1343" href="commutative-algebra.integral-domains.html#1214" class="Bound">R</a>

  <a id="1348" href="commutative-algebra.integral-domains.html#1348" class="Function">ring-Integral-Domain</a> <a id="1369" class="Symbol">:</a> <a id="1371" href="ring-theory.rings.html#2551" class="Function">Ring</a> <a id="1376" href="commutative-algebra.integral-domains.html#1202" class="Bound">l</a>
  <a id="1380" href="commutative-algebra.integral-domains.html#1348" class="Function">ring-Integral-Domain</a> <a id="1401" class="Symbol">=</a> <a id="1403" href="commutative-algebra.commutative-rings.html#1676" class="Function">ring-Commutative-Ring</a> <a id="1425" href="commutative-algebra.integral-domains.html#1248" class="Function">commutative-ring-Integral-Domain</a>

  <a id="1461" href="commutative-algebra.integral-domains.html#1461" class="Function">set-Integral-Domain</a> <a id="1481" class="Symbol">:</a> <a id="1483" href="foundation-core.sets.html#1190" class="Function">UU-Set</a> <a id="1490" href="commutative-algebra.integral-domains.html#1202" class="Bound">l</a>
  <a id="1494" href="commutative-algebra.integral-domains.html#1461" class="Function">set-Integral-Domain</a> <a id="1514" class="Symbol">=</a> <a id="1516" href="ring-theory.rings.html#2757" class="Function">set-Ring</a> <a id="1525" href="commutative-algebra.integral-domains.html#1348" class="Function">ring-Integral-Domain</a>

  <a id="1549" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a> <a id="1570" class="Symbol">:</a> <a id="1572" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1575" href="commutative-algebra.integral-domains.html#1202" class="Bound">l</a>
  <a id="1579" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a> <a id="1600" class="Symbol">=</a> <a id="1602" href="ring-theory.rings.html#2808" class="Function">type-Ring</a> <a id="1612" href="commutative-algebra.integral-domains.html#1348" class="Function">ring-Integral-Domain</a>

  <a id="1636" href="commutative-algebra.integral-domains.html#1636" class="Function">is-set-type-Integral-Domain</a> <a id="1664" class="Symbol">:</a> <a id="1666" href="foundation-core.sets.html#1113" class="Function">is-set</a> <a id="1673" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a>
  <a id="1696" href="commutative-algebra.integral-domains.html#1636" class="Function">is-set-type-Integral-Domain</a> <a id="1724" class="Symbol">=</a> <a id="1726" href="ring-theory.rings.html#2858" class="Function">is-set-type-Ring</a> <a id="1743" href="commutative-algebra.integral-domains.html#1348" class="Function">ring-Integral-Domain</a>

  <a id="1767" href="commutative-algebra.integral-domains.html#1767" class="Function">add-Integral-Domain</a> <a id="1787" class="Symbol">:</a> <a id="1789" class="Symbol">(</a><a id="1790" href="commutative-algebra.integral-domains.html#1790" class="Bound">x</a> <a id="1792" href="commutative-algebra.integral-domains.html#1792" class="Bound">y</a> <a id="1794" class="Symbol">:</a> <a id="1796" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a><a id="1816" class="Symbol">)</a> <a id="1818" class="Symbol">→</a> <a id="1820" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a>
  <a id="1843" href="commutative-algebra.integral-domains.html#1767" class="Function">add-Integral-Domain</a> <a id="1863" class="Symbol">=</a> <a id="1865" href="ring-theory.rings.html#3153" class="Function">add-Ring</a> <a id="1874" href="commutative-algebra.integral-domains.html#1348" class="Function">ring-Integral-Domain</a>

  <a id="1898" href="commutative-algebra.integral-domains.html#1898" class="Function">zero-Integral-Domain</a> <a id="1919" class="Symbol">:</a> <a id="1921" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a>
  <a id="1944" href="commutative-algebra.integral-domains.html#1898" class="Function">zero-Integral-Domain</a> <a id="1965" class="Symbol">=</a> <a id="1967" href="ring-theory.rings.html#5170" class="Function">zero-Ring</a> <a id="1977" href="commutative-algebra.integral-domains.html#1348" class="Function">ring-Integral-Domain</a>

  <a id="2001" href="commutative-algebra.integral-domains.html#2001" class="Function">neg-Integral-Domain</a> <a id="2021" class="Symbol">:</a> <a id="2023" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a> <a id="2044" class="Symbol">→</a> <a id="2046" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a>
  <a id="2069" href="commutative-algebra.integral-domains.html#2001" class="Function">neg-Integral-Domain</a> <a id="2089" class="Symbol">=</a> <a id="2091" href="ring-theory.rings.html#5990" class="Function">neg-Ring</a> <a id="2100" href="commutative-algebra.integral-domains.html#1348" class="Function">ring-Integral-Domain</a>

  <a id="2124" href="commutative-algebra.integral-domains.html#2124" class="Function">mul-Integral-Domain</a> <a id="2144" class="Symbol">:</a> <a id="2146" class="Symbol">(</a><a id="2147" href="commutative-algebra.integral-domains.html#2147" class="Bound">x</a> <a id="2149" href="commutative-algebra.integral-domains.html#2149" class="Bound">y</a> <a id="2151" class="Symbol">:</a> <a id="2153" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a><a id="2173" class="Symbol">)</a> <a id="2175" class="Symbol">→</a> <a id="2177" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a>
  <a id="2200" href="commutative-algebra.integral-domains.html#2124" class="Function">mul-Integral-Domain</a> <a id="2220" class="Symbol">=</a> <a id="2222" href="ring-theory.rings.html#6590" class="Function">mul-Ring</a> <a id="2231" href="commutative-algebra.integral-domains.html#1348" class="Function">ring-Integral-Domain</a>

  <a id="2255" href="commutative-algebra.integral-domains.html#2255" class="Function">one-Integral-Domain</a> <a id="2275" class="Symbol">:</a> <a id="2277" href="commutative-algebra.integral-domains.html#1549" class="Function">type-Integral-Domain</a>
  <a id="2300" href="commutative-algebra.integral-domains.html#2255" class="Function">one-Integral-Domain</a> <a id="2320" class="Symbol">=</a> <a id="2322" href="ring-theory.rings.html#8018" class="Function">one-Ring</a> <a id="2331" href="commutative-algebra.integral-domains.html#1348" class="Function">ring-Integral-Domain</a>
</pre>