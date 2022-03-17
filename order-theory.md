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
<a id="447" class="Keyword">open</a> <a id="452" class="Keyword">import</a> <a id="459" href="order-theory.interval-subposets.html" class="Module">order-theory.interval-subposets</a> <a id="491" class="Keyword">public</a>
<a id="498" class="Keyword">open</a> <a id="503" class="Keyword">import</a> <a id="510" href="order-theory.largest-elements-posets.html" class="Module">order-theory.largest-elements-posets</a> <a id="547" class="Keyword">public</a>
<a id="554" class="Keyword">open</a> <a id="559" class="Keyword">import</a> <a id="566" href="order-theory.largest-elements-preorders.html" class="Module">order-theory.largest-elements-preorders</a> <a id="606" class="Keyword">public</a>
<a id="613" class="Keyword">open</a> <a id="618" class="Keyword">import</a> <a id="625" href="order-theory.least-elements-posets.html" class="Module">order-theory.least-elements-posets</a> <a id="660" class="Keyword">public</a>
<a id="667" class="Keyword">open</a> <a id="672" class="Keyword">import</a> <a id="679" href="order-theory.least-elements-preorders.html" class="Module">order-theory.least-elements-preorders</a> <a id="717" class="Keyword">public</a>
<a id="724" class="Keyword">open</a> <a id="729" class="Keyword">import</a> <a id="736" href="order-theory.locally-finite-posets.html" class="Module">order-theory.locally-finite-posets</a> <a id="771" class="Keyword">public</a>
<a id="778" class="Keyword">open</a> <a id="783" class="Keyword">import</a> <a id="790" href="order-theory.maximal-chains-posets.html" class="Module">order-theory.maximal-chains-posets</a> <a id="825" class="Keyword">public</a>
<a id="832" class="Keyword">open</a> <a id="837" class="Keyword">import</a> <a id="844" href="order-theory.maximal-chains-preorders.html" class="Module">order-theory.maximal-chains-preorders</a> <a id="882" class="Keyword">public</a>
<a id="889" class="Keyword">open</a> <a id="894" class="Keyword">import</a> <a id="901" href="order-theory.planar-binary-trees.html" class="Module">order-theory.planar-binary-trees</a> <a id="934" class="Keyword">public</a>
<a id="941" class="Keyword">open</a> <a id="946" class="Keyword">import</a> <a id="953" href="order-theory.posets.html" class="Module">order-theory.posets</a> <a id="973" class="Keyword">public</a>
<a id="980" class="Keyword">open</a> <a id="985" class="Keyword">import</a> <a id="992" href="order-theory.preorders.html" class="Module">order-theory.preorders</a> <a id="1015" class="Keyword">public</a>
<a id="1022" class="Keyword">open</a> <a id="1027" class="Keyword">import</a> <a id="1034" href="order-theory.subposets.html" class="Module">order-theory.subposets</a> <a id="1057" class="Keyword">public</a>
<a id="1064" class="Keyword">open</a> <a id="1069" class="Keyword">import</a> <a id="1076" href="order-theory.subpreorders.html" class="Module">order-theory.subpreorders</a> <a id="1102" class="Keyword">public</a>
<a id="1109" class="Keyword">open</a> <a id="1114" class="Keyword">import</a> <a id="1121" href="order-theory.total-posets.html" class="Module">order-theory.total-posets</a> <a id="1147" class="Keyword">public</a>
<a id="1154" class="Keyword">open</a> <a id="1159" class="Keyword">import</a> <a id="1166" href="order-theory.total-preorders.html" class="Module">order-theory.total-preorders</a> <a id="1195" class="Keyword">public</a>
</pre>