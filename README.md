# js-function-fun
Fun with JavaScript functions

## Functions

<dl>
<dt><a href="#identity">identity(x)</a> ⇒ <code>any</code></dt>
<dd><p>Write a function <code>identity</code> that
takes an argument and returns
that argument</p>
</dd>
<dt><a href="#addBinary">addBinary(a, b)</a> ⇒ <code>number</code></dt>
<dd><p>Write a binary function <code>addBinary</code>
that takes two numbers and returns
their sum</p>
</dd>
<dt><a href="#subBinary">subBinary(a, b)</a> ⇒ <code>number</code></dt>
<dd><p>Write a binary function <code>subBinary</code>
that takes two numbers and returns
their difference</p>
</dd>
<dt><a href="#mulBinary">mulBinary(a, b)</a> ⇒ <code>number</code></dt>
<dd><p>Write a binary function <code>mulBinary</code>
that takes two numbers and returns
their product</p>
</dd>
<dt><a href="#add">add(...nums)</a> ⇒ <code>number</code></dt>
<dd><p>Write a function <code>add</code> that
is generalized for any
amount of arguments</p>
</dd>
<dt><a href="#sub">sub(...nums)</a> ⇒ <code>number</code></dt>
<dd><p>Write a function <code>sub</code> that
is generalized for any
amount of arguments</p>
</dd>
<dt><a href="#mul">mul(...nums)</a> ⇒ <code>number</code></dt>
<dd><p>Write a function <code>mul</code> that
is generalized for any
amount of arguments</p>
</dd>
<dt><a href="#addTail">addTail(...nums)</a> ⇒ <code>number</code></dt>
<dd><p>Write a function <code>addTail</code> that
is the generalized <code>add</code> function
with tail recursion</p>
</dd>
<dt><a href="#mulTail">mulTail(...nums)</a> ⇒ <code>number</code></dt>
<dd><p>Write a function <code>mulTail</code> that
is the generalized <code>mul</code> function
with tail recursion</p>
</dd>
<dt><a href="#acc">acc(funct, start)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>acc</code> that
takes a function and a
starting value and returns
a function that runs the
initial function on each
argument</p>
</dd>
<dt><a href="#accTail">accTail(funct, start)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>accTail</code> that
does what <code>acc</code> does but uses
tail recursion</p>
</dd>
<dt><a href="#identityf">identityf(x)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>identityf</code>
that takes an argument and
returns a function that
returns that argument</p>
</dd>
<dt><a href="#addf">addf(a)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>addf</code> that
adds from two invocations</p>
</dd>
<dt><a href="#liftf">liftf(binary)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>liftf</code> that
takes a binary function, and
makes it callable with two
invocations</p>
</dd>
<dt><a href="#pure">pure(x, y)</a> ⇒ <code>array</code></dt>
<dd><p>Write a <a href="https://en.wikipedia.org/wiki/Pure_function">pure</a> function <code>pure</code> that
is a wrapper arround the impure
function <code>impure</code></p>
<pre>function impure(x) {
  y++;
  z = x * y;
}

var y = 5, z;

impure(20);
z; // 120

