## input and output
***Output:***
```js
console.log("running")                // console mostly used for debug
alert("what, what, what, ")           // pop up dialogue
document.write("hellow");             // web page
```

***input:***
```js
var age = prompt("tell me your age?")					// pop up
```


<br/>

<br/>


## Alert vs prompt vs confirm

An ***alert box*** is used when you want to ensure that information gets through to the user.
<br/>When an alert box pops up, the user must click OK to proceed.
<br/>The alert function takes a single parameter, which is the text displayed in the popup box.
<br/>**example:**
```js
alert("session starts now.")           // pop up dialogue
```

<br/>

A ***prompt box*** is often used to have the user input a value before entering a page.
<br/>When a prompt box pops up, the user will have to click either OK or Cancel to proceed after entering the input value.
<br/>If the user clicks OK, the box returns the input value. If the user clicks Cancel, the box returns null.
<br/>***The prompt() method takes two parameters:-*** 
- The first is the label, which you want to display in the text box.
- The second is a default string to display in the text box (optional).

**example:**
```js
var age = prompt("tell me your age?", "Age in Numbers");
```

<br/>

A ***confirm box*** is often used to have the user verify or accept something.
<br/>When a confirm box pops up, the user must click either OK or Cancel to proceed.
<br/>If the user clicks OK, the box returns true. If the user clicks Cancel, the box returns false.
<br/>**example:** 
```js
var result = confirm("Do you really want to leave this page?");
if (result == true) {
    alert("Thanks for visiting");
}
else {
    alert("Thanks for staying with us");
}
```


<br/>

<br/>


## Note: 
***most of the time js will be used to modify and add html elements to the web page.***
