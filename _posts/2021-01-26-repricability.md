---
layout: post
title: 'Reproducibility & Replicability'
date: 2021-01-26
comments: true
tags: [research, ai, conferences]
---

# Introduction

There are two major areas of concern in science with respect to scientific results. These are reproducibility and replicability of results.  I initially thought the words reproducibility and replicability can be used interchangeably and that there was a consensus within the scientific community about the meaning of each word.  However [1] distinguishes between these two words in the following way:

* ***"Reproducibility is obtaining consistent results using the same data, computational steps, methods and code; and conditions of analysis.***
* ***"Replicability is obtaining consistent results across studies aimed at answering the same scientific question by collecting  its own data.***

We can think of these two words as distinguishing the actions of two groups.  Reproducibility concerns the people who initially carried out the experiment and have presented it.  The action this group of people have to do to enable reproducibility is to provide all artifacts used to arrive at the scientific result. Replicability concerns a different group of researchers that aim to arrive at the same result using a different set of artifacts, thereby confirming the hypothesis set out by the first group.

As a researcher in Artificial Intellegince I have come to understand how sensitive Deep Reinforcement Learning algorithms are.  In addition, the algorithms proposed are sometimes hard to follow or implement.  One may need a lot of experience before finally being able to tackle implementing and tweaking a DRL algorithm to successfully run and learn in the environment it is deployed in.  Of course this experience is acquired given enough time; there will come a point when a researcher will be able to understand how abstract notions like a 'policy' come to be represented in DRL and transfer this from pseudocode to actual code.  In my opinion the process of acquiring the experience can be expedited and the methods through which it can be can bring benefits to the AI community.

In this post the focus is reproducibility through code because in my opinion having the code that was used to obtain the results can be extremely beneficial for other people doing similar research.  Below I outline several advantages that can be brought about when reproducibility is a 'must have' rather than a 'nice to have' requirement when writing and subsequently submitting papers.

> Note: The points made here are entirely biased given my little experience as a researcher, however I strongly believe that they can at least be of some value.  I understand that the nature of research is quite messy and at times no time is spent on polishing up the code however something is better than nothing.

# Immediate Verification of Results

The first advantage is that having a requirement for researchers to also provide the code that created the results can provide the means for an immediate verification by the reviewer which can in effect score more points when submitting.  This can help answer the question of how reliable or valid the results are.  Having an easy to run code accompanying the paper can help reinforce the idea presented but also provide reliable evidence for it.  Additionally, the results presented in the paper were created using code.  So even if the code is not clean or strictly following software engineering practices it at least still executes.

# Easier for New Researchers to Understand SOA

The biggest hurdle in my experience as a researcher until now was to get implementations of DRL algorithms.  Of course there are implementations to be found but sometimes they are quite abstracted to the point where it is hard to fully grasp the specific algorithm's nuances.  A new PhD candidate will therefore find it way easier and quicker to pick up the state of the art, especially in a highly competitive and fast paced field such as AI.  Having code to play with and see how the abstract terms take form in code is quite important when the time for experiments has come.  It will aslo enable for more time to think about experiments and understand the results rather than struggling to get the algorithm implementation.

# Improving Transparency of Work

One expectation I had early on when I started my PhD was that papers reflect the code to a great extent and that simply following the paper instructions I would be able to reach more or less at the same results.  From my experience reading and writing papers (only 1 awaiting the result still...) I came to realise how wrong I was.  There are many small but extremely important details that are sometimes left out of the paper.  These details may reduce the significance of the result or were simply not important to highlight the main idea.  Such a detail in my opinion can make the difference for someone new who does not have extensive experience in research yet. For example, normalising observations or rewards when training DRL algorithms.  Such details may not appear in a paper but they tend to make a difference.

# Conclusion
I hope this post sheds some light to the importance of having a code repository ready when a paper is submitted to a conference.  This should not be such a difficult task.  The newest papers I have read may come with code and this is becoming more frequent, especially with initiatives such as [Papers with Code](https://paperswithcode.com/).  However my honest opinion is that code should an important criterion in accepting a paper for a conference if not a requirement.  I believe this can be an improvement to AI research in general.  What are your thoughts?

# References
[1] Understanding Reproducibility and Replicability. [https://www.ncbi.nlm.nih.gov/books/NBK547546/](https://www.ncbi.nlm.nih.gov/books/NBK547546/)