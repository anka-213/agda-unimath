---
title: Unpointed maps between pointed types
---

<pre class="Agda"><a id="62" class="Keyword">module</a> <a id="69" href="structured-types.unpointed-maps.html" class="Module">structured-types.unpointed-maps</a> <a id="101" class="Keyword">where</a>

<a id="108" class="Keyword">open</a> <a id="113" class="Keyword">import</a> <a id="120" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="152" class="Keyword">open</a> <a id="157" class="Keyword">import</a> <a id="164" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="192" class="Keyword">open</a> <a id="197" class="Keyword">import</a> <a id="204" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a>
</pre>
## Idea

The type of unpointed maps between pointed types is a pointed type, pointed at the constant function.

## Definition

<pre class="Agda"><a id="unpointed-map-Pointed-Type"></a><a id="375" href="structured-types.unpointed-maps.html#375" class="Function">unpointed-map-Pointed-Type</a> <a id="402" class="Symbol">:</a>
  <a id="406" class="Symbol">{</a><a id="407" href="structured-types.unpointed-maps.html#407" class="Bound">l1</a> <a id="410" href="structured-types.unpointed-maps.html#410" class="Bound">l2</a> <a id="413" class="Symbol">:</a> <a id="415" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="420" class="Symbol">}</a> <a id="422" class="Symbol">→</a> <a id="424" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="437" href="structured-types.unpointed-maps.html#407" class="Bound">l1</a> <a id="440" class="Symbol">→</a> <a id="442" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="455" href="structured-types.unpointed-maps.html#410" class="Bound">l2</a> <a id="458" class="Symbol">→</a> <a id="460" href="structured-types.pointed-types.html#383" class="Function">Pointed-Type</a> <a id="473" class="Symbol">(</a><a id="474" href="structured-types.unpointed-maps.html#407" class="Bound">l1</a> <a id="477" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="479" href="structured-types.unpointed-maps.html#410" class="Bound">l2</a><a id="481" class="Symbol">)</a>
<a id="483" href="foundation-core.dependent-pair-types.html#605" class="Field">pr1</a> <a id="487" class="Symbol">(</a><a id="488" href="structured-types.unpointed-maps.html#375" class="Function">unpointed-map-Pointed-Type</a> <a id="515" href="structured-types.unpointed-maps.html#515" class="Bound">A</a> <a id="517" href="structured-types.unpointed-maps.html#517" class="Bound">B</a><a id="518" class="Symbol">)</a> <a id="520" class="Symbol">=</a> <a id="522" href="structured-types.pointed-types.html#518" class="Function">type-Pointed-Type</a> <a id="540" href="structured-types.unpointed-maps.html#515" class="Bound">A</a> <a id="542" class="Symbol">→</a> <a id="544" href="structured-types.pointed-types.html#518" class="Function">type-Pointed-Type</a> <a id="562" href="structured-types.unpointed-maps.html#517" class="Bound">B</a>
<a id="564" href="foundation-core.dependent-pair-types.html#617" class="Field">pr2</a> <a id="568" class="Symbol">(</a><a id="569" href="structured-types.unpointed-maps.html#375" class="Function">unpointed-map-Pointed-Type</a> <a id="596" href="structured-types.unpointed-maps.html#596" class="Bound">A</a> <a id="598" href="structured-types.unpointed-maps.html#598" class="Bound">B</a><a id="599" class="Symbol">)</a> <a id="601" href="structured-types.unpointed-maps.html#601" class="Bound">x</a> <a id="603" class="Symbol">=</a> <a id="605" href="structured-types.pointed-types.html#576" class="Function">pt-Pointed-Type</a> <a id="621" href="structured-types.unpointed-maps.html#598" class="Bound">B</a>
</pre>