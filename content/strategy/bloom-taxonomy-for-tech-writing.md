---
title: "Bloom's Taxonomy for Technical Documentation"
description: ""
date: 2024-06-09T11:18:02+02:00
keywords: []
draft: false
toc: true
---

![objectives](/images/pexels-tirachard-kumtanom-112571-733856.jpg)
<p style="text-align: center; font-style: italic">Photo by <a href="https://www.pexels.com/photo/woman-writing-on-a-notebook-beside-teacup-and-tablet-computer-733856/" target="_blank" rel="noreferrer noopener">Tirachard Kumtanom</a> from Pexels</p>

_How do you define the success of technical documentation, and how do you measure it?_

Whether managing a tech writing team or writing as an individual contributor, you're likely to face these questions or wonder about them from time to time. Readability, typos, release frequency, time on page, unique users, pages per session, are all among the metrics that have been tried but to no one's satisfaction.

Could it be that the dilemma is caused by the ambiguity around the nature of technical documentation? Taken as just another type of writing, it's natural to be concerned about grammar and style; viewed as written website content, statistics about webpage interaction come to mind. So, what are we missing here?

Given that the primary goal of technical documentation is to help people acquire and apply knowledge of technical systems, software, services, and so on, it doesn't take much to see _**technical documentation is, at its heart, learning materials.**_

## Bloom's taxonomy

Once we (re)established the educational purpose of technical documentation, an immediate benefit is that we can actively tap into the rich literature of education and make use of various learning theories and models.

Bloom's taxonomy is a hierarchical model widely used in the educational setting. It covers learning objectives in three domains: **cognitive** - _thinking skills_, **affective** - _emotional responses_, and **sensor** - _physical skills_.

Objectives in the cognitive domain are knowledge-based. Therefore, they are more related to our subject matter: technical documentation in the software industry. The original version of the cognitive domain was published in 1956, and a revised version in 2001.

![image](https://www.simplypsychology.org/wp-content/uploads/blooms-1024x512.jpg)
*image source: [SimplyPsychology: Bloom’s Taxonomy Of Learning](https://www.simplypsychology.org/blooms-taxonomy.html)*

The revised version replaces nouns with verbs to emphasize:

- Learning is an active process.

- It's important to include measurable behaviors in learning objectives.

Also, evaluation and synthesis (create) were swapped. I like to see this as echoing the concept of "generative learning" advanced in Peter M. Senge's [The Fifth Discipline](https://www.goodreads.com/book/show/19236648-the-fifth-discipline), the desired outcome of learning.

Critics of Bloom's Taxonomy argue effective learning and knowledge application should not be presented as a linear process. What they fail to appreciate is that giving a complex topic a clear structure is in itself no small accomplishment.

## Learning objectives of technical documentation

Bloom's taxonomy proves to be a concrete framework that helps educators understand the mental processes of learning and identify key learning objectives. When we see technical documentation as learning materials, we can also benefit from it in defining documentation objectives and developing effective content.

At each cognitive level, there are certain verbs to further clarify the relevant thinking activities.

| <div style="width:128px">Cognitive level</div> | Cognitive tasks | Verbs (keywords) |
| :-------------- | :-------------- | :--------------- |
| 1 - Remember | Recall facts and basic concepts. | define, list, identify, repeat |
| 2 - Understand | Summarize and describe main ideas in own word | describe, explain, outline |
| 3 - Apply | Apply knowledge in a new but similar context | illustrate, complete, solve |
| 4 - Analyze | Break knowledge into parts and explore relationships | categorize, distinguish, relate |
| 5 - Evaluate | Critically examining relevant and available information to make judgments | assess, rate, justify |
| 6 - Create | Use information to create something new | adapt, assemble, design, revise |

Using Bloom’s Taxonomy verbs to construct learning objectives not only guide target audience through a structured and progressive understanding of the subject matter, but also outline the specific needs the technical documentation should fulfill to help learners be successful at work.

## An example

Now let's try to write, _with assistance of ChatGPT_, a learning objective per cognitive level for the API documentation of an online payment system:

**1. Remember**: By referencing the API documentation, a junior developer can identify at least 6 key API endpoints and their primary usage within the first 30 minutes of reading.

**2. Understand**: After reading the Authentication section, a junior developer can explain the purpose and typical use cases of the authorization endpoint.

**3. Apply**: By following step-by-step instructions in the documentation, a mid-level developer can use the API to complete a successful payment transaction in a sandbox environment within a 1-hour hands-on session.

**4. Analyze**: By reviewing documentation and examples for at most 45 minutes, a mid-level developer can distinguish between synchronous and asynchronous payment processing methods in the API and compare and contrast at least three key differences.

**5. Evaluate**: By reviewing the API documentation and the provided reference materials, a senior developer can produce a report with at least 3 security considerations for each authentication method in the online payment system over a 2-hour evaluation period.

**6. Create**: By using the provided API documentation and sample code, a senior developer can develop a new API client library in a preferred programming language with all necessary endpoints and error handling, within a 4-hour development period.

## References

- Niall McNulty: [Everything you’ve ever wanted to know about Bloom’s Taxonomy](https://www.niallmcnulty.com/2019/12/introduction-to-blooms-taxonomy/)

- SimplyPsychology: [Bloom’s Taxonomy Of Learning](https://www.simplypsychology.org/blooms-taxonomy.html)

- Halyna Kornuta, Ron Germaine: [Cognitive Level: Bloom’s Taxonomy of Educational Objectives](https://www.csustan.edu/sites/default/files/OAQA/documents/BloomsTaxonomyMay2009.pdf)
