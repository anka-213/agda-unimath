---
title: Multiset coefficients
---

<pre class="Agda"><a id="47" class="Keyword">module</a> <a id="54" href="elementary-number-theory.multiset-coefficients.html" class="Module">elementary-number-theory.multiset-coefficients</a> <a id="101" class="Keyword">where</a>

<a id="108" class="Keyword">open</a> <a id="113" class="Keyword">import</a> <a id="120" href="elementary-number-theory.addition-natural-numbers.html" class="Module">elementary-number-theory.addition-natural-numbers</a>
<a id="170" class="Keyword">open</a> <a id="175" class="Keyword">import</a> <a id="182" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a>
</pre>
## Idea

The multiset coefficients count the number of multisets of size `k` of elements of a set of size `n`. In oter words, it counts the number of connected componets of the type

```md
  Σ (A : Fin n → 𝔽), ∥ Fin k ≃ Σ (i : Fin n), A i ∥. 
```

## Definition

<pre class="Agda"><a id="multiset-coefficient"></a><a id="499" href="elementary-number-theory.multiset-coefficients.html#499" class="Function">multiset-coefficient</a> <a id="520" class="Symbol">:</a> <a id="522" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="524" class="Symbol">→</a> <a id="526" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="528" class="Symbol">→</a> <a id="530" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a>
<a id="532" href="elementary-number-theory.multiset-coefficients.html#499" class="Function">multiset-coefficient</a> <a id="553" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a> <a id="560" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a> <a id="567" class="Symbol">=</a> <a id="569" class="Number">1</a>
<a id="571" href="elementary-number-theory.multiset-coefficients.html#499" class="Function">multiset-coefficient</a> <a id="592" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a> <a id="599" class="Symbol">(</a><a id="600" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="607" href="elementary-number-theory.multiset-coefficients.html#607" class="Bound">k</a><a id="608" class="Symbol">)</a> <a id="610" class="Symbol">=</a> <a id="612" class="Number">0</a>
<a id="614" href="elementary-number-theory.multiset-coefficients.html#499" class="Function">multiset-coefficient</a> <a id="635" class="Symbol">(</a><a id="636" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="643" href="elementary-number-theory.multiset-coefficients.html#643" class="Bound">n</a><a id="644" class="Symbol">)</a> <a id="646" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a> <a id="653" class="Symbol">=</a> <a id="655" class="Number">1</a>
<a id="657" href="elementary-number-theory.multiset-coefficients.html#499" class="Function">multiset-coefficient</a> <a id="678" class="Symbol">(</a><a id="679" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="686" href="elementary-number-theory.multiset-coefficients.html#686" class="Bound">n</a><a id="687" class="Symbol">)</a> <a id="689" class="Symbol">(</a><a id="690" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="697" href="elementary-number-theory.multiset-coefficients.html#697" class="Bound">k</a><a id="698" class="Symbol">)</a> <a id="700" class="Symbol">=</a>
  <a id="704" href="elementary-number-theory.addition-natural-numbers.html#1096" class="Function">add-ℕ</a> <a id="710" class="Symbol">(</a><a id="711" href="elementary-number-theory.multiset-coefficients.html#499" class="Function">multiset-coefficient</a> <a id="732" class="Symbol">(</a><a id="733" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="740" href="elementary-number-theory.multiset-coefficients.html#686" class="Bound">n</a><a id="741" class="Symbol">)</a> <a id="743" href="elementary-number-theory.multiset-coefficients.html#697" class="Bound">k</a><a id="744" class="Symbol">)</a> <a id="746" class="Symbol">(</a><a id="747" href="elementary-number-theory.multiset-coefficients.html#499" class="Function">multiset-coefficient</a> <a id="768" href="elementary-number-theory.multiset-coefficients.html#686" class="Bound">n</a> <a id="770" class="Symbol">(</a><a id="771" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="778" href="elementary-number-theory.multiset-coefficients.html#697" class="Bound">k</a><a id="779" class="Symbol">))</a>
</pre>