# Pointed types

<pre class="Agda"><a id="26" class="Symbol">{-#</a> <a id="30" class="Keyword">OPTIONS</a> <a id="38" class="Pragma">--without-K</a> <a id="50" class="Pragma">--exact-split</a> <a id="64" class="Symbol">#-}</a>

<a id="69" class="Keyword">module</a> <a id="76" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a> <a id="116" class="Keyword">where</a>

<a id="123" class="Keyword">open</a> <a id="128" class="Keyword">import</a> <a id="135" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="167" class="Keyword">using</a> <a id="173" class="Symbol">(</a><a id="174" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="175" class="Symbol">;</a> <a id="177" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="181" class="Symbol">;</a> <a id="183" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="186" class="Symbol">;</a> <a id="188" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="191" class="Symbol">)</a>
<a id="193" class="Keyword">open</a> <a id="198" class="Keyword">import</a> <a id="205" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="232" class="Keyword">using</a> <a id="238" class="Symbol">(</a><a id="239" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="244" class="Symbol">;</a> <a id="246" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="248" class="Symbol">;</a> <a id="250" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="254" class="Symbol">)</a>
</pre>
## Idea

A pointed type is a type `A` equipped with an element `a : A`.

## Definition

### The universe of pointed types

<pre class="Agda"><a id="Pointed-Type"></a><a id="392" href="synthetic-homotopy-theory.pointed-types.html#392" class="Function">Pointed-Type</a> <a id="405" class="Symbol">:</a> <a id="407" class="Symbol">(</a><a id="408" href="synthetic-homotopy-theory.pointed-types.html#408" class="Bound">l</a> <a id="410" class="Symbol">:</a> <a id="412" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="417" class="Symbol">)</a> <a id="419" class="Symbol">→</a> <a id="421" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="424" class="Symbol">(</a><a id="425" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="430" href="synthetic-homotopy-theory.pointed-types.html#408" class="Bound">l</a><a id="431" class="Symbol">)</a>
<a id="433" href="synthetic-homotopy-theory.pointed-types.html#392" class="Function">Pointed-Type</a> <a id="446" href="synthetic-homotopy-theory.pointed-types.html#446" class="Bound">l</a> <a id="448" class="Symbol">=</a> <a id="450" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="452" class="Symbol">(</a><a id="453" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="456" href="synthetic-homotopy-theory.pointed-types.html#446" class="Bound">l</a><a id="457" class="Symbol">)</a> <a id="459" class="Symbol">(λ</a> <a id="462" href="synthetic-homotopy-theory.pointed-types.html#462" class="Bound">X</a> <a id="464" class="Symbol">→</a> <a id="466" href="synthetic-homotopy-theory.pointed-types.html#462" class="Bound">X</a><a id="467" class="Symbol">)</a>

<a id="470" class="Keyword">module</a> <a id="477" href="synthetic-homotopy-theory.pointed-types.html#477" class="Module">_</a>
  <a id="481" class="Symbol">{</a><a id="482" href="synthetic-homotopy-theory.pointed-types.html#482" class="Bound">l</a> <a id="484" class="Symbol">:</a> <a id="486" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="491" class="Symbol">}</a> <a id="493" class="Symbol">(</a><a id="494" href="synthetic-homotopy-theory.pointed-types.html#494" class="Bound">A</a> <a id="496" class="Symbol">:</a> <a id="498" href="synthetic-homotopy-theory.pointed-types.html#392" class="Function">Pointed-Type</a> <a id="511" href="synthetic-homotopy-theory.pointed-types.html#482" class="Bound">l</a><a id="512" class="Symbol">)</a>
  <a id="516" class="Keyword">where</a>
  
  <a id="527" href="synthetic-homotopy-theory.pointed-types.html#527" class="Function">type-Pointed-Type</a> <a id="545" class="Symbol">:</a> <a id="547" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="550" href="synthetic-homotopy-theory.pointed-types.html#482" class="Bound">l</a>
  <a id="554" href="synthetic-homotopy-theory.pointed-types.html#527" class="Function">type-Pointed-Type</a> <a id="572" class="Symbol">=</a> <a id="574" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="578" href="synthetic-homotopy-theory.pointed-types.html#494" class="Bound">A</a>
  
  <a id="585" href="synthetic-homotopy-theory.pointed-types.html#585" class="Function">pt-Pointed-Type</a> <a id="601" class="Symbol">:</a> <a id="603" href="synthetic-homotopy-theory.pointed-types.html#527" class="Function">type-Pointed-Type</a>
  <a id="623" href="synthetic-homotopy-theory.pointed-types.html#585" class="Function">pt-Pointed-Type</a> <a id="639" class="Symbol">=</a> <a id="641" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="645" href="synthetic-homotopy-theory.pointed-types.html#494" class="Bound">A</a>
</pre>