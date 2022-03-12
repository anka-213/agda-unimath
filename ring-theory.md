---
title: Formalisation of the Symmetry Book
---

<pre class="Agda"><a id="60" class="Symbol">{-#</a> <a id="64" class="Keyword">OPTIONS</a> <a id="72" class="Pragma">--without-K</a> <a id="84" class="Pragma">--exact-split</a> <a id="98" class="Symbol">#-}</a>

<a id="103" class="Keyword">module</a> <a id="110" href="ring-theory.html" class="Module">ring-theory</a> <a id="122" class="Keyword">where</a>

<a id="129" class="Keyword">open</a> <a id="134" class="Keyword">import</a> <a id="141" href="ring-theory.rings.html" class="Module">ring-theory.rings</a> <a id="159" class="Keyword">public</a>
<a id="166" class="Keyword">open</a> <a id="171" class="Keyword">import</a> <a id="178" href="ring-theory.rings-with-properties.html" class="Module">ring-theory.rings-with-properties</a> <a id="212" class="Keyword">public</a>
<a id="219" class="Keyword">open</a> <a id="224" class="Keyword">import</a> <a id="231" href="ring-theory.ideals.html" class="Module">ring-theory.ideals</a> <a id="250" class="Keyword">public</a>
<a id="257" class="Keyword">open</a> <a id="262" class="Keyword">import</a> <a id="269" href="ring-theory.localizations-rings.html" class="Module">ring-theory.localizations-rings</a> <a id="301" class="Keyword">public</a>
<a id="308" class="Keyword">open</a> <a id="313" class="Keyword">import</a> <a id="320" href="ring-theory.eisenstein-integers.html" class="Module">ring-theory.eisenstein-integers</a> <a id="352" class="Keyword">public</a>
<a id="359" class="Keyword">open</a> <a id="364" class="Keyword">import</a> <a id="371" href="ring-theory.gaussian-integers.html" class="Module">ring-theory.gaussian-integers</a> <a id="401" class="Keyword">public</a>
</pre>