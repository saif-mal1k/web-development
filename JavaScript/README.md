# JavaScript notes


<br/>


<details>
	<summary> <b><em> what is JavaScript ? </em></b> </summary>
<p>

<b><em>Answer:</em></b>

- an interpreted scripting language i.e directly embedded into HTML page to add interactivity to the page.
- Everyone can use JavaScript without purchasing a license
	
</p>
</details>

<br/>

<details>
	<summary> <b><em> where is JavaScript Used ? </em></b> </summary>
<p>

<b><em>Answer:</em></b>

- ***web development***
	- JavaScript gives HTML designers a programming tool.
	- JavaScript can dynamically create, edit and delete HTML elements.
	- JavaScript can react to events.
	- JavaScript can be used to validate data.
	- JavaScript can be used to create, read cookies.
	
- ***Salesforce development***

	- JavaScript is used in creating lwc components.
	
</p>
</details>

<br/>

<details>
	<summary> <b><em> How JavaScript Works ? </em></b> </summary>
<p>

<b><em>Answer:</em></b>
	
### In Browser
A browser’s primary job is to act as a client for a web server. It requests resources over the Internet, using one of several protocols (usually HTTP/HTTPS). Once a server passes it some of those resources, the browser needs to do something with them. At a minimum HTML and CSS are rendered into a page. When a resource contains some JavaScript, the browser reaches over to the JavaScript runtime engine to parse, evaluate, and execute that code. 

Likewise, while a script is executing it can also reach back to the browser to do things like modify the web page, interact with the local environment, or interact with other web resources.

### In server


</p>
</details>

<br/>

<details>
	<summary> <b><em> popular JavaScript Frameworks, Libraries ??????? </em></b> </summary>
<p>

<b><em>Answer:</em></b>
	
	
</p>
</details>

<br/>

<details>
	<summary> <b><em> Javascript <code> API's</code> ? </em></b> </summary>
<p>

<b><em>Answer:</em></b>

- Interact with the structure of the current page rendered in the browser (Document Object Model or ``DOM API``)
- Perform asynchronous requests to the server without leaving the current page (``Fetch API``)
- Interact with device features surfaced to the browser (geolocation, device orientation, client-side data storage & to cache the data locally)
	
	
</p>
</details>

<br/>


<br/>


# JS Overview

<br/>

- <b>OBJECT ORIENTED</b>


<br/>

- <b>ANONYMOUS FUNCTIONS</b>
> Anonymous functions are functions that are dynamically declared at runtime. They’re called anonymous functions because they aren’t given a name in the same way as normal functions.

<br/>

- <b>FUNCTIONS AS FIRST-CLASS OBJECTS</b>
> Functions in JavaScript are first class objects. This means that JavaScript functions are just a special type of object that can do all the things that regular objects can do.

<br/>

- <b>LOOSE TYPING </b>

<br/>

- <b>SCOPING AND HOISTING </b>
> <b>Scoping:</b> In JavaScript, functions are our de facto scope delimiters for declaring vars, which means that usual blocks from loops and conditionals (such as if, for, while, switch and try) DON'T delimit scope, unlike most other languages. Therefore, those blocks will share the same scope as the function which contains them. This way, it might be dangerous to declare vars inside blocks as it would seem the var belongs to that block only.

><b>Hoisting:</b> On runtime, all var and function declarations are moved to the beginning of each function (its scope) - this is known as Hoisting. Having said so, it is a good practice to declare all the vars altogether on the first line, in order to avoid false expectations with a var that got declared late but happened to hold a value before - this is a common problem for programmers coming from languages with block scope.

<br/>

- <b>FUNCTION BINDING</b>
> Function binding is most probably the least of your concerns when beginning with JavaScript, but when you realize that you need a solution to the problem of how to keep the context of this within another function, then you might realize that what you actually need is Function.prototype.bind().

<br/>

- <b>CLOSURE FUNCTION</b>
> Closures are functions that refer to independent (free) variables. In other words, the function defined in the closure 'remembers' the environment in which it was created in. It is an important concept to understand as it can be useful during development, like emulating private methods. It can also help to learn how to avoid common mistakes, like creating closures in loops.

<br/>

- <b>STRICT MODE</b>
> ECMAScript 5's strict mode is a way to opt in to a restricted variant of JavaScript. Strict mode isn't just a subset: it intentionally has different semantics from normal code. Browsers not supporting strict mode will run strict mode code with different behavior from browsers that do, so don't rely on strict mode without feature-testing for support for the relevant aspects of strict mode. Strict mode code and non-strict mode code can coexist, so scripts can opt into strict mode incrementally.

<br/>

- <b>IMMEDIATELY-INVOKED FUNCTION EXPRESSION (IIFE)</b>
> An immediately-invoked function expression is a pattern which produces a lexical scope using JavaScript's function scoping. Immediately-invoked function expressions can be used to avoid variable hoisting from within blocks, protect against polluting the global environment and simultaneously allow public access to methods while retaining privacy for variables defined within the function.



