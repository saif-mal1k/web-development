
## Compound Statement:
<b>A compound statement is any number and kind of statement grouped together within curly braces. {}</b>
we group multiple statements in a block together so that we can use it (compound statement) where java expects only one statement.

<b>ex:</b>
```js
if (true) true;		// this statement is valid since if is expecting only one statement.
```

<b>but if you want to write multiple statements in place of this true if (true) true; you can only do that by using a compound statement.</b>

<b>ex:</b>
```js
if (true) {
	console.log(“hello!”);
	console.log(“isn’t it awesome”);
	prompt(“what do you say”)
}	// using a compound statement
```


<br/>


<br/>


## Shadowing:
Variable shadowing occurs <b>when a variable of an inner scope is defined with the same name as a variable in the outer scope.</b> In the inner scope, both variables' scope overlap, and the inner shadows outer.

To avoid shadowing, the variable in the function scope should be <b>declared using the var keyword</b> so that it becomes accessible to the function only.

Illegal Shadowing: <b>while shadowing a variable, it should not cross the boundary of the scope</b>, i.e. we can shadow var variable by let variable but cannot do the opposite.

 	 	 
<table>
<tbody>
<tr>
<td>
<p>Illegal shadowing</p>
</td>
<td>
<p>Okay</p>
</td>
<td>
<p>Okay</p>
</td>
</tr>
<tr>
<td>
  
![image](https://user-images.githubusercontent.com/63545175/168575314-1d9689ea-fe63-4c89-bb4e-0af7fe553140.png)

</td>
<td>
  
![image](https://user-images.githubusercontent.com/63545175/168575329-af28c5b9-b690-44f3-b3ec-dc3c3c68a89e.png)

</td>
<td>
  
![image](https://user-images.githubusercontent.com/63545175/168575340-e0b568b2-354f-42f9-850e-66f429ff03ae.png)

</td>
</tr>
<tr>
<td>
<p>Inside block, a&rsquo;s scope overlaps, and <strong>let</strong> <em>variable</em> should not be redeclared. <strong>Error</strong></p>
</td>
<td>
<p>Outer a is function scoped, inner a in block scoped. hence valid.</p>
</td>
<td>
<p>Var is function scoped and now inner a is in different function.</p>
</td>
</tr>
</tbody>
</table>


<br/>


<table>
<tr>
<td colspan="2" align="center">
  <b> important: example of shadowing “REMEMBER IT”  </b> 
</td>  
</tr>
<tr>
<td>
  
```js
var x = 1;

function addTwo() {
  x = x + 2;
}

addTwo();
x = x + 1;
console.log(x);
  
```  
  
</td>  
<td>

```js
var x = 1;

function addTwo(x) {
  x = x + 2;
}

addTwo(x);
x = x + 1;
console.log(x);
  
```
  
</td>  
</tr>
<tr>
<td>
  
  
<b>output:</b> 4 
  
<b>tip:</b>  The variable x is declared in the global scope and used throughout the entire snippet of code. the global variable x is assigned the value of 1.
Then, the function addTwo() increments the variable by 2.
Next, the variable is incremented by 1.
Finally, it's printed out using console.log

  
</td>  
<td>
  
<b>output:</b> 2
  
<b>tip:</b> Here, there are two x variables, one in the global scope and one inside the addTwo() function scope. The global variable x is incremented by 1. Since the global variable's original value was 1, and it was incremented by 1, console.log will print out 2.
The variable assignment inside the function addTwo() only has function scope, so its affect is not reflected outside the function.

  
</td>  
</tr>  
<table>
  
<br/>
  
<b><em>imp summary:</em></b>
- If an identifier is declared in global scope, it's available everywhere.
- If an identifier is declared in function scope, it's available in the function it was declared in (even if function is declared inside the function).
  

<br/>
  
