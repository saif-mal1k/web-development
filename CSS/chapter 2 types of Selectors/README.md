# types of selector:
## ``“simple selector”``
- “simple selector selects elements based on <b>name / id / class</b> ” 

***remember: A CSS rule looks like this:***
```css
  selector {property: value; ...}
```
**tip: 💡** _when a simple selector select elements based on element tag it is known as element selector, when a simple selector selects element based on id its called id selector and when it selects based on class its called class selecter._

<br/>

## ``“Multiple selector”``
***The CSS rule for addressing multiple HTML elements looks like this:***
```css
  selector1, selector2, selectorN {property: value;}
```
```css
  p,div,header {text-align: center;}	//This is the CSS rule to center all paragraphs.
```

<br/>

## ``“Universal selector”  All Selector``
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

## Classes  “class selector”
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
<table width="678">
<tbody>
<tr>
<td width="271">
<p><strong>Inside CSS</strong></p>
</td>
<td width="407">
<p><strong>Inside HTML body</strong></p>
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
  
![image](https://user-images.githubusercontent.com/63545175/163440233-19c06ac0-c6f3-46f1-8c81-a4ee71265d58.png)  
</td>
</tr>
</tbody>
</table>

<br/>

## IDs	“ id selector ”
***Addressing an ID in CSS is simply done by using a hashtag (#) in front of the id name.***
```css
  #id-name { ... }
```

**Tip: 💡**  _``/* IDs are very useful, especially if you have single HTML elements which must be styled in a different way. */``_

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