impure(25);
z; // 175</pre></dd>
<dt><a href="#curryBinary">curryBinary(binary, a)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>curryBinary</code> that
takes a binary function and
an argument, and returns a
function that can take a
second argument</p>
</dd>
<dt><a href="#curry">curry(func, ...outer)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>curry</code> that
is generalized for any amount
of arguments</p>
</dd>
<dt><a href="#inc">inc(x)</a> ⇒ <code>number</code></dt>
<dd><p>Without writting any new functions,
show multiple ways to create the <code>inc</code>
function</p>
</dd>
<dt><a href="#twiceUnary">twiceUnary(binary)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>twiceUnary</code>
that takes a binary function
and returns a unary function
that passes its argument to
the binary function twice</p>
</dd>
<dt><a href="#doubl">doubl(x)</a> ⇒ <code>number</code></dt>
<dd><p>Use the function <code>twiceUnary</code> to
create the <code>doubl</code> function</p>
</dd>
<dt><a href="#square">square(x)</a> ⇒ <code>number</code></dt>
<dd><p>Use the function <code>twiceUnary</code> to
create the <code>square</code> function</p>
</dd>
<dt><a href="#twice">twice(x)</a> ⇒ <code>any</code></dt>
<dd><p>Write a function <code>twice</code> that
is generalized for any amount
of arguments</p>
</dd>
<dt><a href="#reverseBinary">reverseBinary(binary)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>reverseBinary</code> that
reverses the arguments of a
binary function</p>
</dd>
<dt><a href="#reverse">reverse(func)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>reverse</code> that
is generalized for any amount
of arguments</p>
</dd>
<dt><a href="#composeuTwo">composeuTwo(unary1, unary2)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>composeuTwo</code> that
takes two unary functions and
returns a unary function that
calls them both</p>
</dd>
<dt><a href="#composeu">composeu(...funcs)</a> ⇒ <code>any</code></dt>
<dd><p>Write a function <code>composeu</code> that
is generalized for any amount
of arguments</p>
</dd>
<dt><a href="#composeb">composeb(binary1, func2)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>composeb</code> that
takes two binary functions and
returns a function that calls
them both</p>
</dd>
<dt><a href="#limitBinary">limitBinary(binary, lmt)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>limitBinary</code>
that allows a binary function
to be called a limited number
of times</p>
</dd>
<dt><a href="#limit">limit(func, lmt)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>limit</code> that
is generalized for any amount
of arguments</p>
</dd>
<dt><a href="#genFrom">genFrom(x)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>genFrom</code> that
produces a generator that will
produces a series of values</p>
</dd>
<dt><a href="#genTo">genTo(gen, lmt)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>genTo</code> that
takes a generator and an end
limit, and returns a generator
that will produce numbers up
to that limit</p>
</dd>
<dt><a href="#genFromTo">genFromTo(start, end)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>genFromTo</code> that
produces a generator that will
produce values in a range</p>
</dd>
<dt><a href="#elementGen">elementGen(array, gen)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>elementGen</code> that
takes an array and a generator
and returns a generator that will
produce elements from the array</p>
</dd>
<dt><a href="#element">element(array, gen)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>element</code> that is a
modified <code>elementGen</code> function so that
the generator argument is optional.
If a generator is not provided, then
each of the elements of the array
will be produced.</p>
</dd>
<dt><a href="#collect">collect(gen, array)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>collect</code> that takes a
generator and an array and produces
a function that will collect the results
in the array</p>
</dd>
<dt><a href="#filter">filter(gen, predicate)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>filter</code> that takes a
generator and a predicate and produces
a generator that produces only the
values approved by the predicate</p>
</dd>
<dt><a href="#filterTail">filterTail(gen, predicate)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>filterTail</code> that uses
tail-recursion to perform the filtering</p>
</dd>
<dt><a href="#concatTwo">concatTwo(gen1, gen2)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>concatTwo</code> that takes
two generators and produces a generator
that combines the sequences</p>
</dd>
<dt><a href="#concat">concat(...gens)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>concat</code> that
is generalized for any amount
of arguments</p>
</dd>
<dt><a href="#concatTail">concatTail(...gens)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>concatTail</code> that uses
tail-recursion to perform the concating</p>
</dd>
<dt><a href="#gensymf">gensymf(symbol)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>gensymf</code> that
makes a function that generates
unique symbols</p>
</dd>
<dt><a href="#gensymff">gensymff(unary, seed)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>gensymff</code> that
takes a unary function and a
seed and returns a <code>gensymf</code></p>
</dd>
<dt><a href="#fibonaccif">fibonaccif(first, second)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>fibonaccif</code> that
returns a generator that will
return the next fibonacci number</p>
</dd>
<dt><a href="#counter">counter(i)</a> ⇒ <code>object</code></dt>
<dd><p>Write a function <code>counter</code> that
returns an object containing
two functions that implement
an up/down counter, hiding
the counter</p>
</dd>
<dt><a href="#revocableBinary">revocableBinary(binary)</a> ⇒ <code>object</code></dt>
<dd><p>Write a function <code>revocableBinary</code>
that takes a binary function, and
returns an object containing an
<code>invoke</code> function that can invoke a
function and a <code>revoke</code> function
that disables the <code>invoke</code> function</p>
</dd>
<dt><a href="#revocable">revocable(func)</a> ⇒ <code>object</code></dt>
<dd><p>Write a function <code>revocable</code> that
is generalized for any amount of
arguments</p>
</dd>
<dt><a href="#extract">extract(array, prop)</a> ⇒ <code>array</code></dt>
<dd><p>Write a function <code>extract</code> that
takes an array of objects and an
object property name and converts
each object in the array by
extracting that property</p>
</dd>
<dt><a href="#m">m(value, source)</a> ⇒ <code>object</code></dt>
<dd><p>Write a function <code>m</code> that
takes a value and an
optional source string
and returns them in an
object</p>
</dd>
<dt><a href="#addmTwo">addmTwo(m1, m2)</a> ⇒ <code>object</code></dt>
<dd><p>Write a function <code>addmTwo</code> that
adds two <code>m</code> objects and
returns an <code>m</code> object</p>
</dd>
<dt><a href="#addm">addm(...ms)</a> ⇒ <code>object</code></dt>
<dd><p>Write a function <code>addm</code> that
is generalized for any amount of
arguments</p>
</dd>
<dt><a href="#liftmBinaryM">liftmBinaryM(binary, op)</a> ⇒ <code>object</code></dt>
<dd><p>Write a function <code>liftmBinaryM</code> that
takes a binary function and
a string and returns a function
that acts on <code>m</code> objects</p>
</dd>
<dt><a href="#liftmBinary">liftmBinary(binary, op)</a> ⇒ <code>object</code></dt>
<dd><p>Write a function <code>liftmBinary</code> that
is a modified function <code>liftmBinaryM</code>
that can accept arguments that
are either numbers or m objects</p>
</dd>
<dt><a href="#liftm">liftm(func, op)</a> ⇒ <code>object</code></dt>
<dd><p>Write a function <code>liftm</code> that
is generalized for any amount of
arguments</p>
</dd>
<dt><a href="#exp">exp(value)</a> ⇒ <code>any</code></dt>
<dd><p>Write a function <code>exp</code> that
evaluates simple array
expressions</p>
</dd>
<dt><a href="#expn">expn(value)</a> ⇒ <code>any</code></dt>
<dd><p>Write a function <code>expn</code>
that is a modified <code>exp</code> that
can evaluate nested array
expressions</p>
</dd>
<dt><a href="#addg">addg(value)</a> ⇒ <code>number</code> | <code>undefined</code></dt>
<dd><p>Write a function <code>addg</code> that
adds from many invocations,
until it sees an empty
invocation</p>
</dd>
<dt><a href="#liftg">liftg(binary)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>liftg</code> that
will take a binary function
and apply it to many invocations</p>
</dd>
<dt><a href="#arrayg">arrayg(value)</a> ⇒ <code>array</code></dt>
<dd><p>Write a function <code>arrayg</code> that
will build an array from many
invocations</p>
</dd>
<dt><a href="#continuizeu">continuizeu(unary)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>continuizeu</code>
that takes a unary function
and returns a function that
takes a callback and an
argument</p>
</dd>
<dt><a href="#continuize">continuize(any)</a> ⇒ <code>function</code></dt>
<dd><p>Write a function <code>continuize</code>
that takes a function and
returns a function that
takes a callback and an
argument</p>
</dd>
<dt><a href="#vector">vector()</a></dt>
<dd><p>Make an array wrapper object
with methods <code>get</code>, <code>store</code>,
and <code>append</code>, such that an
attacker cannot get access
to the private array</p>
</dd>
<dt><a href="#exploitVector">exploitVector()</a></dt>
<dd><p>Let&#39;s assume your <code>vector</code>
implementation looks like
something like this:</p>
<pre>function vector() {
  var array = [];
  return {
    append: function append(v) {
      array.push(v);
    },
    get: function get(i) {
      return array[i];
    },
    store: function store(i, v) {
      array[i] = v;
    }
  };
}</pre>

