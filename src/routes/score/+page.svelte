

<script>
	// @ts-ignore

	import { merge_ssr_styles } from 'svelte/internal';
	//	import { onMount } from "svelte";
	import { fade } from 'svelte/transition';
	// import Index from "./index.svelte";
	import { top } from '../stores.js';
	import { userName } from '../stores.js';
    var m3 = M(3);
    var s = ret; 
	console.log('top is', top);

var m2 = M(32);	
var m0 = M([]);
		m2 = M(m2(s));
function nav2 () {
	let n = m2(ret)[5];
	m2(ar => m0(ret).slice(-n)[0])
	update();
	sfunc();
	return m2;
}
var QQ;
$: QQ = m2(ret)[6];

function back () {
	if (ar3.length < 3) return;
	var o = ar3.pop();
	m2(ar => o);
	update();
	sfunc();
	return m2;
}

function splash (a) {
    m2 = M(a);
	// console.log("In splash @@@ m2(ret) is",m0(ret).join(", "));
    update();
    sfunc();
}

 /*   m0(ar => ar.concat(clone([m2(ret)])));
	m2(v => [[1,2,3,4], [], ["+"], [], [0], [], [0], []]);
    m0(ar => ar.concat(clone([m2(ret)])));
	m2(v => [[0,7,0,7], [], ["+"], [], [0], [], [0], []]);
    m0(ar => ar.concat(clone([m2(ret)]))); */
console.log("**********************************************");
console.log("At the top. m0(ret) is", m0(ret));
console.log("**********************************************");

	var PIN, WINNERS;
	var WIN = 1000.0;
	var FIN = 1001.0;
	var FINAL;
	var millisec = 0;
	var seconds = 0;
	var timer;
	var d2;
	var startStop = 'Start';
	var value;
	var d2 = '';
	var A,
		B,
		C,
		D,
		AA,
		BB,
		CC,
		DD,
		EE,
		FF,
		GG,
		HH = 'wait';
	var N = 0;
	var l = console.log;
	var b0 = 'none';
	var b1 = 'none';
	var b2 = 'none';
	var b3 = 'none';
	var index;
	var b4 = 'none';
	var b5 = 'none';
	var b6 = 'none';
	var b7 = 'none';
	var s = ret;
	var AA;
	var BB;
	var CC;
	var DD;
	var EEE = 'awaiting selection';
	var FF;
	var WW;
	var XX;
	var YY;
	var ZZ;
	var SCORE;
	$: SCORE = [0];
	var ZYXW;
	var WXYZ;

	var zeros = () => {
		var arr2 = [
			[0,0,0,0],
			[],
			['+'],
			[],
			[0],
			[],
			0,
			[]
		]};

function ret () {};

function M (x) {
    return function go (func) {
        if (func === ret) return x
        else x = func(x);
        return go;
  }
}

	var runRoller = (b = 0) => {
		var arr2 = [
			[0,0,0,0],
			[],
			['+'],
			[],
			[b],
			[],
			0,
			[]
		];
		m2 = M(arr2);
		updateRoll(m2);
		resettimer();
		resettimer();
	};

	var runRoll;
	runRoll = (b) => {
		var arr = [
			[
				Math.floor(Math.random() * 6) + 1,
				Math.floor(Math.random() * 6) + 1,
				Math.floor(Math.random() * 12) + 1,
				Math.floor(Math.random() * 20) + 1
			],
			[],
			['+'],
			[],
			[b],
			[1],
			1,
			[]
		];
		QQ = 1;
		m2(a => arr);
		ar3 = [clone(arr),clone(arr), clone(arr)];
		EEE = 'yet to be selected';
		updateRoll(m2);
		// m2(fu);
		if (tog) display();
	    console.log("In runRoll. m0(ret) is", m0(ret));
		return m2;
	};
	var Z = '';
	$: Z;
	var x;
	function updateRoll(m) {
		console.log('In updateRoll. m(s) is', m(s));
		AA = m(s)[0][0];
		BB = m(s)[0][1];
		CC = m(s)[0][2];
		DD = m(s)[0][3];

		WW = m(s)[1][0];
		XX = m(s)[1][1];
		YY = m(s)[1][2];
		ZZ = m(s)[1][3];
		EE = m(s)[2];
		FF = m(s)[3];
		SCORE = m(s)[4];
		b0 = b1 = b2 = b3 = 'inline';
		b4 = b5 = b6 = b7 = 'none';
	}
	function sfunc() {
		b0 = b1 = b2 = b3 = b4 = b5 = b6 = b7 = 'none';
		if (AA != (undefined && 0)) b0 = 'inline';
		if (BB != (undefined && 0)) b1 = 'inline';
		if (CC != (undefined && 0)) b2 = 'inline';
		if (DD != (undefined && 0)) b3 = 'inline';
		if (WW != (undefined && 0)) b4 = 'inline';
		if (XX != (undefined && 0)) b5 = 'inline';
		if (YY != (undefined && 0)) b6 = 'inline';
		if (ZZ != (undefined && 0)) b7 = 'inline';
	}

	var update = function update() {
		AA = m2(s)[0][0];
		BB = m2(s)[0][1];
		CC = m2(s)[0][2];
		DD = m2(s)[0][3];
		EE = m2(s)[2];
		FF = m2(s)[3];
		SCORE = m2(s)[4];
		WW = m2(s)[1][0];
		XX = m2(s)[1][1];
		YY = m2(s)[1][2];
		ZZ = m2(s)[1][3];
	};
