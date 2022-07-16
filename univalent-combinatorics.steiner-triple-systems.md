---
title: Steiner triple systems
---

<pre class="Agda"><a id="48" class="Symbol">{-#</a> <a id="52" class="Keyword">OPTIONS</a> <a id="60" class="Pragma">--without-K</a> <a id="72" class="Pragma">--exact-split</a> <a id="86" class="Symbol">#-}</a>

<a id="91" class="Keyword">module</a> <a id="98" href="univalent-combinatorics.steiner-triple-systems.html" class="Module">univalent-combinatorics.steiner-triple-systems</a> <a id="145" class="Keyword">where</a>

<a id="152" class="Keyword">open</a> <a id="157" class="Keyword">import</a> <a id="164" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="206" class="Keyword">open</a> <a id="211" class="Keyword">import</a> <a id="218" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="246" class="Keyword">open</a> <a id="251" class="Keyword">import</a> <a id="258" href="univalent-combinatorics.steiner-systems.html" class="Module">univalent-combinatorics.steiner-systems</a>
</pre>
## Definition

<pre class="Agda"><a id="Steiner-Triple-System"></a><a id="326" href="univalent-combinatorics.steiner-triple-systems.html#326" class="Function">Steiner-Triple-System</a> <a id="348" class="Symbol">:</a> <a id="350" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a> <a id="352" class="Symbol">→</a> <a id="354" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="357" class="Symbol">(</a><a id="358" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="363" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="368" class="Symbol">)</a>
<a id="370" href="univalent-combinatorics.steiner-triple-systems.html#326" class="Function">Steiner-Triple-System</a> <a id="392" href="univalent-combinatorics.steiner-triple-systems.html#392" class="Bound">n</a> <a id="394" class="Symbol">=</a> <a id="396" href="univalent-combinatorics.steiner-systems.html#796" class="Function">Steiner-System</a> <a id="411" class="Number">2</a> <a id="413" class="Number">3</a> <a id="415" href="univalent-combinatorics.steiner-triple-systems.html#392" class="Bound">n</a>
</pre>