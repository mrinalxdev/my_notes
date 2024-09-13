`Microservice or Micro-Web services was coined by Dr Peter Rodgers in 2005`

#### Defining Micro-services in one line 
A component or a piece of code which performs one single thing very well, while communicating with other pieces of code or services using a protocol of communication. 

## Fundamentals of Micro-services
>There are 5 key fundamentals which defines a how a Micro-service is built and modelled
#### These 5 key concepts are
- High Cohesion & Low Coupling
- Independent Deployability
- Business Domain Modelling
- Observability
- Team Organisation

## Monoliths Vs Micro-services

> A monolith is a single codebase which can have separate modules inside but there will be single client layer and a single database.

![[Monolith.png]]
*image above shows the different variations in a monolith architecture.*
1. Its a typical three-tier architecture , as there is a modularisation in code and there a single database with single layer of client app.
2. There will be no modularisation of code and will be a just single file of code.
3. There will be modularisation of code along with different databases.
4. There will be modularisation of code is done but deployed as a single codebase with a single database. 


![[Microservices.png]]
*image above shows the architecture of Micro-service : DB --> database

In single micro-service we can observe that some major points
1. Every single service is a different component with their own dedicated database.
2. An API Gateway to guard the client apps and route them

# Key concepts of building and modelling a Micro-service

- ### High Cohesion and Low Coupling

	First We need to discuss what is cohesion ?
			Cohesion means if there is a service named Orders then every features, data, functions related to Order should within the Order service or nearer to the service.
			In Easy Language *All features, business logic, data should be in kept nearest to the service*.

