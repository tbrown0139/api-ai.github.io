---
layout: post
title: Create Intents with System Entities
tags: 
  - System Entities
published: true
---

For your convenience, we have included pre-defined system entities.  We take care of common entities so that you don’t have to.  System entities include things such as countries, capitals, music artists/genres, times, dates, numbers, names, colors and more (you can find a list in the [entity overview](http://api.ai/docs/getting-started/entity-overview.html#system-entities)). When you use the system entities, there is variability included for incoming values (e.g. USA can be referred to as the States or the United States of America).

A simple example is found below, where we are including a few system entities for an intent to travel. 

<img src="/images/Screen Shot 2014-12-02 at 8.44.07 PM.png" width="636" />

To make this intent even more robust, we can make some more improvements by using <a href="http://api.ai/docs/getting-started/entity-overview.html#entity-types">inline entities</a>:

<img src="/images/Screen Shot 2014-12-02 at 8.54.31 PM.png" width="636" />

 Here, we are defining an inline entity that includes a broad set of US destinations that you can refer to.  We do this by using an inline entity format: “@{... , <list of different entities> , ….}:alias”.  The intent defines two alisases - "place" and "date" - that will be returned to you in the JSON object. You can try it out by entering this example and saying something like: “I want to visit the Statue of Liberty on Jan 3rd”.

Similarly, inline entity syntax is used to define a number of synonyms: “@{want to, wanna, have to}”.  Because there was no alias added at the end of this inline entity, nothing will be returned in the JSON.  This approach can be used to easily add multiple variations in one intent and reduce the number of user expressions that you need to provide.

If you find that a system entity is missing - <a href="http://api.ai/contacts/">let us know</a> and we will fix it!
