### images
<table>
<tr>
<td>

![image](https://user-images.githubusercontent.com/63545175/180634955-9412b477-3e35-414b-9f09-883edeaccb0c.png)
</td>
<td>
  
![image](https://user-images.githubusercontent.com/63545175/180635004-862c05fb-dcba-4019-88fb-8f9921485092.png)
  
</td>
</tr>
</table> 
  


<br/>


### code

```html
<!DOCTYPE html>
<html lang="en" class="theme-light">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <link rel="stylesheet" href="./styles.css" type="text/css" />
  <style>

.theme-light {
  --color-primary: white;
  --color-secondary: #ffd500;
  --text-color1: #000000;
  --text-color2: #8c8c8e;
}
.theme-dark {
  --color-primary: black; /* #000000 */
  --color-secondary: #00ffea;
  --text-color1: #fafafc;
  --text-color2: #8c8c8e;
}

body{
  background-color: var(--color-secondary);
  color: var(--font-color);
}


/* The switch - the box around the slider */
.switch {
  position: relative;
  display: inline-block;
  width: 60px;
  height: 24px;
}

/* Hide default HTML checkbox */
.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

/* The slider */
.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: white;
  -webkit-transition: 0.4s;
  transition: 0.4s;
}


input:checked + .slider {
  background-color: black;
}

input:focus + .slider {
  box-shadow: 0 0 1px black;
}



/* Rounded sliders */
.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}

  </style>
</head>

<body>
    <label id="switch" class="switch">
            <input type="checkbox" onchange="toggleTheme()" id="slider">
            <span class="slider round"></span>
    </label>

    <br/>

    <h1> Hello!  </h1>

    <!-- <button id="switch" onclick="toggleTheme()">Switch</button> -->
  <script>
 // function to set a given theme/color-scheme
        function setTheme(themeName) {
            localStorage.setItem('theme', themeName);
            document.documentElement.className = themeName;
        }

        // function to toggle between dark theme and light theme
        function toggleTheme() {
            if (localStorage.getItem('theme') === 'theme-dark') {
                setTheme('theme-light');
            } else {
                setTheme('theme-dark');
            }
        }

        // initial theme setup
        (function () {
            if (localStorage.getItem('theme') === 'theme-dark') {
                setTheme('theme-dark');
                document.getElementById('slider').checked = false;
            } else {
                setTheme('theme-light');
              document.getElementById('slider').checked = true;
            }
        })();

  </script>
</body>

</html>
```
