---
title: Alkanes
---

<pre class="Agda"><a id="33" class="Symbol">{-#</a> <a id="37" class="Keyword">OPTIONS</a> <a id="45" class="Pragma">--without-K</a> <a id="57" class="Pragma">--exact-split</a> <a id="71" class="Symbol">#-}</a>

<a id="76" class="Keyword">module</a> <a id="83" href="organic-chemistry.alkanes.html" class="Module">organic-chemistry.alkanes</a> <a id="109" class="Keyword">where</a>

<a id="116" class="Keyword">open</a> <a id="121" class="Keyword">import</a> <a id="128" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="156" class="Keyword">open</a> <a id="161" class="Keyword">import</a> <a id="168" href="organic-chemistry.saturated-carbons.html" class="Module">organic-chemistry.saturated-carbons</a>
<a id="204" class="Keyword">open</a> <a id="209" class="Keyword">import</a> <a id="216" href="organic-chemistry.hydrocarbons.html" class="Module">organic-chemistry.hydrocarbons</a>
</pre>
## Idea

An **alkane** is a hydrocarbon that only has saturated carbons, i.e., it does not have any double or triple carbon-carbon bonds.

## Definition

<pre class="Agda"><a id="is-alkane-hydrocarbon"></a><a id="414" href="organic-chemistry.alkanes.html#414" class="Function">is-alkane-hydrocarbon</a> <a id="436" class="Symbol">:</a> <a id="438" class="Symbol">{</a><a id="439" href="organic-chemistry.alkanes.html#439" class="Bound">l1</a> <a id="442" href="organic-chemistry.alkanes.html#442" class="Bound">l2</a> <a id="445" class="Symbol">:</a> <a id="447" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="452" class="Symbol">}</a> <a id="454" class="Symbol">→</a> <a id="456" href="organic-chemistry.hydrocarbons.html#1564" class="Function">hydrocarbon</a> <a id="468" href="organic-chemistry.alkanes.html#439" class="Bound">l1</a> <a id="471" href="organic-chemistry.alkanes.html#442" class="Bound">l2</a> <a id="474" class="Symbol">→</a> <a id="476" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="479" class="Symbol">(</a><a id="480" href="organic-chemistry.alkanes.html#439" class="Bound">l1</a> <a id="483" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="485" href="organic-chemistry.alkanes.html#442" class="Bound">l2</a><a id="487" class="Symbol">)</a>
<a id="489" href="organic-chemistry.alkanes.html#414" class="Function">is-alkane-hydrocarbon</a> <a id="511" href="organic-chemistry.alkanes.html#511" class="Bound">H</a> <a id="513" class="Symbol">=</a> <a id="515" class="Symbol">∀</a> <a id="517" href="organic-chemistry.alkanes.html#517" class="Bound">c</a> <a id="519" class="Symbol">→</a> <a id="521" href="organic-chemistry.saturated-carbons.html#847" class="Function">is-saturated-carbon-hydrocarbon</a> <a id="553" href="organic-chemistry.alkanes.html#511" class="Bound">H</a> <a id="555" href="organic-chemistry.alkanes.html#517" class="Bound">c</a>
</pre>