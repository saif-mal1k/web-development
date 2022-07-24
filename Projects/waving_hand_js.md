### images


![image](https://user-images.githubusercontent.com/63545175/180640191-d23354cb-6629-49ab-b673-d92573a3fce8.png)


### code 

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <!-- waving hand and all round borders -->
    <style>
      * {
        border-radius: 8px !important;
      }

      .wave {
        animation-name: wave-animation; /* Refers to the name of your @keyframes element below */
        animation-duration: 2.5s; /* Change to speed up or slow down */
        animation-iteration-count: infinite; /* Never stop waving :) */
        transform-origin: 70% 70%; /* Pivot around the bottom-left palm */
        display: inline-block;
      }

      @keyframes wave-animation {
        0% {
          transform: rotate(0deg);
        }
        10% {
          transform: rotate(14deg);
        } /* The following five values can be played with to make the waving more or less extreme */
        20% {
          transform: rotate(-8deg);
        }
        30% {
          transform: rotate(14deg);
        }
        40% {
          transform: rotate(-4deg);
        }
        50% {
          transform: rotate(10deg);
        }
        60% {
          transform: rotate(0deg);
        } /* Reset for the last half to pause */
        100% {
          transform: rotate(0deg);
        }
      }
    </style>
    <!-- waving hand & all round borders / -->
  </head>
  <body>
    <script>
      // function to set a given theme/color-scheme
      function setTheme(themeName) {
        localStorage.setItem("theme", themeName);
        document.documentElement.className = themeName;
      }

      // function to toggle between dark theme and light theme
      function toggleTheme() {
        if (localStorage.getItem("theme") === "theme-dark") {
          setTheme("theme-light");
        } else {
          setTheme("theme-dark");
        }
      }

      // initial theme setup
      (function () {
        if (localStorage.getItem("theme") === "theme-dark") {
          setTheme("theme-dark");
          document.getElementById("slider").checked = false;
        } else {
          setTheme("theme-light");
          document.getElementById("slider").checked = true;
        }
      })();
    </script>

    <!-- title -->
    <h1 class="mb-15">
      Hello! <span class="wave" style="font-size: 50px">👋</span>
      <br />
      <span style="font-size: 20px"> My name is ... </span>
    </h1>
  </body>
</html>

```
