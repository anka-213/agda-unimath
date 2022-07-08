---
title: Bracelets
---

<pre class="Agda"><a id="35" class="Symbol">{-#</a> <a id="39" class="Keyword">OPTIONS</a> <a id="47" class="Pragma">--without-K</a> <a id="59" class="Pragma">--exact-split</a> <a id="73" class="Symbol">#-}</a>

<a id="78" class="Keyword">module</a> <a id="85" href="univalent-combinatorics.bracelets.html" class="Module">univalent-combinatorics.bracelets</a> <a id="119" class="Keyword">where</a>

<a id="126" class="Keyword">open</a> <a id="131" class="Keyword">import</a> <a id="138" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>

<a id="180" class="Keyword">open</a> <a id="185" class="Keyword">import</a> <a id="192" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="224" class="Keyword">open</a> <a id="229" class="Keyword">import</a> <a id="236" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="264" class="Keyword">open</a> <a id="269" class="Keyword">import</a> <a id="276" href="graph-theory.polygons.html" class="Module">graph-theory.polygons</a>

<a id="299" class="Keyword">open</a> <a id="304" class="Keyword">import</a> <a id="311" href="univalent-combinatorics.standard-finite-types.html" class="Module">univalent-combinatorics.standard-finite-types</a>
</pre>
## Definition

### Bracelets

<pre class="Agda"><a id="bracelet"></a><a id="400" href="univalent-combinatorics.bracelets.html#400" class="Function">bracelet</a> <a id="409" class="Symbol">:</a> <a id="411" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a> <a id="413" class="Symbol">→</a> <a id="415" href="elementary-number-theory.natural-numbers.html#1530" class="Datatype">ℕ</a> <a id="417" class="Symbol">→</a> <a id="419" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="422" class="Symbol">(</a><a id="423" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="428" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="433" class="Symbol">)</a>
<a id="435" href="univalent-combinatorics.bracelets.html#400" class="Function">bracelet</a> <a id="444" href="univalent-combinatorics.bracelets.html#444" class="Bound">m</a> <a id="446" href="univalent-combinatorics.bracelets.html#446" class="Bound">n</a> <a id="448" class="Symbol">=</a> <a id="450" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="452" class="Symbol">(</a><a id="453" href="graph-theory.polygons.html#2934" class="Function">Polygon</a> <a id="461" href="univalent-combinatorics.bracelets.html#444" class="Bound">m</a><a id="462" class="Symbol">)</a> <a id="464" class="Symbol">(λ</a> <a id="467" href="univalent-combinatorics.bracelets.html#467" class="Bound">X</a> <a id="469" class="Symbol">→</a> <a id="471" href="graph-theory.polygons.html#3392" class="Function">vertex-Polygon</a> <a id="486" href="univalent-combinatorics.bracelets.html#444" class="Bound">m</a> <a id="488" href="univalent-combinatorics.bracelets.html#467" class="Bound">X</a> <a id="490" class="Symbol">→</a> <a id="492" href="univalent-combinatorics.standard-finite-types.html#2396" class="Function">Fin</a> <a id="496" href="univalent-combinatorics.bracelets.html#446" class="Bound">n</a><a id="497" class="Symbol">)</a>
</pre>