# Principal group actions

<pre class="Agda"><a id="36" class="Symbol">{-#</a> <a id="40" class="Keyword">OPTIONS</a> <a id="48" class="Pragma">--without-K</a> <a id="60" class="Pragma">--exact-split</a> <a id="74" class="Symbol">#-}</a>

<a id="79" class="Keyword">module</a> <a id="86" href="group-theory.principal-group-actions.html" class="Module">group-theory.principal-group-actions</a> <a id="123" class="Keyword">where</a>

<a id="130" class="Keyword">open</a> <a id="135" class="Keyword">import</a> <a id="142" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="174" class="Keyword">using</a> <a id="180" class="Symbol">(</a><a id="181" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="182" class="Symbol">;</a> <a id="184" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="188" class="Symbol">;</a> <a id="190" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="193" class="Symbol">;</a> <a id="195" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="198" class="Symbol">)</a>
<a id="200" class="Keyword">open</a> <a id="205" class="Keyword">import</a> <a id="212" href="foundation.equivalences.html" class="Module">foundation.equivalences</a> <a id="236" class="Keyword">using</a> <a id="242" class="Symbol">(</a><a id="243" href="foundation.equivalences.html#14746" class="Function">eq-htpy-equiv</a><a id="256" class="Symbol">)</a>
<a id="258" class="Keyword">open</a> <a id="263" class="Keyword">import</a> <a id="270" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="297" class="Keyword">using</a> <a id="303" class="Symbol">(</a><a id="304" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="309" class="Symbol">)</a>

<a id="312" class="Keyword">open</a> <a id="317" class="Keyword">import</a> <a id="324" href="group-theory.group-actions.html" class="Module">group-theory.group-actions</a> <a id="351" class="Keyword">using</a> <a id="357" class="Symbol">(</a><a id="358" href="group-theory.group-actions.html#1192" class="Function">Abstract-Group-Action</a><a id="379" class="Symbol">)</a>
<a id="381" class="Keyword">open</a> <a id="386" class="Keyword">import</a> <a id="393" href="group-theory.groups.html" class="Module">group-theory.groups</a> <a id="413" class="Keyword">using</a>
  <a id="421" class="Symbol">(</a> <a id="423" href="group-theory.groups.html#2398" class="Function">Group</a><a id="428" class="Symbol">;</a> <a id="430" href="group-theory.groups.html#2581" class="Function">set-Group</a><a id="439" class="Symbol">;</a> <a id="441" href="group-theory.groups.html#5518" class="Function">equiv-mul-Group</a><a id="456" class="Symbol">;</a> <a id="458" href="group-theory.groups.html#3235" class="Function">associative-mul-Group</a><a id="479" class="Symbol">)</a>
</pre>
## Idea

The principal group action is the action of a group on itself by multiplication from the left

## Definition

<pre class="Agda"><a id="613" class="Keyword">module</a> <a id="620" href="group-theory.principal-group-actions.html#620" class="Module">_</a>
  <a id="624" class="Symbol">{</a><a id="625" href="group-theory.principal-group-actions.html#625" class="Bound">l1</a> <a id="628" class="Symbol">:</a> <a id="630" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="635" class="Symbol">}</a> <a id="637" class="Symbol">(</a><a id="638" href="group-theory.principal-group-actions.html#638" class="Bound">G</a> <a id="640" class="Symbol">:</a> <a id="642" href="group-theory.groups.html#2398" class="Function">Group</a> <a id="648" href="group-theory.principal-group-actions.html#625" class="Bound">l1</a><a id="650" class="Symbol">)</a>
  <a id="654" class="Keyword">where</a>
  
  <a id="665" href="group-theory.principal-group-actions.html#665" class="Function">principal-Abstract-Group-Action</a> <a id="697" class="Symbol">:</a> <a id="699" href="group-theory.group-actions.html#1192" class="Function">Abstract-Group-Action</a> <a id="721" href="group-theory.principal-group-actions.html#638" class="Bound">G</a> <a id="723" href="group-theory.principal-group-actions.html#625" class="Bound">l1</a>
  <a id="728" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="732" href="group-theory.principal-group-actions.html#665" class="Function">principal-Abstract-Group-Action</a> <a id="764" class="Symbol">=</a> <a id="766" href="group-theory.groups.html#2581" class="Function">set-Group</a> <a id="776" href="group-theory.principal-group-actions.html#638" class="Bound">G</a>
  <a id="780" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a> <a id="784" class="Symbol">(</a><a id="785" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="789" href="group-theory.principal-group-actions.html#665" class="Function">principal-Abstract-Group-Action</a><a id="820" class="Symbol">)</a> <a id="822" href="group-theory.principal-group-actions.html#822" class="Bound">g</a> <a id="824" class="Symbol">=</a> <a id="826" href="group-theory.groups.html#5518" class="Function">equiv-mul-Group</a> <a id="842" href="group-theory.principal-group-actions.html#638" class="Bound">G</a> <a id="844" href="group-theory.principal-group-actions.html#822" class="Bound">g</a>
  <a id="848" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="852" class="Symbol">(</a><a id="853" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a> <a id="857" href="group-theory.principal-group-actions.html#665" class="Function">principal-Abstract-Group-Action</a><a id="888" class="Symbol">)</a> <a id="890" href="group-theory.principal-group-actions.html#890" class="Bound">g</a> <a id="892" href="group-theory.principal-group-actions.html#892" class="Bound">h</a> <a id="894" class="Symbol">=</a>
    <a id="900" href="foundation.equivalences.html#14746" class="Function">eq-htpy-equiv</a> <a id="914" class="Symbol">(</a><a id="915" href="group-theory.groups.html#3235" class="Function">associative-mul-Group</a> <a id="937" href="group-theory.principal-group-actions.html#638" class="Bound">G</a> <a id="939" href="group-theory.principal-group-actions.html#890" class="Bound">g</a> <a id="941" href="group-theory.principal-group-actions.html#892" class="Bound">h</a><a id="942" class="Symbol">)</a>
</pre>