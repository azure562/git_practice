---
title: "Google Analytics for Tech Docs"
date: 2021-10-01T19:24:22+02:00
slug: ""
description: ""
keywords: ["hugo", "Google Analytics"]
tags: ["hugo", "GoogleAnalytics"]
math: false
toc: true
---

You might have heard about the [build-measure-learn feedback loop](http://theleanstartup.com/principles), a core component of the Lean Startup 🦄 methodology. **Measure** is important to learn how customers/audiences respond to a product or service.

But, how do you measure the performance of your tech docs? 📚

In this article, I'll share some learnings when using Google Analytics to understand visitors' reactions to a tech docs website.

## What is Google Analytics?

First thing first, Google Analytics:
- is a platform for tracking website performance
- uses a simple Javascript code to gather data
- puts a cookie in the browser to report user interactions
- is free 🤗

There are tons of tutorials about Google Analytics. You can also follow the free online courses at [Google Analytics Academy](https://analytics.google.com/analytics/academy/) and earn certificates.

## What can it do?

Well, Google Analytics can do many things. For online tech docs, we are mainly interested in the following:

* Where did the visitors come from? 🌐
* How many visitors during a certain period? 🧑🏿‍🤝‍🧑🏻
* How much time did they spend on the pages? 👀
* How did they interact with the individual pages? 🤸

Answers to these questions are found in the **Audience** reports and **Behavior** reports, using data collected through **Pageview hits** and **Event hits** (Transaction/Ecommerce hits usually do not apply to tech docs).

*The examples below are captured using [Google Merchandise Store demo account](https://analytics.google.com/analytics/web/demoAccount?appstate=report%2Fvisitors-overview%2Fa54516992w87479473p92320289%2F%253F_u.date00%253D20150801%2526_u.date01%253D20150831%2F).*

## Audience

The question of *where did they come from* is answered in the `Audience -> Geo -> Location` report.

![location](/images/ga-demo-geo.PNG)

## Behavior

When a user landed on a page, a **pageview hit** is sent to Google Analytics.

### All Pages

To check out which pages are the most popular and the average time a visitor spent on individual pages, we go to the `Behavior -> Site Content -> All Pages` report. 

![pageview](/images/ga-demo-pageview.PNG)

### Content DrillDown

But more interesting is the `Behavior -> Site Content -> Content DrillDown` report. Try to view it as a pie chart.

![content drilldown](/images/ga-demo-contentdrilldown.PNG)

💡 For a tech docs website, there are usually several top-level doc entries. Content DrillDown report can give you a clear idea about visitors' preferences.

### User Flow – Is there a common pattern?

One question people are curious about is: can Google Analytics tell us whether the visitors follow a common pattern? 🗺️ For example, which page is the most common landing page, which page does a visitor usually go next?

For this purpose, we need to look at the **Behavior Flow** report.

![Behavior flow](/images/ga-demo-behaviorflow.PNG)

This information could be helpful when considering the information structure of the doc website.  

## Event Hits – It’s about interaction

The biggest puzzle for any author, including a tech author, is the reaction from the audience. Do they like what they see/read, or do they hate it, or are just indifferent?

A simple trick to find it out is to place some emojis (😀 🙁 😕) on your web pages, and send an event hit when a user clicks any of them.

Have a look at DOCSY's [User Feedback widget](https://www.docsy.dev/docs/adding-content/feedback/#user-feedback).


The syntax for GA event hit is as below:

```
ga('send', 'event', eventCategory, eventAction, eventLable, eventValue)
```

Once you understand how GA event hit works, you can track more interactions.

For example, to send an event hit when a user clicks a button:

```
<button type="button" onclick="ga('send', 'event', {{ .Inner }}, {{ with .Get "href" }}{{.}}{{ end }}, window.location.pathname);">
```

For details, refer to [Sending Data to Google Analytics](https://developers.google.com/analytics/devguides/collection/analyticsjs/sending-hits).

At this point, you might get curious about what a visitor would say if they are given the opportunity. Adding a Microsoft Office Form or Google Form could be an option.

## Cookie Consent and GDPR

Yes, Google Analytics uses cookies. With 🍪 there comes all the headache of privacy concerns.

If you are in a tech doc team of a company, you may want to contact the marketing department for a cookie consent management tool, and consult with your legal department for professional guidance 📜.

Reference information:

* [The Real Story on Cookies: Dispelling Common Myths About the GDPR and Consent](https://torquemag.io/2018/08/cookie-law-and-consent/)
* [Google Analytics Cookie Consent](https://consent.guide/google-analytics-cookie-consent/)
* [Google Analytics Cookie Usage on Websites](https://developers.google.com/analytics/devguides/collection/analyticsjs/cookie-usage)
* [Turn "Do Not Track" on or off](https://support.google.com/chrome/answer/2790761?visit_id=637326372745325164-3057588087&p=settings_do_not_track&rd=1)
* [IP Anonymization (or IP masking) in Google Analytics](https://support.google.com/analytics/answer/2763052?hl=en&ref_topic=2919631)

## Set it Up in Hugo

Hugo has [internal templates](https://gohugo.io/templates/internal#google-analytics) for Google Analytics tracking.

Once the tracking code is added to the site config file, e.g., `Config.toml`, there is data ready for scrutinizing.

```
googleAnalytics = "UA-123456789-1"
```

More reference information:

* [Hugo and the General Data Protection Regulation (GDPR)](https://gohugo.io/about/hugo-and-gdpr/)
* [A GDPR cookie-consent banner for Hugo](https://liatas.com/posts/hugo-gdpr-cookie-consent-banner/)
* [A cookie-consent popup](https://www.cssscript.com/cookie-consent-popup-purecookie/)