/*
	$: AA = m2(s)[0][0];
	$: BB = m2(s)[0][1];
	$: CC = m2(s)[0][2];
	$: DD = m2(s)[0][3];
	$: EE = m2(s)[2];
	$: FF = m2(s)[3];
	$: SCORE = m2(s)[4];
	$: WW = m2(s)[1][0];
	$: XX = m2(s)[1][1];
	$: YY = m2(s)[1][2];
	$: ZZ = m2(s)[1][3];    */

	var ZWIN = '';
	var mon3 = M([1, 2, 3, 4]);

	function calc(aa, bb, c) {
		var a = parseInt(aa, 10);
		var b = parseInt(bb, 10);
		if (c === '+') return a + b;
		else if (c === '*') return a * b;
		else if (c === '-') return a - b;
		else if (c === '/') return a / b;
		else if (c === '@') return ' ' + a + b;
		else return 'fubar';
	}

	function g(ar) {
		var x = ar.pop() ** 3;
		ar.unshift(x);
		return ar;
	}

	function g2(ar) {
		return ar.flatMap((v) => (v + 1) ** 3);
	}
	function g3(ar) {
		return ar.flatMap((v) => Math.round(v ** (1 / 3)));
	}

	function clone(x) {
		return JSON.parse(JSON.stringify(x));
	}

	function test() {
        console.log("m2(ret)is", m2(ret));
        console.log("ar3 is", ar3);
	}

	var ar3;
	$: ar3 = [];
	$: ar3.length;
	
	function fu(a) {
		var result;
		var a1;

		if (a[1].length === 2 && a[2].length === 1) {
			a1 = a[1];
			result = calc(a[1][0], a[1][1], a[2][0]);
			a[0].push(result);
			a[3].push(result);
			a[1] = [];
			a[5][0] += 1;
			a[6] += 1;
			m2(v => a);
		}

		if (a[1].length === 3) {
			a[0].push(a[1].pop());
		}

		if (result == 20 && intersection(a1, a[3]).length > 0) {
			if (a[4][0] == 2) {
				resettimer();
				PIN = FIN;
				if (FIN < WIN) WIN = FIN;
				ZWIN = 'You win! Your score is ';
				WINNERS = WIN;
				top.set([WIN]);
				setTimeout(() => runRoller(),4000);
				// setTimeout(() => a[4][0] = 0,8000);
			} else {
				var aint = parseInt(a[4], 10);
				aint += 1;
				Z = '           Your score increased to ' + aint;
				runRoll(aint);
			}
			setTimeout(() => (Z = ZWIN = ''), 8000);
		}
		ar3.push(clone(a));
		ar3 = ar3;
		update();
		sfunc();
		return m2(s);
	}

	var fmon = (f) => (x) => x(f);
	var reset = (x) => [1, 2, 3, 4];

	var click0 = (a) => {
		a[1].push(a[0][0]);
		a[0].shift();
		m2 = M(a);
		m2(fu);
		// sfunc();
	};

	/* var click0 = a => {
    a[1].push(a[0].splice(0,1)[0]);
    m2 = M(a);

}; */

	var click1 = (a) => {
		a[1].push(a[0].splice(1, 1)[0]);
		m2 = M(a);
		m2 = m2(fu);
	};

	var click2 = (a) => {
		a[1].push(a[0].splice(2, 1)[0]);
		m2 = M(a);
		m2 = m2(fu);
	};

	var click3 = (a) => {
		a[1].push(a[0].splice(3, 1)[0]);
		m2 = M(a);
		m2 = m2(fu);
	};

	function clic0(m) {
		EEE = 'add';
		m[2] = '+';
		m2 = M(m);
	}

	$: clic1 = (m) => {
		EEE = 'subtract';
		m[2] = '-';
		m2 = M(m);
	};

	function clic2(m) {
		EEE = 'multiply';
		m[2] = '*';
		m2 = M(m);
	}

	function clic3(m) {
		EEE = 'divide';
		m[2] = '/';
		m2 = M(m);
	}

	function clic4(m) {
		EEE = 'concat';
		m[2] = '@';
		m2 = M(m);
	}

	$: Z = Z;

	var m4 = M(3.1415926535);
	var cube = (x) => x ** 3;
	var pow = n => x => x**n;
	var square = x => x*x; 
	var add = (n) => (x) => 1 * x + 1 * n;
	var mult = (n) => (x) => x * n;
	var reset2 = (n) => (x) => (x = n);

	function squareFu() {
		m4 = m4(square);
	}
	function cubeFu() {
		m4 = m4(cube);
	}

	function divFraction(x) {
		var y = x.split('/');
		if (y.length > 1) {
			return y[0] / y[1];
		} else {
			return y[0];
		}
	}
	var powFu = function powFu(e) {
		var p = divFraction(e.target.value);
		if (e.keyCode == 13) {
			m4 = m4(pow(p));
		}
	};

	var addFu = function addFu(e) {
		if (e.keyCode == 13) {
			m4 = m4(add(e.target.value));
		}
	};

	var multFu = function multFu(e) {
		if (e.keyCode == 13) {
			m4 = m4(mult(divFraction(e.target.value)));
		}
	};

	var resetFu = function resetFu(e) {
		if (e.keyCode == 13) {
			m4 = m4(reset2(divFraction(e.target.value)));
		}
	};

	function intersection(a, b) {
		return a.filter((x) => b.includes(x));
	}

	$: XO = m2(s);

	var tog = true;

	var display = function display() {
		tog = false;
		if (millisec >= 9) {
			millisec = 0;
			seconds += 1;
		} else millisec += 1;
		d2 = seconds + '.' + millisec;
		timer = setTimeout(() => display(), 100);
	};

	function starttimer() {
		if (timer > 0) {
			return;
		}
		display();
	}
	function stoptimer() {
		clearTimeout(timer);
		timer = 0;
	}

	function startstoptimer() {
		if (startStop === 'Start') startStop = 'Stop';
		else startStop = 'Start';
		if (timer > 0) {
			clearTimeout(timer);
			timer = 0;
		} else {
			display();
		}
	}

	function resettimer() {
		clearTimeout(timer);
		FIN = d2;
		var temp = m2(s);
		temp[4] = [0];
		m2 = M(temp);
		millisec = 0;
		seconds = 0;
		d2 = seconds + '.' + millisec;
		tog = true;
	}

	var fuDem = `function fu (a) {                                    // fu
  a[5].push(clone(a));
  a[7].push(clone(a)); // All game states for use in "Back" and "Forward."
  a[6][0] += 1;
    // a[1].push(a[0].pop());
  var result;
  SCORE = a[4];
  var a1;
  if (a[1].length === 2 && a[2].length === 1)   {
    a1 = a[1];
    result = calc(a[1][0], a[1][1],a[2][0]);
    a[0].push(result);
    a[3].push(result);
    a[1] = [];
    m2 = M(a);
  }

  if (a[1].length === 3) {
    a[0].push(a[1].pop());
  }

  if (result == 20 && intersection(a1, a[3]).length > 0) {
      if (SCORE === 4) {
          ZWIN = "You win! "
          a[4][0] = 0;
          runRoll(0);
      }
      else {
          var aint = parseInt(a[4][0], 10);
          aint += 1;
          Z = "           Your score increased to " + aint;
          runRoll(aint);
      }
      setTimeout(() => Z = ZWIN = "", 3000);
  }
  update();
  sfunc();
  return m2(s);
};

var update = () => { // The button displays will correspond to the values in m2.
  AA = m2(s)[0][0];
  BB = m2(s)[0][1];
  CC = m2(s)[0][2];
  DD = m2(s)[0][3];
  EE = m2(s)[2];
  FF = m2(s)[3];
  SCORE = m2(s)[4];
  WW = m2(s)[1][0];
  XX = m2(s)[1][1];
  YY = m2(s)[1][2];
  ZZ = m2(s)[1][3];
}

function sfunc () {
    b0 = b1 = b2 = b3 = b4 = b5 = b6 = b7 = "none"; // All button displays controlled by b's disappear.
    if (AA != (undefined && 0)) b0 = "inline"; // Next, selected buttons are diplayed.
    if (BB != (undefined && 0)) b1 = "inline";
    if (CC != (undefined && 0)) b2 = "inline";
    if (DD != (undefined && 0)) b3 = "inline";
    if (WW != (undefined && 0)) b4 = "inline";
    if (XX != (undefined && 0)) b5 = "inline";
    if (YY != (undefined && 0)) b6 = "inline";
    if (ZZ != (undefined && 0)) b7 = "inline";
}`;


