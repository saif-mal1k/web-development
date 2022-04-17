## 💡 Script Loading Strategies?
	
<b><em>tip1:</em></b> <em>it is recommended to include javascript only at the end inside body element, because elements must be rendered before execution of javascript.</em>

<br/> 

<b><em>tip2:</em></b> <em>another way to overcome the error, below code can put inside head or anywhere inside body and it must work perfectly.</em>

```html
<script>
	document.addEventListner(“DOMContentLoaded”, function() {
		/*javascript code/functionality/statements that we need */
	});
</script>
```

<br/>

<b><em>tip3:</em></b> <em>in case of external javascript file we can use an attribute called defer, The defer is a Boolean value, used to indicate that script is executed after the document has been parsed. It works only with external scripts.</em>

```html
<script src="script.js" language="JavaScript" type="text/javaScript" defer></script>
```

<br/>

</p>

<details>
	<summary> <b><em>summary:</em></b> </summary>
<p>

- **async** and **defer** both instruct the browser to download the script(s) in a separate thread, while the rest of the page (the DOM, etc.) is downloading, so the page loading is not blocked by the scripts.

- If your scripts should be run immediately and they don't have any dependencies, then use ***``async``***.

- If your scripts need to wait for parsing and depend on other scripts and/or the DOM being in place, load them using ***``defer``*** and put their corresponding <script> elements in the order you want the browser to execute them.
</p>
</details>
	
</details>