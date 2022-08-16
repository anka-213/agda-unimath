---
title: The dihedral groups
---

<pre class="Agda"><a id="45" class="Keyword">module</a> <a id="52" href="group-theory.dihedral-groups.html" class="Module">group-theory.dihedral-groups</a> <a id="81" class="Keyword">where</a>

<a id="88" class="Keyword">open</a> <a id="93" class="Keyword">import</a> <a id="100" href="elementary-number-theory.groups-of-modular-arithmetic.html" class="Module">elementary-number-theory.groups-of-modular-arithmetic</a>
<a id="154" class="Keyword">open</a> <a id="159" class="Keyword">import</a> <a id="166" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="208" class="Keyword">open</a> <a id="213" class="Keyword">import</a> <a id="220" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="248" class="Keyword">open</a> <a id="253" class="Keyword">import</a> <a id="260" href="group-theory.dihedral-group-construction.html" class="Module">group-theory.dihedral-group-construction</a>
<a id="301" class="Keyword">open</a> <a id="306" class="Keyword">import</a> <a id="313" href="group-theory.groups.html" class="Module">group-theory.groups</a>
</pre>
## Idea

The dihedral group `D_k` is defined by the dihedral group construction applied to the cyclic group `ℤ-Mod k`.

## Definition

<pre class="Agda"><a id="dihedral-group"></a><a id="481" href="group-theory.dihedral-groups.html#481" class="Function">dihedral-group</a> <a id="496" class="Symbol">:</a> <a id="498" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="500" class="Symbol">→</a> <a id="502" href="group-theory.groups.html#2650" class="Function">Group</a> <a id="508" href="Agda.Primitive.html#764" class="Primitive">lzero</a>
<a id="514" href="group-theory.dihedral-groups.html#481" class="Function">dihedral-group</a> <a id="529" href="group-theory.dihedral-groups.html#529" class="Bound">k</a> <a id="531" class="Symbol">=</a> <a id="533" href="group-theory.dihedral-group-construction.html#5214" class="Function">dihedral-group-Ab</a> <a id="551" class="Symbol">(</a><a id="552" href="elementary-number-theory.groups-of-modular-arithmetic.html#1524" class="Function">ℤ-Mod-Ab</a> <a id="561" href="group-theory.dihedral-groups.html#529" class="Bound">k</a><a id="562" class="Symbol">)</a>
</pre>