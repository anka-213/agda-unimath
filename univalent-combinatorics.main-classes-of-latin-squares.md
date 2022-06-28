---
title: The groupoid of main classes of Latin squares
---

<pre class="Agda"><a id="71" class="Symbol">{-#</a> <a id="75" class="Keyword">OPTIONS</a> <a id="83" class="Pragma">--without-K</a> <a id="95" class="Pragma">--exact-split</a> <a id="109" class="Symbol">#-}</a>

<a id="114" class="Keyword">module</a> <a id="121" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a> <a id="175" class="Keyword">where</a>

<a id="182" class="Keyword">open</a> <a id="187" class="Keyword">import</a> <a id="194" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="236" class="Keyword">open</a> <a id="241" class="Keyword">import</a> <a id="248" href="foundation.mere-equivalences.html" class="Module">foundation.mere-equivalences</a>
<a id="277" class="Keyword">open</a> <a id="282" class="Keyword">import</a> <a id="289" href="foundation.set-truncations.html" class="Module">foundation.set-truncations</a>
<a id="316" class="Keyword">open</a> <a id="321" class="Keyword">import</a> <a id="328" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="356" class="Keyword">open</a> <a id="361" class="Keyword">import</a> <a id="368" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
<a id="425" class="Keyword">open</a> <a id="430" class="Keyword">import</a> <a id="437" href="univalent-combinatorics.pi-finite-types.html" class="Module">univalent-combinatorics.pi-finite-types</a>
<a id="477" class="Keyword">open</a> <a id="482" class="Keyword">import</a> <a id="489" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
</pre>
## Idea

The groupoid of main classes of latin squares consists of unordered triples of inhabited types equipped with a ternary 1-1 correspondence.

## Definition

### Main classes of general latin squares

<pre class="Agda"><a id="Main-Class-Latin-Squares"></a><a id="755" href="univalent-combinatorics.main-classes-of-latin-squares.html#755" class="Function">Main-Class-Latin-Squares</a> <a id="780" class="Symbol">:</a> <a id="782" class="Symbol">(</a><a id="783" href="univalent-combinatorics.main-classes-of-latin-squares.html#783" class="Bound">l1</a> <a id="786" href="univalent-combinatorics.main-classes-of-latin-squares.html#786" class="Bound">l2</a> <a id="789" class="Symbol">:</a> <a id="791" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="796" class="Symbol">)</a> <a id="798" class="Symbol">→</a> <a id="800" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="803" class="Symbol">(</a><a id="804" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="809" href="univalent-combinatorics.main-classes-of-latin-squares.html#783" class="Bound">l1</a> <a id="812" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="814" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="819" href="univalent-combinatorics.main-classes-of-latin-squares.html#786" class="Bound">l2</a><a id="821" class="Symbol">)</a>
<a id="823" href="univalent-combinatorics.main-classes-of-latin-squares.html#755" class="Function">Main-Class-Latin-Squares</a> <a id="848" href="univalent-combinatorics.main-classes-of-latin-squares.html#848" class="Bound">l1</a> <a id="851" href="univalent-combinatorics.main-classes-of-latin-squares.html#851" class="Bound">l2</a> <a id="854" class="Symbol">=</a> <a id="856" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html#1086" class="Function">Main-Class-Latin-Hypercube</a> <a id="883" href="univalent-combinatorics.main-classes-of-latin-squares.html#848" class="Bound">l1</a> <a id="886" href="univalent-combinatorics.main-classes-of-latin-squares.html#851" class="Bound">l2</a> <a id="889" class="Number">2</a>
</pre>
### Main classes of latin squares of fixed finite order

<pre class="Agda"><a id="Main-Class-Latin-Square-of-Order"></a><a id="961" href="univalent-combinatorics.main-classes-of-latin-squares.html#961" class="Function">Main-Class-Latin-Square-of-Order</a> <a id="994" class="Symbol">:</a> <a id="996" class="Symbol">(</a><a id="997" href="univalent-combinatorics.main-classes-of-latin-squares.html#997" class="Bound">m</a> <a id="999" class="Symbol">:</a> <a id="1001" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="1002" class="Symbol">)</a> <a id="1004" class="Symbol">→</a> <a id="1006" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1009" class="Symbol">(</a><a id="1010" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1015" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="1020" class="Symbol">)</a>
<a id="1022" href="univalent-combinatorics.main-classes-of-latin-squares.html#961" class="Function">Main-Class-Latin-Square-of-Order</a> <a id="1055" href="univalent-combinatorics.main-classes-of-latin-squares.html#1055" class="Bound">m</a> <a id="1057" class="Symbol">=</a>
  <a id="1061" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html#2087" class="Function">Main-Class-Latin-Hypercube-of-Order</a> <a id="1097" class="Number">2</a> <a id="1099" href="univalent-combinatorics.main-classes-of-latin-squares.html#1055" class="Bound">m</a>
</pre>
## Properties

### The groupoid of main classes of latin squares of fixed order is π-finite

