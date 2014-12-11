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

To make this more robust and to step up the complexity a notch, we can look at the example below.  Here, we are defining an entity that includes a broad set of US destinations that you can refer to.  We do this by having “@{... , <list of different entities> , ….}:parameter”.  The named entity will be assigned to the “place” parameter along with the respective date to be returned to you in the JSON object. You can try it out by entering this example and saying something like: “I want to visit the Statue of Liberty on Jan 3rd”.

<img src="/images/Screen Shot 2014-12-02 at 8.54.31 PM.png" width="636" />

We can note that I similarly used the “@{... , …, …}” convention for “@{want to, wanna, have to}”.  Because there was no parameter added to the end, nothing will be returned.  This can be used to easily add multiple variations in one intent.

If you find that a system entity is missing - let us know and we will fix it!
