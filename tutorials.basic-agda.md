# Tutorial on basic use of Agda

<pre class="Agda"><a id="42" class="Symbol">{-#</a> <a id="46" class="Keyword">OPTIONS</a> <a id="54" class="Pragma">--without-K</a> <a id="66" class="Pragma">--exact-split</a> <a id="80" class="Pragma">--allow-unsolved-metas</a> <a id="103" class="Symbol">#-}</a>

<a id="108" class="Keyword">module</a> <a id="115" href="tutorials.basic-agda.html" class="Module">tutorials.basic-agda</a> <a id="136" class="Keyword">where</a>
</pre>
## Introduction

Welcome to the tutorial on basic use of Agda. Agda is a computer proof assistant. It can be used for formal mathematical reasoning, verification of software, and implementation and design of dependently typed programming languages. Here we will focus solely on the first use of Agda, as a proof assistant for mathematical reasoning.

## Further resources

There are many online resources that can help you learn more about Agda

* [The official Agda documentation](https://agda.readthedocs.io/en/v2.6.2.1/)
* [Martin Escardo's Univalent Foundations of Mathematics with Agda](https://www.cs.bham.ac.uk/~mhe/HoTT-UF-in-Agda-Lecture-Notes/)
* [Thorsten Altenkirch's Computer Aided Formal Reasoning](http://www.cs.nott.ac.uk/~psztxa/g53cfr/)

## How to use Agda

To obtain Agda, follow the instructions from the [installation manual](https://agda.readthedocs.io/en/v2.6.2.1/getting-started/installation.html) of the official Agda documentation. Agda can be used in either emacs or vscode. Here we will focus on Agda in emacs.

This tutorial is written in a literate Agda file. In our case, the file is named `basic-agda.lagda.md`, which means that we can write markdown code between the blocks of Agda code. A block of Agda code is opened with three back ticks followed by the letters `agda`, and it is closed with three back ticks. For example, the following block of Agda code introduces the type of natural numbers:

<pre class="Agda"><a id="1588" class="Keyword">data</a> <a id="ℕ"></a><a id="1593" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a> <a id="1595" class="Symbol">:</a> <a id="1597" href="Agda.Primitive.html#326" class="Primitive">Set</a> <a id="1601" class="Keyword">where</a>
  <a id="ℕ.zero-ℕ"></a><a id="1609" href="tutorials.basic-agda.html#1609" class="InductiveConstructor">zero-ℕ</a> <a id="1616" class="Symbol">:</a> <a id="1618" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a>
  <a id="ℕ.succ-ℕ"></a><a id="1622" href="tutorials.basic-agda.html#1622" class="InductiveConstructor">succ-ℕ</a> <a id="1629" class="Symbol">:</a> <a id="1631" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a> <a id="1633" class="Symbol">→</a> <a id="1635" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a>
</pre>
In emacs mode, the symbol ℕ for the natural numbers is obtained by typing `\bN`. Likewise, the arrow is obtained by typing `\to`. The emacs mode has support for many unicode characters. The [official documentation](https://agda.readthedocs.io/en/v2.6.2.1/tools/emacs-mode.html#unicode-input) explains how to use them.

### Defining basic operations on natural numbers

<pre class="Agda"><a id="add-ℕ"></a><a id="2019" href="tutorials.basic-agda.html#2019" class="Function">add-ℕ</a> <a id="2025" class="Symbol">:</a> <a id="2027" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a> <a id="2029" class="Symbol">→</a> <a id="2031" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a> <a id="2033" class="Symbol">→</a> <a id="2035" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a>
<a id="2037" href="tutorials.basic-agda.html#2019" class="Function">add-ℕ</a> <a id="2043" href="tutorials.basic-agda.html#2043" class="Bound">x</a> <a id="2045" href="tutorials.basic-agda.html#1609" class="InductiveConstructor">zero-ℕ</a> <a id="2052" class="Symbol">=</a> <a id="2054" href="tutorials.basic-agda.html#2043" class="Bound">x</a>
<a id="2056" href="tutorials.basic-agda.html#2019" class="Function">add-ℕ</a> <a id="2062" href="tutorials.basic-agda.html#2062" class="Bound">x</a> <a id="2064" class="Symbol">(</a><a id="2065" href="tutorials.basic-agda.html#1622" class="InductiveConstructor">succ-ℕ</a> <a id="2072" href="tutorials.basic-agda.html#2072" class="Bound">y</a><a id="2073" class="Symbol">)</a> <a id="2075" class="Symbol">=</a> <a id="2077" href="tutorials.basic-agda.html#1622" class="InductiveConstructor">succ-ℕ</a> <a id="2084" class="Symbol">(</a><a id="2085" href="tutorials.basic-agda.html#2019" class="Function">add-ℕ</a> <a id="2091" href="tutorials.basic-agda.html#2062" class="Bound">x</a> <a id="2093" href="tutorials.basic-agda.html#2072" class="Bound">y</a><a id="2094" class="Symbol">)</a>

<a id="mul-ℕ"></a><a id="2097" href="tutorials.basic-agda.html#2097" class="Function">mul-ℕ</a> <a id="2103" class="Symbol">:</a> <a id="2105" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a> <a id="2107" class="Symbol">→</a> <a id="2109" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a> <a id="2111" class="Symbol">→</a> <a id="2113" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a>
<a id="2115" href="tutorials.basic-agda.html#2097" class="Function">mul-ℕ</a> <a id="2121" class="Symbol">=</a> <a id="2123" class="Hole">{!!}</a>

<a id="exp-ℕ"></a><a id="2129" href="tutorials.basic-agda.html#2129" class="Function">exp-ℕ</a> <a id="2135" class="Symbol">:</a> <a id="2137" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a> <a id="2139" class="Symbol">→</a> <a id="2141" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a> <a id="2143" class="Symbol">→</a> <a id="2145" href="tutorials.basic-agda.html#1593" class="Datatype">ℕ</a>
<a id="2147" href="tutorials.basic-agda.html#2129" class="Function">exp-ℕ</a> <a id="2153" class="Symbol">=</a> <a id="2155" class="Hole">{!!}</a>
</pre>
### Equality in Agda

Equality in a proof assistant is expressed by the identity type

<pre class="Agda"><a id="2260" class="Keyword">data</a> <a id="Id"></a><a id="2265" href="tutorials.basic-agda.html#2265" class="Datatype">Id</a> <a id="2268" class="Symbol">{</a><a id="2269" href="tutorials.basic-agda.html#2269" class="Bound">X</a> <a id="2271" class="Symbol">:</a> <a id="2273" href="Agda.Primitive.html#326" class="Primitive">Set</a><a id="2276" class="Symbol">}</a> <a id="2278" class="Symbol">(</a><a id="2279" href="tutorials.basic-agda.html#2279" class="Bound">x</a> <a id="2281" class="Symbol">:</a> <a id="2283" href="tutorials.basic-agda.html#2269" class="Bound">X</a><a id="2284" class="Symbol">)</a> <a id="2286" class="Symbol">:</a> <a id="2288" href="tutorials.basic-agda.html#2269" class="Bound">X</a> <a id="2290" class="Symbol">→</a> <a id="2292" href="Agda.Primitive.html#326" class="Primitive">Set</a> <a id="2296" class="Keyword">where</a>
  <a id="Id.refl"></a><a id="2304" href="tutorials.basic-agda.html#2304" class="InductiveConstructor">refl</a> <a id="2309" class="Symbol">:</a> <a id="2311" href="tutorials.basic-agda.html#2265" class="Datatype">Id</a> <a id="2314" href="tutorials.basic-agda.html#2279" class="Bound">x</a> <a id="2316" href="tutorials.basic-agda.html#2279" class="Bound">x</a>
</pre>
### Equality is an equivalence relation

### Every function preserves equality

### Addition on ℕ satisfies the usual laws

###
