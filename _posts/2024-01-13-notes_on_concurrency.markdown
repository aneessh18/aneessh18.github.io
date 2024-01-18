---
permalink: notes-on-concurrency
title: Notes on Concurrency - 1
layout: post
---

1. CountDownLatch is effectively a centralized barrier where the gate is closed until the set timer is exhausted 
2. Using `sychronized` block is an effective solution for most of the problems. 
3. If multiple threads are trying to access the critical section of a particular resource, then is better to have a lock (mutex) on the resource itself. For ex: In case of ticket booking systems, every ticket must be represented as an object and it should have private `Object` which is used as lock for mutations. This way only the threads competing for the same resources are blocked, instead of linearising all of them.

TBC. 