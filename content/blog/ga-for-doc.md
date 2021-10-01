---
title: "Leverage Google Analytics for better tech doc engagement"
date: 2021-10-01T19:24:22+02:00
slug: ""
description: ""
keywords: []
draft: true
tags: []
math: false
toc: true
---

# Google Analytics for Tech Documentation

We hear Google Analytics a lot, and here are a few things about it:

* It is a platform for tracking web site performance
* It uses a simple Javascript code to gather data
* It puts a cookie in the browser to report user interactions
* It is free

There are tons of tutorials about Google Analytics, here is just one of them: [The Beginner's Definitive Guide to Google Analytics](https://www.semrush.com/blog/beginners-definitive-guide-to-google-analytics/)

So, what does it do, to be more specific?

What data does it collect?

* How many visitors
* From where
* How much time they spend on your pages
* How they interact with your pages

What kinds of hits it gives you?

* Pageview hits
* Event hits
* Transaction/Ecommerce hit (you might not need this one for tech documentation)

## Set it Up for Hugo

Hugo has internal templates for Google Analytics tracking.

Once the tracking code is added to the site config file, e.g., `Config.toml`, there is data ready for scrutinizing.

```
googleAnalytics = "UA-123456789-1"
```

## Pageview Hits – It’s about view

### Which pages, for how long?

At the most basic level, there is always **Pageview Hit**.

### User Flow – Is there a common pattern?

No surprise that most of the time visitors land on the Homepage.

Dive deeper - Full page report reveals more

Top-level doc landing page

There are usually several top-level doc entries on a doc website, which is the most popular? Checking individual top-level doc
entries yields the relevant data.

Does it mean some pages are just bad?

Same function to be performed in different ways, thus in two docs.

The REST API page obviously attracts more attention.

On the other hand, it could mean the UI is intuitive enough thus not much need to check up docs.

Another reason to avoid spending too much time documenting UI (provided your UI is good)!

How we decided to go responsive

When Google Analytics shows there were mobile phone visitors who stayed very briefly, we took it as a sign that the documentation portal needs to go responsive.

The change was made by the end of March 2020. In July we had 6 Mobile phone readers, with 8 sessions in total, and on average they spent nearly 4 minutes browsing 10 pages per session.

## Event Hits – It’s about interaction

For more details, refer to the official website of [Google Analytics](https://developers.google.com/analytics) and the section for developers, for example, [Sending Data to Google Analytics](https://developers.google.com/analytics/devguides/collection/analyticsjs/sending-hits).


### What do you think about this page?

The biggest puzzle for any author, even a tech author, is the reaction from the audience. Do they like a page, or they hate it?

In February 2020, we added the three emoijs to documentation portal.

In April we got an unhappy face for one page. Though the feedback was from internal, we decided to let our visitors speak up more…

By the end of May 2020, we added an Office Form to collect feedback.

And the page url is sent to Google Analytics as an event hit

### More interactions

There are many ways to interact with a doc website.

Download a Postman collection, Download resources for integration, Open a PDF file, Switch between Web UI page to API page

## Why GA for Tech Doc?

Tech Documentation can Assist in Marketing and Sales:

* Technology is complicated and fast-evolving.
* Technical expertise plays important role from the very beginning of customer engagement.
* Accurate/consistent product information depends on the collaboration between product/engineering/marketing/sales, etc.
* Engineering team furnishes technical details, product team defines the scenarios/context, marketing/sales give it the flavor.

Content Ecosystem for Product Success

* The success of a product depends on efforts across teams/departments.
* Knowledge/information that could bring success is often scattered.
* A content ecosystem that encourages sharing/contributing while able to maintain consistency is a boon.

*Instruct, Inform, Interact*

You may want to contact marketing for a cookie consent management tool, and don't forget to consult with your legal team for legal concerns.

https://www.cssscript.com/cookie-consent-popup-purecookie/

## Further Reading

* [Google Analytics Cookie Consent](https://consent.guide/google-analytics-cookie-consent/)
* [Google Analytics Cookie Usage on Websites](https://developers.google.com/analytics/devguides/collection/analyticsjs/cookie-usage)
* [The Real Story on Cookies: Dispelling Common Myths About the GDPR and Consent](https://torquemag.io/2018/08/cookie-law-and-consent/)
* [Hugo and the General Data Protection Regulation (GDPR)](https://gohugo.io/about/hugo-and-gdpr/)
* [A GDPR cookie-consent banner for Hugo](https://liatas.com/posts/hugo-gdpr-cookie-consent-banner/)
* [Turn "Do Not Track" on or off](https://support.google.com/chrome/answer/2790761?visit_id=637326372745325164-3057588087&p=settings_do_not_track&rd=1)
