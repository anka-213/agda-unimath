---
title: Distributive Lattices
---

<pre class="Agda"><a id="47" class="Symbol">{-#</a> <a id="51" class="Keyword">OPTIONS</a> <a id="59" class="Pragma">--without-K</a> <a id="71" class="Pragma">--exact-split</a> <a id="85" class="Symbol">#-}</a>

<a id="90" class="Keyword">module</a> <a id="97" href="order-theory.distributive-lattices.html" class="Module">order-theory.distributive-lattices</a> <a id="132" class="Keyword">where</a>

<a id="139" class="Keyword">open</a> <a id="144" class="Keyword">import</a> <a id="151" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a>
<a id="183" class="Keyword">open</a> <a id="188" class="Keyword">import</a> <a id="195" href="foundation.propositions.html" class="Module">foundation.propositions</a>
<a id="219" class="Keyword">open</a> <a id="224" class="Keyword">import</a> <a id="231" href="foundation.sets.html" class="Module">foundation.sets</a>
<a id="247" class="Keyword">open</a> <a id="252" class="Keyword">import</a> <a id="259" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a>

<a id="287" class="Keyword">open</a> <a id="292" class="Keyword">import</a> <a id="299" href="order-theory.lattices.html" class="Module">order-theory.lattices</a>
</pre>
## Idea

A distributive lattice is a lattice in which meets distribute over joins.

## Definition

<pre class="Agda"><a id="433" class="Keyword">module</a> <a id="440" href="order-theory.distributive-lattices.html#440" class="Module">_</a>
  <a id="444" class="Symbol">{</a><a id="445" href="order-theory.distributive-lattices.html#445" class="Bound">l1</a> <a id="448" href="order-theory.distributive-lattices.html#448" class="Bound">l2</a> <a id="451" class="Symbol">:</a> <a id="453" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="458" class="Symbol">}</a> <a id="460" class="Symbol">(</a><a id="461" href="order-theory.distributive-lattices.html#461" class="Bound">L</a> <a id="463" class="Symbol">:</a> <a id="465" href="order-theory.lattices.html#1097" class="Function">Lattice</a> <a id="473" href="order-theory.distributive-lattices.html#445" class="Bound">l1</a> <a id="476" href="order-theory.distributive-lattices.html#448" class="Bound">l2</a><a id="478" class="Symbol">)</a>
  <a id="482" class="Keyword">where</a>

  <a id="491" href="order-theory.distributive-lattices.html#491" class="Function">is-distributive-lattice-Prop</a> <a id="520" class="Symbol">:</a> <a id="522" href="foundation-core.propositions.html#1393" class="Function">UU-Prop</a> <a id="530" href="order-theory.distributive-lattices.html#445" class="Bound">l1</a>
  <a id="535" href="order-theory.distributive-lattices.html#491" class="Function">is-distributive-lattice-Prop</a> <a id="564" class="Symbol">=</a>
    <a id="570" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a>
      <a id="583" class="Symbol">(</a> <a id="585" href="order-theory.lattices.html#1311" class="Function">element-Lattice</a> <a id="601" href="order-theory.distributive-lattices.html#461" class="Bound">L</a><a id="602" class="Symbol">)</a>
      <a id="610" class="Symbol">(</a> <a id="612" class="Symbol">λ</a> <a id="614" href="order-theory.distributive-lattices.html#614" class="Bound">x</a> <a id="616" class="Symbol">→</a>
        <a id="626" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a>
          <a id="643" class="Symbol">(</a> <a id="645" href="order-theory.lattices.html#1311" class="Function">element-Lattice</a> <a id="661" href="order-theory.distributive-lattices.html#461" class="Bound">L</a><a id="662" class="Symbol">)</a>
          <a id="674" class="Symbol">(</a> <a id="676" class="Symbol">λ</a> <a id="678" href="order-theory.distributive-lattices.html#678" class="Bound">y</a> <a id="680" class="Symbol">→</a>
            <a id="694" href="foundation-core.propositions.html#6694" class="Function">Π-Prop</a>
              <a id="715" class="Symbol">(</a> <a id="717" href="order-theory.lattices.html#1311" class="Function">element-Lattice</a> <a id="733" href="order-theory.distributive-lattices.html#461" class="Bound">L</a><a id="734" class="Symbol">)</a>
              <a id="750" class="Symbol">(</a> <a id="752" class="Symbol">λ</a> <a id="754" href="order-theory.distributive-lattices.html#754" class="Bound">z</a> <a id="756" class="Symbol">→</a>
                <a id="774" href="foundation-core.sets.html#1420" class="Function">Id-Prop</a>
                  <a id="800" class="Symbol">(</a> <a id="802" href="order-theory.lattices.html#2292" class="Function">element-lattice-Set</a> <a id="822" href="order-theory.distributive-lattices.html#461" class="Bound">L</a><a id="823" class="Symbol">)</a>
                  <a id="843" class="Symbol">(</a> <a id="845" href="order-theory.lattices.html#2774" class="Function">meet-Lattice</a> <a id="858" href="order-theory.distributive-lattices.html#461" class="Bound">L</a> <a id="860" href="order-theory.distributive-lattices.html#614" class="Bound">x</a> <a id="862" class="Symbol">(</a><a id="863" href="order-theory.lattices.html#3193" class="Function">join-Lattice</a> <a id="876" href="order-theory.distributive-lattices.html#461" class="Bound">L</a> <a id="878" href="order-theory.distributive-lattices.html#678" class="Bound">y</a> <a id="880" href="order-theory.distributive-lattices.html#754" class="Bound">z</a><a id="881" class="Symbol">))</a>
                  <a id="902" class="Symbol">(</a> <a id="904" href="order-theory.lattices.html#3193" class="Function">join-Lattice</a> <a id="917" href="order-theory.distributive-lattices.html#461" class="Bound">L</a> <a id="919" class="Symbol">(</a><a id="920" href="order-theory.lattices.html#2774" class="Function">meet-Lattice</a> <a id="933" href="order-theory.distributive-lattices.html#461" class="Bound">L</a> <a id="935" href="order-theory.distributive-lattices.html#614" class="Bound">x</a> <a id="937" href="order-theory.distributive-lattices.html#678" class="Bound">y</a><a id="938" class="Symbol">)</a> <a id="940" class="Symbol">(</a><a id="941" href="order-theory.lattices.html#2774" class="Function">meet-Lattice</a> <a id="954" href="order-theory.distributive-lattices.html#461" class="Bound">L</a> <a id="956" href="order-theory.distributive-lattices.html#614" class="Bound">x</a> <a id="958" href="order-theory.distributive-lattices.html#754" class="Bound">z</a><a id="959" class="Symbol">)))))</a>

  <a id="968" href="order-theory.distributive-lattices.html#968" class="Function">is-distributive-Lattice</a> <a id="992" class="Symbol">:</a> <a id="994" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="997" href="order-theory.distributive-lattices.html#445" class="Bound">l1</a>
  <a id="1002" href="order-theory.distributive-lattices.html#968" class="Function">is-distributive-Lattice</a> <a id="1026" class="Symbol">=</a> <a id="1028" href="foundation-core.propositions.html#1495" class="Function">type-Prop</a> <a id="1038" href="order-theory.distributive-lattices.html#491" class="Function">is-distributive-lattice-Prop</a>

  <a id="1070" href="order-theory.distributive-lattices.html#1070" class="Function">is-prop-is-distributive-Lattice</a> <a id="1102" class="Symbol">:</a> <a id="1104" href="foundation-core.propositions.html#1309" class="Function">is-prop</a> <a id="1112" href="order-theory.distributive-lattices.html#968" class="Function">is-distributive-Lattice</a>
  <a id="1138" href="order-theory.distributive-lattices.html#1070" class="Function">is-prop-is-distributive-Lattice</a> <a id="1170" class="Symbol">=</a>
    <a id="1176" href="foundation-core.propositions.html#1562" class="Function">is-prop-type-Prop</a> <a id="1194" href="order-theory.distributive-lattices.html#491" class="Function">is-distributive-lattice-Prop</a>

<a id="Distributive-Lattice"></a><a id="1224" href="order-theory.distributive-lattices.html#1224" class="Function">Distributive-Lattice</a> <a id="1245" class="Symbol">:</a>
  <a id="1249" class="Symbol">(</a><a id="1250" href="order-theory.distributive-lattices.html#1250" class="Bound">l1</a> <a id="1253" href="order-theory.distributive-lattices.html#1253" class="Bound">l2</a> <a id="1256" class="Symbol">:</a> <a id="1258" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1263" class="Symbol">)</a> <a id="1265" class="Symbol">→</a> <a id="1267" href="foundation-core.universe-levels.html#235" class="Primitive">UU</a> <a id="1270" class="Symbol">(</a><a id="1271" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1276" href="order-theory.distributive-lattices.html#1250" class="Bound">l1</a> <a id="1279" href="Agda.Primitive.html#810" class="Primitive Operator">⊔</a> <a id="1281" href="Agda.Primitive.html#780" class="Primitive">lsuc</a> <a id="1286" href="order-theory.distributive-lattices.html#1253" class="Bound">l2</a><a id="1288" class="Symbol">)</a>
<a id="1290" href="order-theory.distributive-lattices.html#1224" class="Function">Distributive-Lattice</a> <a id="1311" href="order-theory.distributive-lattices.html#1311" class="Bound">l1</a> <a id="1314" href="order-theory.distributive-lattices.html#1314" class="Bound">l2</a> <a id="1317" class="Symbol">=</a>
  <a id="1321" href="foundation-core.dependent-pair-types.html#515" class="Record">Σ</a> <a id="1323" class="Symbol">(</a><a id="1324" href="order-theory.lattices.html#1097" class="Function">Lattice</a> <a id="1332" href="order-theory.distributive-lattices.html#1311" class="Bound">l1</a> <a id="1335" href="order-theory.distributive-lattices.html#1314" class="Bound">l2</a><a id="1337" class="Symbol">)</a> <a id="1339" href="order-theory.distributive-lattices.html#968" class="Function">is-distributive-Lattice</a>
</pre>