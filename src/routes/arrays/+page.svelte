

<script>

import { fade } from 'svelte/transition';
import img4 from "$lib/array_screenshot4.png";

const M = `const log = console.log;
const ret = function ret () {};

function M (x = null) {
	return function go (func) {
		if (func === ret) return x;
		else x = func(x);
		return go;
	}
}`

var M2Def = `function M2 (x = []) {
    return function go (func) {
        if (func === ret) return x[x.length - 1];
        else if (func === arr) return x;
        else x.push(func(x[x.length - 1]));
        return go;
    }
}
const ma = M2([3]);
ma(v=>v**3)(v=>v+v)(v=>v+46);

ma(arr);  // [ 3, 27, 54, 100 ]
ma(ret);  // 100`;

var M3Def = `function M3 (x = []) {
    return function go (func) {
        if (func === ret) return x[x.length - 1];
        else if (func === arr) return x;
        else x = func(x);
        return go;
    }
};`;

var M3_0 = `const mb = M3([0,1]);
mb(fib(9))(ret);  // 21
mb(arr);  // [ 0, 1, 1, 2, 3, 5, 8, 13, 21 ]`;

var fib = `const m2 = M([0,1]);

const fib = n => x => {
    var k = 3;
    while (k <= n) {
        x = [...x, x[x.length - 1] + x[x.length - 2]];
        k+=1;
    }
    return x;
}

m2(fib(10))(ret) // [ 0, 1, 1, 2, 3, 5, 8, 13, 21, 34 ]);`


var M3_1 = `mb(fib(3))(ret);   // 34`;
var M3_2 = `mb(fib(25))(ret); // 2178309`; 

var eval1 = `var m = M();
m(()=>"z=>Math.sqrt((z[0]**2) + (z[1]**2))")(eval);
m(ret)(([3,4]))  // 5 `

var eval2 = `var m2 = M("(v=>(v**4 + 19)/2 - 8)");
var fu = m2(eval)(ret);
fu(3);  // 42 `;



var code1 = `const ma = MA([3])
ma(v=>v**3)(v=>v+v)(v=>v+46);

log("ma(arr) is", ma(arr));  // [3, 27, 54, 100]
log("ma(ret) is",ma(ret));   // 100`;

</script>

<svelte:head>
	<title>Arrays In Monads</title>
</svelte:head>
<br />
<div style="font-family: Times New Roman; text-align:center; font-size: 32px;" transition:fade>
	<br />

Arrays In Monads
</div>
<br />
<p>Here we examine two variations on the basic m-M(x) closures, both designed for use when x is an array. In the m2-M2(x) closure, x is an array whose values don't change as the return values of func(x[x.length - 1]) are pushed into x after every function m2(func) function call. In the m3-M3 closure, func in m3(func) operates on the entire array x, not just its last element. </p>
    
<p>M2 and M3 are not necessary for composing functions on arrays. The <a href="../score">Solitaire Game of Score</a> uses the basic monad generator M with an 8-member array. Below, Fibonacci numbers are generated inside the basic m-M(x) closure.   
<pre>{M}</pre>
<br>
<pre>{fib}</pre>
<p>The above code uses fib(10), which needs another argument. When m2(fib(10)) executes, the return value of fib(10)(x[x.length - 1]) is appended to the array x.</p>

<p>When a function m2 is created by running m2 = M2(x), x has to be an array. It can return x[x.length - 1] or x depending on whether ret or arr is called. Here's the definition of M2 and an example:    </p>
<pre>{M2Def}</pre>
<br>
<p>As mentioned above, m-M3(x) closures hold arrays that are operated on in their entireties. Here's its definition:</p>
<pre>{M3Def}</pre>
<p>The closure mb-M3 is created and mb(fib(9)) is run as follows:  </p>
<pre>{M3_0}</pre>
<p> Because k in fib starts at 2, mb(fib(3)) will cause one more iteration.</p>
<pre>{M3_1}</pre>
<p>We can extend the series 22 more times as follows:</p>
<pre>{M3_2}</pre>
<br>
<p>Since we're just playing with monads to get a feel for their possibilities, I'll demonstrate how user submitted strings could perform computations in m-M(x) closures. It's a safe bet that this won't be implemented on this site. </p>
<pre>{eval1}</pre>
<p>Or, we could define the closure to hold a function string, rather than null.</p>
<pre>{eval2}</pre>
<p>Here's a screenshot of my tests of a function named "fib" in the Firefox Developer Console. After tweaking to make it full screen, it now comes up like this whenever I press F12. Keybindings are available for Vim, Emacs, and Sublime Text.</p>
<br>

<!-- svelte-ignore a11y-img-redundant-alt -->
<img src = {img4} style="width:1300px;height:800px;padding-left=0px" alt = "image" />

<p></p>