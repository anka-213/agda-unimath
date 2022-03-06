# Universe levels

<pre class="Agda"><a id="28" class="Symbol">{-#</a> <a id="32" class="Keyword">OPTIONS</a> <a id="40" class="Pragma">--without-K</a> <a id="52" class="Pragma">--exact-split</a> <a id="66" class="Pragma">--safe</a> <a id="73" class="Pragma">--no-import-sorts</a> <a id="91" class="Symbol">#-}</a>

<a id="96" class="Keyword">module</a> <a id="103" href="foundation-core.universe-levels.html" class="Module">foundation-core.universe-levels</a> <a id="135" class="Keyword">where</a>

<a id="142" class="Keyword">open</a> <a id="147" class="Keyword">import</a> <a id="154" href="Agda.Primitive.html" class="Module">Agda.Primitive</a>
  <a id="171" class="Keyword">using</a> <a id="177" class="Symbol">(</a><a id="178" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="183" class="Symbol">;</a> <a id="185" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="190" class="Symbol">;</a> <a id="192" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="196" class="Symbol">;</a> <a id="198" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="201" class="Symbol">)</a>
  <a id="205" class="Keyword">renaming</a> <a id="214" class="Symbol">(</a><a id="215" href="Agda.Primitive.html#326" class="Primitive">Set</a> <a id="219" class="Symbol">to</a> <a id="222" class="Primitive">UU</a><a id="224" class="Symbol">;</a> <a id="226" href="Agda.Primitive.html#381" class="Primitive">Setω</a> <a id="231" class="Symbol">to</a> <a id="234" class="Primitive">UUω</a><a id="237" class="Symbol">)</a>
  <a id="241" class="Keyword">public</a>
</pre>
## Idea

We import Agda's built in mechanism of universe levels. The universes are called `UU`, which stands for `univalent universe`, although we will not immediately assume that universes are univalent.
