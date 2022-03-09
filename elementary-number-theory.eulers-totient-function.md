# Euler's totient function

<pre class="Agda"><a id="37" class="Symbol">{-#</a> <a id="41" class="Keyword">OPTIONS</a> <a id="49" class="Pragma">--without-K</a> <a id="61" class="Pragma">--exact-split</a> <a id="75" class="Pragma">--allow-unsolved-metas</a> <a id="98" class="Symbol">#-}</a>

<a id="103" class="Keyword">module</a> <a id="110" href="elementary-number-theory.eulers-totient-function.html" class="Module">elementary-number-theory.eulers-totient-function</a> <a id="159" class="Keyword">where</a>

<a id="166" class="Keyword">open</a> <a id="171" class="Keyword">import</a> <a id="178" href="elementary-number-theory.html" class="Module">elementary-number-theory</a>
<a id="203" class="Keyword">open</a> <a id="208" class="Keyword">import</a> <a id="215" href="foundation.html" class="Module">foundation</a>
<a id="226" class="Keyword">open</a> <a id="231" class="Keyword">import</a> <a id="238" href="univalent-combinatorics.html" class="Module">univalent-combinatorics</a>
</pre>
## Idea

Euler's totient function `φ : ℕ → ℕ` is the function that maps a natural number `n` to the number of `x < n` that are relatively prime with `n`.

## Definition

