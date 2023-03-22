<script>

	// import { merge_ssr_styles } from 'svelte/internal';
	import { fade } from 'svelte/transition';
    import img2 from "$lib/screenshot.png"

function M (x) {
	return function go (func) {
		if (func === ret) return x;
		else x = func(x);
		return go;
	}
}
	
var nul = `const m = M();
const c = 2;
console.log("The value in the closure is", m(ret));
m(()=>c)(x=>x**6)(x=>x+36)(Math.sqrt);
console.log("The value in the closure is now", m(ret));
console.log("c is, of couse, still", c);`;

const entry1 = `The value in the closure is undefined
The value in the closure is now 10
c is, of couse, still 2`;

const anon = `    M(3)(v=>v**3)(v=>v*3)(v=>v+19)(Math.sqrt)(ret);  // 10`

var retDemo = `M(3)(v=>v**3)  // 27
M(3)(v=>v**3)(v=>v*3)  // 81
M(3)(v=>v**3)(v=>v*3)(v=>v+19)  // 100
M(3)(v=>v**3)(v=>v*3)(v=>v+19)(Math.sqrt)  // 10
M(3)(v=>v**3)(v=>v*3)(v=>v+19)(Math.sqrt)(v => v-4)(ret)  // 6
M(6)(v=>v*7)(ret)  // 42
M(M(6)(ret))(v=>v*7)(ret)  // 42
M(M(3)(v=>v**3)(v=>v*3)(v=>v+19)(Math.sqrt)(v => v-4)(ret))(v=>v*7)(ret)  // 42`

var retDemo2 = `M(M(3)(v=>v**3)(v=>v*3)(v=>v+19)(Math.sqrt)(v => v-4)(ret))(v=>v*7)(ret)
M(6)(v=>v*7)(ret)`;

</script>
<style></style>


<svelte:head>
	<title>A Different Kind of JavaScript Monad</title>
</svelte:head>
<br />
<div style="font-family: Times New Roman; text-align:center; font-size: 32px;" transition:fade>
	<br />

A Different Kind of JavaScript Monad
</div>
<br />

<p>It's unfortunate, I think, that many potential readers, and some who have gotten this far, will miss out on knowing and understanding what follows on the basis of their jumping to the incorrect conclusion that I don't know the meaning of "JavaScript monad." I know what Category theory monads are, and I have worked rather extensively with Haskell monads, which were inspired by their Category Theory counterpart.</p>
<p>Many (I suspect almost all) authors, bloggers, and online video presentors who provide definitions of "JavaScript monads" try to constrain JavaScript to be more like Haskell, insisting on pure functions and immutable named values (including procedures). I'm fine with that when it's clear that they are proposing possible definitions. I'll be disappointed if my proposed definition of a monad as an m-M(x) closure (where x can be any value and M is defined below) is rejected on grounds that it doesn't fit what some coders have been misled into thinking only the Haskell-like monads are valid. </p>
<p>Basic m-M(x) closures include myriad possible closures that deftly facilitate the composition of functions on encapsulated data. In this presentation, they range from x being a primitive value to x being an eight-member array representing the state of gameplay in<a href='../score'>The Solitaire Game of Score</a>. Here are the general definitions of "M" and "m": </p>
<pre>{M}</pre>
<p>As is apparent in the definition, m is the function "go" returned by M. Its arguments are functions that operate on the value held in the m-M(x) closure.</p> <p>The following code demonstrates three things: (1) A monad can be defined without specifying a value, as in m = M(), (2) A value, for example 7, can be inserted with the function "()=>7", and (3) these monads don't mutate, or attempt to mutate, the values they receive, as in c = const 2, ()=>c below. </p>
<pre>{nul}</pre>
<p>The console entries are:</p>
<pre>{entry1}</pre>

<p>The function "()=>2" inserted the number 2 in the closure.</p>

<h2>Stand-alone M can facilitate anonymous function composition.</h2>
<pre>{anon}</pre>
<p>Composition doesn't get more concise and transparent than that!</p>

<p>The "ret" flag can appear anywhere in a computution, not just at the end. Here's an example:</p>
<pre>{retDemo}</pre>
<p>The last line (above) shows M(3) followed by five functions and dev. That is followed by (v=>v*7) and dev again. That expression <span class="pre"> M(3)(v=>v**3)(v=>v*3)(v=>v+19)(Math.sqrt)(v=>v-4)(ret)</span> resolves to the number 6, so <span class="pre"> M(M(3)(v=>v**3)(v=>v*3)(v=>v+19)(Math.sqrt)(v => v-4)(ret))(ret)</span> has the same effect as M(6)(ret) which has the same effect on the final outcome as the number 6, establishing the equivalence of the following two expressions:</p>
<pre>{retDemo2}</pre>

<p>I test the code displayed on these pages in the Firefox browser's Web Developer Tools. The screen (see below) loads when I press F12. I'm working in NewbornOS, which is based on Arch Linux. More information is available at <a href="https://firefox-dev.tools/">Developer Tools</a> The screenshot below shows the Developer Tools console as it appeared when I tested a function named "fib". There's more about that on the <a href="../arrays">arrays page</a>.</p>

<img src = {img2} style="width:1300px;height:800px;padding-left=0px" alt = "image" />

<p>That's just about all for this page. Click <a href="../interactive demos">interactive demos</a> to see some simple interactive demonstrations. The solitaire simulated dice game of Score, in which the "x" in M(x) is an eight member array, is the most complicated interactive demo. Here's a link: <a href="../score">Score</a> </p>
