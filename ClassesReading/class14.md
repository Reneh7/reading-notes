# Class Fourteen Reading

## Define the term “hashing”

Hashing is a process in computer science and cryptography where an algorithm takes an input (or 'message') and returns a fixed-size string of bytes. The output, typically a 'hash value' or 'digest,' is unique to the specific input data. Hashing is designed to be a one-way function, meaning it should be computationally infeasible to reverse the process and determine the original input from the hash value. Hash functions are commonly used for data retrieval, data verification, and security purposes, such as password storage, data integrity checking, and digital signatures.

## Explain to a non-technical friend what a hash function does to a password

A hash function, in simple terms, is like a password protector. When you create a password for an online account, the website doesn't store it as plain text. Instead, it runs your password through a hash function, which converts it into a unique series of letters and numbers, like a secret code. This code is stored in the website's database, not your actual password. When you log in, the website takes what you type as your password, turns it into the same secret code, and checks if it matches what's in its database. If they match, you're granted access. Hash functions are crucial for security because they keep your password hidden, even from the website itself, making it much harder for hackers to decipher.

## What does it mean to ‘salt’ a password?

To "salt" a password means to add an extra layer of security by appending a random string of characters (the salt) to the user's password before hashing it. This salt is unique for each user and is stored alongside the hashed password in a database. Salting passwords helps protect against common attacks, like rainbow table attacks, where attackers precompute hashes for a list of possible passwords. By salting each password differently, even if two users have the same password, their hashed passwords will look completely different due to the unique salts. This makes it significantly more challenging for attackers to crack passwords, enhancing overall security.

## What piece of information would a hacker need to access in order to find the ‘salt’ string for your passwords?

A hacker would typically need access to the database where user credentials are stored. The salt is usually stored alongside the hashed password in the database. Therefore, if an attacker gains unauthorized access to the database, they can potentially obtain both the hashed password and the corresponding salt for each user. Protecting the database and implementing strong security measures is crucial to prevent such breaches and safeguard user information.

## How does the Blowfish block cipher handle the increased computation speed of new computers?

Blowfish is a symmetric-key block cipher designed with a variable key length, which allows it to adapt to the increased computation speed of new computers. It does so by allowing users to set a key length from 32 bits up to 448 bits. As computing power increases, users can choose longer key lengths to enhance security. Blowfish also employs a Feistel network structure, which makes it computationally efficient while remaining secure. This flexibility in key length and its efficient structure make Blowfish a cipher that can scale with advancements in computer processing capabilities, ensuring that it can provide strong encryption even on modern, high-speed computers.

## What are the issue with the two most commong password hashes for Java (“Java password hash” and “Java password encryption”)?

The two most common password hashing methods in Java, "Java password hash" and "Java password encryption," have significant security issues. Java password hashing algorithms like MD5 or SHA-1 are fast but vulnerable to attacks due to their lack of salting and susceptibility to rainbow table attacks. On the other hand, Java password encryption using algorithms like AES is not designed for securely hashing passwords, as it is reversible and involves complex key management. To securely hash passwords in Java, it is advisable to use dedicated password hashing libraries like BCrypt or PBKDF2, which address these issues by providing slow, salted, and secure hashing mechanisms specifically designed for password protection.
