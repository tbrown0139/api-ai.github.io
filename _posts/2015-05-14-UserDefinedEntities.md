---
layout: post
title: User Defined Entities
tags: 
  - Entities
  - User Specific Entities
  - Request Level Entities
published: true
---

As an api.ai super user, you already understand the power behind the platform.  Your implementation is reaching its final stage, and you have started to ask for more advanced capabilities.  Most frequently, developers just like you are interested in being able to customize entities on the user/request level.  

Let’s take a look at a quick scenario.  You are a developer with an application to control all of the devices and settings in your smart home.  Out of the box a user can refer to their objects in generic ways like “turn the lights on in my office”.  But - what if the user wants a more personalized experience?  If this is the case, the end user must be able to add their own names to refer to specific objects.  For example, rather than referring to a generic office entity, they could say  “turn on the lights in my mancave”.

In order to work with user entities:

1) Create an entity (e.g. @houselocation and @device entities for a smart home app)
Populate the entity with default values (e.g. @houselocation has:Kitchen, Living Room, Bedroom and @object has Lights)


2) Create an intent that uses this entity (e.g. "Turn on the @device in the @houselocation")


3) Utilize the new entities parameter in the query endpoint.
The entities object accepts an array of entities, following the format used in http://api.ai/docs/reference/#get-eid

The submitted entities will replace entities defined in the developer console just for this one request.

<img src="/images/example.png" width="500" />


Here's the curl example:

<img src="/images/Curl.png" width="636" />


The specified entity needs to exist in the developer console. The UI does not allow for creating an empty entity, so you must have some default value there.

On the Android SDK level:
To use the SDK please use the directive below instead of pulling it from the repo: 
	
<img src="/images/SDKdirective.png" width="300"/>

Usage example:

<img src="/images/UsageExample.png" width="636" />	
  

Finer grain controls for the entities are coming soon.
