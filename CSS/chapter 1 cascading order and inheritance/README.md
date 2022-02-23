# How CSS is rendered and applied
***if you ever got into a problem where, element’s style is not looking or behaving like you intended.  
this is a very common problem and below can be the solution.***

_"Conflicts between CSS rules addressing the same element may arise. 
Most of them can be solved by considering the rules of cascading order and inheritance._"

<br/>

## CASCADING ORDER &nbsp;&nbsp;&nbsp; “cascading means flowing down”
HTML documents are loaded and read sequentially from top to bottom, so it is important where a style attribute is declared. 
<br/>CSS rules written further below in a file will be read and interpreted later than the ones at the top. 
<br/>This applies for one CSS file as well as for the whole HTML document incorporating many styles. 

<br/>

<details>
<summary><b>
Que: what happens when we have two different rules for same element?
</b></summary>
<p>
 
**Ans:** the last rule being read will get applied to the element.

<br/> 
</p>
</details>


<details>
<summary><b>
Que: but what happens when we add inline CSS? while having rule with same property for same element in external  CSS.
</b></summary>
<p>
 
**Ans:** in case of external CSS and inline CSS, rules in the CSS file will get ignored. and inline CSS will get applied.
The reason is that the reference to CSS file being in head, firstly external CSS is loaded in the background. Subsequently, the inline CSS is loaded and interpreted together with the HTML file and therefore overwrites the previous rules.

**note:** _if there are two different rules for different properties for same element then both rules are applied, even if they are in different external files and even if one is inline while other is external._
 
<br/>
</p>
</details>


<details>
<summary><b>
Que: what happens when external and internal CSS come together?
</b></summary>
<p>
 
**Ans:** this is easy. It depends on the order in which they are declared. 
when first an external style is referenced and then  the internal style will be applied. 
the last rules being interpreted will result in final style .
 
</p>
</details>

<br/>

<details>
<summary>
💡 <b><em> tip: </em></b>
</summary>
<p>
 
- When using all three variants of CSS (e.g. on big websites) you usually reference the external styles first, then apply an internal CSS to the HTML file (e.g. a subsite), and then sometimes use inline CSS for quick tests.
 
***For this scenario the cascading order would be:	“cascading means flowing down”***
1.	The browsers default is applied first (= the user settings).
2.	Then the external styles are loaded.
3.	Then the internal style is added.
4.	And finally the inline style is applied.
</p>
</details>

<br/>
 
<br/>

***Besides the cascading order, there is another main reason why an HTML element’s style might not look or behave like you intended.***

<br/>

## INHERITANCE of properties from Parent element by Child elements in HTML 
In case of nested elements inside HTML, 
***There are two kinds of style “properties”:*** 
- those that are, always inherited (_they have values inherited from parent element)._ 
- and those that are, not inherited by default, _and have initial (default values)._

<b><em> example: </em></b>
<div align="center">
<img width="850" src="../images/inheritance-css.png" alt="example of inheritance">
</div>
 
**note:** Here, the color property as well as the font-size property are inherited automatically, whereas the border property is not inherited.

<details>
<summary>
 💡 <b><em> tip: </b></em>
</summary>
<p>

In many cases you have to find out yourself what properties are inherited and which not. But as a rule of thumb, most text- and font-related properties are inherited and everything size- and positioning-related is not. 
<br/>You can take a look at <a href="https://www.w3.org/TR/CSS21/propidx.html" title="W3 school"> _this_ </a> slightly outdated list of properties and their inheritance status. 
</p>
</details>

<br/>

### Controlling Inheritance
***also, you can manually overwrite inherited properties or force inheritance.***

#### Inherit
Child element inherit style properties from Parent element.
```HTML
<div style= “color: blue;”>
        <p style= “color: inherit; ”> HELLO! </p>
</div> 
```

#### Initial
Child element use its default value for the property. “remember they are set by browser”
```HTML
<div style= “color: blue;”>
        <p style= “color: initial; ”> HELLO! </p>
</div>
```

#### Unset
The unset  CSS keyword resets a property to its inherited value if the property naturally inherits from its parent, and to its initial value if not.


<br/>

## Specificity  and !important  keyword 
### what is specificity ?
_If there are two or more conflicting CSS rules that point to the same element, the browser follows some rules to determine which one is most specific and therefore wins out.
<br/>Think of specificity as a score/rank that determines which style declarations are ultimately applied to an element._

### Specificity Hierarchy
_There are four categories which define the specificity level of a selector:_
- **Inline styles** - ``Example: <h1 style="color: #ffffff;">.``
- **IDs** - An ID is a unique identifier for the page elements, such as #navbar.
- **Classes, attributes and pseudo-classes** - This category includes .classes, [attributes] and pseudo-classes such as :hover, :focus etc.
- **Elements and pseudo-elements** - This category includes element names and pseudo-elements, such as h1, div, :before and :after.

**note:** *The universal selector ``(*)`` has low specificity, while ID selectors are highly specific! , learn to calculate specificity here.*
 
### ***examples*** :
<div align="center">
<img src="../images/specificity examples.png" alt="examples" width="650"> 
</div>

<br/>

### **``!important`` Keyword**
- “this keyword increases the specificity of a property to infinity”. 
- technically it overrules every other CSS rule Present for the same property.

<table align="center">
<tr>
<td>
<img src="../images/important keyword in css rule.png" alt="example" width="900">
</td>
</tr>


<br/>






