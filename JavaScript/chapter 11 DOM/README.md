## DOM
When you open any webpage in a browser, the HTML of the page is loaded and rendered visually on the screen. To accomplish that, the browser builds the Document Object Model of that page, which is an object oriented model of its logical structure.

![image](https://user-images.githubusercontent.com/63545175/197961209-c267e73c-689b-4d0a-b28a-4b8dc7a6786e.png)

- Think of the DOM as a tree. It starts at the root of the browser’s display functionality: the ``window``. 
- From there, the page is encapsulated in ``window.document``, with the page’s body in ``window.document.body`` and soon.
- JavaScript can be used to manipulate the DOM Tree of a page dynamically to add, delete and modify elements, and their attributes.

### DOM Tree
- HTML elements become interrelated nodes in the tree.
- Nodes can have many child nodes(contained elements) and 1 parent node(Container element). 
- Nodes on the same tree level are called siblings.

<b>For the example above:</b>
- ``<document>`` has one child (``<body>``) and one parent (``<window>``);
- ``<body>`` has two children (``<div>``, ``<div>``);

  
  
<br/>


  
> Web Development frameworks such as LWC & React, they abstract away and simplify DOM interactions, and often automatically apply polyfills for missing features. 


<br/>

---  
  
<br/>


<br/>


# DOM manipulation

## Document Object:
all elements are treated as objects in js and the document object is the owner (or root) of all objects in your webpage. 
it can be used to access all elements on the DOM. So, if you want to access objects in an HTML page, you always start with accessing the document object.  

```js
//example

document.body.innerHTML="some content for body";

//innerHTML property can be used on almost all HTML elements to change its content.

```

## Selecting , Creating , Removing , Replacing Elements:

### selecting elements:

```js
//finds element by id
var elem = document.getElementById("demo");
elem.innerHTML = "Hello World!";
```

```js
//finds elements by class name
//returns a collection of all elements in the document with the specified class name.

//if our HTML page contained three elements with class="demo"
var arr =  document.getElementsByClassName("demo");
//accessing the second element
arr[1].innerHTML = "Hi";
```

```html
<body>
  
  <!--finds elements by tag name-->
  <!--returns all of the elements of the specified tag name as an array.-->
  
  <p>hello</p>
  <p>how</p>
  <p>are u.</p>

  <script>
     var arr = document.getElementsByTagName("p");
     for (var x = 0; x < arr.length; x++) {
         arr[x].innerHTML = "Hi there";
     }
  </script>
</body>
```


