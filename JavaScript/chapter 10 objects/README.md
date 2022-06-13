# Objects

- JavaScript variables are containers for data values. Objects are variables too, but they can contain many values. 

- They have <b>properties</b> ( <em>that store information about the object</em>) and the <b>properties</b> ( <em>that point to functions called methods</em>). 

- Methods are accessed the same way as other properties of objects, and can be invoked the same way as regular functions, except they automatically have access to the other properties of their parent object.

```js
var person = {
 name: "John", 
 age: 31,
 print: function () {
     console.log("name: ",this.name);
 }
};
```

### Accessing object Properties
You can access object properties in two ways.
```js
objectName.propertyName 		// dot Notation
//or
objectName['propertyName']	// bracket Notation
```

> <b>note:</b> in bracket notation property is in <b><em>"" quotes.</em></b>


### Accessing object Methods
```js
objectName.methodName()		// using dot Notation
```


> <b>tip:</b> it’s a preffered choice to use <b><em>. dot</em></b> to call methods and <b><em>[] bracket</em></b> to get properties values.



<br/>


<br/>



## Creating Objects

### 1. using Object Literal / Object Initializer Notation
```js
var person = {
 name: "John", 
 age: 31,
 print: function () {
     console.log("name: ",this.name);
 }
};
```

> <b>Note: </b> <br/>
>- Object Literal Notation allows you to create only a single object.
Sometimes, we need to set an <b>"object type"</b> that can be used to create a number of objects of a single type.<br/>
>- The standard way to create an "object type" is to use an object <b>constructor function.</b>


<br/>


### 2. using object constructor function
<em>The object constructor, takes parameters and assigns them to the object properties.</em>
```js
function person(name, age, color) {
  this.name = name;
  this.age = age;
  this.favColor = color;
  this.changeName = function(newName) {
    this.name = newName;
  }
}
```

> <b>Note:</b> <br/>
> - The <b>this</b> keyword refers to the <b>current object</b>, meaning that you can access the objects properties and methods using it.<br/>
> - Note that <b>this</b> is not a variable. It is a keyword, and its value cannot be changed.


#### Creating Objects
Once you have an object constructor, you can use the <b>new</b> keyword to create new objects of the same type.
```js
const myObject = new Person("Johny","22","Blue");
```


<br/>



> <b> important note:</b> <br/>
> ●	don't start your property name with a number. <br/>
> ●	You don't need to wrap the string in quotes! If it's a multi-word property, use camel case. Don't use hyphens in your property names

<b>example:</b>
```js
var richard = {
  "1stSon": true;		// accessing, richard.1stSon // error
  "loves-snow": true;		// accessing, richard.loves-snow // error
};
```


<br/>


<br/>


<br/>


## Objects are Mutable
> <b>Tip:</b> objects are mutable (with a few exceptions), so data within them can be altered. New properties can be added, and existing properties can be modified by simply specifying the property name and assigning (or re-assigning) a value. Additionally, properties and methods of an object can be deleted as well with the delete operator, which directly mutates the object.

### creating and modifying properties
```js
myObject.property = “add property or modify if exist”;
myObject[“property”] = “add property or modify if exist”;
```

### Removing Properties
```js
delete myObject.property;	// deletes property from my object, return true if successful
```


> **<b>imp note:</b> <br/>
> when re-assigning an object to a new variable, and then changing that copy. since <b><em>objects are passed by reference</em></b>, the original object is changed as well.  



<br/>


<br/>


<br/>


# How to deep copy objects ??????????????	
						------------------------------------------- ?

# what is a object() Keyword ??????????????	
						------------------------------------------- ?



