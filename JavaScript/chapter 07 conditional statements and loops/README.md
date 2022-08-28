## JavaScript Statements:

 although it is not necessary to use <b>“ ; ”</b> for single line statements but it is always recommended to always end statements with a semi-colon <b>“ ; ”</b>.

<br/>


## equality and strict equality

== is used for comparing two variables, but it ignores the datatype of variable. 
type coercion still happens with regular (==) equality. i.e, at first it implicitly converts (type coercion) datatype of one variable to match that of another. then compares the variables. 

=== is used for comparing two variables, but this operator also checks datatype and then compares two values. 
Strict (===) prevents type coercion. i.e, this strict comparison operator compares data in its original form. 

<b>example:</b>
```js
if (4 == “4”)		//returns true
if (4 === “4”) 		//returns false
```

<br/>


## Boolean true and false:
```js
- 0, null, NaN, undefined, “” , false,		<---------they all coerce to being false.

- true, “Hello”, 1, -1, “false”	 		<---------they all coerce to being true.
```


<br/>


## Conditional Statements:
### ⋅	if else if
```js
if (expression)
	statements;
else if (expression2)
	{statements;}
else{statements;}
```

><b>tip: 💡</b> don’t forget <b>false && false</b> evaluate to <b>false</b>.


<br/>


### ternary operator
```js
var ans = conditional ? (if condition is true) : (if condition is false);
```


<br/>

<br/>  
  
  
## switch case statement:
```js  
var expression = prompt (“enter your choice”);
switch (expression){
	case value1:
		statements;
		break;
	case value2:
		statements;
		break;
	default:
		statements;
}
```
  
> <b>note: 📝</b> if you don’t use break then every case after the switched case will also get executed, sometimes that is also useful.  

  
<br/>
  
  
<br/>  
  
  
## Loops (for loop, while loop, for Each loop):
- always make sure you have all 3 start , stop, step coditions.

<b>while:</b>
```js
while (expression){
	statements;
}
``` 
  
<b>do while:</b>
```
do {
	statements;
} while(expression);
```

> <b>note: 📝</b> In do while, Note the semicolon used at the end of the do...while loop. This is important.

  
<br/>
  
  
<br/>  
  
  
  
## for loop 	- loops through a block of code a number of times
```js  
for (initialization; condition; updation;){
    statements;
  }
```
  
- initialization statement is executed (one time) before the execution of the code block.
- condition statement defines the condition for executing the code block.
- updation statement is executed (every time) after the code block has been executed.

### for/of 		- loops through the values of an iterable object
```js  
for (each of object) {
        statements;
}
```

### for/in 	- loops through the properties of an object
```js  
for (key in object) {		// each can be key or value
    statements;
}
```  

<br/>
  
  
<b> example of for/of & for/in: </b>
    
<table>  
<tr>
<td>

![image](https://user-images.githubusercontent.com/63545175/168578977-51b1a068-ce0b-4e8a-b604-23ca239ecde6.png)

</td>  
<td>

![image](https://user-images.githubusercontent.com/63545175/168578995-b9492beb-60ff-44bf-867b-8d8c00b4bb3f.png)

</td>  
</tr> 
</table>  

<br/>
  
### forEach 		- loops through each value in an array
```js
const array1 = ['a', 'b', 'c'];

array1.forEach(element => console.log(element));
```

<details>
<summary> <b><em>ways to use for each</em></b> </summary>
<p>

```js  
// Arrow function
forEach((element) => { /* … */ })
forEach((element, index) => { /* … */ })
forEach((element, index, array) => { /* … */ })

// Callback function
forEach(callbackFn)
forEach(callbackFn, thisArg)

// Inline callback function
forEach(function(element) { /* … */ })
forEach(function(element, index) { /* … */ })
forEach(function(element, index, array){ /* … */ })
forEach(function(element, index, array) { /* … */ }, thisArg)
```
</p>
</details>


  
  
  