<p>Can you spot any security concerns with
this approach? Mainly, can we get access
to the <code>array</code> outside of <code>vector</code>?
Note<em>: the issue has nothing to do with
prototypes and we can assume that global
prototypes cannot be altered.
Hint</em>: Think about using <code>this</code> in a
method invocation. Can we override a
method of <code>vector</code>?</p>
</dd>
<dt><a href="#vectorSafe">vectorSafe()</a></dt>
<dd><p>How would you rewrite <code>vector</code> to deal
with the issue from above?</p>
</dd>
<dt><a href="#pubsub">pubsub()</a></dt>
<dd><p>Make a function <code>pubsub</code> that
makes a publish/subscribe object.
It will reliably deliver all
publications to all subscribers
in the right order.</p>
</dd>
</dl>

<a name="identity"></a>

## identity(x) ⇒ <code>any</code>
Write a function `identity` that
takes an argument and returns
that argument

**Kind**: global function  

| Param | Type |
| --- | --- |
| x | <code>any</code> |

**Example**  
```js
identity(3) // 3
```
<a name="addBinary"></a>

## addBinary(a, b) ⇒ <code>number</code>
Write a binary function `addBinary`
that takes two numbers and returns
their sum

**Kind**: global function  

| Param | Type |
| --- | --- |
| a | <code>number</code> |
| b | <code>number</code> |

**Example**  
```js
addBinary(3, 4) // 3 + 4 = 7
```
<a name="subBinary"></a>

## subBinary(a, b) ⇒ <code>number</code>
Write a binary function `subBinary`
that takes two numbers and returns
their difference

**Kind**: global function  

| Param | Type |
| --- | --- |
| a | <code>number</code> |
| b | <code>number</code> |

**Example**  
```js
subBinary(3, 4) // 3 - 4 = -1
```
<a name="mulBinary"></a>

## mulBinary(a, b) ⇒ <code>number</code>
Write a binary function `mulBinary`
that takes two numbers and returns
their product

**Kind**: global function  

| Param | Type |
| --- | --- |
| a | <code>number</code> |
| b | <code>number</code> |

**Example**  
```js
mulBinary(3, 4) // 3 * 4 = -1
```
<a name="add"></a>

## add(...nums) ⇒ <code>number</code>
Write a function `add` that
is generalized for any
amount of arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| ...nums | <code>number</code> |

**Example**  
```js
add(1, 2, 4) // 1 + 2 + 4 = 7
```
<a name="sub"></a>

## sub(...nums) ⇒ <code>number</code>
Write a function `sub` that
is generalized for any
amount of arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| ...nums | <code>number</code> |

**Example**  
```js
sub(1, 2, 4) // 1 - 2 - 4 = -5
```
<a name="mul"></a>

## mul(...nums) ⇒ <code>number</code>
Write a function `mul` that
is generalized for any
amount of arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| ...nums | <code>number</code> |

