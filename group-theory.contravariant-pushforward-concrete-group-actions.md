---
title: Contravariant pushforwards of concrete group actions
---

<pre class="Agda"><a id="78" class="Symbol">{-#</a> <a id="82" class="Keyword">OPTIONS</a> <a id="90" class="Pragma">--without-K</a> <a id="102" class="Pragma">--exact-split</a> <a id="116" class="Symbol">#-}</a>

<a id="121" class="Keyword">module</a> <a id="128" href="group-theory.contravariant-pushforward-concrete-group-actions.html" class="Module">group-theory.contravariant-pushforward-concrete-group-actions</a> <a id="190" class="Keyword">where</a>

<a id="197" class="Keyword">open</a> <a id="202" class="Keyword">import</a> <a id="209" href="foundation.identity-types.html" class="Module">foundation.identity-types</a>
<a id="235" class="Keyword">open</a> <a id="240" class="Keyword">import</a> <a id="247" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="275" class="Keyword">open</a> <a id="280" class="Keyword">import</a> <a id="287" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="323" class="Keyword">open</a> <a id="328" class="Keyword">import</a> <a id="335" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
<a id="364" class="Keyword">open</a> <a id="369" class="Keyword">import</a> <a id="376" href="group-theory.homomorphisms-concrete-group-actions.html" class="Module">group-theory.homomorphisms-concrete-group-actions</a>
<a id="426" class="Keyword">open</a> <a id="431" class="Keyword">import</a> <a id="438" href="group-theory.substitutions-concrete-group-actions.html" class="Module">group-theory.substitutions-concrete-group-actions</a>
</pre>
## Idea

## Definition

<pre class="Agda"><a id="525" class="Keyword">module</a> <a id="532" href="group-theory.contravariant-pushforward-concrete-group-actions.html#532" class="Module">_</a>
  <a id="536" class="Symbol">{</a><a id="537" href="group-theory.contravariant-pushforward-concrete-group-actions.html#537" class="Bound">l1</a> <a id="540" href="group-theory.contravariant-pushforward-concrete-group-actions.html#540" class="Bound">l2</a> <a id="543" class="Symbol">:</a> <a id="545" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="550" class="Symbol">}</a> <a id="552" class="Symbol">(</a><a id="553" href="group-theory.contravariant-pushforward-concrete-group-actions.html#553" class="Bound">G</a> <a id="555" class="Symbol">:</a> <a id="557" href="group-theory.concrete-groups.html#1988" class="Function">Concrete-Group</a> <a id="572" href="group-theory.contravariant-pushforward-concrete-group-actions.html#537" class="Bound">l1</a><a id="574" class="Symbol">)</a> <a id="576" class="Symbol">(</a><a id="577" href="group-theory.contravariant-pushforward-concrete-group-actions.html#577" class="Bound">H</a> <a id="579" class="Symbol">:</a> <a id="581" href="group-theory.concrete-groups.html#1988" class="Function">Concrete-Group</a> <a id="596" href="group-theory.contravariant-pushforward-concrete-group-actions.html#540" class="Bound">l2</a><a id="598" class="Symbol">)</a>
  <a id="602" class="Symbol">(</a><a id="603" href="group-theory.contravariant-pushforward-concrete-group-actions.html#603" class="Bound">f</a> <a id="605" class="Symbol">:</a> <a id="607" href="group-theory.concrete-groups.html#6994" class="Function">hom-Concrete-Group</a> <a id="626" href="group-theory.contravariant-pushforward-concrete-group-actions.html#553" class="Bound">G</a> <a id="628" href="group-theory.contravariant-pushforward-concrete-group-actions.html#577" class="Bound">H</a><a id="629" class="Symbol">)</a>
  <a id="633" class="Keyword">where</a>

<a id="640" class="Comment">{-
  contravariant-pushforward-action-Concrete-Group :
    {l : Level} → action-Concrete-Group l G → action-Concrete-Group {!!} H
  contravariant-pushforward-action-Concrete-Group X y = {!!}
  
    -- The following should be constructed as a set
    hom-action-Concrete-Group G X
      ( subst-action-Concrete-Group G H f (λ y → Id (shape-Concrete-Group H) y))
      -}</a>
</pre>