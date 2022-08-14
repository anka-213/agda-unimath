---
title: Structured types
---

<pre class="Agda"><a id="42" class="Symbol">{-#</a> <a id="46" class="Keyword">OPTIONS</a> <a id="54" class="Pragma">--without-K</a> <a id="66" class="Pragma">--exact-split</a> <a id="80" class="Symbol">#-}</a>

<a id="85" class="Keyword">module</a> <a id="92" href="structured-types.html" class="Module">structured-types</a> <a id="109" class="Keyword">where</a>
</pre>
<pre class="Agda"><a id="128" class="Keyword">open</a> <a id="133" class="Keyword">import</a> <a id="140" href="structured-types.coherent-h-spaces.html" class="Module">structured-types.coherent-h-spaces</a> <a id="175" class="Keyword">public</a>
<a id="182" class="Keyword">open</a> <a id="187" class="Keyword">import</a> <a id="194" href="structured-types.contractible-pointed-types.html" class="Module">structured-types.contractible-pointed-types</a> <a id="238" class="Keyword">public</a>
<a id="245" class="Keyword">open</a> <a id="250" class="Keyword">import</a> <a id="257" href="structured-types.equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.equivalences-types-equipped-with-endomorphisms</a> <a id="321" class="Keyword">public</a>
<a id="328" class="Keyword">open</a> <a id="333" class="Keyword">import</a> <a id="340" href="structured-types.faithful-pointed-maps.html" class="Module">structured-types.faithful-pointed-maps</a> <a id="379" class="Keyword">public</a>
<a id="386" class="Keyword">open</a> <a id="391" class="Keyword">import</a> <a id="398" href="structured-types.finite-multiplication-magmas.html" class="Module">structured-types.finite-multiplication-magmas</a> <a id="444" class="Keyword">public</a>
<a id="451" class="Keyword">open</a> <a id="456" class="Keyword">import</a> <a id="463" href="structured-types.magmas.html" class="Module">structured-types.magmas</a> <a id="487" class="Keyword">public</a>
<a id="494" class="Keyword">open</a> <a id="499" class="Keyword">import</a> <a id="506" href="structured-types.mere-equivalences-types-equipped-with-endomorphisms.html" class="Module">structured-types.mere-equivalences-types-equipped-with-endomorphisms</a> <a id="575" class="Keyword">public</a>
<a id="582" class="Keyword">open</a> <a id="587" class="Keyword">import</a> <a id="594" href="structured-types.morphisms-coherent-h-spaces.html" class="Module">structured-types.morphisms-coherent-h-spaces</a> <a id="639" class="Keyword">public</a>
<a id="646" class="Keyword">open</a> <a id="651" class="Keyword">import</a> <a id="658" href="structured-types.morphisms-magmas.html" class="Module">structured-types.morphisms-magmas</a> <a id="692" class="Keyword">public</a>
<a id="699" class="Keyword">open</a> <a id="704" class="Keyword">import</a> <a id="711" href="structured-types.morphisms-types-equipped-with-endomorphisms.html" class="Module">structured-types.morphisms-types-equipped-with-endomorphisms</a> <a id="772" class="Keyword">public</a>
<a id="779" class="Keyword">open</a> <a id="784" class="Keyword">import</a> <a id="791" href="structured-types.pointed-dependent-functions.html" class="Module">structured-types.pointed-dependent-functions</a> <a id="836" class="Keyword">public</a>
<a id="843" class="Keyword">open</a> <a id="848" class="Keyword">import</a> <a id="855" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a> <a id="893" class="Keyword">public</a>
<a id="900" class="Keyword">open</a> <a id="905" class="Keyword">import</a> <a id="912" href="structured-types.pointed-families-of-types.html" class="Module">structured-types.pointed-families-of-types</a> <a id="955" class="Keyword">public</a>
<a id="962" class="Keyword">open</a> <a id="967" class="Keyword">import</a> <a id="974" href="structured-types.pointed-homotopies.html" class="Module">structured-types.pointed-homotopies</a> <a id="1010" class="Keyword">public</a>
<a id="1017" class="Keyword">open</a> <a id="1022" class="Keyword">import</a> <a id="1029" href="structured-types.pointed-maps.html" class="Module">structured-types.pointed-maps</a> <a id="1059" class="Keyword">public</a>
<a id="1066" class="Keyword">open</a> <a id="1071" class="Keyword">import</a> <a id="1078" href="structured-types.pointed-types.html" class="Module">structured-types.pointed-types</a> <a id="1109" class="Keyword">public</a>
<a id="1116" class="Keyword">open</a> <a id="1121" class="Keyword">import</a> <a id="1128" href="structured-types.pointed-types-equipped-with-automorphisms.html" class="Module">structured-types.pointed-types-equipped-with-automorphisms</a> <a id="1187" class="Keyword">public</a>
<a id="1194" class="Keyword">open</a> <a id="1199" class="Keyword">import</a> <a id="1206" href="structured-types.types-equipped-with-automorphisms.html" class="Module">structured-types.types-equipped-with-automorphisms</a> <a id="1257" class="Keyword">public</a>
<a id="1264" class="Keyword">open</a> <a id="1269" class="Keyword">import</a> <a id="1276" href="structured-types.types-equipped-with-endomorphisms.html" class="Module">structured-types.types-equipped-with-endomorphisms</a> <a id="1327" class="Keyword">public</a>
<a id="1334" class="Keyword">open</a> <a id="1339" class="Keyword">import</a> <a id="1346" href="structured-types.universal-property-lists-wild-monoids.html" class="Module">structured-types.universal-property-lists-wild-monoids</a> <a id="1401" class="Keyword">public</a>
<a id="1408" class="Keyword">open</a> <a id="1413" class="Keyword">import</a> <a id="1420" href="structured-types.wild-groups.html" class="Module">structured-types.wild-groups</a> <a id="1449" class="Keyword">public</a>
<a id="1456" class="Keyword">open</a> <a id="1461" class="Keyword">import</a> <a id="1468" href="structured-types.wild-loops.html" class="Module">structured-types.wild-loops</a> <a id="1496" class="Keyword">public</a>
<a id="1503" class="Keyword">open</a> <a id="1508" class="Keyword">import</a> <a id="1515" href="structured-types.wild-monoids.html" class="Module">structured-types.wild-monoids</a> <a id="1545" class="Keyword">public</a>
<a id="1552" class="Keyword">open</a> <a id="1557" class="Keyword">import</a> <a id="1564" href="structured-types.wild-quasigroups.html" class="Module">structured-types.wild-quasigroups</a> <a id="1598" class="Keyword">public</a>
<a id="1605" class="Keyword">open</a> <a id="1610" class="Keyword">import</a> <a id="1617" href="structured-types.wild-semigroups.html" class="Module">structured-types.wild-semigroups</a> <a id="1650" class="Keyword">public</a>
</pre>