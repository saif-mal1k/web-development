
## Syntax of a CSS rule
***A CSS rule looks like this:-***
```CSS
	  selector {
	  	property: value; 
	  	...
	  }
```
**note:** _the value here is different from ``<element attribute= “value”> </element>``_
  
<br/>

<br/>

## Ways to add CSS to HTML doc:
### using Style attribute: ( inline CSS)
using the style attribute inside your HTML element’s opening tag.
```HTML	
  <h1 style="text-align: center; font-family: Georgia ; ">Welcome to mysite</h1>
```
**tip:** _The advantage of this technique is that you can style every element individually._ 
<br/>_But the drawback is that you must style every element individually which can get very time-consuming and cumbersome._


### Internal CSS
using the ``<style></style>`` element inside the ``<head></head>`` of html document. 
```HTML
<head>
      <style>
        	#index-heading{ text-align: center; font-family: Georgia ;}
        	.class-align-right{text-align: right;}
      </style> 
</head>
```
**note:** _Inside this ``<style></style>`` element you can write CSS._


### External CSS
using a link element (to reference to your external CSS file) in the head of your HTML file.
```HTML
<head>
	<link rel="stylesheet" href="path/name.css" />
</head>
```
<details>
  <summary>
    <b> 💡 tip: </b>
  </summary>
<p>

-	often, Using internal and inline CSS leads to bad code, since structure and style are not seperated and after some time they are hard to manage. This is why external CSS is the standard in web-development.
- There is no limit on how many stylesheets you can include. Simply add as many <link /> tags as you wish. Of course, online sources are also possible. However, too many online sources may slow down your app.
- you can use _Inline CSS_ for debugging, _Internal CSS_ for certain properties to be applied to a single page, all that while using _External CSS._

</p>
</details>

