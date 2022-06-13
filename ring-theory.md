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
<a id="537" class="Keyword">open</a> <a id="542" class="Keyword">import</a> <a id="549" href="ring-theory.local-rings.html" class="Module">ring-theory.local-rings</a> <a id="573" class="Keyword">public</a>
<a id="580" class="Keyword">open</a> <a id="585" class="Keyword">import</a> <a id="592" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a> <a id="624" class="Keyword">public</a>
<a id="631" class="Keyword">open</a> <a id="636" class="Keyword">import</a> <a id="643" href="ring-theory.modules-rings.html" class="Module">ring-theory.modules-rings</a> <a id="669" class="Keyword">public</a>
<a id="676" class="Keyword">open</a> <a id="681" class="Keyword">import</a> <a id="688" href="ring-theory.nil-ideals-rings.html" class="Module">ring-theory.nil-ideals-rings</a> <a id="717" class="Keyword">public</a>
<a id="724" class="Keyword">open</a> <a id="729" class="Keyword">import</a> <a id="736" href="ring-theory.nilpotent-elements-rings.html" class="Module">ring-theory.nilpotent-elements-rings</a> <a id="773" class="Keyword">public</a>
<a id="780" class="Keyword">open</a> <a id="785" class="Keyword">import</a> <a id="792" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a> <a id="821" class="Keyword">public</a>
<a id="828" class="Keyword">open</a> <a id="833" class="Keyword">import</a> <a id="840" href="ring-theory.opposite-rings.html" class="Module">ring-theory.opposite-rings</a> <a id="867" class="Keyword">public</a>
<a id="874" class="Keyword">open</a> <a id="879" class="Keyword">import</a> <a id="886" href="ring-theory.powers-of-elements-rings.html" class="Module">ring-theory.powers-of-elements-rings</a> <a id="923" class="Keyword">public</a>
<a id="930" class="Keyword">open</a> <a id="935" class="Keyword">import</a> <a id="942" href="ring-theory.products-rings.html" class="Module">ring-theory.products-rings</a> <a id="969" class="Keyword">public</a>
<a id="976" class="Keyword">open</a> <a id="981" class="Keyword">import</a> <a id="988" href="ring-theory.radical-ideals-rings.html" class="Module">ring-theory.radical-ideals-rings</a> <a id="1021" class="Keyword">public</a>
<a id="1028" class="Keyword">open</a> <a id="1033" class="Keyword">import</a> <a id="1040" href="ring-theory.rings.html" class="Module">ring-theory.rings</a> <a id="1058" class="Keyword">public</a>
<a id="1065" class="Keyword">open</a> <a id="1070" class="Keyword">import</a> <a id="1077" href="ring-theory.subsets-rings.html" class="Module">ring-theory.subsets-rings</a> <a id="1103" class="Keyword">public</a>
</pre>