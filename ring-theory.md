---
title: Ring theory
---

<pre class="Agda"><a id="37" class="Symbol">{-#</a> <a id="41" class="Keyword">OPTIONS</a> <a id="49" class="Pragma">--without-K</a> <a id="61" class="Pragma">--exact-split</a> <a id="75" class="Symbol">#-}</a>

<a id="80" class="Keyword">module</a> <a id="87" href="ring-theory.html" class="Module">ring-theory</a> <a id="99" class="Keyword">where</a>

<a id="106" class="Keyword">open</a> <a id="111" class="Keyword">import</a> <a id="118" href="ring-theory.dependent-products-rings.html" class="Module">ring-theory.dependent-products-rings</a> <a id="155" class="Keyword">public</a>
<a id="162" class="Keyword">open</a> <a id="167" class="Keyword">import</a> <a id="174" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a> <a id="201" class="Keyword">public</a>
<a id="208" class="Keyword">open</a> <a id="213" class="Keyword">import</a> <a id="220" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a> <a id="252" class="Keyword">public</a>
<a id="259" class="Keyword">open</a> <a id="264" class="Keyword">import</a> <a id="271" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a> <a id="317" class="Keyword">public</a>
<a id="324" class="Keyword">open</a> <a id="329" class="Keyword">import</a> <a id="336" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a> <a id="361" class="Keyword">public</a>
<a id="368" class="Keyword">open</a> <a id="373" class="Keyword">import</a> <a id="380" href="ring-theory.invariant-basis-property-rings.html" class="Module">ring-theory.invariant-basis-property-rings</a> <a id="423" class="Keyword">public</a>
<a id="430" class="Keyword">open</a> <a id="435" class="Keyword">import</a> <a id="442" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a> <a id="480" class="Keyword">public</a>
<a id="487" class="Keyword">open</a> <a id="492" class="Keyword">import</a> <a id="499" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a> <a id="530" class="Keyword">public</a>
<a id="537" class="Keyword">open</a> <a id="542" class="Keyword">import</a> <a id="549" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a> <a id="581" class="Keyword">public</a>
<a id="588" class="Keyword">open</a> <a id="593" class="Keyword">import</a> <a id="600" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a> <a id="626" class="Keyword">public</a>
<a id="633" class="Keyword">open</a> <a id="638" class="Keyword">import</a> <a id="645" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a> <a id="674" class="Keyword">public</a>
<a id="681" class="Keyword">open</a> <a id="686" class="Keyword">import</a> <a id="693" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a> <a id="730" class="Keyword">public</a>
<a id="737" class="Keyword">open</a> <a id="742" class="Keyword">import</a> <a id="749" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a> <a id="778" class="Keyword">public</a>
<a id="785" class="Keyword">open</a> <a id="790" class="Keyword">import</a> <a id="797" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a> <a id="824" class="Keyword">public</a>
<a id="831" class="Keyword">open</a> <a id="836" class="Keyword">import</a> <a id="843" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a> <a id="880" class="Keyword">public</a>
<a id="887" class="Keyword">open</a> <a id="892" class="Keyword">import</a> <a id="899" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a> <a id="926" class="Keyword">public</a>
<a id="933" class="Keyword">open</a> <a id="938" class="Keyword">import</a> <a id="945" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a> <a id="978" class="Keyword">public</a>
<a id="985" class="Keyword">open</a> <a id="990" class="Keyword">import</a> <a id="997" href="ring-theory.rings.html" class="Module">ring-theory.rings</a> <a id="1015" class="Keyword">public</a>
<a id="1022" class="Keyword">open</a> <a id="1027" class="Keyword">import</a> <a id="1034" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a> <a id="1060" class="Keyword">public</a>
</pre>