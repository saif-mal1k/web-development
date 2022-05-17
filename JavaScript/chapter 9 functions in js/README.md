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

### Inline function expressions
<b>JavaScript allow's you to pass a function inline as an argument to another function.</b>

<b>example:</b>

```js
// Function declaration that takes in two arguments: a function for displaying
// a message, along with a name of a movie
function movies(messageFunction, name) {
  messageFunction(name);
}

// Call the movies function, pass in the function and name of movie
movies(function displayFavorite(movieName) {
  console.log("My favorite movie is " + movieName);
}, "KGF");
```

<b>Output:</b>
My favorite movie is KGF


<br/>


### Why use anonymous inline function expressions?
<b>Anonymous inline function expressions are often used with function callbacks that are probably not going to be reused elsewhere.</b>


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


## Default Values
```js
function orderChickenWith(sidedish="whatever!"){
    return "chicken with "+sidedish;
}

console.log(orderChickenWith("noodles"));
console.log(orderChickenWith());
```

<br/>


## Parameter vs Argument
- A <b>parameter</b> is always going to be a variable name and appears in the function declaration. 
- an <b>argument</b> is always going to be a value (i.e. any of the JavaScript data types - a number, a string, a boolean, etc.) and will always appear in the code when the function is called or invoked.

<br/>


## Passing Arguments (passing variables by value vs by reference):

### Passing a Primitive
In JavaScript, <b>primitive datatypes are immutable.</b> In other words, any changes made to an argument inside a function effectively creates a copy local to that function, and does not affect the primitive outside of that function. 
see also function scope vs block scope, shadowing.

### Passing an Object
On the other hand, <b>objects in JavaScript are mutable.</b> If you pass an object into a function, Javascript passes a reference to that object. 


<br/>


## Que: How do you pass variable number of arguments in JavaScript?
<b>Ans:</b> When you call a function in JavaScript, you can pass in any number of arguments, regardless of what the function declaration specifies.

### just use the arguments object.
```js
function foo() {
  for (var i = 0; i < arguments.length; i++) {
    console.log(arguments[i]);
  }
}
```

> <b>tip: 💡</b> If you pass more arguments than are defined, they will be assigned to an array called arguments. 
> <br/> They can be used like this: arguments[0], arguments[1], etc.


<br/>


> <b>Note: 📝</b> If a function is called with missing arguments (fewer than declared), the missing values are set to undefined, which indicates that a variable has not been assigned a value.
> <br/>
> <b>Note: 📝</b> If you do not return anything from a function, it will return undefined.


<br/>


## Opening Curly Brace Placement (NOT just a style)

<table>
<tr>
<td colspan="2">

<b>Que:</b> {} on the same or next line, is it just a practice?  
</td>  
</tr>  
<tr>
<td>

<img src="https://user-images.githubusercontent.com/63545175/168779907-df66f75b-0a6b-4825-80bf-dd19eeafbece.png" alt="image"/>  
</td>  
<td>

<img src="https://user-images.githubusercontent.com/63545175/168780533-320aa6ec-afa3-4742-961b-fbb83bfcba01.png" alt="image"/>  
</td>  
</tr>
<tr>
<td colspan="2">
  
> now why is a() not executing ? actually both a() and return statement are executing but return statement is not executing the way we want it to. the JS engine since it don’t read anything after return statement in that line it automatically places a semi- colon after it. and hence object after return statement won’t execute.
> <br/> <b>tip: 💡</b> in JS it is not necessary to place ; at the end of statement, placing ; at the end of statement is a good practice. 
> <br/> javascript do allow comma trailing that allow you to add , after “malik” and add new property in next line.

</td>  
</tr>  
<table>
  

<br/>
  

## Anonymous functions:
An anonymous function is a <b>function without a function name.</b> Only function expressions can be anonymous, function declarations must have a name. Function expressions are used to define an <b>unnamed (anonymous)</b> function.
  
> <b><em>when a function is assigned to a variable it becomes function expression.</em></b> and the function itself is known as <b><em>anonymous function</em></b>, a function with no name.  

<img src="https://user-images.githubusercontent.com/63545175/168785406-bab0f990-e933-4f15-a8c4-7bfcad764046.png" alt="image" width="620px">

And, if you <b>try accessing the value of the variable</b> catSays, you'll even see the function returned back to you. to <b>call the function</b> just add ```()``` 
  
<img src="https://user-images.githubusercontent.com/63545175/168788350-a31d30ec-4c42-45d8-8987-8a6d2418a674.png" alt="image" width="620px">
  

<br/>
  
<b>important note: 📝</b> 
- All <b>function declarations are hoisted</b> and loaded before the script is actually run. <b>Function expressions are not hoisted</b>, since they involve variable assignment, and only variable declarations are hoisted. The function expression will not be loaded until the interpreter reaches it in the script.  
  

<br/>
  

### why use named function expressions to create anonymous functions?
<b>note:</b> Named functions <b>are great for a smoother debugging experience</b>, since those functions will have a useful name to display in stack traces. They're completely optional. 
  
  
<br/>
  
  
## Functions as parameters / callback
when a function is passed into another function it is called a callback.

<b>callback example:</b>
  
```js  
// function expression catSays
var catSays = function(max) {
  var catMessage = "";
  for (var i = 0; i < max; i++) {
    catMessage += "meow ";
  }
  return catMessage;
};

// function declaration helloCat accepting a callback
function helloCat(callbackFunc) {
  return "Hello " + callbackFunc(3);
}

// pass in catSays as a callback function
helloCat(catSays);
```  

                          
<br/>
  
  
<br/>
  
  

## ARROW FUNCTIONS 

### Why do we use fat arrows?
Arrow functions allow us to use the fat arrow => operator to quickly define JavaScript functions, with or without parameters. We are able to omit the curly braces and the function and return keywords when creating a new JavaScript function to write shorter function syntax.

  
### What is the difference between arrow function and normal function?
Unlike regular functions, arrow functions do not have their own this . 
The value of this inside an arrow function remains the same throughout the lifecycle of the function and is always bound to the value of this in the closest non-arrow parent function.
Arguments objects are not available in arrow functions, but are available in regular functions. Regular functions created using function declarations or expressions are 'constructible' and 'callable'.


### When should I not use arrow functions?
An arrow function doesn't have its own this value and the arguments object. Therefore, you should not use it as an event handler, a method of an object literal, a prototype method, or when you have a function that uses the arguments object.
  
  
### example: 
  ?????????
                          
                          
                          
