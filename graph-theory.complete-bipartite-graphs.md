---
title: Complete bipartite graphs
---

<pre class="Agda"><a id="51" class="Symbol">{-#</a> <a id="55" class="Keyword">OPTIONS</a> <a id="63" class="Pragma">--without-K</a> <a id="75" class="Pragma">--exact-split</a> <a id="89" class="Symbol">#-}</a>

<a id="94" class="Keyword">module</a> <a id="101" href="graph-theory.complete-bipartite-graphs.html" class="Module">graph-theory.complete-bipartite-graphs</a> <a id="140" class="Keyword">where</a>

<a id="147" class="Keyword">open</a> <a id="152" class="Keyword">import</a> <a id="159" href="foundation.coproduct-types.html" class="Module">foundation.coproduct-types</a>
<a id="186" class="Keyword">open</a> <a id="191" class="Keyword">import</a> <a id="198" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="230" class="Keyword">open</a> <a id="235" class="Keyword">import</a> <a id="242" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a>

<a id="270" class="Keyword">open</a> <a id="275" class="Keyword">import</a> <a id="282" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>

<a id="310" class="Keyword">open</a> <a id="315" class="Keyword">import</a> <a id="322" href="univalent-combinatorics.2-element-types.html" class="Module">univalent-combinatorics.2-element-types</a>
<a id="362" class="Keyword">open</a> <a id="367" class="Keyword">import</a> <a id="374" href="univalent-combinatorics.cartesian-product-types.html" class="Module">univalent-combinatorics.cartesian-product-types</a>
<a id="422" class="Keyword">open</a> <a id="427" class="Keyword">import</a> <a id="434" href="univalent-combinatorics.coproduct-types.html" class="Module">univalent-combinatorics.coproduct-types</a>
<a id="474" class="Keyword">open</a> <a id="479" class="Keyword">import</a> <a id="486" href="univalent-combinatorics.dependent-sum-finite-types.html" class="Module">univalent-combinatorics.dependent-sum-finite-types</a>
<a id="537" class="Keyword">open</a> <a id="542" class="Keyword">import</a> <a id="549" href="univalent-combinatorics.fibers-of-maps.html" class="Module">univalent-combinatorics.fibers-of-maps</a>
<a id="588" class="Keyword">open</a> <a id="593" class="Keyword">import</a> <a id="600" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
</pre>
## Definition

<pre class="Agda"><a id="complete-bipartite-Undirected-Graph-𝔽"></a><a id="665" href="graph-theory.complete-bipartite-graphs.html#665" class="Function">complete-bipartite-Undirected-Graph-𝔽</a> <a id="703" class="Symbol">:</a> <a id="705" href="univalent-combinatorics.finite-types.html#4877" class="Function">𝔽</a> <a id="707" class="Symbol">→</a> <a id="709" href="univalent-combinatorics.finite-types.html#4877" class="Function">𝔽</a> <a id="711" class="Symbol">→</a> <a id="713" href="graph-theory.finite-graphs.html#1298" class="Function">Undirected-Graph-𝔽</a>
<a id="732" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="736" class="Symbol">(</a><a id="737" href="graph-theory.complete-bipartite-graphs.html#665" class="Function">complete-bipartite-Undirected-Graph-𝔽</a> <a id="775" href="graph-theory.complete-bipartite-graphs.html#775" class="Bound">X</a> <a id="777" href="graph-theory.complete-bipartite-graphs.html#777" class="Bound">Y</a><a id="778" class="Symbol">)</a> <a id="780" class="Symbol">=</a> <a id="782" href="univalent-combinatorics.coproduct-types.html#5414" class="Function">coprod-𝔽</a> <a id="791" href="graph-theory.complete-bipartite-graphs.html#775" class="Bound">X</a> <a id="793" href="graph-theory.complete-bipartite-graphs.html#777" class="Bound">Y</a>
<a id="795" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="799" class="Symbol">(</a><a id="800" href="graph-theory.complete-bipartite-graphs.html#665" class="Function">complete-bipartite-Undirected-Graph-𝔽</a> <a id="838" href="graph-theory.complete-bipartite-graphs.html#838" class="Bound">X</a> <a id="840" href="graph-theory.complete-bipartite-graphs.html#840" class="Bound">Y</a><a id="841" class="Symbol">)</a> <a id="843" href="graph-theory.complete-bipartite-graphs.html#843" class="Bound">p</a> <a id="845" class="Symbol">=</a>
  <a id="849" href="univalent-combinatorics.cartesian-product-types.html#5725" class="Function">prod-𝔽</a> <a id="856" class="Symbol">(</a> <a id="858" href="univalent-combinatorics.dependent-sum-finite-types.html#2958" class="Function">Σ-𝔽</a> <a id="862" href="graph-theory.complete-bipartite-graphs.html#838" class="Bound">X</a>
           <a id="875" class="Symbol">(</a> <a id="877" class="Symbol">λ</a> <a id="879" href="graph-theory.complete-bipartite-graphs.html#879" class="Bound">x</a> <a id="881" class="Symbol">→</a>
             <a id="896" href="univalent-combinatorics.fibers-of-maps.html#3421" class="Function">fib-𝔽</a>
               <a id="917" class="Symbol">(</a> <a id="919" href="univalent-combinatorics.2-element-types.html#5284" class="Function">finite-type-2-Element-Type</a> <a id="946" class="Symbol">(</a><a id="947" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="951" href="graph-theory.complete-bipartite-graphs.html#843" class="Bound">p</a><a id="952" class="Symbol">))</a>
               <a id="970" class="Symbol">(</a> <a id="972" href="univalent-combinatorics.coproduct-types.html#5414" class="Function">coprod-𝔽</a> <a id="981" href="graph-theory.complete-bipartite-graphs.html#838" class="Bound">X</a> <a id="983" href="graph-theory.complete-bipartite-graphs.html#840" class="Bound">Y</a><a id="984" class="Symbol">)</a>
               <a id="1001" class="Symbol">(</a> <a id="1003" href="foundation.unordered-pairs.html#3488" class="Function">element-unordered-pair</a> <a id="1026" href="graph-theory.complete-bipartite-graphs.html#843" class="Bound">p</a><a id="1027" class="Symbol">)</a>
               <a id="1044" class="Symbol">(</a> <a id="1046" href="foundation.coproduct-types.html#1250" class="InductiveConstructor">inl</a> <a id="1050" href="graph-theory.complete-bipartite-graphs.html#879" class="Bound">x</a><a id="1051" class="Symbol">)))</a>
         <a id="1064" class="Symbol">(</a> <a id="1066" href="univalent-combinatorics.dependent-sum-finite-types.html#2958" class="Function">Σ-𝔽</a> <a id="1070" href="graph-theory.complete-bipartite-graphs.html#840" class="Bound">Y</a>
           <a id="1083" class="Symbol">(</a> <a id="1085" class="Symbol">λ</a> <a id="1087" href="graph-theory.complete-bipartite-graphs.html#1087" class="Bound">y</a> <a id="1089" class="Symbol">→</a>
             <a id="1104" href="univalent-combinatorics.fibers-of-maps.html#3421" class="Function">fib-𝔽</a>
               <a id="1125" class="Symbol">(</a> <a id="1127" href="univalent-combinatorics.2-element-types.html#5284" class="Function">finite-type-2-Element-Type</a> <a id="1154" class="Symbol">(</a><a id="1155" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="1159" href="graph-theory.complete-bipartite-graphs.html#843" class="Bound">p</a><a id="1160" class="Symbol">))</a>
               <a id="1178" class="Symbol">(</a> <a id="1180" href="univalent-combinatorics.coproduct-types.html#5414" class="Function">coprod-𝔽</a> <a id="1189" href="graph-theory.complete-bipartite-graphs.html#838" class="Bound">X</a> <a id="1191" href="graph-theory.complete-bipartite-graphs.html#840" class="Bound">Y</a><a id="1192" class="Symbol">)</a>
               <a id="1209" class="Symbol">(</a> <a id="1211" href="foundation.unordered-pairs.html#3488" class="Function">element-unordered-pair</a> <a id="1234" href="graph-theory.complete-bipartite-graphs.html#843" class="Bound">p</a><a id="1235" class="Symbol">)</a>
               <a id="1252" class="Symbol">(</a> <a id="1254" href="foundation.coproduct-types.html#1268" class="InductiveConstructor">inr</a> <a id="1258" href="graph-theory.complete-bipartite-graphs.html#1087" class="Bound">y</a><a id="1259" class="Symbol">)))</a>
</pre>