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
<a id="426" class="Keyword">open</a> <a id="431" class="Keyword">import</a> <a id="438" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a>
</pre>
## Idea

## Definition

<pre class="Agda"><a id="532" class="Keyword">module</a> <a id="539" href="group-theory.contravariant-pushforward-concrete-group-actions.html#539" class="Module">_</a>
  <a id="543" class="Symbol">{</a><a id="544" href="group-theory.contravariant-pushforward-concrete-group-actions.html#544" class="Bound">l1</a> <a id="547" href="group-theory.contravariant-pushforward-concrete-group-actions.html#547" class="Bound">l2</a> <a id="550" class="Symbol">:</a> <a id="552" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="557" class="Symbol">}</a> <a id="559" class="Symbol">(</a><a id="560" href="group-theory.contravariant-pushforward-concrete-group-actions.html#560" class="Bound">G</a> <a id="562" class="Symbol">:</a> <a id="564" href="group-theory.concrete-groups.html#2028" class="Function">Concrete-Group</a> <a id="579" href="group-theory.contravariant-pushforward-concrete-group-actions.html#544" class="Bound">l1</a><a id="581" class="Symbol">)</a> <a id="583" class="Symbol">(</a><a id="584" href="group-theory.contravariant-pushforward-concrete-group-actions.html#584" class="Bound">H</a> <a id="586" class="Symbol">:</a> <a id="588" href="group-theory.concrete-groups.html#2028" class="Function">Concrete-Group</a> <a id="603" href="group-theory.contravariant-pushforward-concrete-group-actions.html#547" class="Bound">l2</a><a id="605" class="Symbol">)</a>
  <a id="609" class="Symbol">(</a><a id="610" href="group-theory.contravariant-pushforward-concrete-group-actions.html#610" class="Bound">f</a> <a id="612" class="Symbol">:</a> <a id="614" href="group-theory.concrete-groups.html#7034" class="Function">hom-Concrete-Group</a> <a id="633" href="group-theory.contravariant-pushforward-concrete-group-actions.html#560" class="Bound">G</a> <a id="635" href="group-theory.contravariant-pushforward-concrete-group-actions.html#584" class="Bound">H</a><a id="636" class="Symbol">)</a>
  <a id="640" class="Keyword">where</a>

<a id="647" class="Comment">{-
  contravariant-pushforward-action-Concrete-Group :
    {l : Level} → action-Concrete-Group l G → action-Concrete-Group {!!} H
  contravariant-pushforward-action-Concrete-Group X y = {!!}
  
    -- The following should be constructed as a set
    hom-action-Concrete-Group G X
      ( subst-action-Concrete-Group G H f (λ y → Id (shape-Concrete-Group H) y))
      -}</a>
</pre>