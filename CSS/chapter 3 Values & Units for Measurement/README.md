## Concept of Computed Values 
### specified values: 
cascading and inheritance results in specified value that will be used for an element.

### computed value 
computed value is the specified value that is actually applied to an element after cascading order and inheritance is computed. 


> <b>Note:</b> _In case of the font-size property, the paragraphs in the division inherit a font-size of ``10px`` just like the ``<span>``. But simultaneously, the lower CSS rule sets the font-size of all paragraphs to ``300%``, resulting in a computed value of ``10 pixels x 300% = 30`` pixels inside the division. The paragraph outside the division doesn’t inherit the division’s font size which results in a font size three times as big as the initial value set in your browser._

<br/>

## Absolute Units and Relative Units:
> <b>"Before we can make use of media like images and videos in our app, it is important to know how to scale them. For this purpose, we need units."</b> 

***There are absolute and relative units.***
- Among the **absolute units** are **centimeters (cm), inches (in)** and **points (pt)**. The problem is that one centimeter looks small on a computer screen but is relatively large on a mobile device. It is recommended to use relative units instead. 
The only exception is pixel (px) because it is the unit which most images and videos use. To obtain a font-size of 28 pixels you would write: selector {font-size: 28px;}
- In many cases, **relative units** like **em** and **percent (%)** should be preferred. When using percent, the size is relative to the containing block.
![image](https://user-images.githubusercontent.com/63545175/163573991-71a5848b-6a81-4ce9-8ebc-1e1159cbc282.png)