var monad = `function M (x) {
    return function go (func) {
        if (func === ret) return x
        else x = func(x);
        return go;
  }
}`;

var retCode = `function ret () {}`

var monad3 = `var mon3 = M([1,2,3,4]);
    function g(ar) {
        var x = (ar.pop())**3;
        ar.unshift(x);
        return ar;
};
function g2 (ar) {return (ar.flatMap(v => (v+1)**3))};
function g3 (ar) {return (ar.flatMap(v => Math.round(v**(1/3))))};`;

	var simple = `var s = 'stop';
var m4 = M(3);   // creates a new monad named "m4".
var cube = x => x**3;
var square = x => x*x;
var pow = n => x => x**n;
var add = n => x => 1*x + 1*n;
var mult = n => x => x * n;
var reset2 = n => x => x = n;`;

	var runR = `runRoll = x => {
    m2 = M([ [Math.floor(Math.random()*6) + 1, Math.floor(Math.random()*6) + 1, Math.floor(Math.random()*12) + 1, Math.floor(Math.random()*20) + 1], [], [], [], [x] ]);
    updateRoll();
    EEE = "yet to be selected";
    XO = m2('stop');
    AR = [];
    index = 0;
}

const updateRoll = () => {
  AA = m2(s)[0][0];
  BB = m2(s)[0][1];
  CC = m2(s)[0][2];
  DD = m2(s)[0][3];

  WW = m2(s)[1][0];
  XX = m2(s)[1][1];
  YY = m2(s)[1][2];
  ZZ = m2(s)[1][3];
  EE = m2(s)[2];
  FF = m2(s)[3];
  SCORE = m2(s)[4];
  b0 = b1 = b2 = b3 = "inline";
  b4 = b5 = b6 = b7 = 'none';
};`;

	var clickFuncs = `var click0 = a => {
    a[1].push(a[0][0])
    a[0].shift();
    m2 = M(a);
    m2(fu);
    // sfunc();
};

var click1 = a => {
    a[1].push(a[0].splice(1,1)[0]);
    m2 = M(a);
    m2 = m2(fu);
};

var click2 = a => {
    a[1].push(a[0].splice(2,1)[0]);
    m2 = M(a);
    m2 = m2(fu);
};

var click3 = a => {
    a[1].push(a[0].splice(3,1)[0]);
    m2 = M(a);
    m2 = m2(fu);
};

function clic0 (m) {
  EEE = "add";
  m[2] = "+";
  m2 = M(m) ;
}

$: clic1 = m => {
  EEE = "subtract";
  m[2] = "-";
  m2 = M(m) ;
}

function clic2 (m) {
  EEE = "multiply";
  m[2] = "*";
  m2 = M(m) ;
}

function clic3 (m) {
  EEE = "divide";
  m[2] = "/";
  m2 = M(m) ;
}

function clic4 (m) {
  EEE = "concat";
  m[2] = "@"
  m2 = M(m);
};`;

	var putBack = `if (a[1].length === 3) {
    a[0].push(a[1].pop());  // Returns a clicked third number.
  };`;

	var fuFuncs = `function squareFu () {m4 = m4(square)};
function cubeFu () {m4 = m4(cube)};

function divFraction (x) {
    var y = x.split('/');
    if(y.length > 1){
        return (y[0] / y[1])
    }
    else{
        return y[0];
    }
}

var powFu = function powFu (e) {
    var p = divFraction(e.target.value);
    if (e.keyCode == 13) {
        m4 = m4(pow(p));
    }
};

var addFu = function addFu (e) {
    if (e.keyCode == 13) {
        m4 = m4(add(e.target.value));
    };
  };

var multFu = function multFu (e) {
    if (e.keyCode == 13) {
        m4 = m4(mult(divFraction(e.target.value)))};
};

var resetFu = function resetFu (e) {
    if (e.keyCode == 13) {
        m4 = m4(reset2(divFraction(e.target.value)))
    };
};`;

	var example0 = `var mon = M(2); // mon's value is the anonymous function returned by M.     `;

	var example3 = `var mon = M(2);
mon(v=>v**4)(v=>v+5)(v=>v*2);`;
	// The value of x can be obtained later
	var example4 = `mon(ret);  // 42
mon(v => v*v);`;
	// And later:
	var example5 = `mon(ret);  // 1764`;

	var oldMonad = `function M (x) {
    return function go (func) {
        if (typeof func === "function") {
            x = func(x);
            return go;
        }
        else if (func === "stop") return x;
    }
};`;

	var buttons = `<button style = "display: {b0}" on:click = {() => m2(click0)}>{AA}</button>
<button style = "display: {b1}" on:click = {() => m2(click1)}>{BB}</button>
<button style = "display: {b2}" on:click = {() => m2(click2)}>{CC}</button>
<button style = "display: {b3}" on:click = {() => m2(click3)}>{DD}</button>

<span style = "margin-left: 8%; font-size: 22px">The operator is {m2(s)[2]}</span>

<br><br>
<button on:click = {() => m2(clic0)}>add</button>
<button on:click = {() => m2(clic1)}>subtract</button>
<button on:click = {() => m2(clic2)}>multiply</button>
<button on:click = {() => m2(clic3)}>divide</button>
<button on:click = {() => m2(clic4)}>concat</button>
`;
	var backDem = `back = a => {
    if (a[5].length < 1) {
      m2 = M(a);
      console.log("You're already all the way back")
      return;
    }
    else {
        var b = a[5][a[5].length - 1];
        b[7] = a[7];
        m2 = M(b);
        update();
        sfunc();
    }
};

var forward;
$: forward = a => {
    var index = a[6][0];
    if (a[5].length === a[7].length) {
        console.log("Already at the top");
        m2 = M(a);
        return;
    }
    else {
        var b = a[7][index + 1];
        b[7] = a[7];
        m2 = M(b);
        update();
        sfunc();
    }
};`;

