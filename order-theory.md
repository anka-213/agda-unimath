# Order theory

<pre class="Agda"><a id="25" class="Symbol">{-#</a> <a id="29" class="Keyword">OPTIONS</a> <a id="37" class="Pragma">--without-K</a> <a id="49" class="Pragma">--exact-split</a> <a id="63" class="Symbol">#-}</a>

<a id="68" class="Keyword">module</a> <a id="75" href="order-theory.html" class="Module">order-theory</a> <a id="88" class="Keyword">where</a>

<a id="95" class="Keyword">open</a> <a id="100" class="Keyword">import</a> <a id="107" href="order-theory.chains-posets.html" class="Module">order-theory.chains-posets</a> <a id="134" class="Keyword">public</a>
<a id="141" class="Keyword">open</a> <a id="146" class="Keyword">import</a> <a id="153" href="order-theory.chains-preorders.html" class="Module">order-theory.chains-preorders</a> <a id="183" class="Keyword">public</a>
<a id="190" class="Keyword">open</a> <a id="195" class="Keyword">import</a> <a id="202" href="order-theory.decidable-subposets.html" class="Module">order-theory.decidable-subposets</a> <a id="235" class="Keyword">public</a>
<a id="242" class="Keyword">open</a> <a id="247" class="Keyword">import</a> <a id="254" href="order-theory.decidable-subpreorders.html" class="Module">order-theory.decidable-subpreorders</a> <a id="290" class="Keyword">public</a>
<a id="297" class="Keyword">open</a> <a id="302" class="Keyword">import</a> <a id="309" href="order-theory.finite-posets.html" class="Module">order-theory.finite-posets</a> <a id="336" class="Keyword">public</a>
<a id="343" class="Keyword">open</a> <a id="348" class="Keyword">import</a> <a id="355" href="order-theory.finite-preorders.html" class="Module">order-theory.finite-preorders</a> <a id="385" class="Keyword">public</a>
<a id="392" class="Keyword">open</a> <a id="397" class="Keyword">import</a> <a id="404" href="order-theory.finitely-graded-posets.html" class="Module">order-theory.finitely-graded-posets</a> <a id="440" class="Keyword">public</a>
<a id="447" class="Keyword">open</a> <a id="452" class="Keyword">import</a> <a id="459" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a> <a id="496" class="Keyword">public</a>
<a id="503" class="Keyword">open</a> <a id="508" class="Keyword">import</a> <a id="515" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a> <a id="555" class="Keyword">public</a>
<a id="562" class="Keyword">open</a> <a id="567" class="Keyword">import</a> <a id="574" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a> <a id="609" class="Keyword">public</a>
<a id="616" class="Keyword">open</a> <a id="621" class="Keyword">import</a> <a id="628" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a> <a id="666" class="Keyword">public</a>
<a id="673" class="Keyword">open</a> <a id="678" class="Keyword">import</a> <a id="685" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a> <a id="720" class="Keyword">public</a>
<a id="727" class="Keyword">open</a> <a id="732" class="Keyword">import</a> <a id="739" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a> <a id="774" class="Keyword">public</a>
<a id="781" class="Keyword">open</a> <a id="786" class="Keyword">import</a> <a id="793" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a> <a id="831" class="Keyword">public</a>
<a id="838" class="Keyword">open</a> <a id="843" class="Keyword">import</a> <a id="850" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a> <a id="883" class="Keyword">public</a>
<a id="890" class="Keyword">open</a> <a id="895" class="Keyword">import</a> <a id="902" href="order-theory.posets.html" class="Module">order-theory.posets</a> <a id="922" class="Keyword">public</a>
<a id="929" class="Keyword">open</a> <a id="934" class="Keyword">import</a> <a id="941" href="order-theory.preorders.html" class="Module">order-theory.preorders</a> <a id="964" class="Keyword">public</a>
<a id="971" class="Keyword">open</a> <a id="976" class="Keyword">import</a> <a id="983" href="order-theory.subposets.html" class="Module">order-theory.subposets</a> <a id="1006" class="Keyword">public</a>
<a id="1013" class="Keyword">open</a> <a id="1018" class="Keyword">import</a> <a id="1025" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a> <a id="1051" class="Keyword">public</a>
<a id="1058" class="Keyword">open</a> <a id="1063" class="Keyword">import</a> <a id="1070" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a> <a id="1096" class="Keyword">public</a>
<a id="1103" class="Keyword">open</a> <a id="1108" class="Keyword">import</a> <a id="1115" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a> <a id="1144" class="Keyword">public</a>
</pre>