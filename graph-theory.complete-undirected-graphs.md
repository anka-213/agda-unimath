---
title: Complete undirected graphs
---

<pre class="Agda"><a id="52" class="Symbol">{-#</a> <a id="56" class="Keyword">OPTIONS</a> <a id="64" class="Pragma">--without-K</a> <a id="76" class="Pragma">--exact-split</a> <a id="90" class="Symbol">#-}</a>

<a id="95" class="Keyword">module</a> <a id="102" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a> <a id="142" class="Keyword">where</a>

<a id="149" class="Keyword">open</a> <a id="154" class="Keyword">import</a> <a id="161" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="203" class="Keyword">open</a> <a id="208" class="Keyword">import</a> <a id="215" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>

<a id="243" class="Keyword">open</a> <a id="248" class="Keyword">import</a> <a id="255" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
</pre>
## Idea

A complete undirected graph is a complete multipartite graph in which every block has exactly one vertex. In other words, it is an undirected graph in which every vertex is connected to every other vertex.

There are many ways of presenting complete undirected graphs. For example, the type of edges in a complete undirected graph is a 2-element subtype of the type of its vertices.

## Definition

<pre class="Agda"><a id="complete-Undirected-Graph-𝔽"></a><a id="713" href="graph-theory.complete-undirected-graphs.html#713" class="Function">complete-Undirected-Graph-𝔽</a> <a id="741" class="Symbol">:</a> <a id="743" href="univalent-combinatorics.finite-types.html#4743" class="Function">𝔽</a> <a id="745" class="Symbol">→</a> <a id="747" href="graph-theory.finite-graphs.html#1298" class="Function">Undirected-Graph-𝔽</a>
<a id="766" href="graph-theory.complete-undirected-graphs.html#713" class="Function">complete-Undirected-Graph-𝔽</a> <a id="794" href="graph-theory.complete-undirected-graphs.html#794" class="Bound">X</a> <a id="796" class="Symbol">=</a> <a id="798" href="graph-theory.complete-multipartite-graphs.html#826" class="Function">complete-multipartite-Undirected-Graph-𝔽</a> <a id="839" href="graph-theory.complete-undirected-graphs.html#794" class="Bound">X</a> <a id="841" class="Symbol">(λ</a> <a id="844" href="graph-theory.complete-undirected-graphs.html#844" class="Bound">x</a> <a id="846" class="Symbol">→</a> <a id="848" href="univalent-combinatorics.finite-types.html#8782" class="Function">unit-𝔽</a><a id="854" class="Symbol">)</a>
</pre>