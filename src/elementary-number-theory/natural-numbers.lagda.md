# The type of natural numbers

```agda
{-# OPTIONS --without-K --exact-split #-}

module elementary-number-theory.natural-numbers where

open import foundation-core.empty-types using (ex-falso)

open import foundation.booleans using (bool; Eq-bool; true; false)
open import foundation.contractible-types using (eq-is-contr)
open import foundation.dependent-pair-types using (Σ; pair; pr1; pr2)
open import foundation.equivalences using
  ( is-equiv; is-equiv-has-inverse; _≃_)
open import foundation.function-extensionality using (eq-htpy)
open import foundation.functions using (id; _∘_)
open import foundation.homotopies using (_~_)
open import foundation.identity-types using (Id; refl; ap)
open import foundation.injective-maps using (is-injective)
open import foundation.logical-equivalences using (_↔_)
open import foundation.negation using (¬)
open import foundation.unit-type using (star; unit)
open import foundation.universal-property-empty-type using
  ( universal-property-empty')
open import foundation.universe-levels using (Level; lzero; UU)
open import foundation.w-types using (𝕎; constant-𝕎; tree-𝕎)
```

## Idea

The type of natural numbers is inductively generated by the zero element and the successor function. The induction principle for the natural numbers works to construct sections of type families over the natural numbers.

## Definitions

### The inductive definition of the type of natural numbers

```agda
data ℕ : UU lzero where
  zero-ℕ : ℕ
  succ-ℕ : ℕ → ℕ

{-# BUILTIN NATURAL ℕ #-}
```

### Useful predicates on the natural numbers

These predicates can of course be asserted directly without much trouble. However, using the defined predicates ensures uniformity, and helps naming definitions.

```agda
is-zero-ℕ : ℕ → UU lzero
is-zero-ℕ n = Id n zero-ℕ

is-zero-ℕ' : ℕ → UU lzero
is-zero-ℕ' n = Id zero-ℕ n

is-successor-ℕ : ℕ → UU lzero
is-successor-ℕ n = Σ ℕ (λ y → Id n (succ-ℕ y))

is-nonzero-ℕ : ℕ → UU lzero
is-nonzero-ℕ n = ¬ (is-zero-ℕ n)

is-one-ℕ : ℕ → UU lzero
is-one-ℕ n = Id n 1

is-one-ℕ' : ℕ → UU lzero
is-one-ℕ' n = Id 1 n

is-not-one-ℕ : ℕ → UU lzero
is-not-one-ℕ n = ¬ (is-one-ℕ n)

is-not-one-ℕ' : ℕ → UU lzero
is-not-one-ℕ' n = ¬ (is-one-ℕ' n)
```

### The type of natural numbers defined as a W-type

```agda
Nat-𝕎 : UU lzero
Nat-𝕎 = 𝕎 bool (Eq-bool true)

zero-Nat-𝕎 : Nat-𝕎
zero-Nat-𝕎 = constant-𝕎 false id

succ-Nat-𝕎 : Nat-𝕎 → Nat-𝕎
succ-Nat-𝕎 x = tree-𝕎 true (λ y → x)
```

## Properties

### The induction principle of ℕ

```agda
ind-ℕ :
  {i : Level} {P : ℕ → UU i} →
  P 0 → ((n : ℕ) → P n → P(succ-ℕ n)) → ((n : ℕ) → P n)
ind-ℕ p0 pS 0 = p0
ind-ℕ p0 pS (succ-ℕ n) = pS n (ind-ℕ p0 pS n)
```

### Peano's 7th axiom

```agda
is-injective-succ-ℕ : is-injective succ-ℕ
is-injective-succ-ℕ refl = refl

private
  Peano-7 :
    (x y : ℕ) → (Id x y) ↔ (Id (succ-ℕ x) (succ-ℕ y))
  pr1 (Peano-7 x y) refl = refl
  pr2 (Peano-7 x y) = is-injective-succ-ℕ
```

### Peano's 8th axiom

