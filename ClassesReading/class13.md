# Class Thirteen Reading

## Name a few real life examples of “One To Many” relatioships

- Author and Books: An author can write multiple books, but each book is authored by one author.
- Parent and Children: A parent can have multiple children, but each child has only one set of parents.
- Customer and Orders: A customer can place multiple orders, but each order is associated with one customer.
- University and Students: A university can have many students, but each student belongs to one university.
- Department and Employees: A department can have several employees, but each employee works in one department.

## Given two entities, one named Player and one named Team, if you wanted to create a one to many relationship with those entities which would be the one and which would be the many?

In a one-to-many relationship between the Player and Team entities, the "Team" entity would typically be the "one," and the "Player" entity would be the "many." This means that one team can have multiple players, but each player belongs to only one team.

## Explain one to many relationships to a non-technical friend

Sure! Imagine you have two things: a class of students and a class of teachers. In a "one-to-many" relationship, one teacher can have many students, but each student has only one teacher. It's like a teacher in a classroom – they can teach many students, but each student has their own teacher.

## Describe the difference between a unit test and an integration test

Unit tests, as the name suggests, focus on testing individual components or functions in isolation, ensuring that they behave correctly when given various inputs. They are typically fast to execute and use mock objects to isolate dependencies. In contrast, integration tests examine the interactions and integration points between different components or even entire systems. They often involve real external dependencies like databases and are designed to ensure that the various parts of a system work together seamlessly. While unit tests pinpoint specific code correctness, integration tests validate the overall system's behavior and interoperability.

## What is the object that provides support for Sprin MVC Testing?

MockMvc object. MockMvc is part of the Spring Test module and is used for testing Spring MVC applications. It allows you to send HTTP requests to your controllers and perform assertions on the responses, making it a valuable tool for testing the behavior of your Spring MVC application's endpoints without the need to deploy it in a real web server.

## What does the “perform()” method do in a Spring integration test?

The perform() method is used to simulate sending an HTTP request to a specific endpoint in your Spring MVC application. This method allows you to specify the HTTP method (e.g., GET, POST, PUT, DELETE), set request parameters, add request headers, and provide request content if needed. After configuring the request, you can call perform() to execute the request.
