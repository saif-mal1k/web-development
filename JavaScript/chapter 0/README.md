# ways to add JavaScript to your html file 

## internal JavaScript:
```html
<head>
    <! –– inside head ––>		
    <script language="JavaScript" type="text/JavaScript">
            // JavaScript code
    </script>
</head>
<body>

    <! –– inside body ––>
    <script>
		/* JavaScript code */
    </script>
</body>
```

<br>

## external JavaScript:
```html
<head>
    <script src="script.js" language="JavaScript" type="text/javaScript">
    </script>
</head>
```

<br/>

<details>
	<summary> 💡 <b><em> script loading strategies? </b></em></summary>
<p>
	
***tip1:*** _it is recommended to include javascript only at the end inside body element, because elements must be rendered before execution of javascript._
<br/> ***tip2:*** _another way to overcome the error, below code can put inside head or anywhere inside body and it must work perfectly._
```html
<script>
	document.addEventListner(“DOMContentLoaded”, function() {
		/*javascript code/functionality/statements that we need */
	});
</script>
```
***tip3:*** _in case of external javascript file we can use an attribute called defer, The defer is a Boolean value, used to indicate that script is executed after the document has been parsed. It works only with external scripts._
```html
<script src="script.js" language="JavaScript" type="text/javaScript" defer></script>
```
