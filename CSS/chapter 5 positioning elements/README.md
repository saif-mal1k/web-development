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

<details>
  <summary> <b><em>example:</em></b> </summary>
<p>
  
***image:***
<image src="https://user-images.githubusercontent.com/63545175/188061355-7593d209-b703-442e-afaf-3317df9ea9e6.png" width="480px">

<image src="https://user-images.githubusercontent.com/63545175/188061631-a561e1ab-7d5a-4967-88b7-ccb20c83b005.png" width="720px">


***code:***
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bruntwood.co</title>
    <style>
        
        #main{
            margin-top: 50px;
            width: calc(100vw - 70px) ;
            height: calc(100vh - 140px);
            
            text-align: center;
            font-size: 100px;
        }

        body{
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
                        background: #00fff742;

        }
        #above-the-fold{
            width: calc(100vw - 80px) ;

            height: calc(100vh - 50px);
            padding: 15px;
            margin: 5px;
        }

        header{
            float:left;
        }
        nav{
            float: right;
        }
        nav span{
            
            font-weight: 500;
            display: inline-block;
                        margin: 10px;

            
        }

        span{
            width: 80px;
            padding: 5px;
            text-align: center;
        }

        span:hover{
            font-weight: bolder;
        }
        footer{
            background-color: rgba(186, 157, 147, 0.651);
            height: 100px;
            width: calc(100vw - 60px) ;
                        padding: 15px;

 
        }

        .contactChat{
            position: fixed;
            bottom: 35px;
            right: 35px;;
            border-radius: 50%;
            width: 50px;
            height: 50px;
            text-align: center;
            font-size: 30px;
            background-color: black;
            border-style: solid;
        }

        .contactChat:hover{
            background-color: #00fff7;
            color: black;
        }

    </style>
</head>
<body>
    <div id="above-the-fold">

        <!-- welcome page -->

    </div>

    <div class="contactChat">
        💬
    </div>

    <footer>
        <div>
            <!-- contact info and ... -->
        </div>
    </footer>
</body>
</html>
```
  
</p>
</details>  


### ``sticky`` positioning
- static positioning works just like static positioning. when the offset limits are achieved then it just sticks there.

<details>
  <summary> <b><em>example:</em></b> </summary>
<p>

![image](https://user-images.githubusercontent.com/63545175/188058865-4dd087a6-0d57-4d37-8f6d-cec19d38caa9.png)

***code:***
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sticky positioning</title>
    <style>
        
        .Stickyheading {
            position: sticky;
            position: -webkit-sticky;
            top: 8px;
            width: calc(100% - 40px);
            z-index: 1;
            margin: auto;
            background-color: black;
            color: cornsilk; 
            font-size: x-large;
            padding: 20px 20px 20px 20px;           
        }

        .content {
            margin: 20px 10px 0px 10px;
            padding: 5px 5px 5px 5px; 
            position: relative;
            background-color: #f2f2f2;
            font-size: large;
        }

    </style>
</head>
<body>

    <div class="Stickyheading">
        Cars
    </div>
    <div class="content">
        <p>
        these are the Cars.
        </p>
        <ol type="i" >
            <li>sedan</li>
            <li>hatchback</li>
            <li>coupe</li>
            <li>sports utility vehicle</li>
        </ol>
    </div>

    <br/>
    
    <div class="Stickyheading">
        Bike
    </div>
    <div class="content">
        <p>
        these are the Bikes.
        </p>
        <ol type="i" >
            <li>sportsbike</li>
            <li>cruiser</li>
        </ol>
    </div>

</body>
</html>
```
</p>
</details>



<br/>

<br/>

---
  
## Z-INDEX
 - controlls the stacking order of the elements.
 - ``z-index: 0;`` means that the element will be in normal document flow.
 - ``z-index: 1;`` means that the element will be above the elements in normal document flow.
 - ``z-index: 2;`` means that the elements will be above the elements with ``z-index: 1;``.
 - and soon. 

<details>
  <summary> <b><em>example:</em></b> </summary>
<p>

<table>
<tr>
<td colspan="2"> 

<image src="https://user-images.githubusercontent.com/63545175/187840635-caad94f6-091f-44c6-97d6-4015c5797994.png" width="520px">
</td>
</tr>
<tr>
<td> 

<image src="https://user-images.githubusercontent.com/63545175/187838482-5ec44c6d-681f-4d53-8f5b-9eddf680613d.png" width="420px">
</td>
<td>
  
<image src="https://user-images.githubusercontent.com/63545175/187839583-bba48975-354a-4aff-b307-68604d66a340.png" width="360px">
</td>  
</tr>
<tr>
<td> 

<image src="https://user-images.githubusercontent.com/63545175/187839736-a5d83273-31cc-4aff-944f-f2d8f38ff097.png" width="420px">
<td>
  
<image src="https://user-images.githubusercontent.com/63545175/187839856-a3e04784-31aa-4947-8521-c3d3622292b2.png" width="360px">
</td>  
</tr>
</table>  
  
</p>
</details>
  
  

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

## centering div and centering text ???

***reference:*** https://blog.hubspot.com/website/center-div-css#center-div-css ???






  
<br/>
  
<br/>

  
<br/>
  
<br/>

    
<br/>
  
<br/>

---
  
---

***references:***  
  
1. https://youtu.be/UO8ed-JB4So?t=1002 ?????

  
  
