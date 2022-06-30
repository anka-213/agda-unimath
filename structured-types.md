---
title: Wild algebra
---

<pre class="Agda"><a id="38" class="Symbol">{-#</a> <a id="42" class="Keyword">OPTIONS</a> <a id="50" class="Pragma">--without-K</a> <a id="62" class="Pragma">--exact-split</a> <a id="76" class="Symbol">#-}</a>

<a id="81" class="Keyword">module</a> <a id="88" href="structured-types.html" class="Module">structured-types</a> <a id="105" class="Keyword">where</a>
</pre>
<pre class="Agda"><a id="124" class="Keyword">open</a> <a id="129" class="Keyword">import</a> <a id="136" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a> <a id="171" class="Keyword">public</a>
<a id="178" class="Keyword">open</a> <a id="183" class="Keyword">import</a> <a id="190" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a> <a id="234" class="Keyword">public</a>
<a id="241" class="Keyword">open</a> <a id="246" class="Keyword">import</a> <a id="253" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a> <a id="317" class="Keyword">public</a>
<a id="324" class="Keyword">open</a> <a id="329" class="Keyword">import</a> <a id="336" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a> <a id="382" class="Keyword">public</a>
<a id="389" class="Keyword">open</a> <a id="394" class="Keyword">import</a> <a id="401" href="structured-types.magmas.html" class="Module">structured-types.magmas</a> <a id="425" class="Keyword">public</a>
<a id="432" class="Keyword">open</a> <a id="437" class="Keyword">import</a> <a id="444" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a> <a id="513" class="Keyword">public</a>
<a id="520" class="Keyword">open</a> <a id="525" class="Keyword">import</a> <a id="532" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a> <a id="577" class="Keyword">public</a>
<a id="584" class="Keyword">open</a> <a id="589" class="Keyword">import</a> <a id="596" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a> <a id="630" class="Keyword">public</a>
<a id="637" class="Keyword">open</a> <a id="642" class="Keyword">import</a> <a id="649" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a> <a id="710" class="Keyword">public</a>
<a id="717" class="Keyword">open</a> <a id="722" class="Keyword">import</a> <a id="729" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a> <a id="774" class="Keyword">public</a>
<a id="781" class="Keyword">open</a> <a id="786" class="Keyword">import</a> <a id="793" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a> <a id="831" class="Keyword">public</a>
<a id="838" class="Keyword">open</a> <a id="843" class="Keyword">import</a> <a id="850" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a> <a id="893" class="Keyword">public</a>
<a id="900" class="Keyword">open</a> <a id="905" class="Keyword">import</a> <a id="912" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a> <a id="948" class="Keyword">public</a>
<a id="955" class="Keyword">open</a> <a id="960" class="Keyword">import</a> <a id="967" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a> <a id="997" class="Keyword">public</a>
<a id="1004" class="Keyword">open</a> <a id="1009" class="Keyword">import</a> <a id="1016" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a> <a id="1047" class="Keyword">public</a>
<a id="1054" class="Keyword">open</a> <a id="1059" class="Keyword">import</a> <a id="1066" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a> <a id="1125" class="Keyword">public</a>
<a id="1132" class="Keyword">open</a> <a id="1137" class="Keyword">import</a> <a id="1144" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a> <a id="1195" class="Keyword">public</a>
<a id="1202" class="Keyword">open</a> <a id="1207" class="Keyword">import</a> <a id="1214" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a> <a id="1265" class="Keyword">public</a>
<a id="1272" class="Keyword">open</a> <a id="1277" class="Keyword">import</a> <a id="1284" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a> <a id="1339" class="Keyword">public</a>
<a id="1346" class="Keyword">open</a> <a id="1351" class="Keyword">import</a> <a id="1358" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a> <a id="1387" class="Keyword">public</a>
<a id="1394" class="Keyword">open</a> <a id="1399" class="Keyword">import</a> <a id="1406" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a> <a id="1434" class="Keyword">public</a>
<a id="1441" class="Keyword">open</a> <a id="1446" class="Keyword">import</a> <a id="1453" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a> <a id="1483" class="Keyword">public</a>
<a id="1490" class="Keyword">open</a> <a id="1495" class="Keyword">import</a> <a id="1502" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a> <a id="1536" class="Keyword">public</a>
<a id="1543" class="Keyword">open</a> <a id="1548" class="Keyword">import</a> <a id="1555" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a> <a id="1588" class="Keyword">public</a>
</pre>