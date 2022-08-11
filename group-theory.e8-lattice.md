---
title: The E₈-lattice
---

<pre class="Agda"><a id="40" class="Keyword">module</a> <a id="47" href="group-theory.e8-lattice.html" class="Module">group-theory.e8-lattice</a> <a id="71" class="Keyword">where</a>

<a id="78" class="Keyword">open</a> <a id="83" class="Keyword">import</a> <a id="90" href="elementary-number-theory.integers.html" class="Module">elementary-number-theory.integers</a>

<a id="125" class="Keyword">open</a> <a id="130" class="Keyword">import</a> <a id="137" href="foundation.equality-coproduct-types.html" class="Module">foundation.equality-coproduct-types</a>
<a id="173" class="Keyword">open</a> <a id="178" class="Keyword">import</a> <a id="185" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="201" class="Keyword">open</a> <a id="206" class="Keyword">import</a> <a id="213" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="241" class="Keyword">open</a> <a id="246" class="Keyword">import</a> <a id="253" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
</pre>
## Definition

### The ambient set of the E₈ lattice

The E₈ lattice itself is a subset of the following set.

<pre class="Agda"><a id="ambient-set-E8-lattice"></a><a id="423" href="group-theory.e8-lattice.html#423" class="Function">ambient-set-E8-lattice</a> <a id="446" class="Symbol">:</a> <a id="448" href="foundation-core.sets.html#1190" class="Function">UU-Set</a> <a id="455" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="461" href="group-theory.e8-lattice.html#423" class="Function">ambient-set-E8-lattice</a> <a id="484" class="Symbol">=</a>
  <a id="488" href="foundation.equality-coproduct-types.html#11165" class="Function">coprod-Set</a> <a id="499" class="Symbol">(</a><a id="500" href="foundation.sets.html#4337" class="Function">hom-Set</a> <a id="508" class="Symbol">(</a><a id="509" href="univalent-combinatorics.standard-finite-types.html#2285" class="Function">Fin-Set</a> <a id="517" class="Number">8</a><a id="518" class="Symbol">)</a> <a id="520" href="elementary-number-theory.integers.html#4352" class="Function">ℤ-Set</a><a id="525" class="Symbol">)</a> <a id="527" class="Symbol">(</a><a id="528" href="foundation.sets.html#4337" class="Function">hom-Set</a> <a id="536" class="Symbol">(</a><a id="537" href="univalent-combinatorics.standard-finite-types.html#2285" class="Function">Fin-Set</a> <a id="545" class="Number">8</a><a id="546" class="Symbol">)</a> <a id="548" href="elementary-number-theory.integers.html#4352" class="Function">ℤ-Set</a><a id="553" class="Symbol">)</a>
</pre>