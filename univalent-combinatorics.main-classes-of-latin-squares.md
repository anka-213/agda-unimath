---
title: The groupoid of main classes of Latin squares
---

<pre class="Agda"><a id="71" class="Symbol">{-#</a> <a id="75" class="Keyword">OPTIONS</a> <a id="83" class="Pragma">--without-K</a> <a id="95" class="Pragma">--exact-split</a> <a id="109" class="Symbol">#-}</a>

<a id="114" class="Keyword">module</a> <a id="121" href="univalent-combinatorics.main-classes-of-latin-squares.html" class="Module">univalent-combinatorics.main-classes-of-latin-squares</a> <a id="175" class="Keyword">where</a>

<a id="182" class="Keyword">open</a> <a id="187" class="Keyword">import</a> <a id="194" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="222" class="Keyword">open</a> <a id="227" class="Keyword">import</a> <a id="234" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html" class="Module">univalent-combinatorics.main-classes-of-latin-hypercubes</a>
</pre>
## Idea

The groupoid of main classes of latin squares consists of unordered triples of inhabited types equipped with a ternary 1-1 correspondence.

## Definition

<pre class="Agda"><a id="Main-Class-Latin-Squares"></a><a id="468" href="univalent-combinatorics.main-classes-of-latin-squares.html#468" class="Function">Main-Class-Latin-Squares</a> <a id="493" class="Symbol">:</a> <a id="495" class="Symbol">(</a><a id="496" href="univalent-combinatorics.main-classes-of-latin-squares.html#496" class="Bound">l1</a> <a id="499" href="univalent-combinatorics.main-classes-of-latin-squares.html#499" class="Bound">l2</a> <a id="502" class="Symbol">:</a> <a id="504" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="509" class="Symbol">)</a> <a id="511" class="Symbol">→</a> <a id="513" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="516" class="Symbol">(</a><a id="517" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="522" href="univalent-combinatorics.main-classes-of-latin-squares.html#496" class="Bound">l1</a> <a id="525" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="527" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="532" href="univalent-combinatorics.main-classes-of-latin-squares.html#499" class="Bound">l2</a><a id="534" class="Symbol">)</a>
<a id="536" href="univalent-combinatorics.main-classes-of-latin-squares.html#468" class="Function">Main-Class-Latin-Squares</a> <a id="561" href="univalent-combinatorics.main-classes-of-latin-squares.html#561" class="Bound">l1</a> <a id="564" href="univalent-combinatorics.main-classes-of-latin-squares.html#564" class="Bound">l2</a> <a id="567" class="Symbol">=</a> <a id="569" href="univalent-combinatorics.main-classes-of-latin-hypercubes.html#542" class="Function">Main-Class-Latin-Hypercube</a> <a id="596" href="univalent-combinatorics.main-classes-of-latin-squares.html#561" class="Bound">l1</a> <a id="599" href="univalent-combinatorics.main-classes-of-latin-squares.html#564" class="Bound">l2</a> <a id="602" class="Number">2</a>
</pre>