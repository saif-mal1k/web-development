# function in JavaScript:

<br/>


## function statement aka function declaration
```js
  function a () {...}
```

<br/>


<br/>


## First-class Function
- A programming language is said to have <b>First-class functions</b> when functions in that language are treated like any other variable. 
- In JavaScript, functions are called <b>Function Objects</b> because they are objects. Just like objects, functions have properties and methods, they can be stored in a variable or an array, and be passed as arguments to other functions.

> <b>example:</b>
> <br/>
> ```js
> const myArray = [ function alerter() { alert('Hello!'); } ];
> ```
> call above function using <b> ``myArray[0]()``</b>    


<br/>


## Function Expression
<b> When a function is assigned to a variable it becomes Function Expression.</b> 
The function can be named, or anonymous. Use the variable name to call a function defined in a function expression.

> <img width="420px" src="https://user-images.githubusercontent.com/63545175/168762763-1fa3b5af-5985-4d43-8082-367fee4cd76e.png" alt="image">


<br/>


<br/>


## function declaration vs function expression
All <b><em>function declarations are hoisted</em></b> and loaded before the script is actually run. <b><em>Function expressions are not hoisted,</em></b> since they involve variable assignment, and only variable declarations are hoisted. The function expression will not be loaded until the interpreter reaches it in the script.

<b><em>Only function expressions can be anonymous, function declarations must have a name.</em></b>


<br/>


## function invokation / function call

<b>note:</b> you can define a function by any of above two ways, and invoking will be same i.e.

```js
  a();    //executes function aka invokes function
```


<br/>


> <b>tip: 💡</b> you can define function inside another function. 
> <br/> <b>note that</b> variables and functions defined inside function scope aka lexical scope are available only within that function. 
> <br/> when a function invokes, a new execution context for this new function is created. inside global execution context.


<br/>






