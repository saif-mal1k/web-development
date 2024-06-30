## Types of Web Architecture


### Multi tier Architecture

![image](https://github.com/saif-mal1k/web-development/assets/63545175/e06f5518-5a53-4197-a827-c72e5a8249ce)

<br/>


### Client - Server Arcitecture
![image](https://github.com/saif-mal1k/web-development/assets/63545175/4ebf861b-efb5-4056-9b28-a34633b60c87)


<br/>


### Monolithic Architecture
- Easy to develop
- Easy to deploy as there is only one application to 
- Most applications start as monoliths as it's very quicker to get them to the market.

<br/>


### Microservices Architecture


<br/>

#### Monolithic vs Microservices

![image](https://github.com/saif-mal1k/web-development/assets/63545175/17e7c744-1d39-42b1-a864-d0d0cee02ab8)

<table>
<tr>
<th>Monolithic</th>
<th>Micro-services</th>  
</tr>
<tr>
<td>
  
![image](https://github.com/saif-mal1k/web-development/assets/63545175/99223cd7-1c56-4c35-803f-afec9a729d1a)
  
</td>  
<td>

![image](https://github.com/saif-mal1k/web-development/assets/63545175/405f60f2-2ba5-4116-b104-448738a1e8d8)
  
</td>
</tr>  
<tr>
<td>even small changes requires redeployment of whole app</td>
<td>since app is divided into multiple services, each service can be developed and deployed independedntly by separate teams</td>  
</tr>
<tr>
<td>can't scale up one component, has to scale up or scale down whole app.</td>
<td>easier to scale up or scale down since each component is an independent service.</td>  
</tr>
<tr>
<td colspan="2">

Drawbacks of Microservices:
  - complex to build.
  - management overhead as separate team for each service.
  - high infrastructure cost as separate CI/CD pipelines and containers for each service.

Note: 
 - small startup's generally don't prefer microservice start up.
 - large organisations like Netflix use microservice architecture for its obvious benefits. 

</td>  
</tr>
  
</table>


<br/>


### Serverless Architecture / function as a service
ex: aws lamda, firebase cloud functions

<br/>




<br/>

<br/>

<br/>

<br/>


---
### references:
- [Everything You NEED to Know About WEB APP Architecture](https://www.youtube.com/watch?v=sDlCSIDwpDs)
- https://hatchworks.com/blog/software-development/monolithic-vs-microservices/
- [Monolithic vs Microservice](https://www.youtube.com/watch?v=7IFJb-uLEaI&pp=ygUabW9ub2xpdGhpYy12cy1taWNyb3NlcnZpY2U%3D)
- [Monolithic vs Microservice Architecture: Which To Use and When?](https://www.youtube.com/watch?v=NdeTGlZ__Do)


