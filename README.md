# spring-with-mosh

https://www.youtube.com/watch?v=gJrjgg1KVL4

What is Spring Boot? 

The Spring Framework = a toolbox for building applications

Spring is modular, you can choose the components that you want. 

Spring Boot is a layer on top of Spring that takes care of tedious set up. Spring Boot provides sensible defaults and ready-to-use features.



Download Java JDK 23

Create a new Spring Project



Go to https://start.spring.io/

Build Tool: Maven

	Langage: Java

Select latest stable version of Spring Boot: 3.41.

Project MetaData

com.mccullough

Artifact: store

Package name (leave as is)

Packaging: Jar

Java: 23

Dependencies

OK as is. 

Then generate. 


The project: 

`pom.xml => xml format, has configuration data.   The HEART of Maven projects

dependencies = 3rd party libraries or resources we need for our project.

src folder

contains main and test

main contains java folder and resources folder

resources contains application.properties.




To find "snippets" for the required dependencies, you can go to:

https://central.sonatype.com/



Spring MVC stands for Model View Controller

Model = business logic. connected to DB.

View = what the user sees

Controller = like a traffic controller, fields user requests.


Make new file HomeController.java

Add @controller decoration



Set up Automatic refresh:

	Alt-Insert = Generate dependency


Dependency Injection

inject an object into a class. 

Open-closed Principle


Bean = a regular Java object that is managed by Spring

Spring takes care of 
creating it
injecting its dependencies
managing its life cycle

IOC = inversion of control

Configuring Beans Using Annotations

In response to error message: No qualifying bean of type 'com.example.store.OrderService' available

we need to go to OrderService class and decorate with the @Component annotation

@Component tells Spring to manage objects of this type (in this case, OrderService)
Also @Service, @Repository, @Controller

We can also use @Service, they are synonymous for Component

There is 


