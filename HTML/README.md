# HTML notes

<details> 
  <summary><b> how to comment </b></summary>
<p>
    
```HTML
  <!-- this is how to comment -->
```
</p>
</details>
  
<details>
  <summary>
    <b> Escape Sequence in HTML </b>
  </summary>
<p>
  
<table>
<tr>
  <td><b> Code </b></td><td><b>	Symbol </b></td><td><b>	Description </b></td>
</tr>
<tr>
<td> 
    
``&quot;``
</td><td>	"	</td><td> Quotation Mark </td>
</tr>
<tr>
<td>

``&amp;`` 
</td><td>	&	</td><td> Ampersand </td>
</tr>
<tr>
<td> 

``&gt;``	
</td><td> >	</td><td> Greater than </td>
</tr>
<tr>
<td> 
  
``&lt;``	
</td><td> <	</td><td> Less than </td>
</tr>
<tr>
<td> 

``&copy;`` 
</td><td>	© </td><td>	Copyright </td>
</tr>
<tr>  
<td> 

``&reg;``	
</td><td> ®	</td><td> Registered trademark </td>
</tr>
<tr>  
<td> 

``&nbsp;``	
</td><td> 	</td><td> Nonbreaking space </td>
</tr>
<tr>
<td> 
  
``&frac14;`` 
</td><td>	¼	</td><td> Fraction of one fourth </td>
</tr>
<tr>  
<td> 
  
``&frac12;`` 
</td><td>	½	</td><td> Fraction of one half </td>
</tr>
</table>
  

  ***note:*** <b>_``&nbsp;`` adds space that won’t break in any screen size._</b>
<br/>_“ when line fill with words the next word goes to next line, in case we want some words to always be together or in same line we use <b>```&nbsp```</b> for space ”_  
</p>
</details>


<details>
  <summary>
    <b>
HTML doc Structure
    </b>
  </summary>
<p>
  
```HTML
<!DOCTYPE html>                 <!-- tells that this is html document -->
<html lang="en"> <!-- "browser/search engine” this document’s body is english -->
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>title of Document</title>
</head>
<body>
    body of Document, actual content to be displayed by browser.
</body>
</html>
```
</p>  
</details>



## HTML Elements:
_elements are defined using tags._
![Screenshot (497)](https://user-images.githubusercontent.com/63545175/152874165-81b07ea5-57fd-4f7a-9c1d-784437ec0f57.png)
<table>
<tr>
<td width=450> 

<a href="#"><img src="https://user-images.githubusercontent.com/63545175/152875163-ffbb5fdd-5aed-4463-8324-b037c5910c53.png" width="420px"></a>
</td>
<td>

**Block Elements:**
<br/>Takes up the full width available, and force a line break (before and after it).
```
  Ex: <div>,<p>,<h1>…<h6>,<ul>,<li>,<table>
```


**Inline Elements:**
<br/>Takes up only as much width as necessary, and does not force any line break.
```
Ex: <span>, <a></a>, <img>, <iframe>
```
  
</td>
</tr>
</table>

***note:*** You can nest inline elements inside block elements but not the other way around.

<details>
<summary>
  💡 more about html elements
</summary>
<p>
    
***tip:*** The most important block element in HTML is the division element ``(<div></div>)``. This element is heavily used and sometimes whole websites or web apps only consist of divisions. The division forces a line break and is often used as a container of other divisions or other HTML elements.
<br/>The counterpart to division is the inline element ``(<span></span>)``. As we learned, inline elements don’t force a line break and hence, divide the content into logical parts.

***tip:*** div and span are non-semantic tags, but their amazing application is  use “they are used for structuring the html document”.

***tip:*** “ in html5 block elements are roughly flow elements, and inline elements are roughly phrasing elements. ”
</p>
</details>
  
 
  
  
  
