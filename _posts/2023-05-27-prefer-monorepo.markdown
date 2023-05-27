---
layout: Post
title: "Prefer Monorepo"
permalink: prefer-monorepo
--- 

There are numerous reasons to prefer a Monorepo to Microrepos and this post is about the de-duplication. More often than not, when a team size crosses 20, a Microrepo fanatic raises his hand and starts advocating a move for dissolving the Monorepo. "Build times are high", "getting blocked by other teams", "easier path to cloud", "drawing boundaries", and "everyone else is doing it, why not us" would be some of the reasons that get tossed around in upper echelons of management. Unsurprisingly, no one objects to this proposal. Proposals discussed, Jiras created, and smaller pods formed to work in silos. 

But the repercussions are surfaced only after a year. All the initial momentum of cross-collaboration gets tossed out of the window. And one immediate effect of decreased collaboration is duplication of effort. Common functionality that is supposed to sit in one modular is present across two code bases ,DRY principle is violated several times in terms of the effort, as the smaller pods are reinventing the same wheel. The general advice in such scenarios would be to have a common codebase so that the effort gets deduplicated. But in reality, there isn't enough visibility across the pods and there is no forced collaboration between those pods which will again lead to duplication of effort. 

Whereas, if you're operating a Monorepo there is a need for collaboration, which isn't pleasant at first. You need the patience to weather the inertia that people have against forced collaboration. And the benefits are observed after 6-8 months when people reap those benefits of faster execution and acquire a shared understanding of the codebase across the whole team. 

To have a frustration-less Monorepo you need a good manager who has some sort of expertise in Domain knowledge and mid-term vision. Otherwise, you will be looking down a bottomless pit of people ranting about the frequent issues and the only solution would be re-engineering the whole system. There is a caveat here if you're operating a services-oriented (the smaller pods have different working agendas and not a singular goal) team then the benefits of Monorepos are a tad less when compared to product-oriented teams. 