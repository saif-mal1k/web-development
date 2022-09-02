### images
![image](https://user-images.githubusercontent.com/63545175/188058414-0ec9c4c7-2173-4248-9b15-aa095050f326.png)




### code
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


