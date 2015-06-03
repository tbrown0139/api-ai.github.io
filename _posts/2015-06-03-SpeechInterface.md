---
published: false
---

Even a capable developer can get fumbled by the components of a full speech interface.  Some might think, “Voice recognition sounds good enough,” but that’s just the first step. Voice recognition can fulfill your dictation needs, but when applied to use cases that call for a full voice interface, it’s not only inefficient, it’s the lead cause of users screaming and cursing at their technology. It’s our privilege and sacred duty to set the record straight.

The overall processing flow of a comprehensive speech interface consists of 3 key components:

<INSERT IMAGE HERE>

Speech recognition, speech to text, voice recognition, voice to text and automatic speech recognition (ASR) all refer to the same function: transcribing your spoken words. This first step converts your speech to text so that it can be processed (e.g. dictating an email or text to your mom). Devices need that component before anything else can happen.

(Side note: When working with api.ai you have a couple of different options…) 

**Option 1)** You can use our ASR.  This technology is based on statistical and acoustic data from over 2.5 billion processed requests to date.  Once our clients have an implementation with api.ai, we can provide custom language models based on domain knowledge.  Dynamic language models can also be generated or selected based on conversation and dialog focus.

**Option 2)** You can use any 3rd party ASR provider.

The second and most overlooked step is leveraging natural language understanding (NLU) technology. NLU cultivates natural interactions between you and a device; rather than being limited to very basic voice commands or needing to know the magic words to make it work. Let’s break it down:

		Intent Recognition: Needed to understand your user’s intent or meaning.

		Context Management: Needed for multi query cases.

		Conversation Management: Needed to support back-and-forth dialogue.

The speech that has been transcribed into text is still foreign to your technology and it won’t know what to do with it. Step 2 takes your text, which is your natural language input, and turns it into a structured object so that your product will understand. In other words, it uses **Intent Recognition** to understand what the user is asking for.

(Side note: Through advanced techniques in Machine Learning, api.ai can predict 
variations of what the user might say and still translate 
the meaning into the appropriate structured object.)

For example, a user could say, “Set thermostat to 72 degrees,” or “Thermostat to 72,” and the words are transcribed and then translated into an easy to read -- for the device -- structured object. 

<INSERT IMAGE HERE>

That’s an example of a single query interaction scenario. So what if you want to have some back-and-forth conversation with your device? You’d need context and **Context Awareness**. A user might say, “Set alarm for 7am,” and their device would respond, “Alarm set for 7am.” When they realize how unpleasant the 7am hour is, they could say, “That’s too early. Set it for an hour later.” And the device would know what their user was asking and respond, “Ok, alarm set for 8am.”

(Side note: api.ai has a sophistocated context managment toolset and engine implementation that supports both internal and external contextual data (e.g. GUI, gestures, diagnostics etc.).)

**Conversation Management** allows for the engine to seamlessly switch between conversation topics, while remembering what you were talking about (just like you wish your girl/boyfriend would).  Users can also have clarifying conversations with your product in the same session / conversation across devices.

Now the device can transcribe your words, translate them into a readable structured object so that it can understand the user’s intent and context, and support back-and-forth dialogue -- what’s missing? Fulfillment, implementation, follow through. After your device has a clear understanding of what you’re asking, it may need to take action to fulfill your request. Speech interface without fulfillment would look something like this:

		User: Turn on TV.
		*Nothing happens*
		Device: TV is on.
		User: …

So ask yourself, “Am I looking for transcription technology (speech to text)? Or for a back-and-forth dialogue interface that can deliver on my users’ requests?” Because afterall, who wants to live in a world without fulfillment?


Now you are equipped with an understanding of what a full speech interface requires and why it would crumble without each component. Our only hope is that you will take this knowledge and share it with those who think, “Voice recognition. That sounds good enough to me.”

