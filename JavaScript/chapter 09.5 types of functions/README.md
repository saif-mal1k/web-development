# Que: what’s the different ways of using function?????

## 1. function add() {…}  
```js
function displayDone() {
  console.log('welcome again after 2 seconds');
}
// timer value is in milliseconds
setTimeout(displayDone, 2000);
```
in execution context, memory will be allocated with function definition in it. both memory allocation and definition will happen during memory allocation phase.
in program if you have function invocation before function definition. invocation will return undefined.

## 2. var add = function() {…} 
```js
setTimeout(function() {
  console.log('welcome again after 2 seconds');
}, 2000);
```
in execution context it’ll behave like a variable, only memory will be allocated with the place holder undefined. because the function definition will be provided during code execution phase. 
in program if you have function invocation before function definition. invocation will return undefined.

## 3. ()=>{…} //arrow function 
```js
setTimeout(() => {
  console.log('welcome again after 2 seconds');
}, 2000);
```
tip: write js program that invoke all above function types and run debugger for the file and see the callstack and variables scope in vscode debugger.



<br/>


<br/>

### what to use when
- If you know you'll be using the function more than once, create it as normal. 
- If you'll be using it for just the one location, it's generally best to use an anonymous function or arrow function.

<br/>


<br/>



# First class function ???
# Higher order functions???
# Pure Functions
