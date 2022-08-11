---
title: Falling factorials
---

<pre class="Agda"><a id="44" class="Symbol">{-#</a> <a id="48" class="Keyword">OPTIONS</a> <a id="56" class="Pragma">--without-K</a> <a id="68" class="Pragma">--exact-split</a> <a id="82" class="Symbol">#-}</a>

<a id="87" class="Keyword">module</a> <a id="94" href="elementary-number-theory.falling-factorials.html" class="Module">elementary-number-theory.falling-factorials</a> <a id="138" class="Keyword">where</a>

<a id="145" class="Keyword">open</a> <a id="150" class="Keyword">import</a> <a id="157" href="elementary-number-theory.multiplication-natural-numbers.html" class="Module">elementary-number-theory.multiplication-natural-numbers</a> <a id="213" class="Keyword">using</a>
  <a id="221" class="Symbol">(</a> <a id="223" href="elementary-number-theory.multiplication-natural-numbers.html#1286" class="Function">mul-ℕ</a><a id="228" class="Symbol">)</a>
<a id="230" class="Keyword">open</a> <a id="235" class="Keyword">import</a> <a id="242" href="elementary-number-theory.natural-numbers.html" class="Module">elementary-number-theory.natural-numbers</a> <a id="283" class="Keyword">using</a> <a id="289" class="Symbol">(</a><a id="290" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a><a id="291" class="Symbol">;</a> <a id="293" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a><a id="299" class="Symbol">;</a> <a id="301" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a><a id="307" class="Symbol">)</a>
</pre>
## Idea

The falling factorial (n)_m is the number n(n-1)⋯(n-m+1)

## Definition

<pre class="Agda"><a id="falling-factorial-ℕ"></a><a id="404" href="elementary-number-theory.falling-factorials.html#404" class="Function">falling-factorial-ℕ</a> <a id="424" class="Symbol">:</a> <a id="426" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="428" class="Symbol">→</a> <a id="430" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a> <a id="432" class="Symbol">→</a> <a id="434" href="elementary-number-theory.natural-numbers.html#1548" class="Datatype">ℕ</a>
<a id="436" href="elementary-number-theory.falling-factorials.html#404" class="Function">falling-factorial-ℕ</a> <a id="456" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a> <a id="463" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a> <a id="470" class="Symbol">=</a> <a id="472" class="Number">1</a>
<a id="474" href="elementary-number-theory.falling-factorials.html#404" class="Function">falling-factorial-ℕ</a> <a id="494" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a> <a id="501" class="Symbol">(</a><a id="502" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="509" href="elementary-number-theory.falling-factorials.html#509" class="Bound">m</a><a id="510" class="Symbol">)</a> <a id="512" class="Symbol">=</a> <a id="514" class="Number">0</a>
<a id="516" href="elementary-number-theory.falling-factorials.html#404" class="Function">falling-factorial-ℕ</a> <a id="536" class="Symbol">(</a><a id="537" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="544" href="elementary-number-theory.falling-factorials.html#544" class="Bound">n</a><a id="545" class="Symbol">)</a> <a id="547" href="elementary-number-theory.natural-numbers.html#1569" class="InductiveConstructor">zero-ℕ</a> <a id="554" class="Symbol">=</a> <a id="556" class="Number">1</a>
<a id="558" href="elementary-number-theory.falling-factorials.html#404" class="Function">falling-factorial-ℕ</a> <a id="578" class="Symbol">(</a><a id="579" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="586" href="elementary-number-theory.falling-factorials.html#586" class="Bound">n</a><a id="587" class="Symbol">)</a> <a id="589" class="Symbol">(</a><a id="590" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="597" href="elementary-number-theory.falling-factorials.html#597" class="Bound">m</a><a id="598" class="Symbol">)</a> <a id="600" class="Symbol">=</a>
  <a id="604" href="elementary-number-theory.multiplication-natural-numbers.html#1286" class="Function">mul-ℕ</a> <a id="610" class="Symbol">(</a><a id="611" href="elementary-number-theory.natural-numbers.html#1582" class="InductiveConstructor">succ-ℕ</a> <a id="618" href="elementary-number-theory.falling-factorials.html#586" class="Bound">n</a><a id="619" class="Symbol">)</a> <a id="621" class="Symbol">(</a><a id="622" href="elementary-number-theory.falling-factorials.html#404" class="Function">falling-factorial-ℕ</a> <a id="642" href="elementary-number-theory.falling-factorials.html#586" class="Bound">n</a> <a id="644" href="elementary-number-theory.falling-factorials.html#597" class="Bound">m</a><a id="645" class="Symbol">)</a>

<a id="648" class="Comment">{-
Fin-falling-factorial-ℕ :
  (n m : ℕ) → Fin (falling-factorial-ℕ n m) ≃ (Fin m ↪ Fin n)
Fin-falling-factorial-ℕ n m = {!!}
-}</a>

<a id="778" class="Comment">{-
Fin-falling-factorial-ℕ : (n m : ℕ) → Fin (falling-factorial-ℕ n m) ≃ (Fin m ↪ Fin n)
Fin-falling-factorial-ℕ zero-ℕ zero-ℕ =
  equiv-is-contr
    ( is-contr-Fin-one-ℕ)
    ( is-contr-equiv
      ( is-emb id)
      ( left-unit-law-Σ-is-contr
        ( universal-property-empty&#39; empty)
        ( id))
      ( dependent-universal-property-empty&#39;
        ( λ x → (y : empty) → is-equiv (ap id))))
Fin-falling-factorial-ℕ zero-ℕ (succ-ℕ m) =
  equiv-is-empty id (λ f → map-emb f (inr star))
Fin-falling-factorial-ℕ (succ-ℕ n) zero-ℕ =
  equiv-is-contr
    ( is-contr-Fin-one-ℕ)
    ( is-contr-equiv
      ( is-emb ex-falso)
      ( left-unit-law-Σ-is-contr
        ( universal-property-empty&#39; (Fin (succ-ℕ n)))
        ( ex-falso))
      ( dependent-universal-property-empty&#39;
        ( λ x → (y : empty) → is-equiv (ap ex-falso))))
Fin-falling-factorial-ℕ (succ-ℕ n) (succ-ℕ m) =
  ( ( ( right-unit-law-Σ-is-contr
        { B = λ f → is-decidable (fib (map-emb f) (inr star))}
        ( λ f →
          is-proof-irrelevant-is-prop
            ( is-prop-is-decidable
              ( is-prop-map-is-emb (is-emb-map-emb f) (inr star)))
            ( is-decidable-Σ-Fin
              ( λ x →
                has-decidable-equality-Fin (map-emb f x) (inr star))))) ∘e
      ( ( inv-equiv
          ( left-distributive-Σ-coprod
            ( Fin (succ-ℕ m) ↪ Fin (succ-ℕ n))
            ( λ f → fib (map-emb f) (inr star))
            ( λ f → ¬ (fib (map-emb f) (inr star))))) ∘e
        {!!})) ∘e
    ( equiv-coprod (Fin-falling-factorial-ℕ n m) (Fin-falling-factorial-ℕ n (succ-ℕ m)))) ∘e
  ( Fin-add-ℕ (falling-factorial-ℕ n m) (falling-factorial-ℕ n (succ-ℕ m)))
-}</a>
</pre>