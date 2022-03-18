---
title: Formalisation of the Symmetry Book
---

<pre class="Agda"><a id="60" class="Symbol">{-#</a> <a id="64" class="Keyword">OPTIONS</a> <a id="72" class="Pragma">--without-K</a> <a id="84" class="Pragma">--exact-split</a> <a id="98" class="Symbol">#-}</a>

<a id="103" class="Keyword">module</a> <a id="110" href="synthetic-homotopy-theory.html" class="Module">synthetic-homotopy-theory</a> <a id="136" class="Keyword">where</a>

<a id="143" class="Keyword">open</a> <a id="148" class="Keyword">import</a> <a id="155" href="univalent-foundations.html" class="Module">univalent-foundations</a> <a id="177" class="Keyword">public</a>

<a id="185" class="Keyword">open</a> <a id="190" class="Keyword">import</a> <a id="197" href="synthetic-homotopy-theory.23-pullbacks.html" class="Module">synthetic-homotopy-theory.23-pullbacks</a> <a id="236" class="Keyword">public</a>
<a id="243" class="Keyword">open</a> <a id="248" class="Keyword">import</a> <a id="255" href="synthetic-homotopy-theory.24-pushouts.html" class="Module">synthetic-homotopy-theory.24-pushouts</a> <a id="293" class="Keyword">public</a>
<a id="300" class="Keyword">open</a> <a id="305" class="Keyword">import</a> <a id="312" href="synthetic-homotopy-theory.25-cubical-diagrams.html" class="Module">synthetic-homotopy-theory.25-cubical-diagrams</a> <a id="358" class="Keyword">public</a>
<a id="365" class="Keyword">open</a> <a id="370" class="Keyword">import</a> <a id="377" href="synthetic-homotopy-theory.26-descent.html" class="Module">synthetic-homotopy-theory.26-descent</a> <a id="414" class="Keyword">public</a>
<a id="421" class="Keyword">open</a> <a id="426" class="Keyword">import</a> <a id="433" href="synthetic-homotopy-theory.26-id-pushout.html" class="Module">synthetic-homotopy-theory.26-id-pushout</a> <a id="473" class="Keyword">public</a>
<a id="480" class="Keyword">open</a> <a id="485" class="Keyword">import</a> <a id="492" href="synthetic-homotopy-theory.27-sequences.html" class="Module">synthetic-homotopy-theory.27-sequences</a> <a id="531" class="Keyword">public</a>
<a id="538" class="Keyword">open</a> <a id="543" class="Keyword">import</a> <a id="550" href="synthetic-homotopy-theory.circle.html" class="Module">synthetic-homotopy-theory.circle</a> <a id="583" class="Keyword">public</a>
<a id="590" class="Keyword">open</a> <a id="595" class="Keyword">import</a> <a id="602" href="synthetic-homotopy-theory.cyclic-types.html" class="Module">synthetic-homotopy-theory.cyclic-types</a> <a id="641" class="Keyword">public</a>
<a id="648" class="Keyword">open</a> <a id="653" class="Keyword">import</a> <a id="660" href="synthetic-homotopy-theory.double-loop-spaces.html" class="Module">synthetic-homotopy-theory.double-loop-spaces</a> <a id="705" class="Keyword">public</a>
<a id="712" class="Keyword">open</a> <a id="717" class="Keyword">import</a> <a id="724" href="synthetic-homotopy-theory.functoriality-loop-spaces.html" class="Module">synthetic-homotopy-theory.functoriality-loop-spaces</a> <a id="776" class="Keyword">public</a>
<a id="783" class="Keyword">open</a> <a id="788" class="Keyword">import</a> <a id="795" href="synthetic-homotopy-theory.infinite-cyclic-types.html" class="Module">synthetic-homotopy-theory.infinite-cyclic-types</a> <a id="843" class="Keyword">public</a>
<a id="850" class="Keyword">open</a> <a id="855" class="Keyword">import</a> <a id="862" href="synthetic-homotopy-theory.interval-type.html" class="Module">synthetic-homotopy-theory.interval-type</a> <a id="902" class="Keyword">public</a>
<a id="909" class="Keyword">open</a> <a id="914" class="Keyword">import</a> <a id="921" href="synthetic-homotopy-theory.iterated-loop-spaces.html" class="Module">synthetic-homotopy-theory.iterated-loop-spaces</a> <a id="968" class="Keyword">public</a>
<a id="975" class="Keyword">open</a> <a id="980" class="Keyword">import</a> <a id="987" href="synthetic-homotopy-theory.loop-spaces.html" class="Module">synthetic-homotopy-theory.loop-spaces</a> <a id="1025" class="Keyword">public</a>
<a id="1032" class="Keyword">open</a> <a id="1037" class="Keyword">import</a> <a id="1044" href="synthetic-homotopy-theory.pointed-dependent-functions.html" class="Module">synthetic-homotopy-theory.pointed-dependent-functions</a> <a id="1098" class="Keyword">public</a>
<a id="1105" class="Keyword">open</a> <a id="1110" class="Keyword">import</a> <a id="1117" href="synthetic-homotopy-theory.pointed-families-of-types.html" class="Module">synthetic-homotopy-theory.pointed-families-of-types</a> <a id="1169" class="Keyword">public</a>
<a id="1176" class="Keyword">open</a> <a id="1181" class="Keyword">import</a> <a id="1188" href="synthetic-homotopy-theory.pointed-homotopies.html" class="Module">synthetic-homotopy-theory.pointed-homotopies</a> <a id="1233" class="Keyword">public</a>
<a id="1240" class="Keyword">open</a> <a id="1245" class="Keyword">import</a> <a id="1252" href="synthetic-homotopy-theory.pointed-maps.html" class="Module">synthetic-homotopy-theory.pointed-maps</a> <a id="1291" class="Keyword">public</a>
<a id="1298" class="Keyword">open</a> <a id="1303" class="Keyword">import</a> <a id="1310" href="synthetic-homotopy-theory.pointed-types.html" class="Module">synthetic-homotopy-theory.pointed-types</a> <a id="1350" class="Keyword">public</a>
<a id="1357" class="Keyword">open</a> <a id="1362" class="Keyword">import</a> <a id="1369" href="synthetic-homotopy-theory.spaces.html" class="Module">synthetic-homotopy-theory.spaces</a> <a id="1402" class="Keyword">public</a>
<a id="1409" class="Keyword">open</a> <a id="1414" class="Keyword">import</a> <a id="1421" href="synthetic-homotopy-theory.triple-loop-spaces.html" class="Module">synthetic-homotopy-theory.triple-loop-spaces</a> <a id="1466" class="Keyword">public</a>
<a id="1473" class="Keyword">open</a> <a id="1478" class="Keyword">import</a> <a id="1485" href="synthetic-homotopy-theory.universal-cover-circle.html" class="Module">synthetic-homotopy-theory.universal-cover-circle</a> <a id="1534" class="Keyword">public</a>
</pre>