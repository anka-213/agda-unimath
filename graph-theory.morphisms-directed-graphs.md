# Morphisms of directed graphs

<pre class="Agda"><a id="41" class="Symbol">{-#</a> <a id="45" class="Keyword">OPTIONS</a> <a id="53" class="Pragma">--without-K</a> <a id="65" class="Pragma">--exact-split</a> <a id="79" class="Symbol">#-}</a>

<a id="84" class="Keyword">module</a> <a id="91" href="graph-theory.morphisms-directed-graphs.html" class="Module">graph-theory.morphisms-directed-graphs</a> <a id="130" class="Keyword">where</a>

<a id="137" class="Keyword">open</a> <a id="142" class="Keyword">import</a> <a id="149" href="foundation.contractible-types.html" class="Module">foundation.contractible-types</a> <a id="179" class="Keyword">using</a> <a id="185" class="Symbol">(</a><a id="186" href="foundation-core.contractible-types.html#925" class="Function">is-contr</a><a id="194" class="Symbol">;</a> <a id="196" href="foundation-core.contractible-types.html#3739" class="Function">is-contr-equiv&#39;</a><a id="211" class="Symbol">)</a>
<a id="213" class="Keyword">open</a> <a id="218" class="Keyword">import</a> <a id="225" href="foundation.dependent-pair-types.html" class="Module">foundation.dependent-pair-types</a> <a id="257" class="Keyword">using</a> <a id="263" class="Symbol">(</a><a id="264" href="foundation-core.dependent-pair-types.html#502" class="Record">Σ</a><a id="265" class="Symbol">;</a> <a id="267" href="foundation-core.dependent-pair-types.html#575" class="InductiveConstructor">pair</a><a id="271" class="Symbol">;</a> <a id="273" href="foundation-core.dependent-pair-types.html#592" class="Field">pr1</a><a id="276" class="Symbol">;</a> <a id="278" href="foundation-core.dependent-pair-types.html#604" class="Field">pr2</a><a id="281" class="Symbol">)</a>
<a id="283" class="Keyword">open</a> <a id="288" class="Keyword">import</a> <a id="295" href="foundation.equality-dependent-function-types.html" class="Module">foundation.equality-dependent-function-types</a> <a id="340" class="Keyword">using</a>
  <a id="348" class="Symbol">(</a> <a id="350" href="foundation.equality-dependent-function-types.html#1038" class="Function">is-contr-total-Eq-Π</a><a id="369" class="Symbol">)</a>
<a id="371" class="Keyword">open</a> <a id="376" class="Keyword">import</a> <a id="383" href="foundation.equivalences.html" class="Module">foundation.equivalences</a> <a id="407" class="Keyword">using</a> <a id="413" class="Symbol">(</a><a id="414" href="foundation-core.equivalences.html#1542" class="Function">is-equiv</a><a id="422" class="Symbol">;</a> <a id="424" href="foundation-core.equivalences.html#1607" class="Function Operator">_≃_</a><a id="427" class="Symbol">;</a> <a id="429" href="foundation-core.equivalences.html#4173" class="Function">map-inv-is-equiv</a><a id="445" class="Symbol">)</a>
<a id="447" class="Keyword">open</a> <a id="452" class="Keyword">import</a> <a id="459" href="foundation.functions.html" class="Module">foundation.functions</a> <a id="480" class="Keyword">using</a> <a id="486" class="Symbol">(</a><a id="487" href="foundation-core.functions.html#407" class="Function Operator">_∘_</a><a id="490" class="Symbol">;</a> <a id="492" href="foundation-core.functions.html#309" class="Function">id</a><a id="494" class="Symbol">)</a>
<a id="496" class="Keyword">open</a> <a id="501" class="Keyword">import</a> <a id="508" href="foundation.functoriality-dependent-function-types.html" class="Module">foundation.functoriality-dependent-function-types</a> <a id="558" class="Keyword">using</a>
  <a id="566" class="Symbol">(</a> <a id="568" href="foundation.functoriality-dependent-function-types.html#3637" class="Function">equiv-map-Π</a><a id="579" class="Symbol">)</a>
<a id="581" class="Keyword">open</a> <a id="586" class="Keyword">import</a> <a id="593" href="foundation.functoriality-dependent-pair-types.html" class="Module">foundation.functoriality-dependent-pair-types</a> <a id="639" class="Keyword">using</a> <a id="645" class="Symbol">(</a><a id="646" href="foundation-core.functoriality-dependent-pair-types.html#6804" class="Function">equiv-tot</a><a id="655" class="Symbol">)</a>
<a id="657" class="Keyword">open</a> <a id="662" class="Keyword">import</a> <a id="669" href="foundation.fundamental-theorem-of-identity-types.html" class="Module">foundation.fundamental-theorem-of-identity-types</a> <a id="718" class="Keyword">using</a>
  <a id="726" class="Symbol">(</a> <a id="728" href="foundation-core.fundamental-theorem-of-identity-types.html#1888" class="Function">fundamental-theorem-id</a><a id="750" class="Symbol">)</a>
<a id="752" class="Keyword">open</a> <a id="757" class="Keyword">import</a> <a id="764" href="foundation.homotopies.html" class="Module">foundation.homotopies</a> <a id="786" class="Keyword">using</a> <a id="792" class="Symbol">(</a><a id="793" href="foundation-core.homotopies.html#467" class="Function Operator">_~_</a><a id="796" class="Symbol">;</a> <a id="798" href="foundation-core.homotopies.html#632" class="Function">refl-htpy</a><a id="807" class="Symbol">;</a> <a id="809" href="foundation.homotopies.html#3132" class="Function">is-contr-total-htpy</a><a id="828" class="Symbol">)</a>
<a id="830" class="Keyword">open</a> <a id="835" class="Keyword">import</a> <a id="842" href="foundation.identity-types.html" class="Module">foundation.identity-types</a> <a id="868" class="Keyword">using</a> <a id="874" class="Symbol">(</a><a id="875" href="foundation-core.identity-types.html#641" class="Datatype">Id</a><a id="877" class="Symbol">;</a> <a id="879" href="foundation-core.identity-types.html#4583" class="Function">tr</a><a id="881" class="Symbol">;</a> <a id="883" href="foundation-core.identity-types.html#2853" class="Function">ap</a><a id="885" class="Symbol">;</a> <a id="887" href="foundation.identity-types.html#1931" class="Function">equiv-concat</a><a id="899" class="Symbol">;</a> <a id="901" href="foundation-core.identity-types.html#694" class="InductiveConstructor">refl</a><a id="905" class="Symbol">)</a>
<a id="907" class="Keyword">open</a> <a id="912" class="Keyword">import</a> <a id="919" href="foundation.structure-identity-principle.html" class="Module">foundation.structure-identity-principle</a> <a id="959" class="Keyword">using</a>
  <a id="967" class="Symbol">(</a> <a id="969" href="foundation.structure-identity-principle.html#1341" class="Function">is-contr-total-Eq-structure</a><a id="996" class="Symbol">)</a>
<a id="998" class="Keyword">open</a> <a id="1003" class="Keyword">import</a> <a id="1010" href="foundation.universe-levels.html" class="Module">foundation.universe-levels</a> <a id="1037" class="Keyword">using</a> <a id="1043" class="Symbol">(</a><a id="1044" href="Agda.Primitive.html#597" class="Postulate">Level</a><a id="1049" class="Symbol">;</a> <a id="1051" href="foundation-core.universe-levels.html#222" class="Primitive">UU</a><a id="1053" class="Symbol">;</a> <a id="1055" href="Agda.Primitive.html#810" class="Primitive Operator">_⊔_</a><a id="1058" class="Symbol">;</a> <a id="1060" href="Agda.Primitive.html#780" class="Primitive">lsuc</a><a id="1064" class="Symbol">;</a> <a id="1066" href="Agda.Primitive.html#764" class="Primitive">lzero</a><a id="1071" class="Symbol">)</a>
<a id="1073" class="Keyword">open</a> <a id="1078" class="Keyword">import</a> <a id="1085" href="foundation.unordered-pairs.html" class="Module">foundation.unordered-pairs</a> <a id="1112" class="Keyword">using</a>
  <a id="1120" class="Symbol">(</a> <a id="1122" href="foundation.unordered-pairs.html#7646" class="Function">map-unordered-pair</a><a id="1140" class="Symbol">;</a> <a id="1142" href="foundation.unordered-pairs.html#8243" class="Function">htpy-unordered-pair</a><a id="1161" class="Symbol">;</a> <a id="1163" href="foundation.unordered-pairs.html#8564" class="Function">preserves-refl-htpy-unordered-pair</a><a id="1197" class="Symbol">)</a>

<a id="1200" class="Keyword">open</a> <a id="1205" class="Keyword">import</a> <a id="1212" href="graph-theory.directed-graphs.html" class="Module">graph-theory.directed-graphs</a> <a id="1241" class="Keyword">using</a>
  <a id="1249" class="Symbol">(</a> <a id="1251" href="graph-theory.directed-graphs.html#447" class="Function">Graph</a><a id="1256" class="Symbol">;</a> <a id="1258" href="graph-theory.directed-graphs.html#599" class="Function">vertex-Graph</a><a id="1270" class="Symbol">;</a> <a id="1272" href="graph-theory.directed-graphs.html#646" class="Function">edge-Graph</a><a id="1282" class="Symbol">)</a>
</pre>
## Definitions

### Morphisms graphs

<pre class="Agda"><a id="1335" class="Comment">{-
module _
  {l1 l2 l3 l4 : Level}
  (G : Graph l1 l2) (H : Graph l3 l4)
  where

  hom-Graph : UU (lsuc lzero ⊔ l1 ⊔ l2 ⊔ l3 ⊔ l4)
  hom-Graph =
    Σ ( vertex-Graph G → vertex-Graph H )
      ( λ f →
        ( p : unordered-pair-vertices-Graph G) →
        edge-Graph G p →
        edge-Graph H (map-unordered-pair f p))

  vertex-hom-Graph :
    hom-Graph → vertex-Graph G → vertex-Graph H
  vertex-hom-Graph f = pr1 f

  unordered-pair-vertices-hom-Graph :
    hom-Graph →
    unordered-pair-vertices-Graph G →
    unordered-pair-vertices-Graph H
  unordered-pair-vertices-hom-Graph f =
    map-unordered-pair (vertex-hom-Graph f)

  edge-hom-Graph :
    (f : hom-Graph)
    (p : unordered-pair-vertices-Graph G) →
    edge-Graph G p →
    edge-Graph H
      ( unordered-pair-vertices-hom-Graph f p)
  edge-hom-Graph f = pr2 f
-}</a>
</pre>
### Composition of morphisms graphs

<pre class="Agda"><a id="2220" class="Comment">{-
module _
  {l1 l2 l3 l4 l5 l6 : Level}
  (G : Graph l1 l2) (H : Graph l3 l4)
  (K : Graph l5 l6)
  where

  comp-hom-Graph :
    hom-Graph H K → hom-Graph G H →
    hom-Graph G K
  pr1 (comp-hom-Graph (pair gV gE) (pair fV fE)) = gV ∘ fV
  pr2 (comp-hom-Graph (pair gV gE) (pair fV fE)) p e =
    gE (map-unordered-pair fV p) (fE p e)
-}</a>
</pre>
### Identity morphisms graphs

<pre class="Agda"><a id="2605" class="Comment">{-
module _
  {l1 l2 : Level} (G : Graph l1 l2)
  where

  id-hom-Graph : hom-Graph G G
  pr1 id-hom-Graph = id
  pr2 id-hom-Graph p = id
-}</a>
</pre>

## Properties

### Characterizing the identity type of morphisms graphs

<pre class="Agda"><a id="2833" class="Comment">{-
module _
  {l1 l2 l3 l4 : Level}
  (G : Graph l1 l2) (H : Graph l3 l4)
  where

  htpy-hom-Graph :
    (f g : hom-Graph G H) → UU (lsuc lzero ⊔ l1 ⊔ l2 ⊔ l3 ⊔ l4)
  htpy-hom-Graph f g =
    Σ ( vertex-hom-Graph G H f ~ vertex-hom-Graph G H g)
      ( λ α →
        ( p : unordered-pair-vertices-Graph G) →
        ( e : edge-Graph G p) →
        Id ( tr
             ( edge-Graph H)
             ( htpy-unordered-pair α p)
             ( edge-hom-Graph G H f p e))
           ( edge-hom-Graph G H g p e))

  refl-htpy-hom-Graph :
    (f : hom-Graph G H) → htpy-hom-Graph f f
  pr1 (refl-htpy-hom-Graph f) = refl-htpy
  pr2 (refl-htpy-hom-Graph f) p e =
    ap ( λ t →
         tr (edge-Graph H) t (edge-hom-Graph G H f p e))
       ( preserves-refl-htpy-unordered-pair
         ( vertex-hom-Graph G H f) p)

  htpy-eq-hom-Graph :
    (f g : hom-Graph G H) → Id f g → htpy-hom-Graph f g
  htpy-eq-hom-Graph f .f refl = refl-htpy-hom-Graph f

  abstract
    is-contr-total-htpy-hom-Graph :
      (f : hom-Graph G H) →
      is-contr (Σ (hom-Graph G H) (htpy-hom-Graph f))
    is-contr-total-htpy-hom-Graph f =
      is-contr-total-Eq-structure
        ( λ gV gE α →
          ( p : unordered-pair-vertices-Graph G) →
          ( e : edge-Graph G p) →
          Id ( tr
               ( edge-Graph H)
               ( htpy-unordered-pair α p)
               ( edge-hom-Graph G H f p e))
             ( gE p e))
        ( is-contr-total-htpy (vertex-hom-Graph G H f))
        ( pair (vertex-hom-Graph G H f) refl-htpy)
        ( is-contr-equiv&#39;
          ( Σ ( (p : unordered-pair-vertices-Graph G) →
                edge-Graph G p →
                edge-Graph H
                  ( unordered-pair-vertices-hom-Graph G H f p))
              ( λ gE →
                (p : unordered-pair-vertices-Graph G) →
                (e : edge-Graph G p) →
                Id (edge-hom-Graph G H f p e) (gE p e)))
          ( equiv-tot
            ( λ gE →
              equiv-map-Π
                ( λ p →
                  equiv-map-Π
                    ( λ e →
                      equiv-concat
                        ( pr2 (refl-htpy-hom-Graph f) p e)
                        ( gE p e)))))
          ( is-contr-total-Eq-Π
            ( λ p gE →
              ( e : edge-Graph G p) →
              Id (edge-hom-Graph G H f p e) (gE e))
            ( λ p → is-contr-total-htpy (edge-hom-Graph G H f p))))

  is-equiv-htpy-eq-hom-Graph :
    (f g : hom-Graph G H) →
    is-equiv (htpy-eq-hom-Graph f g)
  is-equiv-htpy-eq-hom-Graph f =
    fundamental-theorem-id f
      ( refl-htpy-hom-Graph f)
      ( is-contr-total-htpy-hom-Graph f)
      ( htpy-eq-hom-Graph f)

  extensionality-hom-Graph :
    (f g : hom-Graph G H) → Id f g ≃ htpy-hom-Graph f g
  pr1 (extensionality-hom-Graph f g) =
    htpy-eq-hom-Graph f g
  pr2 (extensionality-hom-Graph f g) =
    is-equiv-htpy-eq-hom-Graph f g

  eq-htpy-hom-Graph :
    (f g : hom-Graph G H) → htpy-hom-Graph f g → Id f g
  eq-htpy-hom-Graph f g =
    map-inv-is-equiv (is-equiv-htpy-eq-hom-Graph f g)
-}</a>
</pre>