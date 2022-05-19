# types of selector:
- ???
	- <a href="#simple-selector"> Simple Selector </a>
	- <a href="#multiple-selector"> Multiple Selector </a>
	- <a href="#universal-selector"> Universal Selector / All Selector </a>
	
- ???
	- <a href="#element-selector"> **Element Selector** </a>
	- <a href="#class-selector"> **Class Selector** </a>
	- <a href="#id-selector"> **Id Selector** </a>
	
- ???
	- <a href="#Attribute-Selector"> **``Attribute Selector``** </a>
	- <a href="#Pseudo-Elements-Selector"> **``Pseudo-Elements Selector``** </a>
	- <a href="#Pseudo-class-selectors"> **``Pseudo-Class Selectors``** </a>
		
- <a href="#Combinator-Selectors">Combinator Selectors</a>
	- <a href="#Combinator-Selectors"> ***Descendant Combinator*** </a>
	- <a href="#Combinator-Selectors"> ***Child Combinator (>)*** </a>
	- <a href="#Combinator-Selectors"> ***Adjacent Sibling Combinator (+)*** </a>	
	- <a href="#Combinator-Selectors"> ***General Sibling Combinator (~)*** </a>	


<br/>

<br/>

<br/>

---
## <a name="simple-selector"></a> ``“simple selector”``
- “simple selector selects elements based on <b>name / id / class</b> ” 

***remember: A CSS rule looks like this:***
```css
  selector {property: value; ...}
```
**tip: 💡** _when a simple selector select elements based on element tag it is known as element selector, when a simple selector selects element based on id its called id selector and when it selects based on class its called class selecter._

<br/>

## <a name="multiple-selector"></a> ``“Multiple selector”``
***The CSS rule for addressing multiple HTML elements looks like this:***
```css
  selector1, selector2, selectorN {property: value;}
```
```css
  p,div,header {text-align: center;}	//This is the CSS rule to center all paragraphs.
```

<br/>

## <a name="universal-selector"></a> ``“Universal selector”  All Selector``
- The all (or universal) selector simply addresses the whole content of the HTML document and therefore also includes the <body></body> element. 

***The CSS rule for styling the whole content of a website looks like this:***
```css
  * {property: value;}
```
**example:** _below is the CSS rule for centering the text of every element of the HTML document and giving them a lightblue background_.
```css
  * {text-align: center; background-color: lightblue;}
```

<br/>

<br/>

<br/>

---

## Element Selector  
***The CSS rule for addressing certain HTML elements looks like this:***
```css
  	tag {property: value;}
```
```css
	p {text-align: center;}			//This is the CSS rule to center all paragraphs.
```

<br/>

## <a name="class-selector"></a> Classes  “class selector”
***The CSS rule for addressing multiple elements with same class attribute is:***
```
  .class-name {property: value;…}		// CSS rule to style any elements that use this class
```
**Note: 💡** _that one class can be assigned to several HTML elements and that one HTML element may have several classes._
**tip:** _To assign several classes to one HTML element, use only one class attribute and separate the different class names by a blank space as in the example below._
<b>
```html
<tag name class="class-name-1 c	lass-name-2"> content </tag name>
```
</b>

<br/>

***example:***
<table>
<tbody>
<tr>
<td>


Inside CSS
</td>
<td>


Inside HTML body
</td>
</tr>
<tr>
<td>


```css
.class-center{text-align: center;}

.class-right{text-align: right;}

.class-color{color: blue;}
```
</td>
<td>


```html  
<h1 class="class-center">Welcome to mysite</h1>
<h3 class="class-right">im happy to help</h3>
<p class="class-right">
        im very much glad that you choose to develop this site.</p>
<footer class="class-center class-color"> 
                   aren't you a celebrity. i won't tell anybody</footer>
```
</td>
</tr>
<tr>
<td colspan="2">
<p><strong>Output:</strong></p>


<img src="https://user-images.githubusercontent.com/63545175/163440233-19c06ac0-c6f3-46f1-8c81-a4ee71265d58.png">  
	  
</td>
</tr>
</tbody>
</table>

<br/>

