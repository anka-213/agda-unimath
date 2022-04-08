---
title: Ring theory
---

<pre class="Agda"><a id="37" class="Symbol">{-#</a> <a id="41" class="Keyword">OPTIONS</a> <a id="49" class="Pragma">--without-K</a> <a id="61" class="Pragma">--exact-split</a> <a id="75" class="Symbol">#-}</a>

<a id="80" class="Keyword">module</a> <a id="87" href="ring-theory.html" class="Module">ring-theory</a> <a id="99" class="Keyword">where</a>

<a id="106" class="Keyword">open</a> <a id="111" class="Keyword">import</a> <a id="118" href="ring-theory.commutative-rings.html" class="Module">ring-theory.commutative-rings</a> <a id="148" class="Keyword">public</a>
<a id="155" class="Keyword">open</a> <a id="160" class="Keyword">import</a> <a id="167" href="ring-theory.discrete-fields.html" class="Module">ring-theory.discrete-fields</a> <a id="195" class="Keyword">public</a>
<a id="202" class="Keyword">open</a> <a id="207" class="Keyword">import</a> <a id="214" href="ring-theory.division-rings.html" class="Module">ring-theory.division-rings</a> <a id="241" class="Keyword">public</a>
<a id="248" class="Keyword">open</a> <a id="253" class="Keyword">import</a> <a id="260" href="ring-theory.eisenstein-integers.html" class="Module">ring-theory.eisenstein-integers</a> <a id="292" class="Keyword">public</a>
<a id="299" class="Keyword">open</a> <a id="304" class="Keyword">import</a> <a id="311" href="ring-theory.gaussian-integers.html" class="Module">ring-theory.gaussian-integers</a> <a id="341" class="Keyword">public</a>
<a id="348" class="Keyword">open</a> <a id="353" class="Keyword">import</a> <a id="360" href="ring-theory.homomorphisms-commutative-rings.html" class="Module">ring-theory.homomorphisms-commutative-rings</a> <a id="404" class="Keyword">public</a>
<a id="411" class="Keyword">open</a> <a id="416" class="Keyword">import</a> <a id="423" href="ring-theory.homomorphisms-rings.html" class="Module">ring-theory.homomorphisms-rings</a> <a id="455" class="Keyword">public</a>
<a id="462" class="Keyword">open</a> <a id="467" class="Keyword">import</a> <a id="474" href="ring-theory.ideals-generated-by-subsets-rings.html" class="Module">ring-theory.ideals-generated-by-subsets-rings</a> <a id="520" class="Keyword">public</a>
<a id="527" class="Keyword">open</a> <a id="532" class="Keyword">import</a> <a id="539" href="ring-theory.ideals-rings.html" class="Module">ring-theory.ideals-rings</a> <a id="564" class="Keyword">public</a>
<a id="571" class="Keyword">open</a> <a id="576" class="Keyword">import</a> <a id="583" href="ring-theory.invertible-elements-rings.html" class="Module">ring-theory.invertible-elements-rings</a> <a id="621" class="Keyword">public</a>
<a id="628" class="Keyword">open</a> <a id="633" class="Keyword">import</a> <a id="640" href="ring-theory.isomorphisms-commutative-rings.html" class="Module">ring-theory.isomorphisms-commutative-rings</a> <a id="683" class="Keyword">public</a>
<a id="690" class="Keyword">open</a> <a id="695" class="Keyword">import</a> <a id="702" href="ring-theory.isomorphisms-rings.html" class="Module">ring-theory.isomorphisms-rings</a> <a id="733" class="Keyword">public</a>
<a id="740" class="Keyword">open</a> <a id="745" class="Keyword">import</a> <a id="752" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a> <a id="784" class="Keyword">public</a>
<a id="791" class="Keyword">open</a> <a id="796" class="Keyword">import</a> <a id="803" href="ring-theory.nontrivial-rings.html" class="Module">ring-theory.nontrivial-rings</a> <a id="832" class="Keyword">public</a>
<a id="839" class="Keyword">open</a> <a id="844" class="Keyword">import</a> <a id="851" href="ring-theory.rings.html" class="Module">ring-theory.rings</a> <a id="869" class="Keyword">public</a>
</pre>