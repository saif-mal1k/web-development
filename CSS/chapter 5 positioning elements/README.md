# positioning elements

---

## display property
  - Every HTML element has a default display value depending on what type of element it is. The default display value for most elements is block or inline.
  - ✅ Yes! block elements can contain inline elements
  - ❌ No! inline elements can't contain block elements

***using diplay property we can set its value to -***
  - **inline** , does'nt allow to set width & height.
  - **block** , allow to set width & height and padding & margin. also automatically add line-break after element.
  - **inline-block** , allow everything block allow but does'nt automatically add line-break after element. 

<br/>
 
***want to Hide an Element? set***
```css
display:none; 
```
or 
```css
visibility:hidden;
```


<br/>

<br/>

---

## position property
  -	position property can have one of ***static*** , ***relative***, ***absolute*** as value.
  -	more types of position can be ``position: fixed;`` , ``position: sticky;`` …
  -	***positioning CSS(offset) properties are left, right, top, bottom***

### ``static`` positioning
- default positioning type for all, except html( _html is relative by default_).
- does not allow positioning offsets.

### ``relative`` positioning
- element is not moved out of normal document flow. (even if moved, its original spot is preserved)
- offsets are applied relative to its position in the normal document flow.

<details>
  <summary> <b><em>example:</em></b> </summary>
<p>

<image src="https://user-images.githubusercontent.com/63545175/187066229-9747a9de-ab3a-49c6-8b21-773631c1ec90.png" width="500px">

**tip:** from top 50px towards bottom. similarly, from left 50px toward right.

<image src="https://user-images.githubusercontent.com/63545175/187066431-ebcc7b00-dad6-4580-b7e1-bc384b0cf837.png" width="500px">
  
</p>
</details>  
  

### ``absolute`` positioning
- requires containing element with its position set to relative.
- on position absolute for contained element, element is moved out of normal document flow, and everything else behave like its not there.
- offsets are applied relative to container(containing element).
  
<details>
  <summary> <b><em>example:</em></b> </summary>
<p>

***without any position property, element1 and element2 both in document flow.*** <br/> note: the container element has its position set to relative.
  
<image src="https://user-images.githubusercontent.com/63545175/187066544-5d52cad1-f106-4cf5-b945-12708f624650.png" width="540px">

***position: absolute;  applied to element1 , hence element1 out of document flow. like it’s not even there. and hence, everything inside container will behave like it’s not even there.***  

<image src="https://user-images.githubusercontent.com/63545175/187066564-f0a6e2b8-0408-4118-90f5-14d037a445b1.png" width="540px">

***if we apply offset they will be relative to container element. and the container element must be position relative.***

<image src="https://user-images.githubusercontent.com/63545175/187066579-20015467-84fe-4f9b-a12a-fcbfdddf5a8c.png" width="540px">

***important: if container element is offset, everything inside will offset with it.***

<image src="https://user-images.githubusercontent.com/63545175/187066793-a16ef67e-86c3-4c4c-a3a4-a8ea87b45710.png" width="540px">

  
</p>
</details>



### ``fixed`` positioning
- ***fixed positioning works relative to the browser window.*** i.e, ***if you resize the browser window it moves with it.***
- element is moved out of the normal document flow.



### ``sticky`` positioning???
- ????



<br/>

<br/>

---
  
## Z-INDEX
 - controlls the stacking order of the elements.
 - https://youtu.be/UO8ed-JB4So?t=1002 ?????
  


<br/>

<br/>

---

## positioning elements by floating

### float	(left, right)
It specifies whether the box should float left or right. float property makes an element rise out of document flow.	

### clear	(left, right, both, none)
The clear property is used to avoid elements after the floating elements which flow around it. “to avoid certain elements from flowing around floating elements”

note: when you float elements the browser takes them out of the regular document flow.

  
  



<br/>

<br/>

---






  
