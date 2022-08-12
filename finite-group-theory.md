---
title: Finite group theory
---

<pre class="Agda"><a id="45" class="Symbol">{-#</a> <a id="49" class="Keyword">OPTIONS</a> <a id="57" class="Pragma">--without-K</a> <a id="69" class="Pragma">--exact-split</a> <a id="83" class="Symbol">#-}</a>

<a id="88" class="Keyword">module</a> <a id="95" href="finite-group-theory.html" class="Module">finite-group-theory</a> <a id="115" class="Keyword">where</a>
</pre>
<pre class="Agda"><a id="134" class="Keyword">open</a> <a id="139" class="Keyword">import</a> <a id="146" href="finite-group-theory.abstract-quaternion-group.html" class="Module">finite-group-theory.abstract-quaternion-group</a> <a id="192" class="Keyword">public</a>
<a id="199" class="Keyword">open</a> <a id="204" class="Keyword">import</a> <a id="211" href="finite-group-theory.alternating-groups.html" class="Module">finite-group-theory.alternating-groups</a> <a id="250" class="Keyword">public</a>
<a id="257" class="Keyword">open</a> <a id="262" class="Keyword">import</a> <a id="269" href="finite-group-theory.cartier-delooping-sign-homomorphism.html" class="Module">finite-group-theory.cartier-delooping-sign-homomorphism</a> <a id="325" class="Keyword">public</a>
<a id="332" class="Keyword">open</a> <a id="337" class="Keyword">import</a> <a id="344" href="finite-group-theory.concrete-quaternion-group.html" class="Module">finite-group-theory.concrete-quaternion-group</a> <a id="390" class="Keyword">public</a>
<a id="397" class="Keyword">open</a> <a id="402" class="Keyword">import</a> <a id="409" href="finite-group-theory.finite-groups.html" class="Module">finite-group-theory.finite-groups</a> <a id="443" class="Keyword">public</a>
<a id="450" class="Keyword">open</a> <a id="455" class="Keyword">import</a> <a id="462" href="finite-group-theory.finite-monoids.html" class="Module">finite-group-theory.finite-monoids</a> <a id="497" class="Keyword">public</a>
<a id="504" class="Keyword">open</a> <a id="509" class="Keyword">import</a> <a id="516" href="finite-group-theory.finite-semigroups.html" class="Module">finite-group-theory.finite-semigroups</a> <a id="554" class="Keyword">public</a>
<a id="561" class="Keyword">open</a> <a id="566" class="Keyword">import</a> <a id="573" href="finite-group-theory.finite-type-groups.html" class="Module">finite-group-theory.finite-type-groups</a> <a id="612" class="Keyword">public</a>
<a id="619" class="Keyword">open</a> <a id="624" class="Keyword">import</a> <a id="631" href="finite-group-theory.groups-of-order-2.html" class="Module">finite-group-theory.groups-of-order-2</a> <a id="669" class="Keyword">public</a>
<a id="676" class="Keyword">open</a> <a id="681" class="Keyword">import</a> <a id="688" href="finite-group-theory.orbits-permutations.html" class="Module">finite-group-theory.orbits-permutations</a> <a id="728" class="Keyword">public</a>
<a id="735" class="Keyword">open</a> <a id="740" class="Keyword">import</a> <a id="747" href="finite-group-theory.permutations.html" class="Module">finite-group-theory.permutations</a> <a id="780" class="Keyword">public</a>
<a id="787" class="Keyword">open</a> <a id="792" class="Keyword">import</a> <a id="799" href="finite-group-theory.sign-homomorphism.html" class="Module">finite-group-theory.sign-homomorphism</a> <a id="837" class="Keyword">public</a>
<a id="844" class="Keyword">open</a> <a id="849" class="Keyword">import</a> <a id="856" href="finite-group-theory.simpson-delooping-sign-homomorphism.html" class="Module">finite-group-theory.simpson-delooping-sign-homomorphism</a> <a id="912" class="Keyword">public</a>
<a id="919" class="Keyword">open</a> <a id="924" class="Keyword">import</a> <a id="931" href="finite-group-theory.tetrahedra-in-3-space.html" class="Module">finite-group-theory.tetrahedra-in-3-space</a> <a id="973" class="Keyword">public</a>
<a id="980" class="Keyword">open</a> <a id="985" class="Keyword">import</a> <a id="992" href="finite-group-theory.transpositions.html" class="Module">finite-group-theory.transpositions</a> <a id="1027" class="Keyword">public</a>
</pre>