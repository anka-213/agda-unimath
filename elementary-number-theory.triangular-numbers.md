---
title: The triangular numbers
---

<pre class="Agda"><a id="48" class="Symbol">{-#</a> <a id="52" class="Keyword">OPTIONS</a> <a id="60" class="Pragma">--without-K</a> <a id="72" class="Pragma">--exact-split</a> <a id="86" class="Symbol">#-}</a>

<a id="91" class="Keyword">module</a> <a id="98" href="elementary-number-theory.triangular-numbers.html" class="Module">elementary-number-theory.triangular-numbers</a> <a id="142" class="Keyword">where</a>

<a id="149" class="Keyword">open</a> <a id="154" class="Keyword">import</a> <a id="161" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a> <a id="211" class="Keyword">using</a> <a id="217" class="Symbol">(</a><a id="218" href="elementary-number-theory.addition-natural-numbers.html#1096" class="Function">add-ℕ</a><a id="223" class="Symbol">)</a>
<a id="225" class="Keyword">open</a> <a id="230" class="Keyword">import</a> <a id="237" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="278" class="Keyword">using</a> <a id="284" class="Symbol">(</a><a id="285" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="286" class="Symbol">;</a> <a id="288" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a><a id="294" class="Symbol">)</a>
</pre>
## Definition

<pre class="Agda"><a id="triangular-number-ℕ"></a><a id="324" href="elementary-number-theory.triangular-numbers.html#324" class="Function">triangular-number-ℕ</a> <a id="344" class="Symbol">:</a> <a id="346" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="348" class="Symbol">→</a> <a id="350" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a>
<a id="352" href="elementary-number-theory.triangular-numbers.html#324" class="Function">triangular-number-ℕ</a> <a id="372" class="Number">0</a> <a id="374" class="Symbol">=</a> <a id="376" class="Number">0</a>
<a id="378" href="elementary-number-theory.triangular-numbers.html#324" class="Function">triangular-number-ℕ</a> <a id="398" class="Symbol">(</a><a id="399" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="406" href="elementary-number-theory.triangular-numbers.html#406" class="Bound">n</a><a id="407" class="Symbol">)</a> <a id="409" class="Symbol">=</a> <a id="411" href="elementary-number-theory.addition-natural-numbers.html#1096" class="Function">add-ℕ</a> <a id="417" class="Symbol">(</a><a id="418" href="elementary-number-theory.triangular-numbers.html#324" class="Function">triangular-number-ℕ</a> <a id="438" href="elementary-number-theory.triangular-numbers.html#406" class="Bound">n</a><a id="439" class="Symbol">)</a> <a id="441" class="Symbol">(</a><a id="442" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="449" href="elementary-number-theory.triangular-numbers.html#406" class="Bound">n</a><a id="450" class="Symbol">)</a>
</pre>