**Example**  
```js
mul(1, 2, 4) // 1 * 2 * 4 = 8
```
<a name="addTail"></a>

## addTail(...nums) ⇒ <code>number</code>
Write a function `addTail` that
is the generalized `add` function
with tail recursion

**Kind**: global function  

| Param | Type |
| --- | --- |
| ...nums | <code>number</code> |

**Example**  
```js
addTail(1, 2, 4) // 1 + 2 + 4 = 7
```
<a name="mulTail"></a>

## mulTail(...nums) ⇒ <code>number</code>
Write a function `mulTail` that
is the generalized `mul` function
with tail recursion

**Kind**: global function  

| Param | Type |
| --- | --- |
| ...nums | <code>number</code> |

**Example**  
```js
mulTail(1, 2, 4) // 1 * 2 * 4 = 8
```
<a name="acc"></a>

## acc(funct, start) ⇒ <code>function</code>
Write a function `acc` that
takes a function and a
starting value and returns
a function that runs the
initial function on each
argument

**Kind**: global function  

| Param | Type |
| --- | --- |
| funct | <code>function</code> |
| start | <code>number</code> &#124; <code>string</code> |

**Example**  
```js
let add = acc((total, curr) => total + curr, 0);
add(1, 2, 4) // 7

let mul = acc((total, curr) => total * curr, 1);
mul(1, 2, 4) // 8
```
<a name="accTail"></a>

## accTail(funct, start) ⇒ <code>function</code>
Write a function `accTail` that
does what `acc` does but uses
tail recursion

**Kind**: global function  

| Param | Type |
| --- | --- |
| funct | <code>function</code> |
| start | <code>number</code> &#124; <code>string</code> |

**Example**  
```js
let add = accTail((total, curr) => total + curr, 0);
add(1, 2, 4) // 7

let mul = accTail((total, curr) => total * curr, 1);
mul(1, 2, 4) // 8
```
<a name="identityf"></a>

## identityf(x) ⇒ <code>function</code>
Write a function `identityf`
that takes an argument and
returns a function that
returns that argument

**Kind**: global function  

| Param | Type |
| --- | --- |
| x | <code>any</code> |

**Example**  
```js
let three = identityf(3);
three(); // 3
```
<a name="addf"></a>

## addf(a) ⇒ <code>function</code>
Write a function `addf` that
adds from two invocations

**Kind**: global function  

| Param | Type |
| --- | --- |
| a | <code>number</code> |

**Example**  
```js
addf(3)(4) // 7
```
<a name="liftf"></a>

## liftf(binary) ⇒ <code>function</code>
Write a function `liftf` that
takes a binary function, and
makes it callable with two
invocations

**Kind**: global function  

| Param | Type |
| --- | --- |
| binary | <code>function</code> |

**Example**  
```js
let addf = liftf(add);
addf(3)(4); // 7

liftf(mul)(5)(6) // 30
```
<a name="pure"></a>

