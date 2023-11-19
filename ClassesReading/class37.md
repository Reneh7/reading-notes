# Android Reading 11

## What is Amazon S3?

Amazon S3, or Amazon Simple Storage Service, is a widely-used cloud storage service provided by Amazon Web Services (AWS). S3 allows users to store and retrieve any amount of data at any time through a web interface or programmatically via APIs. It provides highly durable and scalable object storage, with data organized as "buckets" and each object within a bucket identified by a unique key. S3 is designed to be secure, reliable, and cost-effective, making it a popular choice for businesses and developers to store and manage their data in the cloud, serving as a foundation for various applications ranging from simple backups to large-scale data analytics.

## List at least 3 features that it offers to its users

- Scalability: S3 provides virtually limitless scalability, allowing users to store an unlimited amount of data.
- Durability and Reliability: S3 is designed for high durability, with data automatically distributed across multiple locations, ensuring resilience against hardware failures and providing 99.999999999% (11 9's) durability.
- Security and Access Control: S3 offers comprehensive security features, including access control policies, encryption at rest and in transit, and integration with AWS Identity and Access Management (IAM).

## What is an object key?

In Amazon S3, an object key is a unique identifier assigned to each object stored in a bucket. The object key serves as the file name within the bucket and is used to retrieve and manage the object. It is a string that can be up to 1024 bytes in length and can include any combination of Unicode characters. The key plays a crucial role in organizing and accessing data within S3, as it provides a hierarchical structure within a bucket.