## <a name="id-selector"></a> IDs	“ id selector ”
***Addressing an ID in CSS is simply done by using a hashtag (#) in front of the id name.***
```css
  #id-name { ... }
```

**Tip: 💡**  <em><b>``/* IDs are very useful, especially if you have single HTML elements which must be styled in a different way. */``</b></em>

**note:** 
- IDs are similar to classes. 
- The main difference is that an ID can only be assigned once. 
- It is not allowed to give another HTML element the same ID as IDs are unique. 
- For assigning IDs, use the HTML attribute id. 
- Again its value id-name represents the assigned ID and is of your choice as long as it is unique in the HTML document.

```html
  <tag name id="id-name"> content </tag name>
```

<br/>

**tip: 💡** 
- However, assigning meaningless IDs, e.g. div1, won’t be of any use. 
- Such IDs make your code less readable and if you’ve got several of them, you won’t know the difference between them later on. 
- So come up with meaningful ID names, even if it takes some time. 
- Like class names, it is considered good coding practice to separate id names composed of more than one word with a hyphen.

<br/>

**tip: 💡** 
<b>_“remember in html ``label element`` also use value of id attribute in its ``for attribute``, this is the same id attribute that is addressed by id selector"_</b>

<br/>

<br/>

<br/>

---
## <a name="Attribute-Selector"></a> Attribute selectors 
***The [attribute] selector is used to select elements with a specified attribute.***

***syntax:***
```css
	element[attribute] {property: value;…}		      // element with this attrib any value
```
**Note: ``📝``** <b><em>``The [attribute="value"] selector is used to select elements with a specified attribute and value.``</em></b>
```css
	element[attribute= “value”] {property: value;…}	      // element with this attrib and this value
```

***example:***
```css
	a[href= “www.example.com ” ]{
		property: value;
	}
```

### All CSS Attribute selectors:
<b>

<table>
<thead>
<tr>
<th>Selector</th>
<th>Example</th>
<th>Example description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>[attribute]</code></td>
<td><code>[target]</code></td>
<td>Selects all elements with a target attribute</td>
</tr>
<tr>
<td><code>[attribute=value]</code></td>
<td><code>[target=_blank]</code></td>
<td>Selects all elements with <code>target=&quot;_blank&quot;</code></td>
</tr>
<tr>
<td><code>[attribute~=value]</code></td>
<td><code>[title~=flower]</code></td>
<td>Selects all elements with a <code>title</code> attribute containing the word <code>&quot;flower&quot;</code></td>
</tr>
<tr>
<td><code>[attribute|=value]</code></td>
<td><code>[lang|=en]</code></td>
<td>Selects all elements with a <code>lang</code> attribute value <code>starting</code> with <code>&quot;en&quot;</code></td>
</tr>
<tr>
<td><code>[attribute^=value]</code></td>
<td><code>a[href^=&quot;https&quot;]</code></td>
<td>Selects every <a> element whose <code>href</code> attribute value <code>begins</code> with <code>&quot;https&quot;</code></td>
</tr>
<tr>
<td><code>[attribute$=value]</code></td>
<td><code>a[href$=&quot;.pdf&quot;]</code></td>
<td>Selects every <a> element whose <code>href</code> attribute value <code>ends</code> with <code>&quot;.pdf&quot;</code></td>
</tr>
<tr>
<td><code>[attribute*=value]</code></td>
<td><code>a[href*=&quot;w3schools&quot;</code>]</td>
<td>Selects every <a> element whose <code>href</code> attribute value <code>contains</code> the <code>substring</code> <code>&quot;w3schools&quot;</code></td>
</tr>
</tbody>
</table>

 
</b>	

<br/>


## <a name="Pseudo-Elements-Selector"></a>Pseudo-elements selectors

_A CSS pseudo-element is used to <b>``style specified parts of an element.``</b>_
	
***For example, it can be used to:***
- Style the first letter, or line, of an element
- Insert content before, or after, the content of an element

***syntax:***
```css	
	selector::pseudo-element {
	  property: value;
	}	
```	
	
###  All CSS Pseudo Elements:

<b>


|Selector |	Example |	Example description |
|---------|-------------|---------------------------|
| ``::after`` | ``p::after``	| Insert something after the content of each <p> element. |
| ``::before`` | ``p::before``	| Insert something before the content of each <p> element. |
| ``::first-letter`` | ``p::first-letter``	| Selects the first letter of each <p> element. |
| ``::first-line`` | ``p::first-line``	| Selects the first line of each <p> element. |
| ``::marker`` | ``::marker``	| Selects the markers of list items. |
| ``::selection`` | ``p::selection``	| Selects the portion of an element that is selected by a user. |

</b>	
	
<br/>

## <a name="Pseudo-class-selectors"></a> Pseudo-class selectors  <b><em>``important and amazing``</em></b>
_A pseudo-class is used to <b>``define a special state of an element.``</b>_

***For example, it can be used to:***
- Style an element when a user mouses over it.
- Style visited and unvisited links differently.
- Style an element when it gets focus.

***syntax:***
```css
	selector:pseudo-class {
	  property: value;
	}
```

### All Important CSS Pseudo Classes:

<b>	


| Selector	| Example	| Example description | 
|---------------|---------------|---------------------|
| ``:active`` | ``a:active`` |	Selects the active link |
| ``:hover`` | ``a:hover`` |	Selects links on mouse over |
| ``:link`` | ``a:link`` |	Selects all unvisited links |
| ``:visited`` | ``a:visited`` |	Selects all visited links |
| ``:target`` | ``#news:target`` |	Selects the current active #news element (clicked on a URL containing that anchor name) |
| ``:checked`` | ``input:checked`` |	Selects every checked ``<input>`` element |
| ``:disabled`` | ``input:disabled`` |	Selects every disabled ``<input>`` element |
| ``:enabled`` | ``input:enabled`` |	Selects every enabled ``<input>`` element |
| ``:focus`` | ``input:focus`` |	Selects the ``<input>`` element that has focus |
| ``:in-range`` | ``input:in-range`` |	Selects ``<input>`` elements with a value within a specified range |
| ``:out-of-range`` | ``input:out-of-range`` |	Selects ``<input>`` elements with a value outside a specified range |
| ``:valid`` | ``input:valid`` |	Selects all ``<input>`` elements with a valid value |
| ``:invalid`` | ``input:invalid`` |	Selects all ``<input>`` elements with an invalid value |
| ``:optional`` | ``input:optional`` |	Selects ``<input>`` elements with no "required" attribute |
| ``:required`` | ``input:required`` |	Selects ``<input>`` elements with a "required" attribute specified |
| ``:root`` | ``root`` |	Selects the document's root element |

</b>
	
***tip: 💡*** _use curser property inside hover. ``ex: cursor: pointer;`` and enjoy the result._
	
<br/>

<br/>

<br/>

---
	
# <a name="Combinator-Selectors"> Combinator selectors 
Combinator Selector select elements based on a specified relationship between them.

> ***"A combinator is something that explains the relationship between the selectors."***

A CSS selector can contain more than one simple selector. Between the simple selectors, we can include a combinator.

***There are four different combinators in CSS:***
- descendant selector (space) 
- child selector (>)
- adjacent sibling selector (+)
- general sibling selector (~)

<br/>

	
> <b>Note: 💡</b> ``div{...}`` selects all div elements. ``div {...}`` selects all elements that are descendents of div,  ``div p{...}`` selects all ``<p>`` elements that are descendents of ``div``. 

<br/>	
	
<b>


| Selector	| Example	| Example description| 
|---------------|---------------|--------------------|
| ``element element {…}`` | ``div p {…}``	| ``Selects all <p> elements that are descendants of <div> elements.`` |
| ``element>element {…}`` | ``div > p {…}``	| ``Selects all <p> elements that are child of <div> elements.`` |
| ``element+element {…}`` | ``div + p {…}``	| ``Selects the first <p> element that are placed immediately after <div> elements.`` |
| ``element1~element2 {…}`` | ``p ~ ul {…}``	| ``Selects every <ul> element that are preceded by a <p> element.`` |

</b>


<br/>

	
### Descendant Combinator
The descendant selector matches all elements that are descendants of a specified element.
The following example selects all ``<p>`` elements inside ``<div>`` elements: 
```css
	div p {
	  background-color: yellow;
	}
```

<br/>	


### Child Combinator (>)
The child selector selects all elements that are the children of a specified element.
The following example selects all ``<p>`` elements that are children of a ``<div>`` element:
```css
	div > p {
	  background-color: yellow;
	}
```

<br/>	


### Adjacent Sibling Combinator (+)
The adjacent sibling selector is used to select an element that is directly after another specific element.
Sibling elements must have the same parent element, and "adjacent" means "immediately following".
The following example selects the first ``<p>`` element that are placed immediately after ``<div>`` elements:
```css
	div + p {
	  background-color: yellow;
	}
```
	
<br/>

	
### General Sibling Combinator (~)
The general sibling selector selects all elements that are next siblings of a specified element.
The following example selects all ``<p>`` elements that are next siblings of ``<div>`` elements: 
```css
	div ~ p {
	  background-color: yellow;
	}
```



	
	
