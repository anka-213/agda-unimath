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
<a id="588" class="Keyword">open</a> <a id="593" class="Keyword">import</a> <a id="600" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a> <a id="629" class="Keyword">public</a>
<a id="636" class="Keyword">open</a> <a id="641" class="Keyword">import</a> <a id="648" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a> <a id="675" class="Keyword">public</a>
<a id="682" class="Keyword">open</a> <a id="687" class="Keyword">import</a> <a id="694" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a> <a id="721" class="Keyword">public</a>
<a id="728" class="Keyword">open</a> <a id="733" class="Keyword">import</a> <a id="740" href="ring-theory.rings.html" class="Module">ring-theory.rings</a> <a id="758" class="Keyword">public</a>
</pre>