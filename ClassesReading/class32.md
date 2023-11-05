# Android Reading 7

## What makes an API RESTful?

A RESTful API, or Representational State Transfer API, adheres to a set of architectural principles that distinguish it from other types of APIs. What makes an API RESTful is its statelessness, meaning each request from a client to the server must contain all the necessary information, and no session data is stored on the server. It also relies on a clear and consistent set of operations, such as GET (retrieve), POST (create), PUT (update), and DELETE (remove), which are used for interactions. Additionally, RESTful APIs use a uniform and hierarchical resource structure, where resources are uniquely identifiable through URLs. These characteristics ensure that RESTful APIs are simple, scalable, and easily understood, making them a popular choice for web services and web applications.

## What is the benefit of using GraphQL? Any downsides?

GraphQL is a RESTful API that stands out for its efficiency, flexibility, and self-documenting nature. Unlike traditional REST APIs, GraphQL allows clients to request only the data they need, reducing over-fetching and enabling more efficient data retrieval. Its flexibility permits clients to define the shape of the response, making it possible to obtain multiple resources in a single query. Additionally, GraphQL eliminates the need for versioning, streamlining the API evolution process, and simplifying documentation through its introspection system. However, developers should be cautious about query complexity, as complex queries can impact performance. Overall, GraphQL's features make it a compelling choice for modern API development, enhancing both developer and client experiences.

## Describe “serverless” to a new 301 Code Fellows student:

Serverless is a cloud computing model where developers can build and run applications without managing traditional servers. Instead of provisioning and maintaining servers, serverless platforms automatically handle the infrastructure, scaling, and resource allocation as needed. This approach allows developers to focus solely on writing code, improving development speed and reducing operational overhead. Serverless architectures are event-driven, responding to specific triggers or requests, and users only pay for the actual compute resources used, making it a cost-effective and scalable solution for various applications.