var example2 = `var m3 = M(3);
var m4 = M(m3(s));
m3(v => v + 3);
m4(v => v + 4);

log("m3(s) * m4(s) is", m3(s) * m4(s))

m3(s) * m4(s) is 42`;

	var example6 = `M(2)(v=>v+1)(v=>v*2)(v=>v*7)(s) // 42`;

	var async = `var asyncMult = a => async b => {
    var d;
    if (!(b instanceof Promise)) return a * b;
    else d = await b;
    return a * d;
}

var asyncAdd = a => async b => {
    var d;
    if (!(b instanceof Promise)) return a + b;
    else d = await b;
    return a + d;
}

m3(asyncAdd(4))(asyncMult(6))(s).then(v => log("The result is", v));  // The result is 42
m3(asyncAdd(8))(asyncMult(2))(s).then(v => log("Now we are at", v));  // Now we are at 100
m3(asyncAdd(-51))(asyncMult(6/7))(s).then(v => log("And back to", v)) // And back to 42 `;

	var bigMonad = `function Comp ( AR = [] )  {
  var f_, p, run;
  var ar = AR.slice();
  var x = ar.pop();
  return run = (function run (x) {
    if (x === null || x === NaN ||
      x === undefined) x = f_('stop').pop();
    if (x instanceof Filt) {
      var z = ar.pop();
      if (x.filt(z)) x = z; else ar = [];
    }
    else if (x instanceof Promise) x.then(y =>
      {if (y != undefined && typeof y !== "boolean"
        && y === y && y.name !== "f_" && y.name !== "stop" ) {
      ar.push(y);
      diffRender()
    }})
    else if (x != undefined && x === x && x !== false
      && x.name !== "f_" && x.name !== "stop" ) {
      ar.push(x);
      diffRender()
    };
    function f_ (func) {
      if (func === 'stop' || func === 'S') return ar;
      else if (func === 'finish' || func === 'F') return Object.freeze(ar);
      else if (typeof func !== "function") p = func;
      else if (x instanceof Promise) p = x.then(v => func(v));
      else p = func(x);
      return run(p);
    };
    return f_;
  })(x)
}`;

	var caution = `var s = ret;
var log = console.log;

function M(x) {
  return function go(func) {
    if (typeof func === "function") {
      x = func(x);
      return go;
    } else if (func === "stop") return x;
  }
};

var m3 = M(3);

m3(async a => await 888); // m3(s) will return a Promise with value 888.

m3(s).then(v => m3((z => v + 112)));
// m3(s) will return 1000 after the promise is fulfilled.

m3(s).then(v => setTimeout(() => console.log("m3(s) resolved is", v,), 2000));
// The promise is still pending, so the value of "v" is 888.

setTimeout(() => console.log("m3(s) is", m3(s)),0);
// This gets bumped to the bottom of the stack, behind (2).
// m3(s) is called after x has been updated to 1000.

// Result:
16:13:15.590 m3(s) is 1000
16:13:17.590 m3(s) resolved is 888
// Two seconds after "1000" appears in the console log, "888" is displayed.`;


