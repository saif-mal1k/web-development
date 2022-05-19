## anchor tag:
```HTML
<a href=“https://path”  target=“_blank” >	           
	
<!-- attribute target =“_blank” makes it open in new tab. -->
```

<br/>

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

<b>note: 💡</b> frame element has attribute ``name= “ ”`` that allows us to name the frame. 

<br/>

###  title attribute:
- <b>title = “text that will be displayed when hover over by mouse”</b>, title contains text that will be displayed when hover over by mouse. 

<b><em>example:</em></b>
```HTML
  <a href="https://www.google.com" title="secret msg"> Hover Over </a>
```

<b><em> output: </em></b>
<table>
</tr>
<tr>
<td>  
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
  
<b>Moving into the folders</b> 
</td>
<td width="300" align="center">
  
<b>Moving out of the folders</b>  
</td>
</tr>
<tr>
<td>
	
``/folderName`` 
	
</td>
<td>

``../`` _used to go outside a folder._
``../../`` _used to go two folders back._
</td>
</tr>
</table>

<b>tip:</b> use attribute target = ``“_self”``  to make it open in same frame.

<br/>

## External linking to other websites:

```html
<a href=“https://link”  target=“_blank” > 	      
  
<!-- don’t forget to include full link with https -->
```
<b>tip:</b> use attribute target = ``“_blank”``  to make it open in new tab.

<br/>
  
## linking to the sections of a document or sections of same page:

```html
<a href= “#section2”> goto section 2</a>		
<section id= “section2”>
	lorem ipsum gutyt saukg aruvz ufszbu sryjncs ...
</section>

<!-- used as fragment identifiers as it adds #sectionname in url -->
```








  
