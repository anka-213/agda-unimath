---
title: The substitution functor of concrete group actions
---

<pre class="Agda"><a id="76" class="Symbol">{-#</a> <a id="80" class="Keyword">OPTIONS</a> <a id="88" class="Pragma">--without-K</a> <a id="100" class="Pragma">--exact-split</a> <a id="114" class="Symbol">#-}</a>

<a id="119" class="Keyword">module</a> <a id="126" href="group-theory.substitution-functor-concrete-group-actions.html" class="Module">group-theory.substitution-functor-concrete-group-actions</a> <a id="183" class="Keyword">where</a>

<a id="190" class="Keyword">open</a> <a id="195" class="Keyword">import</a> <a id="202" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="230" class="Keyword">open</a> <a id="235" class="Keyword">import</a> <a id="242" href="group-theory.concrete-group-actions.html" class="Module">group-theory.concrete-group-actions</a>
<a id="278" class="Keyword">open</a> <a id="283" class="Keyword">import</a> <a id="290" href="group-theory.concrete-groups.html" class="Module">group-theory.concrete-groups</a>
</pre>
## Definition

### Substitution of concrete group actions

<pre class="Agda"><a id="391" class="Keyword">module</a> <a id="398" href="group-theory.substitution-functor-concrete-group-actions.html#398" class="Module">_</a>
  <a id="402" class="Symbol">{</a><a id="403" href="group-theory.substitution-functor-concrete-group-actions.html#403" class="Bound">l1</a> <a id="406" href="group-theory.substitution-functor-concrete-group-actions.html#406" class="Bound">l2</a> <a id="409" class="Symbol">:</a> <a id="411" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="416" class="Symbol">}</a> <a id="418" class="Symbol">(</a><a id="419" href="group-theory.substitution-functor-concrete-group-actions.html#419" class="Bound">G</a> <a id="421" class="Symbol">:</a> <a id="423" href="group-theory.concrete-groups.html#2024" class="Function">Concrete-Group</a> <a id="438" href="group-theory.substitution-functor-concrete-group-actions.html#403" class="Bound">l1</a><a id="440" class="Symbol">)</a> <a id="442" class="Symbol">(</a><a id="443" href="group-theory.substitution-functor-concrete-group-actions.html#443" class="Bound">H</a> <a id="445" class="Symbol">:</a> <a id="447" href="group-theory.concrete-groups.html#2024" class="Function">Concrete-Group</a> <a id="462" href="group-theory.substitution-functor-concrete-group-actions.html#406" class="Bound">l2</a><a id="464" class="Symbol">)</a>
  <a id="468" class="Symbol">(</a><a id="469" href="group-theory.substitution-functor-concrete-group-actions.html#469" class="Bound">f</a> <a id="471" class="Symbol">:</a> <a id="473" href="group-theory.concrete-groups.html#7018" class="Function">hom-Concrete-Group</a> <a id="492" href="group-theory.substitution-functor-concrete-group-actions.html#419" class="Bound">G</a> <a id="494" href="group-theory.substitution-functor-concrete-group-actions.html#443" class="Bound">H</a><a id="495" class="Symbol">)</a>
  <a id="499" class="Keyword">where</a>

  <a id="508" href="group-theory.substitution-functor-concrete-group-actions.html#508" class="Function">subst-action-Concrete-Group</a> <a id="536" class="Symbol">:</a>
    <a id="542" class="Symbol">{</a><a id="543" href="group-theory.substitution-functor-concrete-group-actions.html#543" class="Bound">l</a> <a id="545" class="Symbol">:</a> <a id="547" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="552" class="Symbol">}</a> <a id="554" class="Symbol">→</a>
    <a id="560" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="582" href="group-theory.substitution-functor-concrete-group-actions.html#543" class="Bound">l</a> <a id="584" href="group-theory.substitution-functor-concrete-group-actions.html#443" class="Bound">H</a> <a id="586" class="Symbol">→</a> <a id="588" href="group-theory.concrete-group-actions.html#807" class="Function">action-Concrete-Group</a> <a id="610" href="group-theory.substitution-functor-concrete-group-actions.html#543" class="Bound">l</a> <a id="612" href="group-theory.substitution-functor-concrete-group-actions.html#419" class="Bound">G</a>
  <a id="616" href="group-theory.substitution-functor-concrete-group-actions.html#508" class="Function">subst-action-Concrete-Group</a> <a id="644" href="group-theory.substitution-functor-concrete-group-actions.html#644" class="Bound">Y</a> <a id="646" href="group-theory.substitution-functor-concrete-group-actions.html#646" class="Bound">x</a> <a id="648" class="Symbol">=</a>
    <a id="654" href="group-theory.substitution-functor-concrete-group-actions.html#644" class="Bound">Y</a> <a id="656" class="Symbol">(</a><a id="657" href="group-theory.concrete-groups.html#7368" class="Function">classifying-map-hom-Concrete-Group</a> <a id="692" href="group-theory.substitution-functor-concrete-group-actions.html#419" class="Bound">G</a> <a id="694" href="group-theory.substitution-functor-concrete-group-actions.html#443" class="Bound">H</a> <a id="696" href="group-theory.substitution-functor-concrete-group-actions.html#469" class="Bound">f</a> <a id="698" href="group-theory.substitution-functor-concrete-group-actions.html#646" class="Bound">x</a><a id="699" class="Symbol">)</a>
</pre>