var start = `m2 = M(
    [ 
      [Math.floor(Math.random() * 6) + 1, Math.floor(Math.random() * 6) + 1,
      Math.floor(Math.random() * 12) + 1, Math.floor(Math.random() * 20) + 1], 
      [], ['+'], [], [0], [], [0], [] 
    ]);`



setTimeout(() => splash( [[1,,,], [], ["+"], [], [0], [], [0], []] ),500);
setTimeout(() => splash( [[0,,,], [], ["+"], [], [0], [], [0], []] ),1000);
setTimeout(() => splash( [[0,0,0,0], [], ["+"], [], [0], [], [0], []] ),1500);
/*  setTimeout(() => splash( [[4,4,4,4], [], ["+"], [], [0], [], [0], []] ),1500);
setTimeout(() => splash( [[3,3,3,3], [], ["+"], [], [0], [], [0], []] ),2000);
setTimeout(() => splash( [[2,2,2,2], [], ["+"], [], [0], [], [0], []] ),2500);
setTimeout(() => splash( [[1,1,1,1], [], ["+"], [], [0], [], [0], []] ),3000);
setTimeout(() => splash( [[0,0,0,0], [], ["+"], [], [0], [], [0], []] ),3500);
setTimeout(() => splash( [[8,8,8,8], [], ["+"], [], [0], [], [0], []] ),4000);
setTimeout(() => splash( [[0,0,0,0], [], ["+"], [], [0], [], [0], []] ),4500);  */


