---
title: Wild algebra
---

<pre class="Agda"><a id="38" class="Symbol">{-#</a> <a id="42" class="Keyword">OPTIONS</a> <a id="50" class="Pragma">--without-K</a> <a id="62" class="Pragma">--exact-split</a> <a id="76" class="Symbol">#-}</a>

<a id="81" class="Keyword">module</a> <a id="88" href="structured-types.html" class="Module">structured-types</a> <a id="105" class="Keyword">where</a>
</pre>
<pre class="Agda"><a id="124" class="Keyword">open</a> <a id="129" class="Keyword">import</a> <a id="136" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a> <a id="200" class="Keyword">public</a>
<a id="207" class="Keyword">open</a> <a id="212" class="Keyword">import</a> <a id="219" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a> <a id="265" class="Keyword">public</a>
<a id="272" class="Keyword">open</a> <a id="277" class="Keyword">import</a> <a id="284" href="structured-types.magmas.html" class="Module">structured-types.magmas</a> <a id="308" class="Keyword">public</a>
<a id="315" class="Keyword">open</a> <a id="320" class="Keyword">import</a> <a id="327" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a> <a id="396" class="Keyword">public</a>
<a id="403" class="Keyword">open</a> <a id="408" class="Keyword">import</a> <a id="415" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a> <a id="449" class="Keyword">public</a>
<a id="456" class="Keyword">open</a> <a id="461" class="Keyword">import</a> <a id="468" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a> <a id="529" class="Keyword">public</a>
<a id="536" class="Keyword">open</a> <a id="541" class="Keyword">import</a> <a id="548" href="structured-types.morphisms-wild-unital-magmas.html" class="Module">structured-types.morphisms-wild-unital-magmas</a> <a id="594" class="Keyword">public</a>
<a id="601" class="Keyword">open</a> <a id="606" class="Keyword">import</a> <a id="613" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a> <a id="658" class="Keyword">public</a>
<a id="665" class="Keyword">open</a> <a id="670" class="Keyword">import</a> <a id="677" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a> <a id="715" class="Keyword">public</a>
<a id="722" class="Keyword">open</a> <a id="727" class="Keyword">import</a> <a id="734" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a> <a id="777" class="Keyword">public</a>
<a id="784" class="Keyword">open</a> <a id="789" class="Keyword">import</a> <a id="796" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a> <a id="832" class="Keyword">public</a>
<a id="839" class="Keyword">open</a> <a id="844" class="Keyword">import</a> <a id="851" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a> <a id="881" class="Keyword">public</a>
<a id="888" class="Keyword">open</a> <a id="893" class="Keyword">import</a> <a id="900" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a> <a id="931" class="Keyword">public</a>
<a id="938" class="Keyword">open</a> <a id="943" class="Keyword">import</a> <a id="950" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a> <a id="1001" class="Keyword">public</a>
<a id="1008" class="Keyword">open</a> <a id="1013" class="Keyword">import</a> <a id="1020" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a> <a id="1075" class="Keyword">public</a>
<a id="1082" class="Keyword">open</a> <a id="1087" class="Keyword">import</a> <a id="1094" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a> <a id="1123" class="Keyword">public</a>
<a id="1130" class="Keyword">open</a> <a id="1135" class="Keyword">import</a> <a id="1142" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a> <a id="1170" class="Keyword">public</a>
<a id="1177" class="Keyword">open</a> <a id="1182" class="Keyword">import</a> <a id="1189" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a> <a id="1219" class="Keyword">public</a>
<a id="1226" class="Keyword">open</a> <a id="1231" class="Keyword">import</a> <a id="1238" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a> <a id="1272" class="Keyword">public</a>
<a id="1279" class="Keyword">open</a> <a id="1284" class="Keyword">import</a> <a id="1291" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a> <a id="1324" class="Keyword">public</a>
<a id="1331" class="Keyword">open</a> <a id="1336" class="Keyword">import</a> <a id="1343" href="structured-types.wild-unital-magmas.html" class="Module">structured-types.wild-unital-magmas</a> <a id="1379" class="Keyword">public</a>
</pre>