---
title: "Code Review Notes" 
layout: post 
permalink: code-review-notes
---

I have had the opportunity to write bad code and read good code in the last couple of years. I don't think code reviews must be done through the lens of objective goals. Code reviews are prone to varied range of subjectiveness and people shouldn't be too religious of it without good reasons. 

The most important constituent of a good code review is common sense which is formed through experience (ex: people appreciate the value of logs truly only after they've experienced a terrible incident). So the below list is based off of my experiences in the Java Ecosystem. 

1. Make the Data Models (DTOs, Entities, POJOs) heavy with data validations. An object created during the Application's life must be valid by default. Don't create data in the runtime if it isn't valid. 
2. All the public methods should be throwing IllegalArgumentExceptions while private methods should be throwing IllegalStateExceptions. 
3. Use utility libraries like Apache Commons, Guava to de-duplicate code.[Guava's philosophy](https://github.com/google/guava/wiki/PhilosophyExplained)

This list be updated on a regular basis. 