</script>

<style>
	pre {margin-left: 3%;}
</style>

<svelte:head>
	<title>The Solitaire Game of Score</title>
</svelte:head>
<br />
<div style="font-family: Times New Roman; text-align:center; font-size: 32px;" transition:fade>
	<br />

	The State of Score Maintained in a Recursive Closure
</div>
<br />
<p> The game is held in the recursive closure returned initially by M(x) where M is: </p>
<pre>{monad}</pre>
<p>and x is an array of eight arrays initially defined as:</p>
<pre>{start}</pre>
<p>It doesn't matter that ret() returns "undefined", without the quotation marks, because it doesn't get called. It's only purpose is to cause go(), the function returned by M, to return the current value of x held in the m = M(x) closure. M can also be used anonymously to chain functions as in <span style="color: #55ffff">M(2)(v=>v+4)(v=>v*7)(ret) = 42</span>. </p>

<p>Here, ret() is defined as  <span style="color: #55ffff">{retCode}</span>. Explanations of how M(x) works are below the game interface (below).
	 </p>
<p>Your score will be the elapsed time after three rounds. A round is completed by computing the number 20 in two or three steps. For example, if your numbers are 1,3,4,20, you can complete the round in two steps with 4-3 and then 1 * 20. You'll have two 1's before the multiplication. It won't matter which one you use. If your first computation is 1 * 20, your numbers will be 3,4,20. You can still subtract 3 from 4 and multiply by 1, finishing in three steps instead of two. </p>
<!-- <h1>{$userName}</h1> -->
<br />
<span>Best Score: {$top} </span>
<h2>{d2}</h2>
<!-- <button on:click={display}>Start</button>
<button on:click={stoptimer}>Stop</button> -->
<br />

<button on:click={runRoller}>Reset</button>
<br /><br />
<button style="display: {b0}" on:click={() => m2(click0)}>{AA}</button>
<button style="display: {b1}" on:click={() => m2(click1)}>{BB}</button>
<button style="display: {b2}" on:click={() => m2(click2)}>{CC}</button>
<button style="display: {b3}" on:click={() => m2(click3)}>{DD}</button>
<span style="margin-left: 8%; font-size: 32px">Operator: {m2(s)[2]}</span>
<span style="margin-left: 64px; font-size: 32px">Score: {m2(s)[4]}</span>

<br /><br />
<button on:click={() => m2(clic0)}>add</button>
<button on:click={() => m2(clic1)}>subtract</button>
<button on:click={() => m2(clic2)}>multiply</button>
<button on:click={() => m2(clic3)}>divide</button>
<button on:click={() => m2(clic4)}>concat</button>

