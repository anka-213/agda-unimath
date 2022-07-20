---
title: Wild algebra
---

<pre class="Agda"><a id="38" class="Symbol">{-#</a> <a id="42" class="Keyword">OPTIONS</a> <a id="50" class="Pragma">--without-K</a> <a id="62" class="Pragma">--exact-split</a> <a id="76" class="Symbol">#-}</a>

<a id="81" class="Keyword">module</a> <a id="88" href="structured-types.html" class="Module">structured-types</a> <a id="105" class="Keyword">where</a>
</pre>
<pre class="Agda"><a id="124" class="Keyword">open</a> <a id="129" class="Keyword">import</a> <a id="136" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a> <a id="171" class="Keyword">public</a>
<a id="178" class="Keyword">open</a> <a id="183" class="Keyword">import</a> <a id="190" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a> <a id="234" class="Keyword">public</a>
<a id="241" class="Keyword">open</a> <a id="246" class="Keyword">import</a> <a id="253" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a> <a id="317" class="Keyword">public</a>
<a id="324" class="Keyword">open</a> <a id="329" class="Keyword">import</a> <a id="336" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a> <a id="375" class="Keyword">public</a>
<a id="382" class="Keyword">open</a> <a id="387" class="Keyword">import</a> <a id="394" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a> <a id="440" class="Keyword">public</a>
<a id="447" class="Keyword">open</a> <a id="452" class="Keyword">import</a> <a id="459" href="structured-types.magmas.html" class="Module">structured-types.magmas</a> <a id="483" class="Keyword">public</a>
<a id="490" class="Keyword">open</a> <a id="495" class="Keyword">import</a> <a id="502" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a> <a id="571" class="Keyword">public</a>
<a id="578" class="Keyword">open</a> <a id="583" class="Keyword">import</a> <a id="590" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a> <a id="635" class="Keyword">public</a>
<a id="642" class="Keyword">open</a> <a id="647" class="Keyword">import</a> <a id="654" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a> <a id="688" class="Keyword">public</a>
<a id="695" class="Keyword">open</a> <a id="700" class="Keyword">import</a> <a id="707" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a> <a id="768" class="Keyword">public</a>
<a id="775" class="Keyword">open</a> <a id="780" class="Keyword">import</a> <a id="787" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a> <a id="832" class="Keyword">public</a>
<a id="839" class="Keyword">open</a> <a id="844" class="Keyword">import</a> <a id="851" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a> <a id="889" class="Keyword">public</a>
<a id="896" class="Keyword">open</a> <a id="901" class="Keyword">import</a> <a id="908" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a> <a id="951" class="Keyword">public</a>
<a id="958" class="Keyword">open</a> <a id="963" class="Keyword">import</a> <a id="970" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a> <a id="1006" class="Keyword">public</a>
<a id="1013" class="Keyword">open</a> <a id="1018" class="Keyword">import</a> <a id="1025" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a> <a id="1055" class="Keyword">public</a>
<a id="1062" class="Keyword">open</a> <a id="1067" class="Keyword">import</a> <a id="1074" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a> <a id="1105" class="Keyword">public</a>
<a id="1112" class="Keyword">open</a> <a id="1117" class="Keyword">import</a> <a id="1124" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a> <a id="1183" class="Keyword">public</a>
<a id="1190" class="Keyword">open</a> <a id="1195" class="Keyword">import</a> <a id="1202" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a> <a id="1253" class="Keyword">public</a>
<a id="1260" class="Keyword">open</a> <a id="1265" class="Keyword">import</a> <a id="1272" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a> <a id="1323" class="Keyword">public</a>
<a id="1330" class="Keyword">open</a> <a id="1335" class="Keyword">import</a> <a id="1342" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a> <a id="1397" class="Keyword">public</a>
<a id="1404" class="Keyword">open</a> <a id="1409" class="Keyword">import</a> <a id="1416" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a> <a id="1445" class="Keyword">public</a>
<a id="1452" class="Keyword">open</a> <a id="1457" class="Keyword">import</a> <a id="1464" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a> <a id="1492" class="Keyword">public</a>
<a id="1499" class="Keyword">open</a> <a id="1504" class="Keyword">import</a> <a id="1511" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a> <a id="1541" class="Keyword">public</a>
<a id="1548" class="Keyword">open</a> <a id="1553" class="Keyword">import</a> <a id="1560" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a> <a id="1594" class="Keyword">public</a>
<a id="1601" class="Keyword">open</a> <a id="1606" class="Keyword">import</a> <a id="1613" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a> <a id="1646" class="Keyword">public</a>
</pre>