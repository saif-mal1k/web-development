# most important concepts:
- remember JavaScript is a synchronous single-threaded language.
- That means the code execution will be done one piece at a time. & in a specified order.

![image](https://user-images.githubusercontent.com/63545175/168548217-d1b2e89c-22fe-4445-bf37-a7d7928f9a1d.png)


<br/>


## execution context and scope chaining
- Everything is executed in an Execution Context.
- Function invocation creates a new Execution Context.
- <b>Each Execution Context has:</b>
  - Its own Variable Environment
  - Special ‘this’ object
  - Reference to its Outer Environment
-	Global Scope does not have an Outer Environment as it’s the most outer there is.

> **note: 📝** call stack maintains the order of execution of execution contexts.


<br/>


### what is scope?
<b>Scope in JavaScript refers ``to the current context of code``, which determines the accessibility of variables to JavaScript. The two types of scope are local and global: Global variables are those declared outside of a block. Local variables are those declared inside of a block.</b>


<br/>

### what is scope chaining
![image](https://user-images.githubusercontent.com/63545175/168549168-04d97ea9-002f-4148-ba81-53cfa950b86e.png)

> **note: 📝** similarly, in the case of a non-declared variable, it will be searched in respective lexical environments and if no lexical environment is left to search in, the JS engine will return “not defined”.

> **tip: 💡** lexical environment is the local memory + lexical environment of parent.


<br/>

## hoisting
<b>whenever we run a JavaScript program an execution context is created, in two phases. in first phase memory context aka, variable environment is created in second phase code context is created. note that in memory context phase, only space is allocated and variables are not initialized they are initialized only when thread of execution reaches the initialization command.</b>

this above nature of JS is called hoisting, and is the reason <b>we can call a function before providing its definition</b>, and when we use a variable early on that is initialize later in code, it says undefined because the space is allocated but variable is not yet defined.

<table>
<tr>
<td>

<a href="#hoisting"> <img src="https://user-images.githubusercontent.com/63545175/168552213-4f9cbf29-707a-492b-9827-4f1514472cf7.png" alt="image"></a>
        
</td>  
<td>

<a href="#hoisting"> <img src="https://user-images.githubusercontent.com/63545175/168552236-9fec7797-e80f-4383-a188-a60065eeb438.png" alt="image"></a>
     
</td>  
</tr>
</table>


<b>imp summary:</b>
- JavaScript hoists function declarations and variable declarations to the top of the current scope in memory context.
- Variable assignments are not hoisted.
- Declare functions and variables at the top of your scripts, so the syntax and behavior are consistent with each other.


<br/>


## closures
<b>A function bundled together (enclosed) with references to its surrounding state (the lexical environment) forms a closure.</b> 
In JavaScript, closures are created every time a function is created, at function creation time.

In other words, a closure gives you access to an outer function’s scope from an inner function.

<table>
<tr>
<td>

<a href="#hoisting"> <img src="https://user-images.githubusercontent.com/63545175/168553158-12aebb17-59af-4f57-85d9-315bc8b10f2b.png" alt="image"></a>
        
</td>  
<td>

<a href="#hoisting"> <img src="https://user-images.githubusercontent.com/63545175/168553195-789f7d8b-7e9f-4f38-878e-73b786d8d0bf.png" alt="image"></a>
     
</td>  
</tr>
</table>

<b><em>example:</b></em>

```apex
 function makeFunc() {
  	var name = 'Mozilla';
 	 function displayName() {
  	 	console.log(name);
  	}
 	return displayName;
}
var myFunc = makeFunc();
myFunc();
```

<b><em>output:</b></em>
```apex
// Mozilla on console, note function displayName reference is stored in function myFunc. 
```

### importance of closures ????


### disadvantage of closures ????


### Garbage collection ????









