# Finitely π-presented types

<pre class="Agda"><a id="39" class="Symbol">{-#</a> <a id="43" class="Keyword">OPTIONS</a> <a id="51" class="Pragma">--without-K</a> <a id="63" class="Pragma">--exact-split</a> <a id="77" class="Pragma">--allow-unsolved-metas</a> <a id="100" class="Symbol">#-}</a>

<a id="105" class="Keyword">module</a> <a id="112" href="univalent-combinatorics.presented-pi-finite-types.html" class="Module">univalent-combinatorics.presented-pi-finite-types</a> <a id="162" class="Keyword">where</a>
</pre>
## Idea

A type `A` is said to be finitely `π_0`-presented if there is a standard pruned tree `T` of height 1 so that `A` has a presentation of cardinality `width T`, and `A` is said to be finitely `π_{n+1}`-presented if there is a standard pruned tree `T` of height `n+2` and a map `f : Fin (width T) → A` so that `η ∘ f : Fin (width T) → ∥A∥_0` is an equivalence, and for each `x : Fin (width T)` the type `Ω (A, f x)` is 
