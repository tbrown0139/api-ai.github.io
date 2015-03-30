---
layout: post
title: "Going with mandatory versioning soon"
tags: 
  - versioning
  - api
published: true
---

Greeting Api.ai Developers!

We are announcing that **starting June 1, 2015**, the versioning ```v``` parameter will be mandatory in all api.ai calls. 
Introduction of the versioning support will allow us to add new functions and make improvements to api.ai that are not backwards compatible. We are using the approach proposed in [Foursquare API](https://developer.foursquare.com/overview/versioning).

Couple of examples of such changes:
	* Domains functionality that you might already have seen in the console
	* Enhacing the return formats for system entities. E.g. ```@sys.date``` entity will be handling dates both in the future and in the past.

To use it, include ```v=YYYYMMDD``` parameter when you make a request. For example, 
```
	https://api.api.ai/v1/query?v=20150330&query=weather&lang=en&sessionId=123
```


Check out our [HTTP API documentation](http://api.ai/docs/reference/#versioning) for more details.
If you have any questions, always feel free to <a href='&#109;&#97;il&#116;&#111;&#58;&#115;u&#37;7&#48;p%6Frt&#64;a%7&#48;&#105;&#46;%61i'>drop us a line</a>.


Happy coding!
Team Api.ai
