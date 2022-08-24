## Box model:
***every element is surrounded with a box.***

![image](https://user-images.githubusercontent.com/63545175/186343526-922e7126-bb1c-4d15-b416-de51c2074da9.png)

<table>
<tr>
<td> 
  
  - ***Margin:*** The margin defines the area between an element’s border and the box of another element. An element’s background color does not apply to the margin! . since, The margin is transparent, margin includes background color of parent element.  
  - ***Border:*** An element’s border wraps content and padding.
</td>
<td> 
  
  - ***Padding:*** The padding creates a gap between the element’s content and border. since, The padding is transparent, The element’s background color applies to the padding as well!
  - ***Content Area:*** Contains the actual content.
</td>
</tr>
</table>


<br/>

<br/>

---

### Width & Height property
***Before setting width and height properties for an element, it’s important to consider which parts of the box model are addressed with these properties-***

  - ***```box-sizing: content-box;```***   default (width and height apply only to the content area).
  - ***```box-sizing: border-box;```***   means that width and height take sum of (border + padding + content).

<table>
<tr>
<td> 
  
***content-box***
  
</td>
<td> 
  
***border-box***
  
</td>
</tr>
<tr>
<td> 
    
![image](https://user-images.githubusercontent.com/63545175/186345543-83e96ac9-0200-4663-8b16-01c81dfde32b.png)

![image](https://user-images.githubusercontent.com/63545175/186345564-dbd476da-408c-4e32-87a5-769576ba9785.png)
  
</td>
<td> 
    
![image](https://user-images.githubusercontent.com/63545175/186345707-b9ae20d7-1e48-4f83-9956-cea9de28d394.png)

![image](https://user-images.githubusercontent.com/63545175/186345738-6edf4bb3-2927-4adc-a75a-1a00ef6862ea.png)

</td>
</tr>
</table>


<br/>

***note:** remember box-sizing is not inherited property means child won’t inherit box-sizing property from parent element, it has to use its own*


<br/>

<br/>

---

### Margin property
```css
  margin: 25px 50px 75px 100px;  /* top right bottom left */
```

```css
  margin: 20px;			/* applies 20px in all */
```

***Note:* 📝** **Negative values are not allowed.**

> ***tip:* 💡** **You can set the margin property to auto to horizontally center the element within its container**. The element will then take up the specified width, and the remaining space will be split equally between the left and right margins.



#### important note 📝
<img src="https://user-images.githubusercontent.com/63545175/186353007-115d39ac-cc1a-41d0-bd64-2777e03b1c6b.png" width="480px"> <img src="https://user-images.githubusercontent.com/63545175/186353025-6dbaf0c4-a412-4fcf-9388-51373596f986.png" width="480px">


<br/>

<br/>

---

### Overflow Property 
***what is Overflow? why it happens “ learn here: https://youtu.be/wKPlQkOdpFQ?t=1058 ”***

![image](https://user-images.githubusercontent.com/63545175/186355612-75b3ce86-d19a-452e-b67e-1f9b7395dc73.png)


<br/>

### how to control overflow: 	
The overflow property specifies whether to clip the content or to add scrollbars when the content of an element is too big to fit in the specified area.

*The **overflow property** has the following values:*
  - **visible** - Default. The overflow is not clipped. The content renders outside the element's box
  - **hidden** - The overflow is clipped, and the rest of the content will be invisible
  - **scroll** - The overflow is clipped, and a scrollbar is added to see the rest of the content
  - **auto** - Similar to scroll, but it adds scrollbars only when necessary


> ***Note:* 📝  
> The overflow property works only for block elements with a specified height. <br/>
> the element must have (width and/or height). Otherwise, the element will just grow with its content.**


***to set the direction of overflow we can use-***
  - **overflow** property gives both vertical and horizontal overflow.
  - **overflow-x** property provides only horizontal overflow, *values are same as overflow property*.
  - **overflow-y** property provides only vertical overflow, *values are same as overflow property*.

<br/>

<br/>

---




