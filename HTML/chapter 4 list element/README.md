# list elements:
## 1. Ordered lists
- Lists in which the sequence of the items is important.
- type : 1, A, a, I, i

<table>
<tr>
<td>

**example:**
</td>
<td>
  
**output:**
</td>
</tr>
<tr>  
<td>

```html
<ol type= “1”>
  <li>Gutenberg develops moveable type (1450s)</li>
  <li>Linotype is introduced (1890s)</li>
  <li>Photocomposition catches on (1950s)</li>
  <li>Type goes digital (1980s)</li>
</ol>
```
</td>
<td>
  
<ol type= “1”>
  <li>Gutenberg develops moveable type (1450s)</li>
  <li>Linotype is introduced (1890s)</li>
  <li>Photocomposition catches on (1950s)</li>
  <li>Type goes digital (1980s)</li>
</ol>
</td>
</tr>
</table>


<br/>




## 2. UnOrdered lists
- Collections of items that appear in no particular order.
- type: square, disc, diamond 

<table>
<tr>
<td width="300">

**example:**
</td>
<td width="300">
  
**output:**
</td>
</tr>
<tr>  
<td>

```html
<ul type= “disc”>
    <li>Serif</li>
    <li>Sans-serif</li>
    <li>Script</li>
    <li>Display</li>
    <li>Dingbats</li>
</ul>
```
</td>
<td>
  
<ul type= “disc”>
    <li>Serif</li>
    <li>Sans-serif</li>
    <li>Script</li>
    <li>Display</li>
    <li>Dingbats</li>
</ul>
</td>
</tr>
</table>



<br/>



## 3. Description lists
- The ``<dl>`` HTML element represents a description list. 
- The element encloses a list of groups of terms (specified using the ``<dt>`` element) and descriptions (provided by ``<dd>`` elements). 
- Common uses for this element are to implement a glossary or to display metadata (a list of key-value pairs).

<table>
<tr>
<td width="300">

**example:**
</td>
<td width="300">
  
**output:**
</td>
</tr>
<tr>  
<td>

```html
<dl>
    <dt>Serif examples</dt>
    <dd>Baskerville</dd>
    <dd>Goudy</dd>
    <dt>Sans-serif examples</dt>
    <dd>Helvetica</dd>
    <dd>Futura</dd>
    <dd>Avenir</dd>
</dl>
```
</td>
<td>
  
<dl>
    <dt>Serif examples</dt>
    <dd>Baskerville</dd>
    <dd>Goudy</dd>
    <dt>Sans-serif examples</dt>
    <dd>Helvetica</dd>
    <dd>Futura</dd>
    <dd>Avenir</dd>
</dl>
</td>
</tr>
</table>


<br/>



## Nested Lists
***💡 tip:*** we can nest list inside another list, so nesting is possible.
<br>***example:***
<table>
<tr>
<td width="300">

```html
<ul type="square">
  <li>sugar</li>
  <li>water</li>
  <ol type="1">
    <li>salt water</li>
    <li>lemon water</li>
  </ol>
</ul>
```
</td>
<td width="300">
  
<ul type="square">
  <li>sugar</li>
  <li>water</li>
  <ol type="1">
    <li>salt water</li>
    <li>lemon water</li>
  </ol>
</ul>
</td>
</tr>
<table>



