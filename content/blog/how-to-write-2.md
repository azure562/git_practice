---
title: "How to Write (and rewrite) - Part II"
date: 2021-10-23T09:06:12+02:00
slug: ""
description: ""
keywords: []
draft: true
tags: []
math: false
toc: true
---

![hard thinking, easy reading](/images/thinking-reading.jpg)

A peculiar challenge of technical communication is to convey complex information without confusing the audience. But what is *complex*?

Merriam-Webster defines [complex](https://www.merriam-webster.com/dictionary/complex) as *"a group of things that are connected in complicated ways"*. In other words, *complex* is the result of the (difficult to analyze, understand, or explain) ways things relate to each other.

So, if we can figure out how to make *the ways things relate to each other* easy to understand, would that solve the problem of conveying complex information? I think the answer is "Yes!" In this blog we are going to explore how to use logic to manage the complexity of technical communication.

## Pyramid Principle

[The Pyramid Principle](https://amzn.to/2qod35k) by Barbara Minto focuses on the logic in writing and thinking. Its major application is on large and complex text (which sounds like what we have 😏).

On the surface, applying Pyramid Principle consists of:

* grouping ideas that support the same main point

* summarizing the grouped ideas

* constructing the pyramid

Following the Principle, the underlying structure of a text would look like below:

![pyramid structure](/images/pyramid-1.PNG?width=350px)

While the methodology is straightforward, to effectively use Pyramid Principle is not as simple. After all, *logic* implies hard thinking.

## Visual Hierarchy

If the author has done his/her part of hard thinking, would that guarantee the result is an **_easy read_** for the audience? Only if we also provide visual cues to help navigate the complexity.

[Visual hierarchy](https://en.wikipedia.org/wiki/Visual_hierarchy) is *a pattern in the visual field* and an important principle in [interaction design](https://www.interaction-design.org/literature/topics/visual-hierarchy). As the *Pyramid structure* already suggests a visual image, it's no surprise that visual hierarchy could be of use in technical communication as well.

Let's see how we can use different styles to build visual hierarchies based on the pyramid structure.

![visual cues](/images/visual-cues.PNG)

💭 *A word of caution: How to decide the size of a chunk (content block) depends on the nature of the content. The goal is to help navigation, not to disrupt the reading flow.*

But are these all there to know about managing the complexity of technical communication? Revealing the underlying structure not only makes the text easy to follow, it can also expose potential weakness in the text. 

## Devise your buckets

In the diagram above we created a visual hierarchy that reflects the underlying pyramid structure of a text. Would it stand up to scrutiny? When reading closely, does it make logical sense? What if some main points overlap, while some main points are missing?

To answer these questions, we take two steps:

* Map out our goal and the main points (buckets):

  Back to the user journey analogy, have we established all the main points necessary to cover the whole journey? Does each main point occupy a unique position on the journey?

* Evaluate the ideas in each bucket.

![buckets and ideas](/images/buckets-ideas.PNG?width=450px)

An ingredient of the Pyramid Principle, the [MECE principle (Mutually Exclusive, Collectively Exhaustive)](https://strategyu.co/wtf-is-mece-mutually-exclusive-collectively-exhaustive/) provides guidance on how to validate the buckets and the ideas within.

Once you have practiced this method for a while, you are likely to find that a more important outcome is that you can identify gaps in the content, and the opportunity to improve the content (substance) without damaging the visual clarity (form).

## Let's practice

[Agile Manifesto](https://agilemanifesto.org/) has four core values and twelve [Principles](https://agilemanifesto.org/principles.html). We know that principles are based on values. How do the Agile principles support the values? Can we group the principles (*ideas*) into the values (*buckets*)?

### My experiment

Below is my experiment (the number preceding each principle indicates its position on the [Principle page](https://agilemanifesto.org/principles.html)).

* Value 1: **Individuals and interactions** over processes and tools

This value seems to be about *team*. So I put the team-related principles here.

```
(5) Build projects around motivated individuals. Give them the environment and support they need, and trust them to get the job done.

(6) The most efficient and effective method of conveying information to and within a development team is face-to-face conversation.

(11) The best architectures, requirements, and designs emerge from self-organizing teams.

(12) At regular intervals, the team reflects on how to become more effective, then tunes and adjusts its behavior accordingly.
```

* Value 2: **Working software** over comprehensive documentation

This value seems to be about *deliverables*.

```
(1) Our highest priority is to satisfy the customer through early and continuous delivery of valuable software.

(3) Deliver working software frequently, from a couple of weeks to a couple of months, with a preference to the shorter timescale.

(7) Working software is the primary measure of progress.

(10) Simplicity--the art of maximizing the amount of work not done--is essential.
```

❓ Is the principle 10 in the right bucket? 

* Value 3: **Customer collaboration** over contract negotiation

This value seems to be about being *customer-centric*.

```
(4) Business people and developers must work together daily throughout the project.

(9) Continuous attention to technical excellence and good design enhances agility. 
```

❓ Where does the principle 9 belong? Is agility a value in itself?

* Value 4: **Responding to change** over following a plan

This value seems relate to *change management*.

```
(2) Welcome changing requirements, even late in development. Agile processes harness change for the customer's competitive advantage.

(8) Agile processes promote sustainable development. The sponsors, developers, and users should be able to maintain a constant pace indefinitely. 
```

❓ Which value does principle 8 reflect?

### Now it's your turn

Do you think there is a different way to structure the principles, or even refine the values?

## Recap

To manage the complexity of technical communication, try the techniques below:

* Use the McKinsey **Pyramid Principle** to expose the underlying structure of a complex text

* Create **visual hierarchies** to help the audience navigate the complex

* Devise **buckets** to support the user journey