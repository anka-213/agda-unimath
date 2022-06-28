# Truncation levels


<pre class="Agda"><a id="31" class="Symbol">{-#</a> <a id="35" class="Keyword">OPTIONS</a> <a id="43" class="Pragma">--without-K</a> <a id="55" class="Pragma">--exact-split</a> <a id="69" class="Symbol">#-}</a>

<a id="74" class="Keyword">module</a> <a id="81" href="foundation.truncation-levels.html" class="Module">foundation.truncation-levels</a> <a id="110" class="Keyword">where</a>

<a id="117" class="Keyword">open</a> <a id="122" class="Keyword">import</a> <a id="129" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a> <a id="163" class="Keyword">public</a>

<a id="171" class="Keyword">open</a> <a id="176" class="Keyword">import</a> <a id="183" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="224" class="Keyword">using</a> <a id="230" class="Symbol">(</a><a id="231" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a><a id="232" class="Symbol">;</a> <a id="234" href="elementary-number-theory.natural-numbers.html#1479" class="InductiveConstructor">zero-ℕ</a><a id="240" class="Symbol">;</a> <a id="242" href="elementary-number-theory.natural-numbers.html#1492" class="InductiveConstructor">succ-ℕ</a><a id="248" class="Symbol">)</a>
</pre>
## Properties

### Natural numbers can be converted into truncation levels

<pre class="Agda"><a id="truncation-level-ℕ"></a><a id="339" href="foundation.truncation-levels.html#339" class="Function">truncation-level-ℕ</a> <a id="358" class="Symbol">:</a> <a id="360" href="elementary-number-theory.natural-numbers.html#1458" class="Datatype">ℕ</a> <a id="362" class="Symbol">→</a> <a id="364" href="foundation-core.truncation-levels.html#395" class="Datatype">𝕋</a>
<a id="366" href="foundation.truncation-levels.html#339" class="Function">truncation-level-ℕ</a> <a id="385" href="elementary-number-theory.natural-numbers.html#1479" class="InductiveConstructor">zero-ℕ</a> <a id="392" class="Symbol">=</a> <a id="394" href="foundation-core.truncation-levels.html#492" class="Function">zero-𝕋</a>
<a id="401" href="foundation.truncation-levels.html#339" class="Function">truncation-level-ℕ</a> <a id="420" class="Symbol">(</a><a id="421" href="elementary-number-theory.natural-numbers.html#1492" class="InductiveConstructor">succ-ℕ</a> <a id="428" href="foundation.truncation-levels.html#428" class="Bound">n</a><a id="429" class="Symbol">)</a> <a id="431" class="Symbol">=</a> <a id="433" href="foundation-core.truncation-levels.html#432" class="InductiveConstructor">succ-𝕋</a> <a id="440" class="Symbol">(</a><a id="441" href="foundation.truncation-levels.html#339" class="Function">truncation-level-ℕ</a> <a id="460" href="foundation.truncation-levels.html#428" class="Bound">n</a><a id="461" class="Symbol">)</a>
</pre>