<span style="margin-left: 20px; color:#bbbbff; font-size:28px">{Z}</span>
<span style="margin-left: 20px; color:#bbbbff; font-size:38px">{ZWIN}</span>
<span style="margin-left: 20px; color:#bbbbff; font-size:38px">{FIN}</span>

<br /><br />
<button on:click={() => runRoll(m2(s)[4][0])}>ROLL</button>
<br /><br />

<button on:click={() => test()}>test</button>
<button style="display: {b4}">{WW}</button>
<button style="display: {b5}">{XX}</button>
<button style="display: {b6}">{YY}</button>
<button style="display: {b7}">{ZZ}</button>
<br /><br />
<button on:click={back}>Back</button>
<h3>{QQ}</h3>
<p>
	Remember, just computing 20 isn't always enough. One of the numbers used to get 20 has to be the
	result of a prior computation
</p>
<p>
	<h2>Background</h2>
	<p>Score is a game involving four dice and two or three-stage arithmetic computations with the goal of arriving at the number 20. My son Alex taught it to me a decade ago, when he was in middle school. I decided to make an online multi-player version. </p>
	<p> After some messy experiences developing a server with other	programming languages, I turned to Haskell for the robust and easily maintainable backend that carried me through several experiments with various front ends. The server can handle a large number of 	number of groups of interacting players. Each group has its own chat box and shared todo list, and all members always see the same dice roll as it gets whittled down by players selecting numbers. </p>
	<p> One of my fondest memories began with Alex asking me to to devise a way to display all solutions to a dice roll or else report that no solution exists. My initial impression was that an algorithm that could so that would be unreasonably complicated and resource intensive. But not long afterward, I was delighted -- maybe "euphoric" is the right word -- as I showed Alex a button on the player interface that would abort gameplay and display every way to get 20 in two or three steps. It even broke the solutions down into categories. My appreciation of the Haskell programming language continued to grow.</p>
	<p> In the online game, players can gain a point by	clicking "Impossible" unless another player finds a solution. In that case, the player who clicked "Impossible" loses a point. Players can change the default number of dice sides from 6,6,12,and 20 and the goal from the default
	value of 20. A drag and drop version of Score is online at <a href="https://score.schalk2.com"
		>https://score.schalk2.com</a
	>.
</p>
<h2>About this Solitaire Version</h2>

<p>
	This demonstration doesn't rely on a remote server, nor does it feature any Haskell code. It's
	just a little solitaire game providing an opportunity to consider the interesting possibilities of
	recursive closures. You can traverse the history of game play for the current roll. If you make a
	mistake, you can take back your move and do something else. If you traverse back and forth very
	far, subsequent computations will be very slow and the program might even crash. If you just take back a move, computations proceed normally.
</p>
<p>
	The function fu() is the brains behing the game of Score. Each time a number or operator is
	clicked, m2(fu) is called, the monad m2 is modified, and the change is reflected in the DOM. The
	state of play in M is an array of seven arrays. Let's call it ar. If an operator op is in ar[2]
	and two numbers a and b are in ar[1], fu calls calc(a,b,op) and the result is added to ar[0] and
	ar[3]. ar[0] are the numbers in the game interface. ar[3] hold numbers that have been computed. At
	least one of the numbers in ar[3] has to be used to compute 20 in order to gain a point. If the
	number of points reaches 5, fu causes "You win" to be displayed, sets the score back to 0, and
	calls runRoll, starting another round of play.
</p>
<p>
	At the end of fu(), two formatting functions are Called. The first, update(), refreshes the game
	buttons, causing them to reflect the current state of ar. The second hides buttons that correspond
	to values of undefine and shows buttons that correspond to numbers in ar. This is done by
	switching variables p in "style = 'display: p' back and forth between "none" and "inline".
</p>
<pre>{fuDem}</pre>

<p>Clicking "ROLL" calls runRoll() which, in turn, calls updateRoll() to re-set HTML variables.</p>
<pre>{runR}</pre>
<p>
	The "x = [ [], [], [], [], [0], [], [0], [] ]" format will be maintained throught game play. x[0]
	simulates the dice roll; x[1] recieves integers that are clicked; x[2] holds the operator; and
	x[4] contains numbers that are computed. x[4] makes sure at least one computed number is involved
	in arriving at 20. That's the reason, toward the end of fu(), that the intersection of a[0] and
	a[4] is examined when 20 is computed. Here are the first few functions called when a number is
	clicked:
