

### code
```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <title>CSS Slider - Template</title>
    <link rel="stylesheet" href="./themes/csslider.light.css" />
    <style>
        .csslider {
            -moz-perspective: 1300px;
            -ms-perspective: 1300px;
            -webkit-perspective: 1300px;
            perspective: 1300px;
            display: inline-block;
            text-align: left;
            position: relative;
            margin-bottom: 22px;
          }
          .csslider > input {
            display: none;
          }
          .csslider > input:nth-of-type(10):checked ~ ul li:first-of-type {
            margin-left: -900%;
          }
          .csslider > input:nth-of-type(9):checked ~ ul li:first-of-type {
            margin-left: -800%;
          }
          .csslider > input:nth-of-type(8):checked ~ ul li:first-of-type {
            margin-left: -700%;
          }
          .csslider > input:nth-of-type(7):checked ~ ul li:first-of-type {
            margin-left: -600%;
          }
          .csslider > input:nth-of-type(6):checked ~ ul li:first-of-type {
            margin-left: -500%;
          }
          .csslider > input:nth-of-type(5):checked ~ ul li:first-of-type {
            margin-left: -400%;
          }
          .csslider > input:nth-of-type(4):checked ~ ul li:first-of-type {
            margin-left: -300%;
          }
          .csslider > input:nth-of-type(3):checked ~ ul li:first-of-type {
            margin-left: -200%;
          }
          .csslider > input:nth-of-type(2):checked ~ ul li:first-of-type {
            margin-left: -100%;
          }
          .csslider > input:nth-of-type(1):checked ~ ul li:first-of-type {
            margin-left: 0%;
          }
          .csslider > ul {
            position: relative;
            width: 820px;
            height: 420px;
            z-index: 1;
            font-size: 0;
            line-height: 0;
            background-color: #d1d1d1;
            border: 10px solid #d1d1d1;
            margin: 0 auto;
            padding: 0;
            overflow: hidden;
            white-space: nowrap;
            -moz-box-sizing: border-box;
            -webkit-box-sizing: border-box;
            box-sizing: border-box;
          }
          .csslider > ul > li {
            position: relative;
            display: inline-block;
            width: 100%;
            height: 100%;
            overflow: hidden;
            font-size: 15px;
            font-size: initial;
            line-height: normal;
            -moz-transition: all 0.5s cubic-bezier(0.4, 1.3, 0.65, 1);
            -o-transition: all 0.5s ease-out;
            -webkit-transition: all 0.5s cubic-bezier(0.4, 1.3, 0.65, 1);
            transition: all 0.5s cubic-bezier(0.4, 1.3, 0.65, 1);
            -moz-background-size: cover;
            -o-background-size: cover;
            -webkit-background-size: cover;
            background-size: cover;
            vertical-align: top;
            -moz-box-sizing: border-box;
            -webkit-box-sizing: border-box;
            box-sizing: border-box;
            white-space: normal;
          }
          .csslider > ul > li.scrollable {
            overflow-y: scroll;
          }
          .csslider > .navigation {
            position: absolute;
            bottom: -10px;
            left: 50%;
            z-index: 10;
            margin-bottom: -10px;
            font-size: 0;
            line-height: 0;
            text-align: center;
            -webkit-touch-callout: none;
            -webkit-user-select: none;
            -khtml-user-select: none;
            -moz-user-select: none;
            -ms-user-select: none;
            user-select: none;
          }
          .csslider > .navigation > div {
            margin-left: -100%;
          }
          .csslider > .navigation label {
            position: relative;
            display: inline-block;
            cursor: pointer;
            border-radius: 50%;
            margin: 0 2px;
            padding: 5px;
            background: #d1d1d1;
          }
          .csslider > .navigation label:hover:after {
            opacity: 1;
          }
          .csslider > .navigation label:after {
            content: '';
            position: absolute;
            left: 50%;
            top: 50%;
            margin-left: -3px;
            margin-top: -3px;
            background: #0097ef;
            border-radius: 50%;
            padding: 3px;
            opacity: 0;
          }
          .csslider > .arrows {
            -webkit-touch-callout: none;
            -webkit-user-select: none;
            -khtml-user-select: none;
            -moz-user-select: none;
            -ms-user-select: none;
            user-select: none;
          }
          .csslider.inside .navigation {
            bottom: 10px;
            margin-bottom: 10px;
          }
          .csslider.inside .navigation label {
            border: 1px solid #7e7e7e;
          }
          .csslider > input:nth-of-type(1):checked ~ .navigation label:nth-of-type(1):after,
          .csslider > input:nth-of-type(2):checked ~ .navigation label:nth-of-type(2):after,
          .csslider > input:nth-of-type(3):checked ~ .navigation label:nth-of-type(3):after,
          .csslider > input:nth-of-type(4):checked ~ .navigation label:nth-of-type(4):after,
          .csslider > input:nth-of-type(5):checked ~ .navigation label:nth-of-type(5):after,
          .csslider > input:nth-of-type(6):checked ~ .navigation label:nth-of-type(6):after,
          .csslider > input:nth-of-type(7):checked ~ .navigation label:nth-of-type(7):after,
          .csslider > input:nth-of-type(8):checked ~ .navigation label:nth-of-type(8):after,
          .csslider > input:nth-of-type(9):checked ~ .navigation label:nth-of-type(9):after,
          .csslider > input:nth-of-type(10):checked ~ .navigation label:nth-of-type(10):after,
          .csslider > input:nth-of-type(11):checked ~ .navigation label:nth-of-type(11):after {
            opacity: 1;
          }
          .csslider > .arrows {
            position: absolute;
            left: -31px;
            top: 50%;
            width: 100%;
            height: 26px;
            padding: 0 31px;
            z-index: 0;
            -moz-box-sizing: content-box;
            -webkit-box-sizing: content-box;
            box-sizing: content-box;
          }
          .csslider > .arrows label {
            display: none;
            position: absolute;
            top: -50%;
            padding: 13px;
            box-shadow: inset 2px -2px 0 1px #d1d1d1;
            cursor: pointer;
            -moz-transition: .15s;
            -o-transition: .15s;
            -webkit-transition: .15s;
            transition: .15s;
          }
          .csslider > .arrows label:hover {
            box-shadow: inset 3px -3px 0 2px #0097ef;
            margin: 0 0px;
          }
          .csslider > .arrows label:before {
            content: '';
            position: absolute;
            top: -100%;
            left: -100%;
            height: 300%;
            width: 300%;
          }
          .csslider.infinity > input:first-of-type:checked ~ .arrows label:last-of-type,
          .csslider > input:nth-of-type(1):checked ~ .arrows label:nth-of-type(0),
          .csslider > input:nth-of-type(2):checked ~ .arrows label:nth-of-type(1),
          .csslider > input:nth-of-type(3):checked ~ .arrows label:nth-of-type(2),
          .csslider > input:nth-of-type(4):checked ~ .arrows label:nth-of-type(3),
          .csslider > input:nth-of-type(5):checked ~ .arrows label:nth-of-type(4),
          .csslider > input:nth-of-type(6):checked ~ .arrows label:nth-of-type(5),
          .csslider > input:nth-of-type(7):checked ~ .arrows label:nth-of-type(6),
          .csslider > input:nth-of-type(8):checked ~ .arrows label:nth-of-type(7),
          .csslider > input:nth-of-type(9):checked ~ .arrows label:nth-of-type(8),
          .csslider > input:nth-of-type(10):checked ~ .arrows label:nth-of-type(9),
          .csslider > input:nth-of-type(11):checked ~ .arrows label:nth-of-type(10) {
            display: block;
            left: 0;
            -moz-transform: rotate(45deg);
            -ms-transform: rotate(45deg);
            -o-transform: rotate(45deg);
            -webkit-transform: rotate(45deg);
            transform: rotate(45deg);
          }
          .csslider.infinity > input:last-of-type:checked ~ .arrows label:first-of-type,
          .csslider > input:nth-of-type(1):checked ~ .arrows label:nth-of-type(2),
          .csslider > input:nth-of-type(2):checked ~ .arrows label:nth-of-type(3),
          .csslider > input:nth-of-type(3):checked ~ .arrows label:nth-of-type(4),
          .csslider > input:nth-of-type(4):checked ~ .arrows label:nth-of-type(5),
          .csslider > input:nth-of-type(5):checked ~ .arrows label:nth-of-type(6),
          .csslider > input:nth-of-type(6):checked ~ .arrows label:nth-of-type(7),
          .csslider > input:nth-of-type(7):checked ~ .arrows label:nth-of-type(8),
          .csslider > input:nth-of-type(8):checked ~ .arrows label:nth-of-type(9),
          .csslider > input:nth-of-type(9):checked ~ .arrows label:nth-of-type(10),
          .csslider > input:nth-of-type(10):checked ~ .arrows label:nth-of-type(11),
          .csslider > input:nth-of-type(11):checked ~ .arrows label:nth-of-type(12) {
            display: block;
            right: 0;
            -moz-transform: rotate(225deg);
            -ms-transform: rotate(225deg);
            -o-transform: rotate(225deg);
            -webkit-transform: rotate(225deg);
            transform: rotate(225deg);
          }
          /*#region MODULES */
          /*#endregion */
          
    </style>
    <style>
        .csslider .navigation label {
            background: #B1B1B1;
        }
        .csslider .arrows label {
            border-left-color: #B1B1B1;
            border-right-color: #B1B1B1;
        }
        .csslider.inside .navigation label {
            border: 1px solid #FFF;
        }

        @import url(http://fonts.googleapis.com/css?family=Raleway:400,700|Lato);

        * {
            margin: 0;
            padding: 0;
        }

        ::-webkit-scrollbar {
            width: 2px;
            background: rgba(255, 255, 255, 0.1);
        }

        ::-webkit-scrollbar-track {
            background: none;
        }

        ::-webkit-scrollbar-thumb {
            background: rgba(0, 94, 168, 0.6);
        }

        ul, ol {
            padding-left: 40px;
        }

        html, body {
            height: 100%;
            text-align: center;
            font: 400 100% 'Raleway', 'Lato';
            color: #333;
            background-color: #FFF;
            background-image: -webkit-radial-gradient(50% 10%, ellipse farthest-corner, #ffffff 35%, #cccccc);
            background-image: -moz-radial-gradient(50% 10%, ellipse farthest-corner, #ffffff 35%, #cccccc);
            background-image: -ms-radial-gradient(50% 10%, ellipse farthest-corner, #ffffff 35%, #cccccc);
            background-image: -o-radial-gradient(50% 10%, ellipse farthest-corner, #ffffff 35%, #cccccc);
            background-image: radial-gradient(farthest-corner ellipse at 50% 10%, #ffffff 35%, #cccccc);
        }

        h1 {
            font-weight: 700;
            font-size: 310%;
        }

        h2 {
            font-weight: 400;
            font-size: 120%;
            color: #008FDF;
        }

        #slider1 {
            margin: 20px;
            font-family: 'Lato';
        }

            #slider1 > ul > li:nth-of-type(3) {
                background: url(./themes/fruit.jpg);
            }

            #slider1 > input:nth-of-type(3):checked ~ ul #bg {
                width: 80%;
                padding: 22px;
                -moz-transition: .5s .5s;
                -o-transition: .5s .5s;
                -webkit-transition: .5s .5s;
                transition: .5s .5s;
            }

                #slider1 > input:nth-of-type(3):checked ~ ul #bg div {
                    -moz-transform: translate(0);
                    -ms-transform: translate(0);
                    -o-transform: translate(0);
                    -webkit-transform: translate(0);
                    transform: translate(0);
                    -moz-transition: .5s .9s;
                    -o-transition: .5s .9s;
                    -webkit-transition: .5s .9s;
                    transition: .5s .9s;
                }

        #bg {
            color: #000;
            padding: 22px 0;
            position: absolute;
            left: 0;
            top: 16%;
            height: 20%;
            width: 0;
            z-index: 10;
            overflow: hidden;
        }

            #bg:before {
                content: '';
                position: absolute;
                left: -1px;
                top: 1px;
                height: 100%;
                width: 100%;
                z-index: -1;
                background: url(./themes/fruit.jpg) 1px 23%;
                -webkit-filter: blur(7px);
            }

            #bg:after {
                content: '';
                position: absolute;
                left: 0;
                top: 0;
                height: 100%;
                width: 100%;
                z-index: 20;
                background: rgba(0, 0, 0, 0.35);
                pointer-events: none;
            }

            #bg div {
                -moz-transform: translate(120%);
                -ms-transform: translate(120%);
                -o-transform: translate(120%);
                -webkit-transform: translate(120%);
                transform: translate(120%);
            }

        .scrollable p {
            padding: 30px;
            text-align: justify;
            line-height: 140%;
            font-size: 120%;
        }
    </style>
</head>
<body>

    
    <div id="slider1" class="csslider infinity inside">
        <input type="radio" name="slides" id="slides_1" checked />
        <input type="radio" name="slides" id="slides_2" />
        <input type="radio" name="slides" id="slides_3" />
        <input type="radio" name="slides" id="slides_4" />
        <ul>
            <li>
                <h1>Say hello to CSS3</h1>
                <p>CSSlider is lightweight & easy to use slider. No JS - pure CSS.</p>
            </li>
            <li>
                <img src="./themes/stones.jpg" />
            </li>
            <li>
                <div id="bg">
                    <div>
                        <h1>CSS Events</h1>
                        <p>When slide 3 is reached - play CSS animation!</p>
                    </div>
                </div>
            </li>
            <li class="scrollable">
                <h1>Lots of text</h1>
                <h2>Scrollable one</h2>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit fusce vel sapien elit in malesuada mi,
                    semper id sollicitudin urna fermentum ut fusce varius nisl ac ipsum gravida vel pretium tellus.
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit fusce vel sapien elit in malesuada mi,
                    semper id sollicitudin urna fermentum ut fusce varius nisl ac ipsum gravida vel pretium tellus.
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit fusce vel sapien elit in malesuada mi,
                    semper id sollicitudin urna fermentum ut fusce varius nisl ac ipsum gravida vel pretium tellus.
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit fusce vel sapien elit in malesuada mi,
                    semper id sollicitudin urna fermentum ut fusce varius nisl ac ipsum gravida vel pretium tellus.
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit fusce vel sapien elit in malesuada mi,
                    semper id sollicitudin urna fermentum ut fusce varius nisl ac ipsum gravida vel pretium tellus.
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit fusce vel sapien elit in malesuada mi,
                    semper id sollicitudin urna fermentum ut fusce varius nisl ac ipsum gravida vel pretium tellus.
                </p>
            </li>
        </ul>
        <div class="arrows">
            <label for="slides_1"></label>
            <label for="slides_2"></label>
            <label for="slides_3"></label>
            <label for="slides_4"></label>
        </div>
        <div class="navigation">
            <div>
                <label for="slides_1"></label>
                <label for="slides_2"></label>
                <label for="slides_3"></label>
                <label for="slides_4"></label>
            </div>
        </div>
    </div>


</body>
</html>

```


