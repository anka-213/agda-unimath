---
title: Finite presentations of types
---

<pre class="Agda"><a id="55" class="Keyword">module</a> <a id="62" href="univalent-combinatorics.finite-presentations.html" class="Module">univalent-combinatorics.finite-presentations</a> <a id="107" class="Keyword">where</a>
</pre>
## Idea

Finitely presented types are types A equipped with a map f : Fin k → A such that the composite

```md
  Fin k → A → type-trunc-Set A
```

is an equivalence.
