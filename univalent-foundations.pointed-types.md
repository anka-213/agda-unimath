# Pointed types

<pre class="Agda"><a id="26" class="Symbol">{-#</a> <a id="30" class="Keyword">OPTIONS</a> <a id="38" class="Pragma">--without-K</a> <a id="50" class="Pragma">--exact-split</a> <a id="64" class="Symbol">#-}</a>

<a id="69" class="Keyword">module</a> <a id="76" href="univalent-foundations.pointed-types.html" class="Module">univalent-foundations.pointed-types</a> <a id="112" class="Keyword">where</a>

<a id="119" class="Keyword">open</a> <a id="124" class="Keyword">import</a> <a id="131" href="foundation.html" class="Module">foundation</a> <a id="142" class="Keyword">public</a>
<a id="149" class="Keyword">open</a> <a id="154" class="Keyword">import</a> <a id="161" href="elementary-number-theory.html" class="Module">elementary-number-theory</a> <a id="186" class="Keyword">public</a>

<a id="194" class="Comment">-- The universe of pointed types</a>

<a id="Pointed-Type"></a><a id="228" href="univalent-foundations.pointed-types.html#228" class="Function">Pointed-Type</a> <a id="241" class="Symbol">:</a> <a id="243" class="Symbol">(</a><a id="244" href="univalent-foundations.pointed-types.html#244" class="Bound">l</a> <a id="246" class="Symbol">:</a> <a id="248" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="253" class="Symbol">)</a> <a id="255" class="Symbol">→</a> <a id="257" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="260" class="Symbol">(</a><a id="261" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="266" href="univalent-foundations.pointed-types.html#244" class="Bound">l</a><a id="267" class="Symbol">)</a>
<a id="269" href="univalent-foundations.pointed-types.html#228" class="Function">Pointed-Type</a> <a id="282" href="univalent-foundations.pointed-types.html#282" class="Bound">l</a> <a id="284" class="Symbol">=</a> <a id="286" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a> <a id="288" class="Symbol">(</a><a id="289" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="292" href="univalent-foundations.pointed-types.html#282" class="Bound">l</a><a id="293" class="Symbol">)</a> <a id="295" class="Symbol">(λ</a> <a id="298" href="univalent-foundations.pointed-types.html#298" class="Bound">X</a> <a id="300" class="Symbol">→</a> <a id="302" href="univalent-foundations.pointed-types.html#298" class="Bound">X</a><a id="303" class="Symbol">)</a>

<a id="306" class="Keyword">module</a> <a id="313" href="univalent-foundations.pointed-types.html#313" class="Module">_</a>
  <a id="317" class="Symbol">{</a><a id="318" href="univalent-foundations.pointed-types.html#318" class="Bound">l</a> <a id="320" class="Symbol">:</a> <a id="322" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="327" class="Symbol">}</a> <a id="329" class="Symbol">(</a><a id="330" href="univalent-foundations.pointed-types.html#330" class="Bound">A</a> <a id="332" class="Symbol">:</a> <a id="334" href="univalent-foundations.pointed-types.html#228" class="Function">Pointed-Type</a> <a id="347" href="univalent-foundations.pointed-types.html#318" class="Bound">l</a><a id="348" class="Symbol">)</a>
  <a id="352" class="Keyword">where</a>
  
  <a id="363" href="univalent-foundations.pointed-types.html#363" class="Function">type-Pointed-Type</a> <a id="381" class="Symbol">:</a> <a id="383" href="Agda.Primitive.html#326" class="Primitive">UU</a> <a id="386" href="univalent-foundations.pointed-types.html#318" class="Bound">l</a>
  <a id="390" href="univalent-foundations.pointed-types.html#363" class="Function">type-Pointed-Type</a> <a id="408" class="Symbol">=</a> <a id="410" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="414" href="univalent-foundations.pointed-types.html#330" class="Bound">A</a>
  
  <a id="421" href="univalent-foundations.pointed-types.html#421" class="Function">pt-Pointed-Type</a> <a id="437" class="Symbol">:</a> <a id="439" href="univalent-foundations.pointed-types.html#363" class="Function">type-Pointed-Type</a>
  <a id="459" href="univalent-foundations.pointed-types.html#421" class="Function">pt-Pointed-Type</a> <a id="475" class="Symbol">=</a> <a id="477" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="481" href="univalent-foundations.pointed-types.html#330" class="Bound">A</a>
</pre>