```agda
private   
  Peano-8 : (x : ℕ) → is-nonzero-ℕ (succ-ℕ x)
  Peano-8 x ()

is-nonzero-succ-ℕ : (x : ℕ) → is-nonzero-ℕ (succ-ℕ x)
is-nonzero-succ-ℕ x ()

is-nonzero-is-successor-ℕ : {x : ℕ} → is-successor-ℕ x → is-nonzero-ℕ x
is-nonzero-is-successor-ℕ (pair x refl) ()

is-successor-is-nonzero-ℕ : {x : ℕ} → is-nonzero-ℕ x → is-successor-ℕ x
is-successor-is-nonzero-ℕ {zero-ℕ} H = ex-falso (H refl)
pr1 (is-successor-is-nonzero-ℕ {succ-ℕ x} H) = x
pr2 (is-successor-is-nonzero-ℕ {succ-ℕ x} H) = refl

has-no-fixed-points-succ-ℕ : (x : ℕ) → ¬ (Id (succ-ℕ x) x)
has-no-fixed-points-succ-ℕ x ()
```

### Basic inequalities

```agda
is-nonzero-one-ℕ : is-nonzero-ℕ 1
is-nonzero-one-ℕ ()

is-not-one-zero-ℕ : is-not-one-ℕ zero-ℕ
is-not-one-zero-ℕ ()

is-not-one-two-ℕ : is-not-one-ℕ 2
is-not-one-two-ℕ ()
```

### The type of natural numbers is equivalent to the W-type Nat-𝕎

```agda
Nat-𝕎-ℕ : ℕ → Nat-𝕎
Nat-𝕎-ℕ zero-ℕ = zero-Nat-𝕎
Nat-𝕎-ℕ (succ-ℕ x) = succ-Nat-𝕎 (Nat-𝕎-ℕ x)

ℕ-Nat-𝕎 : Nat-𝕎 → ℕ
ℕ-Nat-𝕎 (tree-𝕎 true α) = succ-ℕ (ℕ-Nat-𝕎 (α star))
ℕ-Nat-𝕎 (tree-𝕎 false α) = zero-ℕ

issec-ℕ-Nat-𝕎 : (Nat-𝕎-ℕ ∘ ℕ-Nat-𝕎) ~ id
issec-ℕ-Nat-𝕎 (tree-𝕎 true α) =
  ap ( tree-𝕎 true)
     ( eq-htpy H)
  where
  H : (z : unit) → Id (Nat-𝕎-ℕ (ℕ-Nat-𝕎 (α star))) (α z)
  H star = issec-ℕ-Nat-𝕎 (α star)
issec-ℕ-Nat-𝕎 (tree-𝕎 false α) =
  ap (tree-𝕎 false) (eq-is-contr (universal-property-empty' Nat-𝕎))

isretr-ℕ-Nat-𝕎 : (ℕ-Nat-𝕎 ∘ Nat-𝕎-ℕ) ~ id
isretr-ℕ-Nat-𝕎 zero-ℕ = refl
isretr-ℕ-Nat-𝕎 (succ-ℕ x) = ap succ-ℕ (isretr-ℕ-Nat-𝕎 x)

is-equiv-Nat-𝕎-ℕ : is-equiv Nat-𝕎-ℕ
is-equiv-Nat-𝕎-ℕ =
  is-equiv-has-inverse
    ℕ-Nat-𝕎
    issec-ℕ-Nat-𝕎
    isretr-ℕ-Nat-𝕎

equiv-Nat-𝕎-ℕ : ℕ ≃ Nat-𝕎
equiv-Nat-𝕎-ℕ = pair Nat-𝕎-ℕ is-equiv-Nat-𝕎-ℕ

is-equiv-ℕ-Nat-𝕎 : is-equiv ℕ-Nat-𝕎
is-equiv-ℕ-Nat-𝕎 =
  is-equiv-has-inverse
    Nat-𝕎-ℕ
    isretr-ℕ-Nat-𝕎
    issec-ℕ-Nat-𝕎

equiv-ℕ-Nat-𝕎 : Nat-𝕎 ≃ ℕ
equiv-ℕ-Nat-𝕎 = pair ℕ-Nat-𝕎 is-equiv-ℕ-Nat-𝕎
```