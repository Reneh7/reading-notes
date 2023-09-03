# Class Twelve Reading

## How are query methods defined when using Spring Data JPA?

Query methods are defined with utmost simplicity by creating method signatures within a repository interface. These method names follow a naming convention that conveys their intent, allowing Spring Data JPA to automatically generate the corresponding database queries.

## Which dependencies will you need in order to complete the Spring guide?

- Spring Boot Starter Web
- Spring Boot Starter Data JPA
- Spring Boot Starter Thymeleaf
- Spring Boot Starter Test
- Spring Boot Starter Security

## What annotations are used to specify an auto generated identification number for an Entity?

 The @GeneratedValue annotation is typically used to specify an auto-generated identification number for an Entity. This annotation is used in conjunction with @Id to mark a field as the primary key of an Entity and indicate that the value for this field will be generated automatically by the database.

## Which of the Spring Data Repositories covered in the readings has the most methods available to it?

 JpaRepository has the most methods available to it. JpaRepository is part of the Spring Data JPA module, which provides a wide range of built-in methods for performing CRUD (Create, Read, Update, Delete) operations and querying data from a database.

## Name a downstide of a Spring Data Repository

It introduces an additional layer of abstraction and complexity to your application. While Spring Data repositories simplify data access by providing CRUD operations and query methods, they may not cover all the specific and complex database operations your application requires. In such cases, you might need to write custom SQL queries or use native queries, which can bypass the benefits of type safety and abstraction provided by Spring Data.

## How would you define an operation to find a student based on their name in a repo named StudentRepository which extends JpaRepository?

you can use Spring Data JPA's method naming conventions. Spring Data JPA allows you to create query methods by simply declaring their method signature in the repository interface.
