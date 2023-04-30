---
title: "Code Review Notes" 
layout: post 
permalink: code-review-notes
---

I have had the opportunity to write bad code and read good code in the last couple of years. I don't think code reviews must be done through the lens of objective goals. Code reviews are prone to varied range of subjectiveness and people shouldn't be too religious of it without good reasons. 

The most important constituent of a good code review is common sense which is formed through experience (ex: people appreciate the value of logs truly only after they've experienced a terrible incident). So the below list is based off of my experiences in the Java Ecosystem. 

1. Make the Data Models (DTOs, Entities, POJOs) heavy with data validations. An object created during the Application's life must be syntactically valid by default. Don't create data in the runtime if it isn't valid. 
2. All the public methods should consitute a try-catch block that encompass private methods that throw various type of exceptions. 
3. Use utility libraries like Apache Commons, Guava to de-duplicate code.[Guava's philosophy](https://github.com/google/guava/wiki/PhilosophyExplained)
4. Always choose constructor based DI, it is easy to mock the classes and its method responses. 
5. Try to make the methods adhere to the Command Query Segregation principle. 
6. Don't Log obvious statements. A trail of Logs should convey the progress of an application's state 
7. Don't design the structure of code based on its test-coverage aspect. Write the best code you can. 
8. Thoroughly understand the type of expceptions that a external library can throw and plan exception handling around it. 
9. Always handle expceptions in AOP style. It de-clutters the business logic (ExpceptionMapper is a great example)
10. It is good to follow SOLID principles. 

This list will be updated on a regular basis. 