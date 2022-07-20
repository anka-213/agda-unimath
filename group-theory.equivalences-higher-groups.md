---
title: Equivalences of higher groups
---

<pre class="Agda"><a id="55" class="Symbol">{-#</a> <a id="59" class="Keyword">OPTIONS</a> <a id="67" class="Pragma">--without-K</a> <a id="79" class="Pragma">--exact-split</a> <a id="93" class="Symbol">#-}</a>

<a id="98" class="Keyword">module</a> <a id="105" href="group-theory.equivalences-higher-groups.html" class="Module">group-theory.equivalences-higher-groups</a> <a id="145" class="Keyword">where</a>

<a id="152" class="Keyword">open</a> <a id="157" class="Keyword">import</a> <a id="164" href="foundation.functions.html" class="Module">foundation.functions</a>
<a id="185" class="Keyword">open</a> <a id="190" class="Keyword">import</a> <a id="197" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="225" class="Keyword">open</a> <a id="230" class="Keyword">import</a> <a id="237" href="group-theory.higher-groups.html" class="Module">group-theory.higher-groups</a>
<a id="264" class="Keyword">open</a> <a id="269" class="Keyword">import</a> <a id="276" href="group-theory.homomorphisms-higher-groups.html" class="Module">group-theory.homomorphisms-higher-groups</a>

<a id="318" class="Keyword">open</a> <a id="323" class="Keyword">import</a> <a id="330" href="structured-types.pointed-equivalences.html" class="Module">structured-types.pointed-equivalences</a>
</pre>
## Definitions

### Equivalences of higher groups

<pre class="Agda"><a id="432" class="Keyword">module</a> <a id="439" href="group-theory.equivalences-higher-groups.html#439" class="Module">_</a>
  <a id="443" class="Symbol">{</a><a id="444" href="group-theory.equivalences-higher-groups.html#444" class="Bound">l1</a> <a id="447" href="group-theory.equivalences-higher-groups.html#447" class="Bound">l2</a> <a id="450" class="Symbol">:</a> <a id="452" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="457" class="Symbol">}</a> <a id="459" class="Symbol">(</a><a id="460" href="group-theory.equivalences-higher-groups.html#460" class="Bound">G</a> <a id="462" class="Symbol">:</a> <a id="464" href="group-theory.higher-groups.html#1626" class="Function">∞-Group</a> <a id="472" href="group-theory.equivalences-higher-groups.html#444" class="Bound">l1</a><a id="474" class="Symbol">)</a> <a id="476" class="Symbol">(</a><a id="477" href="group-theory.equivalences-higher-groups.html#477" class="Bound">H</a> <a id="479" class="Symbol">:</a> <a id="481" href="group-theory.higher-groups.html#1626" class="Function">∞-Group</a> <a id="489" href="group-theory.equivalences-higher-groups.html#447" class="Bound">l2</a><a id="491" class="Symbol">)</a>
  <a id="495" class="Keyword">where</a>

  <a id="504" href="group-theory.equivalences-higher-groups.html#504" class="Function">equiv-∞-Group</a> <a id="518" class="Symbol">:</a> <a id="520" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="523" class="Symbol">(</a><a id="524" href="group-theory.equivalences-higher-groups.html#444" class="Bound">l1</a> <a id="527" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="529" href="group-theory.equivalences-higher-groups.html#447" class="Bound">l2</a><a id="531" class="Symbol">)</a>
  <a id="535" href="group-theory.equivalences-higher-groups.html#504" class="Function">equiv-∞-Group</a> <a id="549" class="Symbol">=</a>
    <a id="555" href="group-theory.higher-groups.html#1789" class="Function">classifying-pointed-type-∞-Group</a> <a id="588" href="group-theory.equivalences-higher-groups.html#460" class="Bound">G</a> <a id="590" href="structured-types.pointed-equivalences.html#2737" class="Function Operator">≃*</a> <a id="593" href="group-theory.higher-groups.html#1789" class="Function">classifying-pointed-type-∞-Group</a> <a id="626" href="group-theory.equivalences-higher-groups.html#477" class="Bound">H</a>

  <a id="631" href="group-theory.equivalences-higher-groups.html#631" class="Function">hom-equiv-∞-Group</a> <a id="649" class="Symbol">:</a> <a id="651" href="group-theory.equivalences-higher-groups.html#504" class="Function">equiv-∞-Group</a> <a id="665" class="Symbol">→</a> <a id="667" href="group-theory.homomorphisms-higher-groups.html#650" class="Function">hom-∞-Group</a> <a id="679" href="group-theory.equivalences-higher-groups.html#460" class="Bound">G</a> <a id="681" href="group-theory.equivalences-higher-groups.html#477" class="Bound">H</a>
  <a id="685" href="group-theory.equivalences-higher-groups.html#631" class="Function">hom-equiv-∞-Group</a> <a id="703" class="Symbol">=</a>
    <a id="709" href="structured-types.pointed-equivalences.html#3765" class="Function">pointed-map-pointed-equiv</a>
      <a id="741" class="Symbol">(</a> <a id="743" href="group-theory.higher-groups.html#1789" class="Function">classifying-pointed-type-∞-Group</a> <a id="776" href="group-theory.equivalences-higher-groups.html#460" class="Bound">G</a><a id="777" class="Symbol">)</a>
      <a id="785" class="Symbol">(</a> <a id="787" href="group-theory.higher-groups.html#1789" class="Function">classifying-pointed-type-∞-Group</a> <a id="820" href="group-theory.equivalences-higher-groups.html#477" class="Bound">H</a><a id="821" class="Symbol">)</a>

  <a id="826" href="group-theory.equivalences-higher-groups.html#826" class="Function">map-equiv-∞-Group</a> <a id="844" class="Symbol">:</a> <a id="846" href="group-theory.equivalences-higher-groups.html#504" class="Function">equiv-∞-Group</a> <a id="860" class="Symbol">→</a> <a id="862" href="group-theory.higher-groups.html#2808" class="Function">type-∞-Group</a> <a id="875" href="group-theory.equivalences-higher-groups.html#460" class="Bound">G</a> <a id="877" class="Symbol">→</a> <a id="879" href="group-theory.higher-groups.html#2808" class="Function">type-∞-Group</a> <a id="892" href="group-theory.equivalences-higher-groups.html#477" class="Bound">H</a>
  <a id="896" href="group-theory.equivalences-higher-groups.html#826" class="Function">map-equiv-∞-Group</a> <a id="914" class="Symbol">=</a> <a id="916" href="group-theory.homomorphisms-higher-groups.html#1336" class="Function">map-hom-∞-Group</a> <a id="932" href="group-theory.equivalences-higher-groups.html#460" class="Bound">G</a> <a id="934" href="group-theory.equivalences-higher-groups.html#477" class="Bound">H</a> <a id="936" href="foundation-core.functions.html#420" class="Function Operator">∘</a> <a id="938" href="group-theory.equivalences-higher-groups.html#631" class="Function">hom-equiv-∞-Group</a>
</pre>
### The identity equivalence of higher groups

<pre class="Agda"><a id="id-equiv-∞-Group"></a><a id="1016" href="group-theory.equivalences-higher-groups.html#1016" class="Function">id-equiv-∞-Group</a> <a id="1033" class="Symbol">:</a>
  <a id="1037" class="Symbol">{</a><a id="1038" href="group-theory.equivalences-higher-groups.html#1038" class="Bound">l1</a> <a id="1041" class="Symbol">:</a> <a id="1043" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1048" class="Symbol">}</a> <a id="1050" class="Symbol">(</a><a id="1051" href="group-theory.equivalences-higher-groups.html#1051" class="Bound">G</a> <a id="1053" class="Symbol">:</a> <a id="1055" href="group-theory.higher-groups.html#1626" class="Function">∞-Group</a> <a id="1063" href="group-theory.equivalences-higher-groups.html#1038" class="Bound">l1</a><a id="1065" class="Symbol">)</a> <a id="1067" class="Symbol">→</a> <a id="1069" href="group-theory.equivalences-higher-groups.html#504" class="Function">equiv-∞-Group</a> <a id="1083" href="group-theory.equivalences-higher-groups.html#1051" class="Bound">G</a> <a id="1085" href="group-theory.equivalences-higher-groups.html#1051" class="Bound">G</a>
<a id="1087" href="group-theory.equivalences-higher-groups.html#1016" class="Function">id-equiv-∞-Group</a> <a id="1104" href="group-theory.equivalences-higher-groups.html#1104" class="Bound">G</a> <a id="1106" class="Symbol">=</a> <a id="1108" href="structured-types.pointed-equivalences.html#4146" class="Function">id-pointed-equiv</a> <a id="1125" class="Symbol">(</a><a id="1126" href="group-theory.higher-groups.html#1789" class="Function">classifying-pointed-type-∞-Group</a> <a id="1159" href="group-theory.equivalences-higher-groups.html#1104" class="Bound">G</a><a id="1160" class="Symbol">)</a>
</pre>