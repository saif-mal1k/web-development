### Image
![image](https://user-images.githubusercontent.com/63545175/180451954-0fc81434-ea3d-4d99-8ac8-ee7dc5fdf243.png)



### Code 

```
<html>
<head>
    <style>

	#title{
	    padding: 30px;
        margin-bottom: 20px;
	    height: 50px;
        background: #49acc1;
        font-weight: 900;
        font-size: 30px;

	}
	

        td{
            margin:10px;
            padding-left:20px;
            padding-right:30px;
            padding-top:15px;
            padding-bottom:10px;	
            color: white;
            background: #4396c1e0;
            font-weight: bolder;
        }

	input,textarea{
            margin-left:-20px;
            margin-right:-30px;
            margin-top:-15px;
            margin-bottom:-10px;
	    height:40px;
	    width:200px;	
	}

        body{
            background: #00d7ff70;
            font-family: "Audiowide", sans-serif;
        }
	
	table{
	  margin-left: auto;
  	  margin-right: auto;
	}

    #container{
width: fit-content;
height: fit-content;
  border: 5px solid white;
margin-left: auto;
margin-top:auto;
  	  margin-right: auto;

	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%, -50%);

    }


    </style>
</head>
    
<body>
<div id="container">    
    
    <form action="https://webto.salesforce.com/servlet/servlet.WebToCase?encoding=UTF-8" method="POST" style="margin: 0px !important;">

<input type="hidden" name="orgid" value="********">
<input type="hidden" name="retURL" value="http://www.google.com">

<table><thead>
    <tr><th colspan="2" id="title">Raise a Case ...</th>
</tr></thead>

<tbody><tr>
    <td><label for="name">Your Name :</label></td>
    <td><input id="name" maxlength="80" placeholder="First-Name &nbsp; &nbsp; Last-Name" name="name" size="20" type="text"><br></td>
</tr>
<tr>
    <td><label for="email">Your Email :</label></td>
    <td><input id="email" maxlength="80" placeholder="example@xyz.com" name="email" size="20" type="text"><br></td>
</tr>
<tr>
    <td><label for="phone">Phone :</label></td>
    <td><input id="phone" maxlength="40" placeholder="+91 0123456789" name="phone" size="20" type="text"><br></td>
</tr>
<tr>
    <td><label for="subject">Subject :</label></td>
    <td><input id="subject" maxlength="80" placeholder="short about issue" name="subject" size="20" type="text"><br></td>
</tr>
<tr>
    <td colspan="2"><label for="description">Description : </label></td>
</tr>
<tr>
    <td colspan="2"><textarea placeholder="your Query here" name="description" style="width:100%; height:70px; width:345px;"></textarea><br></td>
</tr>
<tr>
    <td colspan="2" align="right">
        <input style="width:345px;" type="submit" name="submit">
    </td>
</tr>
    
</tbody></table>
        


</form>

    
</div>
</body>
</html>
```
