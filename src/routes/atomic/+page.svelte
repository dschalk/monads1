<script>

	// import { merge_ssr_styles } from 'svelte/internal';
	import { fade } from 'svelte/transition';
    
	const M = `function ret () {};  // Used in M1 (below).

function M (x) {
	return function go (func) {
		if (func === ret) return x;
		else x = func(x);
		return go;
	}
}`
</script>


<svelte:head>
	<title>A Different Kind of JavaScript Monad</title>
</svelte:head>
<br />
<div style="font-family: Times New Roman; text-align:center; font-size: 32px;" transition:fade>
	<br />

Reverting Rather Than Failing
</div>
<br />