</p>
<pre>{clickFuncs}</pre>
<p>
	The first line of fu() is the calculation result that is generated whenever there are two items in
	(s)[1] and an operator in m2(s)[3]. The intersection is important in fu()'s bottom test. If
	"intersect", the intersection of m2(s)[1] and m2(s)[3], is empty intersect[0] returns false and
	the last test in fu fails, even though 20 was produced on the second computation.
</p>
<p>
	If no operator has been selected, it's possible to click a third number. The program doesn't
	complain, it just puts the number back for you with:
</p>
<pre>{putBack}</pre>
<p>
	If you roll the dice and keep clicking on the leftmost number, you'll see the numbers shift back
	and forth on every try. The first element of m2(s)[0] keeps getting pulled out of the first
	position and pushed back on the right.
</p>
<p>
	sfunc() does some more DOM housekeeping. The buttons with dice number come and go as their CSS
	display strings are changed back and forth between "none" and "inline". fu() calls sfunc(). Here's
	how it is defined:
</p>

<p>
	For solitaire version presented here, a function named "m2" will will form a closure with M as
	follows: "m2 = M(x)" where x = [ [], [], [], [], [0], [], [0], [] ]. m2 will consume functions
	that, as the definition of M specifies, operate on x inside of M. x corresponds to the state of
	game play. After each click on a number or operator buttom, m2(fu) is called. The record of prior
	states kept in x[7] allows players to traverse the history of their choices.
</p>

<p>
	In the solitaire version of the game of score, x in M(x) is, as mentioned above, the array of
	arrays [ [], [], [], [], [], [], [], [], [] ] where x[0] starts out as four integers simulating a
	throw of two six-sided, one twelve-sided, and one twenty-sided dice. x[1] and x[3] contain the
	number selected by the player, x[2] is the selected operator, and x[4] keeps track of the number
	of successes until the player wins by reaching 5, x[5] contains all prior states as the player
	selects numbers and operators and is used for reversing state a little or all the way back to the
	original roll. x[6] is an index of where in x[5] play is taking place, and x[7] contains every
	state during a round. using x[6] to travers the history of game play in both directions.
</p>

<!-- <button on:click = {m2Func}>m2Func</button>
<button on:click = {update}>Update</button>
<button on:click = {() => m2(fu)}>m2(fu)</button>
<button on:click = {sfunc}>sfunc</button>
-->

<h2>Why I Call Them "Monads"</h2>

<p>
	I call functions returned by M "monads", much to the consternation of some "functional
	programmers" who scoff at the idea that JavaScript could possibly have monads such as those
	defined in the Haskell programming language. Neither my monads nor the Haskell monads are Category
	Theory monads. Haskell monads insulate chained computation from the global space, consuming
	functions that return new Monads. Mine happen to do the same thing. Haskell monads need to
	navegate through various types but I don't bother with that. The definition of "M" shows that the
	returned function responds to arguments that are functions and also to the string "Stop."
</p>

<p>
	In my opinion, trying to define JavaScript objects that resemble the basic monads found in the
	Haskell Prelude module, amusing though it may be, isn't likely to produce anything very useful.
	People who think Haskell, or the supposed mathematical category of Haskell types and functions
	called "Hask", are actually Category Theory categories are mistaken. Category Theory inspired the
	development of Haskell monads and it might not be merely coincidental that the monads I am about
	to define are functionally similar to Haskell monads, though superficially quite different. Both
	transform state along pipelines isolated from their outer scope by operating on functions that
	return new monads. Both preserve state for future transformations or for eventual use in their
	outer scopes. Mine call functions in their outer scopes in order to update the DOM, not having to
	wait to do it in a main() function. I'm not trying to mimic Haskell or any other functional
	programming language.
</p>

Caution:
<pre>{caution}</pre>
<br /><br />

<!-- <style>
	 (A) CONTAINER
#stopwatch {
  display: flex;
  flex-wrap: wrap;
  max-width: 320px;
  margin: 0 auto;
}

#sw-time {
  width: 100%;
  padding: 20px 0;
  font-size: 48px;
  font-weight: bold;
  text-align: center;
  background: #000;
  color: #fff;
}

#sw-rst, #sw-go {
  box-sizing: border-box;
  width: 50%;
  cursor: pointer;
  padding: 20px 0;
  border: 0;
  color: #fff;
  font-size: 20px;
}
#sw-rst { background-color: #a32208; }
#sw-go { background-color: #20a308; }


</style> -->

<slot></slot>
