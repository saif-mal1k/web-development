## anchor tag:
```HTML
<a href=“https://path”  target=“_blank” >	           <!- - attribute target =“_blank” makes it open in new tab. - ->
```
### values for the target attribute:
<table>
  <tr>
    <td> _blank </td>		<td> “Loads the linked document in new tab” </td>
  </tr>
  <tr>
    <td> _self </td>	 <td> “Loads in the same frame which held the link” </td>
  </tr>
  <tr>
    <td> _parent </td>	<td> “loads in Parent frame ” </td>
  </tr>
  <tr>
    <td> name of frame </td>  <td>	“loads in the named frame” </td>
  </tr>
</table>

**note:** frame element has attribute name= “ ” that allows us to name the frame. 


###  title attribute:
<table>
<tr>
<td> title = “text that will be displayed when hover over by mouse” </td>
</tr>
<tr>
<td>
  
```HTML
  <a href="https://www.google.com" title="secret msg"> Hover Over </a>
```
</td>
</tr>
<tr>
<td> <b> output: </b> 
<br/> &nbsp; <a href="https://www.google.com" title="secret msg"> Hover Over </a> 
</tr>
</table>  

<br/>


## related link vs absolute link?


<br/>

## Internal linking to other pages in the same site:
<table>
<tr>
<td width="300" align="center">
  
**Moving into the folders** 
</td>
<td width="300" align="center">
  
**Moving out of the folders**  
</td>
</tr>
<tr>
<td>
  
</td>
<td>

``../`` _used to go outside a folder._
``../../`` _used to go two folders back._
</td>
</tr>
</table>

**tip:** use attribute target = ``“_self”``  to make it open in same frame.

<br/>

## External linking to other websites:
```html
<a href=“https://link”  target=“_blank” > 	      
  
<!-- don’t forget to include full link with https -->
```
**tip:** use attribute target = ``“_blank”``  to make it open in new tab.

<br/>
  
## linking to the sections of a document or sections of same page:
```html
<a href= “#section2”> goto section 2</a>		
<section id= “section2”>
	lorem ipsum gutyt saukg aruvz ufszbu sryjncs ...
</section>

<!-- used as fragment identifiers as it adds #sectionname in url -->
```








  
