### image
<table>
<tr>
<td>

<image src="https://user-images.githubusercontent.com/63545175/188057062-89d496c2-04b5-4362-861c-7d7e4ef127b4.png" width="480px">
</td>
<td>

<image src="https://user-images.githubusercontent.com/63545175/188057186-892de9bf-ec50-458a-93c3-46007d14ab5a.png" width="480px">
</td>
</tr> 
</table>

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
        .large-image {
            position: relative;
            width: 100%;
            height: calc(100vh - 25vh);
            background-image: url("image.jpg");
            background-repeat:  no-repeat;
        }

        .nav-bar {
            position: sticky;
            position: -webkit-sticky;
            top: 8px;
            width: 100%;
            z-index: 1;
            margin: auto;
            background-color: black;
            color: cornsilk;            
        }

        .nav-element {
            font-size: x-large;
            display: inline-block;
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
    <div class="large-image"></div>
    <div class="nav-bar">
    <span class="nav-element"> HOME </span>
    <span class="nav-element"> Contact </span>
    <span class="nav-element"> more </span>
    </div>
    <div class="content">
        <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum veritatis distinctio at iusto fugiat similique blanditiis harum! Corporis accusamus repellat aperiam ducimus tenetur magni possimus explicabo iure? Quisquam, maiores ipsam.
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Obcaecati tempore architecto aut minus earum magni nobis facere, accusantium excepturi perferendis. Officiis incidunt quia eligendi quibusdam consequuntur excepturi sed ad voluptatibus.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex ab quia mollitia ea sapiente reprehenderit quibusdam, autem rem iusto placeat repellendus nam voluptas tenetur, inventore iste debitis. Facilis, possimus numquam?
        </p>
        <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi amet voluptatum corrupti cupiditate natus soluta asperiores sunt, sint voluptas ratione accusamus ipsam quisquam fuga architecto consectetur maiores temporibus cumque praesentium!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio dolorem voluptate quam unde. Nemo iste repudiandae, veritatis rem hic quos, dolore magnam repellat sequi, sit eveniet ipsum. Exercitationem, placeat culpa!
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum veritatis distinctio at iusto fugiat similique blanditiis harum! Corporis accusamus repellat aperiam ducimus tenetur magni possimus explicabo iure? Quisquam, maiores ipsam.
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Obcaecati tempore architecto aut minus earum magni nobis facere, accusantium excepturi perferendis. Officiis incidunt quia eligendi quibusdam consequuntur excepturi sed ad voluptatibus.
        </p>
        <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex ab quia mollitia ea sapiente reprehenderit quibusdam, autem rem iusto placeat repellendus nam voluptas tenetur, inventore iste debitis. Facilis, possimus numquam?
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi amet voluptatum corrupti cupiditate natus soluta asperiores sunt, sint voluptas ratione accusamus ipsam quisquam fuga architecto consectetur maiores temporibus cumque praesentium!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio dolorem voluptate quam unde. Nemo iste repudiandae, veritatis rem hic quos, dolore magnam repellat sequi, sit eveniet ipsum. Exercitationem, placeat culpa!
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum veritatis distinctio at iusto fugiat similique blanditiis harum! Corporis accusamus repellat aperiam ducimus tenetur magni possimus explicabo iure? Quisquam, maiores ipsam.            
        </p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Obcaecati tempore architecto aut minus earum magni nobis facere, accusantium excepturi perferendis. Officiis incidunt quia eligendi quibusdam consequuntur excepturi sed ad voluptatibus.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex ab quia mollitia ea sapiente reprehenderit quibusdam, autem rem iusto placeat repellendus nam voluptas tenetur, inventore iste debitis. Facilis, possimus numquam?
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi amet voluptatum corrupti cupiditate natus soluta asperiores sunt, sint voluptas ratione accusamus ipsam quisquam fuga architecto consectetur maiores temporibus cumque praesentium!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio dolorem voluptate quam unde. Nemo iste repudiandae, veritatis rem hic quos, dolore magnam repellat sequi, sit eveniet ipsum. Exercitationem, placeat culpa!
        <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum veritatis distinctio at iusto fugiat similique blanditiis harum! Corporis accusamus repellat aperiam ducimus tenetur magni possimus explicabo iure? Quisquam, maiores ipsam.
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Obcaecati tempore architecto aut minus earum magni nobis facere, accusantium excepturi perferendis. Officiis incidunt quia eligendi quibusdam consequuntur excepturi sed ad voluptatibus.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex ab quia mollitia ea sapiente reprehenderit quibusdam, autem rem iusto placeat repellendus nam voluptas tenetur, inventore iste debitis. Facilis, possimus numquam?
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi amet voluptatum corrupti cupiditate natus soluta asperiores sunt, sint voluptas ratione accusamus ipsam quisquam fuga architecto consectetur maiores temporibus cumque praesentium!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio dolorem voluptate quam unde. Nemo iste repudiandae, veritatis rem hic quos, dolore magnam repellat sequi, sit eveniet ipsum. Exercitationem, placeat culpa!
        </p>
        <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum veritatis distinctio at iusto fugiat similique blanditiis harum! Corporis accusamus repellat aperiam ducimus tenetur magni possimus explicabo iure? Quisquam, maiores ipsam.
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Obcaecati tempore architecto aut minus earum magni nobis facere, accusantium excepturi perferendis. Officiis incidunt quia eligendi quibusdam consequuntur excepturi sed ad voluptatibus.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex ab quia mollitia ea sapiente reprehenderit quibusdam, autem rem iusto placeat repellendus nam voluptas tenetur, inventore iste debitis. Facilis, possimus numquam?
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi amet voluptatum corrupti cupiditate natus soluta asperiores sunt, sint voluptas ratione accusamus ipsam quisquam fuga architecto consectetur maiores temporibus cumque praesentium!
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio dolorem voluptate quam unde. Nemo iste repudiandae, veritatis rem hic quos, dolore magnam repellat sequi, sit eveniet ipsum. Exercitationem, placeat culpa!            
        </p>
    <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum veritatis distinctio at iusto fugiat similique blanditiis harum! Corporis accusamus repellat aperiam ducimus tenetur magni possimus explicabo iure? Quisquam, maiores ipsam.
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Obcaecati tempore architecto aut minus earum magni nobis facere, accusantium excepturi perferendis. Officiis incidunt quia eligendi quibusdam consequuntur excepturi sed ad voluptatibus.
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex ab quia mollitia ea sapiente reprehenderit quibusdam, autem rem iusto placeat repellendus nam voluptas tenetur, inventore iste debitis. Facilis, possimus numquam?
        </p>

    </div>

</body>
</html>
```


