---
layout: post
title: "Master Git before you collaborate" 
permalink: master-git
---

I made the mistake of not learning Git beyond the basics and only giving a cursory glance at the list of operations it can perform. As it turns out, it is a powerful tool to collaborate and think isolatedly. 

Initially, I made myself acquainted with only the most used git operations. Commit, Push, Pull, Origin, Status, Merge and Fetch. Though I  performed my daily tasks with these commands, I did a lot of work that Git was supposed to do such as stash, reset and revert. 

1. I was hesitant to iterate on code-review feedback because I had to make changes which may have to be discarded in the subsequent review. I figured out that this issue can be resolved by moving that HEAD to different commits (which is agreed upon by both the committer and the reviewer)
2. There were cases where the task I was currently working on became blocked and I had to move on to the next task. But I wasn't comfortable either completely discarding or committing the progress I made corresponding to the blocked task. As a collective result of being dumb then and the task in hand being relatively small, I copied the changes to a file and applied those changes at a later point in time when the work was resumed. As it turns out, you can just *stash* it.

Essentially, I was doing tedious work due to my ignorance regarding Git. My life would have been much simpler, had I learned Git beyond the most used commands. 

**Note to self**: please keep revisting this [page](https://git-scm.com/docs) on a periodic basis and also experiment with them.   