## pure(x, y) ⇒ <code>array</code>
Write a [pure](https://en.wikipedia.org/wiki/Pure_function) function `pure` that
is a wrapper arround the impure
function `impure`

<pre>function impure(x) {
  y++;
  z = x * y;
}

var y = 5, z;

impure(20);
z; // 120

impure(25);
z; // 175</pre>

**Kind**: global function  
**Returns**: <code>array</code> - an array containing  `y` and `z`  

| Param | Type |
| --- | --- |
| x | <code>number</code> |
| y | <code>number</code> |

**Example**  
```js
pure(20, 5) // [ 6, 120 ]
pure(25, 6) // [ 7, 175 ]
```
<a name="curryBinary"></a>

## curryBinary(binary, a) ⇒ <code>function</code>
Write a function `curryBinary` that
takes a binary function and
an argument, and returns a
function that can take a
second argument

**Kind**: global function  

| Param | Type |
| --- | --- |
| binary | <code>function</code> |
| a | <code>any</code> |

**Example**  
```js
let add3 = curryBinary(add, 3);
add3(4); // 7

curry(mul, 5)(6); // 30
```
<a name="curry"></a>

## curry(func, ...outer) ⇒ <code>function</code>
Write a function `curry` that
is generalized for any amount
of arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| func | <code>function</code> |
| ...outer | <code>any</code> |

**Example**  
```js
curry(add, 1, 2, 4)(4, 2, 1) = 1 + 2 + 4 + 4 + 2 + 1 = 14
curry(sub, 1, 2, 4)(4, 2, 1) = 1 - 2 - 4 - 4 - 2 - 1 = 0
curry(mul, 1, 2, 4)(4, 2, 1) = 1 * 2 * 4 * 4 * 2 * 1 = 64
```
<a name="inc"></a>

## inc(x) ⇒ <code>number</code>
Without writting any new functions,
show multiple ways to create the `inc`
function

**Kind**: global function  

| Param | Type |
| --- | --- |
| x | <code>number</code> |

**Example**  
```js
inc(5)      // 6
inc(inc(5)) // 7
```
<a name="twiceUnary"></a>

## twiceUnary(binary) ⇒ <code>function</code>
Write a function `twiceUnary`
that takes a binary function
and returns a unary function
that passes its argument to
the binary function twice

**Kind**: global function  

| Param | Type |
| --- | --- |
| binary | <code>function</code> |

**Example**  
```js
let doubl = twiceUnary(addBinary);
doubl(11) // 22

let square = twiceUnary(mulBinary);
square(11) // 121
```
<a name="doubl"></a>

## doubl(x) ⇒ <code>number</code>
Use the function `twiceUnary` to
create the `doubl` function

**Kind**: global function  

| Param | Type |
| --- | --- |
| x | <code>number</code> |

**Example**  
```js
doubl(11) // 22
```
<a name="square"></a>

## square(x) ⇒ <code>number</code>
Use the function `twiceUnary` to
create the `square` function

**Kind**: global function  

| Param | Type |
| --- | --- |
| x | <code>number</code> |

**Example**  
```js
square(11) // 121
```
<a name="twice"></a>

## twice(x) ⇒ <code>any</code>
Write a function `twice` that
is generalized for any amount
of arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| x | <code>function</code> |

**Example**  
```js
let doubleSum = twice(add);
doubleSum(1, 2, 4) // 1 + 2 + 4 + 1 + 2 + 4 = 14
```
<a name="reverseBinary"></a>

## reverseBinary(binary) ⇒ <code>function</code>
Write a function `reverseBinary` that
reverses the arguments of a
binary function

**Kind**: global function  

| Param | Type |
| --- | --- |
| binary | <code>function</code> |

**Example**  
```js
let bus = reverseBinary(subBinary);
bus(3, 2) // -1
```
<a name="reverse"></a>

## reverse(func) ⇒ <code>function</code>
Write a function `reverse` that
is generalized for any amount
of arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| func | <code>function</code> |

**Example**  
```js
reverse(sub)(1, 2, 4) // 4 - 2 - 1 = 1
```
<a name="composeuTwo"></a>

## composeuTwo(unary1, unary2) ⇒ <code>function</code>
Write a function `composeuTwo` that
takes two unary functions and
returns a unary function that
calls them both

**Kind**: global function  

| Param | Type |
| --- | --- |
| unary1 | <code>function</code> |
| unary2 | <code>function</code> |

**Example**  
```js
composeuTwo(doubl, square)(5) // 100
```
<a name="composeu"></a>

## composeu(...funcs) ⇒ <code>any</code>
Write a function `composeu` that
is generalized for any amount
of arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| ...funcs | <code>function</code> |

**Example**  
```js
composeu(doubl, square, identity, curry(add, 1, 2))(5) // (5 + 5) * (5 + 5) + 1 + 2 = 103
```
<a name="composeb"></a>

## composeb(binary1, func2) ⇒ <code>function</code>
Write a function `composeb` that
takes two binary functions and
returns a function that calls
them both

**Kind**: global function  

| Param | Type |
| --- | --- |
| binary1 | <code>function</code> |
| func2 | <code>function</code> |

**Example**  
```js
composeb(add, mul)(2, 3, 7) // 35
```
<a name="limitBinary"></a>

## limitBinary(binary, lmt) ⇒ <code>function</code>
Write a function `limitBinary`
that allows a binary function
to be called a limited number
of times

**Kind**: global function  

| Param | Type |
| --- | --- |
| binary | <code>function</code> |
| lmt | <code>number</code> |

**Example**  
```js
let addLmtBinary = limitBinary(addBinary, 1);
addLmtBinary(3, 4) // 7
addLmtBinary(3, 5) // undefined
```
<a name="limit"></a>

## limit(func, lmt) ⇒ <code>function</code>
Write a function `limit` that
is generalized for any amount
of arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| func | <code>function</code> |
| lmt | <code>number</code> |

**Example**  
```js
let addLmt = limit(add, 1);
addLmt(1, 2, 4)    // 7
addLmt(3, 5, 9, 2) // undefined
```
<a name="genFrom"></a>

## genFrom(x) ⇒ <code>function</code>
Write a function `genFrom` that
produces a generator that will
produces a series of values

**Kind**: global function  

| Param | Type |
| --- | --- |
| x | <code>number</code> |

**Example**  
```js
let index = genFrom(0);

index() // 0
index() // 1
index() // 2
```
<a name="genTo"></a>

## genTo(gen, lmt) ⇒ <code>function</code>
Write a function `genTo` that
takes a generator and an end
limit, and returns a generator
that will produce numbers up
to that limit

**Kind**: global function  

| Param | Type |
| --- | --- |
| gen | <code>function</code> |
| lmt | <code>number</code> |

**Example**  
```js
let index = genTo(genFrom(1), 3);

index() // 1
index() // 2
index() // undefined
```
<a name="genFromTo"></a>

## genFromTo(start, end) ⇒ <code>function</code>
Write a function `genFromTo` that
produces a generator that will
produce values in a range

**Kind**: global function  

| Param | Type |
| --- | --- |
| start | <code>number</code> |
| end | <code>number</code> |

**Example**  
```js
let index = genFromTo(0, 3);
index() // 0
index() // 1
index() // 2
index() // undefined
```
<a name="elementGen"></a>

## elementGen(array, gen) ⇒ <code>function</code>
Write a function `elementGen` that
takes an array and a generator
and returns a generator that will
produce elements from the array

**Kind**: global function  

| Param | Type |
| --- | --- |
| array | <code>array</code> |
| gen | <code>function</code> |

**Example**  
```js
let ele = elementGen([
  'a', 'b', 'c', 'd'
], genFromTo(1, 3));

ele() // 'b'
ele() // 'c'
ele() // undefined
```
<a name="element"></a>

## element(array, gen) ⇒ <code>function</code>
Write a function `element` that is a
modified `elementGen` function so that
the generator argument is optional.
If a generator is not provided, then
each of the elements of the array
will be produced.

**Kind**: global function  

| Param | Type |
| --- | --- |
| array | <code>array</code> |
| gen | <code>function</code> |

**Example**  
```js
let ele = element([
  'a', 'b', 'c', 'd'
]);

ele() // 'a'
ele() // 'b'
ele() // 'c'
ele() // 'd'
ele() // undefined
```
<a name="collect"></a>

## collect(gen, array) ⇒ <code>function</code>
Write a function `collect` that takes a
generator and an array and produces
a function that will collect the results
in the array

**Kind**: global function  

| Param | Type |
| --- | --- |
| gen | <code>function</code> |
| array | <code>array</code> |

**Example**  
```js
let array = [];
let col = collect(genFromTo(0, 2), array);

col() // 0
col() // 1
col() // undefined
array // [0, 1]
```
<a name="filter"></a>

## filter(gen, predicate) ⇒ <code>function</code>
Write a function `filter` that takes a
generator and a predicate and produces
a generator that produces only the
values approved by the predicate

**Kind**: global function  

| Param | Type |
| --- | --- |
| gen | <code>function</code> |
| predicate | <code>function</code> |

**Example**  
```js
let fil = filter(genFromTo(0, 5), val => val % 3);

fill() // 0
fill() // 3
fill() // undefined
```
<a name="filterTail"></a>

## filterTail(gen, predicate) ⇒ <code>function</code>
Write a function `filterTail` that uses
tail-recursion to perform the filtering

**Kind**: global function  

| Param | Type |
| --- | --- |
| gen | <code>function</code> |
| predicate | <code>function</code> |

**Example**  
```js
let third = val => val % 3 === 0;
let fil = filterTail(genFromTo(0, 5), third);

fill() // 0
fill() // 3
fill() // undefined
```
<a name="concatTwo"></a>

## concatTwo(gen1, gen2) ⇒ <code>function</code>
Write a function `concatTwo` that takes
two generators and produces a generator
that combines the sequences

**Kind**: global function  

| Param | Type |
| --- | --- |
| gen1 | <code>function</code> |
| gen2 | <code>function</code> |

**Example**  
```js
let con = concatTwo(genFromTo(0, 3), genFromTo(0, 2));
con() // 0
con() // 1
con() // 2
con() // 0
con() // 1
con() // undefined
```
<a name="concat"></a>

## concat(...gens) ⇒ <code>function</code>
Write a function `concat` that
is generalized for any amount
of arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| ...gens | <code>function</code> |

**Example**  
```js
let con = concat(genFromTo(0, 3), genFromTo(0, 2), genFromTo(5, 7));
con() // 0
con() // 1
con() // 2
con() // 0
con() // 1
col() // 5
col() // 6
con() // undefined
```
<a name="concatTail"></a>

## concatTail(...gens) ⇒ <code>function</code>
Write a function `concatTail` that uses
tail-recursion to perform the concating

**Kind**: global function  

| Param | Type |
| --- | --- |
| ...gens | <code>function</code> |

**Example**  
```js
let con = concatTail(genFromTo(0, 3), genFromTo(0, 2), genFromTo(5, 7));
con() // 0
con() // 1
con() // 2
con() // 0
con() // 1
col() // 5
col() // 6
con() // undefined
```
<a name="gensymf"></a>

## gensymf(symbol) ⇒ <code>function</code>
Write a function `gensymf` that
makes a function that generates
unique symbols

**Kind**: global function  

| Param | Type |
| --- | --- |
| symbol | <code>string</code> |

**Example**  
```js
let genG = gensymf('G');
let genH = gensymf('H');

genG() // 'G1'
genH() // 'H1'
genG() // 'G2'
genH() // 'H2'
```
<a name="gensymff"></a>

## gensymff(unary, seed) ⇒ <code>function</code>
Write a function `gensymff` that
takes a unary function and a
seed and returns a `gensymf`

**Kind**: global function  

| Param | Type |
| --- | --- |
| unary | <code>function</code> |
| seed | <code>number</code> |

**Example**  
```js
let gensymf = gensymff(inc, 0);
let genG = gensymf('G');
let genH = gensymf('H');

genG() // 'G1'
genH() // 'H1'
genG() // 'G2'
genH() // 'H2'
```
<a name="fibonaccif"></a>

## fibonaccif(first, second) ⇒ <code>function</code>
Write a function `fibonaccif` that
returns a generator that will
return the next fibonacci number

**Kind**: global function  

| Param | Type |
| --- | --- |
| first | <code>number</code> |
| second | <code>number</code> |

**Example**  
```js
let fib = fibonaccif(0, 1);
fib() // 0
fib() // 1
fib() // 2
fib() // 3
fib() // 5
fib() // 8
```
<a name="counter"></a>

## counter(i) ⇒ <code>object</code>
Write a function `counter` that
returns an object containing
two functions that implement
an up/down counter, hiding
the counter

**Kind**: global function  

| Param | Type |
| --- | --- |
| i | <code>number</code> |

**Example**  
```js
let obj = counter(10);
let { up, down } = object;

up()   // 11
down() // 10
down() // 9
up()   // 10
```
<a name="revocableBinary"></a>

## revocableBinary(binary) ⇒ <code>object</code>
Write a function `revocableBinary`
that takes a binary function, and
returns an object containing an
`invoke` function that can invoke a
function and a `revoke` function
that disables the `invoke` function

**Kind**: global function  

| Param | Type |
| --- | --- |
| binary | <code>function</code> |

**Example**  
```js
let rev = revocableBinary(addBinary);

rev.invoke(3, 4); // 7
rev.revoke();
rev.invoke(5, 7); // undefined
```
<a name="revocable"></a>

## revocable(func) ⇒ <code>object</code>
Write a function `revocable` that
is generalized for any amount of
arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| func | <code>function</code> |

**Example**  
```js
let rev = revocable(add);

rev.invoke(3, 4); // 7
rev.revoke();
rev.invoke(5, 7); // undefined
```
<a name="extract"></a>

## extract(array, prop) ⇒ <code>array</code>
Write a function `extract` that
takes an array of objects and an
object property name and converts
each object in the array by
extracting that property

**Kind**: global function  

| Param | Type |
| --- | --- |
| array | <code>array</code> |
| prop | <code>string</code> |

**Example**  
```js
let people = [{ name: 'john'}, { name: 'bob' }];
let names = extract(people, 'name'); // ['john', 'bob']
```
<a name="m"></a>

## m(value, source) ⇒ <code>object</code>
Write a function `m` that
takes a value and an
optional source string
and returns them in an
object

**Kind**: global function  

| Param | Type |
| --- | --- |
| value | <code>any</code> |
| source | <code>any</code> |

**Example**  
```js
JSON.stringify(m(1)) // '{"value":1,"source":"1"}'

JSON.stringify(m(Math.PI, "pi")) // '{"value":3.14159...,"source":"pi"}'
```
<a name="addmTwo"></a>

## addmTwo(m1, m2) ⇒ <code>object</code>
Write a function `addmTwo` that
adds two `m` objects and
returns an `m` object

**Kind**: global function  

| Param | Type |
| --- | --- |
| m1 | <code>function</code> |
| m2 | <code>function</code> |

**Example**  
```js
JSON.stringify(addmTwo(m(3), m(4))) // '{"value":7,"source":"(3+4)"}'

JSON.stringify(addmTwo(m(1), m(Math.PI, "pi"))) // '{"value":4.14159...,"source":"(1+pi)"}'
```
<a name="addm"></a>

## addm(...ms) ⇒ <code>object</code>
Write a function `addm` that
is generalized for any amount of
arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| ...ms | <code>function</code> |

**Example**  
```js
JSON.stringify(addm(m(1), m(2), m(4))) // '{"value":7,"source":"(1+2+4)"}'
```
<a name="liftmBinaryM"></a>

## liftmBinaryM(binary, op) ⇒ <code>object</code>
Write a function `liftmBinaryM` that
takes a binary function and
a string and returns a function
that acts on `m` objects

**Kind**: global function  

| Param | Type |
| --- | --- |
| binary | <code>function</code> |
| op | <code>string</code> |

**Example**  
```js
let addmBinary = liftmBinaryM(addBinary, '+');

JSON.stringify(addmBinary(m(3), m(4))) // '{"value":7,"source":"(3+4)"}'

JSON.stringify(liftmBinaryM(mul, '*')(m(3), m(4))) // '{"value":12,"source":"(3*4)"}'
```
<a name="liftmBinary"></a>

## liftmBinary(binary, op) ⇒ <code>object</code>
Write a function `liftmBinary` that
is a modified function `liftmBinaryM`
that can accept arguments that
are either numbers or m objects

**Kind**: global function  

| Param | Type |
| --- | --- |
| binary | <code>function</code> |
| op | <code>string</code> |

**Example**  
```js
let addmBinary = liftmBinary(addBinary, '+')

JSON.stringify(addmBinary(3, 4)) // '{"value":7,"source":"(3+4)"}'
```
<a name="liftm"></a>

## liftm(func, op) ⇒ <code>object</code>
Write a function `liftm` that
is generalized for any amount of
arguments

**Kind**: global function  

| Param | Type |
| --- | --- |
| func | <code>function</code> |
| op | <code>string</code> |

**Example**  
```js
let addm = liftm(add, '+');

JSON.stringify(addm(m(3), m(4))) // '{"value":7,"source":"(3+4)"}'

JSON.stringify(liftm(mul, '*')(m(3), m(4))) // '{"value":12,"source":"(3*4)"}'
```
<a name="exp"></a>

## exp(value) ⇒ <code>any</code>
Write a function `exp` that
evaluates simple array
expressions

**Kind**: global function  

| Param | Type |
| --- | --- |
| value | <code>any</code> |

**Example**  
```js
let sae = [mul, 1, 2, 4];
exp(sae) // 1 * 2 * 4 = 8
exp(42)  // 42
```
<a name="expn"></a>

## expn(value) ⇒ <code>any</code>
Write a function `expn`
that is a modified `exp` that
can evaluate nested array
expressions

**Kind**: global function  

| Param | Type |
| --- | --- |
| value | <code>any</code> |

**Example**  
```js
let nae = [
  Math.sqrt,
  [
    add,
    [square, 3],
    [square, 4]
  ]
];

expn(nae) // sqrt(((3*3)+(4*4))) === 5
```
<a name="addg"></a>

## addg(value) ⇒ <code>number</code> &#124; <code>undefined</code>
Write a function `addg` that
adds from many invocations,
until it sees an empty
invocation

**Kind**: global function  

| Param | Type |
| --- | --- |
| value | <code>number</code> |

**Example**  
```js
addg()             // undefined
addg(2)()          // 2
addg(2)(7)()       // 9
addg(3)(0)(4)()    // 7
addg(1)(2)(4)(8)() // 15
```
<a name="liftg"></a>

## liftg(binary) ⇒ <code>function</code>
Write a function `liftg` that
will take a binary function
and apply it to many invocations

**Kind**: global function  

| Param | Type |
| --- | --- |
| binary | <code>function</code> |

**Example**  
```js
liftg(mulBinary)()             // undefined
liftg(mulBinary)(3)()          // 3
liftg(mulBinary)(3)(0)(4)()    // 0
liftg(mulBinary)(1)(2)(4)(8)() // 64
```
<a name="arrayg"></a>

## arrayg(value) ⇒ <code>array</code>
Write a function `arrayg` that
will build an array from many
invocations

**Kind**: global function  

| Param | Type |
| --- | --- |
| value | <code>any</code> |

**Example**  
```js
arrayg()          // []
arrayg(3)()       // [3]
arrayg(3)(4)(5)() // [3, 4, 5]
```
<a name="continuizeu"></a>

## continuizeu(unary) ⇒ <code>function</code>
Write a function `continuizeu`
that takes a unary function
and returns a function that
takes a callback and an
argument

**Kind**: global function  

| Param | Type |
| --- | --- |
| unary | <code>function</code> |

**Example**  
```js
sqrtc = continuizeu(Math.sqrt);
sqrtc(console.log, 81); // logs '9'
```
<a name="continuize"></a>

## continuize(any) ⇒ <code>function</code>
Write a function `continuize`
that takes a function and
returns a function that
takes a callback and an
argument

**Kind**: global function  

| Param | Type |
| --- | --- |
| any | <code>function</code> |

**Example**  
```js
sqrtc = continuizeu(Math.sqrt);
sqrtc(console.log, 1, 2, 4); // logs '1 2 4'
```
<a name="vector"></a>

## vector()
Make an array wrapper object
with methods `get`, `store`,
and `append`, such that an
attacker cannot get access
to the private array

**Kind**: global function  
**Example**  
```js
let v = vector();
v.append(7);
v.store(1, 8);
v.get(0);      // 7
v.get(1);      // 8
```
<a name="exploitVector"></a>

## exploitVector()
Let's assume your `vector`
implementation looks like
something like this:

<pre>function vector() {
  var array = [];
  return {
    append: function append(v) {
      array.push(v);
    },
    get: function get(i) {
      return array[i];
    },
    store: function store(i, v) {
      array[i] = v;
    }
  };
}</pre>

Can you spot any security concerns with
this approach? Mainly, can we get access
to the `array` outside of `vector`?
Note*: the issue has nothing to do with
prototypes and we can assume that global
prototypes cannot be altered.
Hint*: Think about using `this` in a
method invocation. Can we override a
method of `vector`?

**Kind**: global function  
**Example**  
```js
var v = vector();
v.append(1);
v.append(2);
var internalData = exploitVector(v); // [1, 2]
```
<a name="vectorSafe"></a>

## vectorSafe()
How would you rewrite `vector` to deal
with the issue from above?

**Kind**: global function  
**Example**  
```js
var v = vectorSafe();
v.append(1);
v.append(2);
var internalData = exploitVector(v); // undefined
```
<a name="pubsub"></a>

## pubsub()
Make a function `pubsub` that
makes a publish/subscribe object.
It will reliably deliver all
publications to all subscribers
in the right order.

**Kind**: global function  
**Example**  
```js
let ps = pubsub();
ps.subscribe(log);
ps.publish('It works!') // log('It works!')
```
