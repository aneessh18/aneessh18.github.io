---
layout: post 
title: "Writing Software Well"
permalink: writing-software-well 
date: 2022-02-05 1:25:00 +530
author: Aneesh  
---

There is a widespread notion in the tech industry that most of the day-to-day operations of a software engineer doesn't involve optimizing code, rather it is
providing reliable functionality for the piece of code you write that in turn manifests itself in a feature. And mostly it is true. Now providing reliable functionality means that your code shouldn't break when exposed to the unknown actions of the user and should also account for conveying meaningful messages in case it observes them.

Writing code in your college is different from the way you operate in the industry, in the sense that there is little to no economical value of the code and the shelf life typically ranges from 1-day (for weekly assignments) to 4 months (for capstone project). And after that mostly it is discarded or it is shoved into Github.

When the code you write has an economical value, it changes the whole way of producing code in a programmer's brain. Suddenly you should account for the downtimes and budget for undocumented user actions that can potentially bring down the service at worst. But the service going down isn't that much of a big deal if the code is functioning properly and can produce reliable results in case of documented actions. It isn't that easy to write a reliable piece of code when you are not the one using it and worse you also use some external services in getting the job done.

Once you add a lot of variables to this process, you're left with pondering over for at least hours even in case of a small change. Because it should satisfy all the unwritten requirements. I felt sad for my inability to produce reliable and compatible code quickly enough until I realized calculating and evaluating all these components in my head was the bottleneck as it was an obscure process. So I started writing down the high-level functionality of what the code should do (in the editor itself) and initiated the process of churning out code. This way also ensures that I can do robust testing.

