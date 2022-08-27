## Data types:
<b>primitive Date Types:</b> String, Number, Boolean, Null, Undefined

<details>
  <summary><b>primitive datatypes are immutable.</b></summary>
<p>

  > In other words, any changes made to an argument inside a function effectively creates a copy local to that function, and does not affect the primitive outside of that function.
</p>
</details>  

<table width="710">
<tbody>
<tr>
<td width="86">
<p><strong>Variable</strong></p>
</td>
<td>
<p><strong>Explanation</strong></p>
</td>
<td width="352">
<p><strong>Example</strong></p>
</td>
</tr>
<tr>
<td width="86">
<p><a href="https://developer.mozilla.org/en-US/docs/Glossary/String"><strong>String</strong></a></p>
</td>
<td>
<p>This is a sequence of text known as a string. To signify that the value is a string, enclose it in single quote marks.</p>
</td>
<td width="352">

```js
let myVariable = 'Bob';  
```
  
</td>
</tr>
<tr>
<td width="86">
<p><a href="https://developer.mozilla.org/en-US/docs/Glossary/Number"><strong>Number</strong></a></p>
</td>
<td>
<p>This is a number. can be float, decimal &hellip;</p>
</td>
<td width="352">

```js
let myVariable = 10;  
```  
  
</td>
</tr>
<tr>
<td width="86">
<p><a href="https://developer.mozilla.org/en-US/docs/Glossary/Boolean"><strong>Boolean</strong></a></p>
</td>
<td>
<p>This is a True/False value. The words true and false are special keywords that don't need quote marks.</p>
<p><strong>In conditional statements 0,Null, NaN, undefined, empty string are equal to false.</strong></p>
</td>
<td width="352">

```js
  let myVariable = true;
```
  
</td>
</tr>
<tr>
<td width="86">
<p><a href="https://developer.mozilla.org/en-US/docs/Glossary/array"><strong>Array</strong></a></p>
</td>
<td>
<p>This is a structure that allows you to store multiple values in a single reference.</p>
</td>
<td width="352">

```js
let myVariable = [1, 'Bob', 'Steve', 10];
``` 
  
Refer to each member of the array like this:
myVariable[0], myVariable[1], etc.  
  
</td>
</tr>
<tr>
<td width="86">
<p><a href="https://developer.mozilla.org/en-US/docs/Glossary/Object"><strong>Object</strong></a></p>
</td>
<td>
<p><strong><em>objects</em>&nbsp;are&nbsp;<em>mutable</em></strong>. This can be anything. Everything in JavaScript is an object and can be stored in a variable. Keep this in mind as you learn.</p>
</td>
<td width="352">

```js
let myVariable = document.querySelector('h1'); 
```  
  
All of the above examples too.
  
  
</td>
</tr>
</tbody>
</table>


> <b>tip: 💡</b> use typeof operator to know datatype. 
> ex: console.log(typeof variableName);


<br/>


### difference between ``null`` and ``undefined`` and ``not defined`` ?
- <b>Null</b>: allows to define datatype as Null. 
- <b>Undefined</b>: means variable memory has been allocated but no value has ever been explicitly set yet in other words <b>declaration no definition</b>. 

<b>while, not defined means no declaration no definition.</b>


<br/>

### What is NaN?
NaN stands for "Not-A-Number" and it's often returned indicating an error with number operations. 

For instance, if you wrote some code that performed a math calculation, and the calculation failed to produce a valid number, NaN might be returned.


<br/>



## JS is Dynamically typed
**Note: 📝**  <b>JS is dynamically typed</b>, this means variables declared using <b>var</b> can store any type of data type like <b>int, string, Boolean</b> and also complex data types like <b>object and array.</b> data type is <b>automatically evaluated at run time.</b> 
hence, same variable can hold different types during the life of its execution.


### Type coercion and Type Casting:
- type coercion is automatically conversion from one data type to 'appropriate' data type. it is done by JS engine.

<b>examples of type coercion:</b>

```js
console.log(4+'4');         //‘44’
console.log(true+4);        //5
console.log(true+'4');      //‘true4’
console.log(1.23+"4")       //‘1.234’
console.log('4'+1.23)       //‘41.23’
console.log(null+2)         //2
console.log(null+'2')       //‘null2’
console.log(undefined+2)    //NaN
console.log(undefined+'2')  //‘undefined2’
```
 