<pre class="Agda"><a id="is-π-finite-Main-Class-Latin-Square-of-Order"></a><a id="1207" href="univalent-combinatorics.main-classes-of-latin-squares.html#1207" class="Function">is-π-finite-Main-Class-Latin-Square-of-Order</a> <a id="1252" class="Symbol">:</a>
  <a id="1256" class="Symbol">(</a><a id="1257" href="univalent-combinatorics.main-classes-of-latin-squares.html#1257" class="Bound">k</a> <a id="1259" href="univalent-combinatorics.main-classes-of-latin-squares.html#1259" class="Bound">m</a> <a id="1261" class="Symbol">:</a> <a id="1263" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="1264" class="Symbol">)</a> <a id="1266" class="Symbol">→</a> <a id="1268" href="univalent-combinatorics.pi-finite-types.html#8749" class="Function">is-π-finite</a> <a id="1280" href="univalent-combinatorics.main-classes-of-latin-squares.html#1257" class="Bound">k</a> <a id="1282" class="Symbol">(</a><a id="1283" href="univalent-combinatorics.main-classes-of-latin-squares.html#961" class="Function">Main-Class-Latin-Square-of-Order</a> <a id="1316" href="univalent-combinatorics.main-classes-of-latin-squares.html#1259" class="Bound">m</a><a id="1317" class="Symbol">)</a>
<a id="1319" href="univalent-combinatorics.main-classes-of-latin-squares.html#1207" class="Function">is-π-finite-Main-Class-Latin-Square-of-Order</a> <a id="1364" href="univalent-combinatorics.main-classes-of-latin-squares.html#1364" class="Bound">k</a> <a id="1366" href="univalent-combinatorics.main-classes-of-latin-squares.html#1366" class="Bound">m</a> <a id="1368" class="Symbol">=</a>
  <a id="1372" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html#3140" class="Function">is-π-finite-Main-Class-Latin-Hypercube-of-Order</a> <a id="1420" href="univalent-combinatorics.main-classes-of-latin-squares.html#1364" class="Bound">k</a> <a id="1422" class="Number">2</a> <a id="1424" href="univalent-combinatorics.main-classes-of-latin-squares.html#1366" class="Bound">m</a>
</pre>
### The sequence of the number of main classes of latin squares of finite order

The following sequence defines [A003090](https://oeis.org/A003090) in the OEIS.

<pre class="Agda"><a id="number-of-main-classes-of-Latin-squares-of-order"></a><a id="1601" href="univalent-combinatorics.main-classes-of-latin-squares.html#1601" class="Function">number-of-main-classes-of-Latin-squares-of-order</a> <a id="1650" class="Symbol">:</a> <a id="1652" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a> <a id="1654" class="Symbol">→</a> <a id="1656" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a>
<a id="1658" href="univalent-combinatorics.main-classes-of-latin-squares.html#1601" class="Function">number-of-main-classes-of-Latin-squares-of-order</a> <a id="1707" class="Symbol">=</a>
  <a id="1711" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html#5196" class="Function">number-of-main-classes-of-Latin-hypercubes-of-order</a> <a id="1763" class="Number">2</a>

<a id="mere-equiv-number-of-main-classes-of-Latin-squares-of-order"></a><a id="1766" href="univalent-combinatorics.main-classes-of-latin-squares.html#1766" class="Function">mere-equiv-number-of-main-classes-of-Latin-squares-of-order</a> <a id="1826" class="Symbol">:</a>
  <a id="1830" class="Symbol">(</a><a id="1831" href="univalent-combinatorics.main-classes-of-latin-squares.html#1831" class="Bound">m</a> <a id="1833" class="Symbol">:</a> <a id="1835" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="1836" class="Symbol">)</a> <a id="1838" class="Symbol">→</a>
  <a id="1842" href="foundation.mere-equivalences.html#1406" class="Function">mere-equiv</a>
    <a id="1857" class="Symbol">(</a> <a id="1859" href="univalent-combinatorics.standard-finite-types.html#2149" class="Function">Fin</a> <a id="1863" class="Symbol">(</a><a id="1864" href="univalent-combinatorics.main-classes-of-latin-squares.html#1601" class="Function">number-of-main-classes-of-Latin-squares-of-order</a> <a id="1913" href="univalent-combinatorics.main-classes-of-latin-squares.html#1831" class="Bound">m</a><a id="1914" class="Symbol">))</a>
    <a id="1921" class="Symbol">(</a> <a id="1923" href="foundation.set-truncations.html#3498" class="Postulate">type-trunc-Set</a> <a id="1938" class="Symbol">(</a><a id="1939" href="univalent-combinatorics.main-classes-of-latin-squares.html#961" class="Function">Main-Class-Latin-Square-of-Order</a> <a id="1972" href="univalent-combinatorics.main-classes-of-latin-squares.html#1831" class="Bound">m</a><a id="1973" class="Symbol">))</a>
<a id="1976" href="univalent-combinatorics.main-classes-of-latin-squares.html#1766" class="Function">mere-equiv-number-of-main-classes-of-Latin-squares-of-order</a> <a id="2036" class="Symbol">=</a>
  <a id="2040" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html#5411" class="Function">mere-equiv-number-of-main-classes-of-Latin-hypercubes-of-order</a> <a id="2103" class="Number">2</a>
</pre>