## What role do the @Controller classes play in a Spring MVC application?

## Controller : 
Request Handler which is handling incoming HTTP requests. Each method within a controller class can be annotated with specific request mapping annotations

## Explain to a non-technical friend what a GET request is.
A GET request is like politely asking the internet library for a specific web page

## What annotation should be placed on your Spring Boot application class?
@SpringBootApplication


## Spring MVC and Thymeleaf

## What method allows for a variable defined in Java (in your Spring Controller) to be dispalyed in HTML with the help of Thymeleaf?
Add attribute to Model via its addAttribute method:

## Explain the role of a @Controller class in a Spring MVC application.

class plays a crucial role in handling incoming HTTP requests and managing the flow of data between the model, 

## What is a model attribute refered to in Thymeleaf?

a model attribute refers to a piece of data that is made available to the Thymeleaf template for rendering. Model attributes are typically set in the Spring Controller or another web framework's equivalent component, and they represent data that you want to display or use in your HTML template.