> <b>tip: 💡</b> ‘string’ + anything = ‘stringanything’ 
> <br/> and, anything + ‘string’ = ‘anythingstring’

  
### how to do type casting in js ???????????

  
<br/> 
  
  
## Keywords (Reserved Words): 
- These are keywords allowed in JavaScript. 
- For example: int, char, if, while, var, and public.


<br/>


## Literals:  
<b>Integer literals: </b>
```
ex: 3, -12, or 10,000,000. 
```

<b>Octal and hexadecimal literals: </b>
A hexadecimal literal begins with an optional minus sign, followed by “0x” or “0X,” followed by a sequence of digits from 0-9 or letters A-F. 
```
ex: -0123 	//octal
    -0xCAFE911	// hexadecimal
```

<b>Floating point literals: </b>
```
ex: 1.413 or 6.02e+23. 
```

<b>String literals: </b>
```
ex: “learn” or “3.14” or ‘name = “my page”’. 
```

<b>template literals vs objects literals:</b>	
					?????


<br/>

### Literal vs  Constant
<b>A literal is a value that is expressed as itself.</b> 
For example, the number 25 or the string "Hello World" are both literals. 

<b>A constant is a data type that substitutes a literal.</b> 
Constants are used when a specific, unchanging value is used various times during the program.



<br/>


## Identifiers (name given to a variable):
<b> rules for identifier (naming a variable)</b>
- must be a combination of character	(“atleast 2 characters”).
- a combination of characters & numbers (“first characters must be a character”).
- may start with _ .
- must not be a keyword.

<b>example:</b>
```js

// Naming Conventions for identifiers( variable names )
// camelCase
    let firstName = "malik"			// camelCase is recommended
// PascalCase
    let FirstName = "malik"
// Snake_Case
    let First_Name = "malik"

```

<br/>


### Constant Identifiers (const variablename):
```js
 const val = 2;	// ‘const’ means that the identifier can't be reassigned.
```

> <b>note: 📝</b> <br> a const must be initialised at the time of declaration otherwise it throws error at runtime. <br/>
<details>
  <summary><b>const does allow to change the value in object. but not the object itself</b></summary>
<p>


*Object reference is protected. The following is NOT allowed.*
```js
const obj = { a: 3 };
obj = { b: 5 } // not allowed  
```  

*Object value is not protected. The following IS allowed:*
```js
const obj = { a: 3 };
obj.a = 5;  // allowed
```
</p>
</details>

<table>
<tr>
<td>
  
<a href="#"> <img src="https://user-images.githubusercontent.com/63545175/168561953-b7e7d0d8-38d0-4d31-ba34-a5d84b104456.png"></a>
  
</td>  
<td>
  
<a href="#"> <img src="https://user-images.githubusercontent.com/63545175/168561966-b3306bb7-ad95-4499-9b48-9598efa5cd21.png"></a>
  
</td>  
</tr>
</table>


<br/>



## Variables:
we can use <b>var</b> keyword to declare and initialize variable of any type.

<b>example:</b> 
```js
	Var x =4; 	// the following defines x as a variable and then assigns x the value 14
	let x = 14; 	
```

> <b>tip: 💡</b>  “toFixed” fix float decimal points:
> <br/>	var ans = 10.12345678.toFixed(2) ;	// ans = 10.12


<br/>


## const, var, let? function scoped, block scoped?
<b>function scoped</b> variable is available anywhere inside of the function it is declared in while a <b>block scoped</b> variable is only available inside of the block (if and loops) it is declared in. <b>var is function scoped, const and let are block scoped.</b>


<table>
<tr>
<td>
  
<a href="#"> <img src="https://user-images.githubusercontent.com/63545175/168563849-4748043d-bf52-446c-b0a1-0c76b597c39c.png"></a>
  
</td>  
<td>
  
<a href="#"> <img src="https://user-images.githubusercontent.com/63545175/168563921-3a0aa630-1984-4241-8886-a05e38a9b988.png"></a>
  
</td>  
</tr>
</table>

<br/>

<b>note:</b>
note: 
- <b>var variables</b> can be <b>redeclared</b> and also <b>redefined.</b>
- <b>let variables</b> can’t be <b>redeclared</b> but can be <b>redefined.</b> 
- <b>const</b> can’t be <b><s>redeclared</s></b> and can’t be <b><s>redefined</s>.</b>


<br/>









