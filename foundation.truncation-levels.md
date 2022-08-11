---
title: Truncation levels
---


<pre class="Agda"><a id="44" class="Symbol">{-#</a> <a id="48" class="Keyword">OPTIONS</a> <a id="56" class="Pragma">--without-K</a> <a id="68" class="Pragma">--exact-split</a> <a id="82" class="Symbol">#-}</a>

<a id="87" class="Keyword">module</a> <a id="94" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a> <a id="123" class="Keyword">where</a>

<a id="130" class="Keyword">open</a> <a id="135" class="Keyword">import</a> <a id="142" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a> <a id="176" class="Keyword">public</a>

<a id="184" class="Keyword">open</a> <a id="189" class="Keyword">import</a> <a id="196" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="237" class="Keyword">using</a> <a id="243" class="Symbol">(</a><a id="244" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="245" class="Symbol">;</a> <a id="247" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a><a id="253" class="Symbol">;</a> <a id="255" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a><a id="261" class="Symbol">)</a>
</pre>
## Properties

### Natural numbers can be converted into truncation levels

<pre class="Agda"><a id="truncation-level-ℕ"></a><a id="352" href="foundation.truncation-levels.html#352" class="Function">truncation-level-ℕ</a> <a id="371" class="Symbol">:</a> <a id="373" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="375" class="Symbol">→</a> <a id="377" href="foundation-core.truncation-levels.html#395" class="Datatype">𝕋</a>
<a id="379" href="foundation.truncation-levels.html#352" class="Function">truncation-level-ℕ</a> <a id="398" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a> <a id="405" class="Symbol">=</a> <a id="407" href="foundation-core.truncation-levels.html#492" class="Function">zero-𝕋</a>
<a id="414" href="foundation.truncation-levels.html#352" class="Function">truncation-level-ℕ</a> <a id="433" class="Symbol">(</a><a id="434" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="441" href="foundation.truncation-levels.html#441" class="Bound">n</a><a id="442" class="Symbol">)</a> <a id="444" class="Symbol">=</a> <a id="446" href="foundation-core.truncation-levels.html#432" class="InductiveConstructor">succ-𝕋</a> <a id="453" class="Symbol">(</a><a id="454" href="foundation.truncation-levels.html#352" class="Function">truncation-level-ℕ</a> <a id="473" href="foundation.truncation-levels.html#441" class="Bound">n</a><a id="474" class="Symbol">)</a>
</pre>