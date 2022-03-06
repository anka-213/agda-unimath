# Decidable subtypes of finite types

<pre class="Agda"><a id="47" class="Symbol">{-#</a> <a id="51" class="Keyword">OPTIONS</a> <a id="59" class="Pragma">--without-K</a> <a id="71" class="Pragma">--exact-split</a> <a id="85" class="Symbol">#-}</a>

<a id="90" class="Keyword">module</a> <a id="97" href="univalent-combinatorics.decidable-subtypes.html" class="Module">univalent-combinatorics.decidable-subtypes</a> <a id="140" class="Keyword">where</a>

<a id="147" class="Keyword">open</a> <a id="152" class="Keyword">import</a> <a id="159" href="foundation.decidable-subtypes.html" class="Module">foundation.decidable-subtypes</a> <a id="189" class="Keyword">public</a>

<a id="197" class="Keyword">open</a> <a id="202" class="Keyword">import</a> <a id="209" href="foundation.decidable-propositions.html" class="Module">foundation.decidable-propositions</a> <a id="243" class="Keyword">using</a>
  <a id="251" class="Symbol">(</a> <a id="253" href="foundation.decidable-propositions.html#2022" class="Function">prop-decidable-Prop</a><a id="272" class="Symbol">;</a> <a id="274" href="foundation.decidable-propositions.html#2361" class="Function">is-decidable-type-decidable-Prop</a><a id="306" class="Symbol">)</a>
<a id="308" class="Keyword">open</a> <a id="313" class="Keyword">import</a> <a id="320" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="347" class="Keyword">using</a> <a id="353" class="Symbol">(</a><a id="354" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="359" class="Symbol">;</a> <a id="361" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="363" class="Symbol">)</a>

<a id="366" class="Keyword">open</a> <a id="371" class="Keyword">import</a> <a id="378" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a> <a id="429" class="Keyword">using</a>
  <a id="437" class="Symbol">(</a> <a id="439" href="univalent-combinatorics.dependent-sum-finite-types.html#2479" class="Function">is-finite-Σ</a><a id="450" class="Symbol">)</a>
<a id="452" class="Keyword">open</a> <a id="457" class="Keyword">import</a> <a id="464" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a> <a id="501" class="Keyword">using</a>
  <a id="509" class="Symbol">(</a> <a id="511" href="univalent-combinatorics.finite-types.html#3732" class="Function">is-finite</a><a id="520" class="Symbol">;</a> <a id="522" href="univalent-combinatorics.finite-types.html#8538" class="Function">is-finite-is-decidable-Prop</a><a id="549" class="Symbol">)</a>
</pre>
## Idea

Decidable subtypes of finite types are finite.

## Properties

<pre class="Agda"><a id="636" class="Keyword">module</a> <a id="643" href="univalent-combinatorics.decidable-subtypes.html#643" class="Module">_</a>
  <a id="647" class="Symbol">{</a><a id="648" href="univalent-combinatorics.decidable-subtypes.html#648" class="Bound">l1</a> <a id="651" href="univalent-combinatorics.decidable-subtypes.html#651" class="Bound">l2</a> <a id="654" class="Symbol">:</a> <a id="656" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="661" class="Symbol">}</a> <a id="663" class="Symbol">{</a><a id="664" href="univalent-combinatorics.decidable-subtypes.html#664" class="Bound">X</a> <a id="666" class="Symbol">:</a> <a id="668" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a> <a id="671" href="univalent-combinatorics.decidable-subtypes.html#648" class="Bound">l1</a><a id="673" class="Symbol">}</a> <a id="675" class="Symbol">(</a><a id="676" href="univalent-combinatorics.decidable-subtypes.html#676" class="Bound">P</a> <a id="678" class="Symbol">:</a> <a id="680" href="foundation.decidable-subtypes.html#819" class="Function">decidable-subtype</a> <a id="698" href="univalent-combinatorics.decidable-subtypes.html#651" class="Bound">l2</a> <a id="701" href="univalent-combinatorics.decidable-subtypes.html#664" class="Bound">X</a><a id="702" class="Symbol">)</a>
  <a id="706" class="Keyword">where</a>

  <a id="715" class="Keyword">abstract</a>
    <a id="728" href="univalent-combinatorics.decidable-subtypes.html#728" class="Function">is-finite-decidable-subtype</a> <a id="756" class="Symbol">:</a>
      <a id="764" href="univalent-combinatorics.finite-types.html#3732" class="Function">is-finite</a> <a id="774" href="univalent-combinatorics.decidable-subtypes.html#664" class="Bound">X</a> <a id="776" class="Symbol">→</a> <a id="778" href="univalent-combinatorics.finite-types.html#3732" class="Function">is-finite</a> <a id="788" class="Symbol">(</a><a id="789" href="foundation.decidable-subtypes.html#1625" class="Function">type-decidable-subtype</a> <a id="812" href="univalent-combinatorics.decidable-subtypes.html#676" class="Bound">P</a><a id="813" class="Symbol">)</a>
    <a id="819" href="univalent-combinatorics.decidable-subtypes.html#728" class="Function">is-finite-decidable-subtype</a> <a id="847" href="univalent-combinatorics.decidable-subtypes.html#847" class="Bound">H</a> <a id="849" class="Symbol">=</a>
      <a id="857" href="univalent-combinatorics.dependent-sum-finite-types.html#2479" class="Function">is-finite-Σ</a> <a id="869" href="univalent-combinatorics.decidable-subtypes.html#847" class="Bound">H</a>
        <a id="879" class="Symbol">(</a> <a id="881" class="Symbol">λ</a> <a id="883" href="univalent-combinatorics.decidable-subtypes.html#883" class="Bound">x</a> <a id="885" class="Symbol">→</a>
          <a id="897" href="univalent-combinatorics.finite-types.html#8538" class="Function">is-finite-is-decidable-Prop</a>
            <a id="937" class="Symbol">(</a> <a id="939" href="foundation.decidable-propositions.html#2022" class="Function">prop-decidable-Prop</a> <a id="959" class="Symbol">(</a><a id="960" href="univalent-combinatorics.decidable-subtypes.html#676" class="Bound">P</a> <a id="962" href="univalent-combinatorics.decidable-subtypes.html#883" class="Bound">x</a><a id="963" class="Symbol">))</a>
            <a id="978" class="Symbol">(</a> <a id="980" href="foundation.decidable-propositions.html#2361" class="Function">is-decidable-type-decidable-Prop</a> <a id="1013" class="Symbol">(</a><a id="1014" href="univalent-combinatorics.decidable-subtypes.html#676" class="Bound">P</a> <a id="1016" href="univalent-combinatorics.decidable-subtypes.html#883" class="Bound">x</a><a id="1017" class="Symbol">)))</a>
</pre>