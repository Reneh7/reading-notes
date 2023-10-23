# Android Reading 4

## What database engine is Room wrapped around? Do you think this is a good choice? Why or why not?

Room is an Android library that provides an abstraction layer on top of SQLite, which is a widely used relational database engine. This choice is generally a good one for Android app development because SQLite is lightweight, efficient, and well-suited for mobile applications. It offers features like ACID transactions, relational data capabilities, and it's built into the Android platform. Room simplifies database interaction, reduces the amount of boilerplate code needed, and offers compile-time checks to catch potential SQL-related errors early. While SQLite may not be the best choice for extremely large, complex, server-side databases, it's well-suited for local storage and mobile app use cases. Room's combination of SQLite's power and Room's developer-friendly features makes it a solid choice for Android database management.

## Do Rooms have any similarities to JPA?

Yes, they both offer high-level abstractions for database access, making it easier for developers to work with databases in their respective environments. They provide object-relational mapping (ORM) capabilities, allowing you to work with database tables using Java/Kotlin objects, and both offer features like annotations to define entity classes and relationships.

## Describe a DAO in your own words

 Data Access Object, is a design pattern used in software development to separate the data access logic from the rest of the application. It acts as an intermediary that abstracts the communication between the application and the database, allowing the application to interact with the database without needing to know the underlying database details.