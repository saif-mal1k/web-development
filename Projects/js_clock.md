### image

![image](https://user-images.githubusercontent.com/63545175/182533342-d4e2b8ec-6b91-4421-8c5c-ac9560f63151.png)



<br/>


<br/>



### code

```html
<html>
  <head>
    <style>
      body{
          font-size: 24px;
          text-align: end;
          font-weight: bolder;
      }
    </style>
  </head>
  <body>
 
    <script>
        function printTime() {
            var d = new Date();
            var hours = d.getHours();
            var mins = d.getMinutes();
            var secs = d.getSeconds();
            document.body.innerHTML = hours+":"+mins+":"+secs;
        }
        setInterval(printTime, 1000);
    </script>
  </body>
</html>
```



