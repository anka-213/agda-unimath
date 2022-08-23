---
title: Complete undirected graphs
---

<pre class="Agda"><a id="52" class="Symbol">{-#</a> <a id="56" class="Keyword">OPTIONS</a> <a id="64" class="Pragma">--without-K</a> <a id="76" class="Pragma">--exact-split</a> <a id="90" class="Symbol">#-}</a>

<a id="95" class="Keyword">module</a> <a id="102" href="graph-theory.complete-undirected-graphs.html" class="Module">graph-theory.complete-undirected-graphs</a> <a id="142" class="Keyword">where</a>

<a id="149" class="Keyword">open</a> <a id="154" class="Keyword">import</a> <a id="161" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="189" class="Keyword">open</a> <a id="194" class="Keyword">import</a> <a id="201" href="graph-theory.complete-multipartite-graphs.html" class="Module">graph-theory.complete-multipartite-graphs</a>
<a id="243" class="Keyword">open</a> <a id="248" class="Keyword">import</a> <a id="255" href="graph-theory.finite-graphs.html" class="Module">graph-theory.finite-graphs</a>

<a id="283" class="Keyword">open</a> <a id="288" class="Keyword">import</a> <a id="295" href="univalent-combinatorics.finite-types.html" class="Module">univalent-combinatorics.finite-types</a>
</pre>
## Idea

A complete undirected graph is a complete multipartite graph in which every block has exactly one vertex. In other words, it is an undirected graph in which every vertex is connected to every other vertex.

There are many ways of presenting complete undirected graphs. For example, the type of edges in a complete undirected graph is a 2-element subtype of the type of its vertices.

## Definition

<pre class="Agda"><a id="complete-Undirected-Graph-𝔽"></a><a id="753" href="graph-theory.complete-undirected-graphs.html#753" class="Function">complete-Undirected-Graph-𝔽</a> <a id="781" class="Symbol">:</a> <a id="783" class="Symbol">{</a><a id="784" href="graph-theory.complete-undirected-graphs.html#784" class="Bound">l</a> <a id="786" class="Symbol">:</a> <a id="788" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="793" class="Symbol">}</a> <a id="795" class="Symbol">→</a> <a id="797" href="univalent-combinatorics.finite-types.html#4550" class="Function">𝔽</a> <a id="799" href="graph-theory.complete-undirected-graphs.html#784" class="Bound">l</a> <a id="801" class="Symbol">→</a> <a id="803" href="graph-theory.finite-graphs.html#1298" class="Function">Undirected-Graph-𝔽</a> <a id="822" href="graph-theory.complete-undirected-graphs.html#784" class="Bound">l</a> <a id="824" href="graph-theory.complete-undirected-graphs.html#784" class="Bound">l</a>
<a id="826" href="graph-theory.complete-undirected-graphs.html#753" class="Function">complete-Undirected-Graph-𝔽</a> <a id="854" href="graph-theory.complete-undirected-graphs.html#854" class="Bound">X</a> <a id="856" class="Symbol">=</a> <a id="858" href="graph-theory.complete-multipartite-graphs.html#865" class="Function">complete-multipartite-Undirected-Graph-𝔽</a> <a id="899" href="graph-theory.complete-undirected-graphs.html#854" class="Bound">X</a> <a id="901" class="Symbol">(λ</a> <a id="904" href="graph-theory.complete-undirected-graphs.html#904" class="Bound">x</a> <a id="906" class="Symbol">→</a> <a id="908" href="univalent-combinatorics.finite-types.html#8209" class="Function">unit-𝔽</a><a id="914" class="Symbol">)</a>
</pre>