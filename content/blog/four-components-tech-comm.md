---
title: "Four Components of Whole Product Technical Communication"
date: 2022-04-26T14:20:02+01:00
slug: ""
description: ""
keywords: []
draft: false
tags: [Content Strategy]
math: false
toc: true
---

![Four components](/images/four-components.jpg)

## Recap and intro

It has been a while, so, here is a recap of what we mean by whole product technical communication:

>Whole product technical communication (WPTC) aims to streamline the communication of technology product information, build a cohesive product experience, and engage customers at every stage through the whole technology/product adoption life cycle.

The main challenge of WPTC is to bridge the gap between marketing and technology; a direct outcome is having technical information in the storefront, i.e., the corporate website.

You might be wondering why this is a challenge. If the technical documentation is already published as web pages, all there left to do is adding a link to the corporate website, with a label saying `Documentation`. Right? 

Maybe you have clicked that label on some polished websites, only to find yourself teleported to a world somewhat disconnected from the previous one. Such an experience will caution you against the WPTC-is-one-link-away perception.

Last time we briefly explored the [RACI matrix](/blog/exec-whole-product-tech-comm/#revised-content-responsibility-matrix) in WPTC, in this post we'll have a look at four areas that are of particular interest to our endeavor.

## #1: Design system

Go back to the example of one product with two faces. How does that come?

The problem is partly caused by necessity. CMS solutions for corporate websites mainly focus on marketing collaterals. They fall short if you are offering sandbox or code examples to engage API users, or doing continuous release for SaaS products. Instead of trying to accommodate a traditional CMS into a modern CI/CD pipeline, if that's even possible, it makes more sense to keep marketing copies and tech docs in different systems.

Nevertheless, difference behind the scene doesn't mean there cannot be a unified front. 

If your organization already has or is building a UI/UX team, chances are you have a [design system](https://www.robertcreative.com/blog/what-is-a-design-system) in place or in progress. To leverage design systems for a consistent look and feel, the first step could be a design audit. Are the UI elements in all the components/interfaces of the product following the same design principles? If not, is that a conscious decision?

![UI elements](/images/ui-for-docs.png)
<p style="text-align: center; font-style: italic">No UI elements in your technical documentation? Think again.</p> 

## #2: Information architecture

Adding new elements into an existing system often entails changes to the system itself, even substantial ones. To incorporate technical information into corporate website, we need to get ready for a (potential) structural overhaul, which is in the domain of information architecture. 

The [Information Architecture Institute](https://www.iainstitute.org/) defines information architecture as "*the art and science of organizing and labeling websites, intranets, online communities and software to support usability and findability.*"

What is the best information architecture for product information?

Ideally, the one you choose takes into consideration of requirements from the multiple stages of product adoption, and can accommodate information in accordance with the whole product model.

Getting the structure right could be the most challenging part of the whole journey. So, how do we get started?

A [content audit](https://www.semrush.com/blog/content-audit-for-content-marketing-strategy/) can help us identify the gaps: do you host duplicated content or miss some pieces? As we are looking at the whole product experience, it's also important to examine the connection between business values and technical aspects. Is the transition between different sections smooth? How difficult it is for visitors from different adoption groups to find the information they need?

![The information they are looking for](/images/looking-for-what.png)

## #3: Content governance

Design systems and information architecture deal with the presentation and organization of information. They lay the foundation of a cohesive experience on a website. With a solid foundation in place, the next challenge is to keep the information across the corporate website consistent.

Nowadays high-tech products are more and more in a collaboration mode with customers. They engage customers by demonstrating how easy it is to use the products and to build upon the technology. Educating customers become a task for multiple teams.

But, how to ensure that pieces of content provided by different teams are always up-to-date while not contradicting each other? 

The answer is maintaining a single source of truth. Or, to be more precise, maintain **a single source for each piece of truth**. The product truth is multifaceted. There is truth about pricing, truth about business domain, and truth about features and bugs. It's important to understand which team is the source of which piece of truth, and respect their authority and responsibility.

Have you ever come across blog posts that serve as release notes, or a configuration instructions page that talks about subscription plans? Content types are like the genres of movies. When you walk into a cinema for a thriller, you do not expect much laughter. Similarly, your audience has different expectations when they browse a blog post and follow an integration page. 

*Think carefully about the purpose of each content type, and keep the information to its proper place, by its proper owner.*

## #4: Analytics

Whether [data-driven, data-informed, or data-inspired](https://towardsdatascience.com/data-driven-vs-data-informed-vs-data-inspired-740eaaec6263), rarely anybody would argue against the importance of making the right decision using the right data.

So, what is the right data to collect regarding technical communication?

In [Lean Analytics](https://leananalyticsbook.com/), the authors argue that, "*at any given time, there’s one metric you should care about above all else*". They further suggest that "*There are three criteria you can use to help choose your [OMTM](https://leananalyticsbook.com/one-metric-that-matters/) (The One Metric That Matters): the business you’re in; the stage of your startup’s growth; and your audience.*"

Similar to the considerations we give when choosing the [Information architecture](#2-information-architecture), to choose the OMTM for whole product technical communication, we need to understand:

* the adoption stage of the product
* the position of the content in the whole product model
* the target audience

Based on this understanding, we can ask relevant questions. For example: What is the percentage of visitors who drop off halfway on your Getting Started page? Are there more hits on your knowledge articles than on your installation pages? Which topics on your Troubleshooting section are most visited? Is there correlation between support calls and your FAQ page?

Make hypothesis, find the metric to validate it, and improve. Also, remember that whether a metric is a [vanity metric](https://www.tableau.com/learn/articles/vanity-metrics) depends on whether we can act on it. A vanity metric at one stage might be the OMTM at another.

## Sum up

When making a plan for whole product technical communication, consider the following:

* leverage design systems for a consistent look and feel
* conduct a content audit to get the information architecture right
* maintain a single source for each piece of truth
* choose the metric that matters for specific content