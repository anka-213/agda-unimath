# Truncation levels


<pre class="Agda"><a id="31" class="Symbol">{-#</a> <a id="35" class="Keyword">OPTIONS</a> <a id="43" class="Pragma">--without-K</a> <a id="55" class="Pragma">--exact-split</a> <a id="69" class="Pragma">--safe</a> <a id="76" class="Symbol">#-}</a>

<a id="81" class="Keyword">module</a> <a id="88" href="foundation-core.truncation-levels.html" class="Module">foundation-core.truncation-levels</a> <a id="122" class="Keyword">where</a>

<a id="129" class="Keyword">open</a> <a id="134" class="Keyword">import</a> <a id="141" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a> <a id="173" class="Keyword">using</a> <a id="179" class="Symbol">(</a><a id="180" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="182" class="Symbol">;</a> <a id="184" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="189" class="Symbol">)</a>
</pre>
## Idea

The type of truncation levels is a type similar to the type of natural numbers, but starting the count at -2, so that sets have truncation level 0.

## Definition

<pre class="Agda"><a id="377" class="Keyword">data</a> <a id="𝕋"></a><a id="382" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a> <a id="384" class="Symbol">:</a> <a id="386" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="389" href="Agda.Primitive.html#764" class="Primitive">lzero</a> <a id="395" class="Keyword">where</a>
  <a id="𝕋.neg-two-𝕋"></a><a id="403" href="foundation-core.truncation-levels.html#403" class="InductiveConstructor">neg-two-𝕋</a> <a id="413" class="Symbol">:</a> <a id="415" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a>
  <a id="𝕋.succ-𝕋"></a><a id="419" href="foundation-core.truncation-levels.html#419" class="InductiveConstructor">succ-𝕋</a> <a id="426" class="Symbol">:</a> <a id="428" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a> <a id="430" class="Symbol">→</a> <a id="432" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a>

<a id="neg-one-𝕋"></a><a id="435" href="foundation-core.truncation-levels.html#435" class="Function">neg-one-𝕋</a> <a id="445" class="Symbol">:</a> <a id="447" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a>
<a id="449" href="foundation-core.truncation-levels.html#435" class="Function">neg-one-𝕋</a> <a id="459" class="Symbol">=</a> <a id="461" href="foundation-core.truncation-levels.html#419" class="InductiveConstructor">succ-𝕋</a> <a id="468" href="foundation-core.truncation-levels.html#403" class="InductiveConstructor">neg-two-𝕋</a>

<a id="zero-𝕋"></a><a id="479" href="foundation-core.truncation-levels.html#479" class="Function">zero-𝕋</a> <a id="486" class="Symbol">:</a> <a id="488" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a>
<a id="490" href="foundation-core.truncation-levels.html#479" class="Function">zero-𝕋</a> <a id="497" class="Symbol">=</a> <a id="499" href="foundation-core.truncation-levels.html#419" class="InductiveConstructor">succ-𝕋</a> <a id="506" href="foundation-core.truncation-levels.html#435" class="Function">neg-one-𝕋</a>

<a id="one-𝕋"></a><a id="517" href="foundation-core.truncation-levels.html#517" class="Function">one-𝕋</a> <a id="523" class="Symbol">:</a> <a id="525" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a>
<a id="527" href="foundation-core.truncation-levels.html#517" class="Function">one-𝕋</a> <a id="533" class="Symbol">=</a> <a id="535" href="foundation-core.truncation-levels.html#419" class="InductiveConstructor">succ-𝕋</a> <a id="542" href="foundation-core.truncation-levels.html#479" class="Function">zero-𝕋</a>

<a id="two-𝕋"></a><a id="550" href="foundation-core.truncation-levels.html#550" class="Function">two-𝕋</a> <a id="556" class="Symbol">:</a> <a id="558" href="foundation-core.truncation-levels.html#382" class="Datatype">𝕋</a>
<a id="560" href="foundation-core.truncation-levels.html#550" class="Function">two-𝕋</a> <a id="566" class="Symbol">=</a> <a id="568" href="foundation-core.truncation-levels.html#419" class="InductiveConstructor">succ-𝕋</a> <a id="575" href="foundation-core.truncation-levels.html#517" class="Function">one-𝕋</a>
</pre>