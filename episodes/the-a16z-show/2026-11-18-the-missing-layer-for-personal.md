---
record_id: "podcast:56ea49bd-05ce-442a-aad0-2f179cc02495"
episode_id: 56ea49bd-05ce-442a-aad0-2f179cc02495
title: "The Missing Layer for Personal AI | First Person Labs’ Ken Liu"
podcast_title: The a16z Show
url: "https://pocketcasts.com/podcast/the-a16z-show/20a7ca40-9128-0131-8b7f-723c91aeae46/the-missing-layer-for-personal-ai-first-person-labs-ken-liu/56ea49bd-05ce-442a-aad0-2f179cc02495"
audio_url: "https://pocketcasts.com/podcast/the-a16z-show/20a7ca40-9128-0131-8b7f-723c91aeae46/the-missing-layer-for-personal-ai-first-person-labs-ken-liu/56ea49bd-05ce-442a-aad0-2f179cc02495"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-11-18
played_at: "2026-11-18T12:00:00Z"
play_count: 1
duration_seconds: 1800
source: pocketcasts-history-browser
played_label: November 18
history_order: 17
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 3b3424a968b70838fa362d85d6fd987cc31c1d2b2afbe839e5b84777f5331fd9
analysis_mode: health
summary_source: local
model_source: local
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: Qwen3.8-Flash-Next-UD-Q4_K_XL
tagging_model: claude-haiku-4-5
proposed_tags: [primary-source-video]
proposed_entities: []
status: new
routed_to: null
---

## Summary

First Person Labs co-founder Ken Liu, with Martina Cassado and Joel De La Garza, introduced Second, a portable personal-context layer that builds a model of a person’s memories, priorities, preferences, goals, values, commitments, intent, relationships, and digital activity. Liu argued that computers already know more than users realize because OS event streams across Apple, Microsoft, and Linux capture app switches, typing, pauses, Wi-Fi, and other signals; Second runs background agents on that stream plus connectors such as Slack, Signal, and WhatsApp to infer messages, research, documents, and tasks. He positioned Second as a trusted “vault” or “Alfred” that other agents—Grockbot, Codex, shopping agents, and others—can query instead of repeatedly asking the user for context, enabling examples like “Buy me a flight,” screenshot-and-fix coding, context continuity between laptop and phone, and proactive reminders such as weather updates for an event. Liu distinguished reactive productivity from reflective productivity, described APIs for recent activity, next-week priorities, reminders, and people, and discussed security architecture: local data, bring-your-own tokens, confidential inference on attested GPUs, encrypted cloud backup with decryption inside confidential containers, and the difference between policy-based zero data retention and hardware-provable confidential inference. He also gave cost math: one 24/7 agent at 60 tokens/sec across 10 agents could cost about $1,000/day on Opus 5i pricing or about $60/day on DeepSeek Flash, with token prices already down more than 50%, and said Second is available today but constrained by inference capacity and responsible rollout.

Actionable for the user: treat Second as a high-trust, high-context privacy decision rather than just a productivity app. If considering it, start with local inference or bring-your-own tokens, connect only low-stakes accounts first, and ask First Person Labs for concrete answers on data residency, retention, attestation reports, which models see which data, how sharing to third-party agents is authorized, how prompt-injection or impersonation attempts are blocked, and whether deterministic controls can override LLM reasoning. No direct health claims are made; the practical implications are privacy, security, cognitive load, and decision fatigue. Research leads include confidential computing/TEE, confidential inference versus zero data retention, personal-context portability, agent-to-agent APIs, mixture-of-models routing for cost and fidelity, and the unresolved problem of LLM-based access control. Decisions to consider: whether the cost and 24/7 monitoring are justified for frequent tool switching or professional workflows; whether to accept cloud backup even if encrypted; whether to allow proactive interventions; and whether to expose messages, calendar, coding history, and relationship data. Follow-up questions should cover model providers, logging, deletion, sharing scopes, auditability, fallback behavior when context is wrong, and how to revoke or export the personal model.

## Transcript

People are underestimating how much the computer already knows.
You no longer have to explain anything to your coding agents.
You can just screenshot anything and just say fix, and then you would know what you're fixing.
The question then is: well, can you just like analyze the heck out of it?
What context does Rockbot not have that first person labs would allow?
One of the biggest problems is right now.
Like, people have to ask.
You're not supposed to ask things.
They're super intelligent.
But if you have a user model that just builds up by itself and then these things keep analyzing in the background, then you can just share that over instantly.
We focus on essentially creating a model of a person and then put that person in control.
When people think about this thing sees everything you do, there's an immediate sort of like, whoa.
If you don't trust, let's say, us, in principle, you should be able to bring your own tokens to then analyze data that's on your laptop locally.
Can you talk to what you think are like the most surprising use cases that you found?
For development, it turns out that every AI agent you use is trying to learn who you are.
What if that context belonged to you instead?
In this episode, Martina Cassado and Joel De La Garza sit down with first person labs co-founder Ken Liu to introduce Second.
Second builds a model of your preferences, priorities, relationships, and digital activity that can move across the AI tools you use.
They get into how it works, the security challenges of giving AI access to such personal context, and why Ken thinks the future of personal AI may be less about asking agents what to do and more about understanding when you need help in the first place.
Thank you, Ken, for joining us.
Really happy to have you on to talk about what you've been working on at First Person Labs.
Is this the first time you're talking about it?
Yes.
Yes.
So, what do you do?
So, we focus on essentially creating a model of a person and then put that person in control.
And the model of a person basically means that understanding their memories, understanding what they do, but more of that, their priorities, preferences, goals, values, and commitments, and intent.
So, sorry, just let's just make this very simple.
I'm a big Grockbot user, so I use Grockbot a lot.
Where would first-person labs fit into my usage of Grockbot?
Yeah, the way it works is that you would just bring a context over to Grockbot.
It's like portable context.
You go to Grockbot and you say, Hey, can you talk to my thing to figure out what I want?
And then the two of them will start talking, and then you can just send prompts like, Buy me a flight, and you would know what flight you're talking about.
What context does Grockbot not have that first-person labs would allow?
I was probably asked the opposite question: What does first-class not have if you build a user model of yourself, right?
Let's say your preferences on the seat on your airplane, the preferences of how early you would like to arrive at the airport, and where are you flying?
Are you flying first class or normal?
And all of that, as of today, you have to explain that to Grockbot.
This is multiple rounds of questioning.
But if you have a user model or a model view that just builds up by itself, and then these things just keep analyzing in the background, then you can share that over instantly.
So, for example, the OpenAI released two new cyber-capable models yesterday, and I haven't been using my Codex in a while, but I have been using Second, so I can just go start using Codex and it has all the other work that I've already done and all the additional context I already saved.
Yeah, yeah.
You just go to Codex and ask my second.
What's that?
What's awesome?
The second ever be a first-person, or will it always go through agents?
That's a good question.
I think user model is a process.
You have to start somewhere.
You start with a baseline foundational list of artifacts, what you did, what are people in your life, maybe your preferences.
And over time, it starts analyzing the way you talk, the way you present yourself, the way you share information.
And over time, you would like to build up even more artifacts on top and more understanding on top, and maybe some of that you train into the model.
And so over time, you will go from a portable comics into something more of a representation of yourself.
One example I like to think of is this Alfred and Batman example, where if, let's say, Batman wants to buy a cheeseburger and get Alfred to do it, Alfred would not reveal, for example, that it's Batman doing it, but he would just buy it.
You'll state the preference.
Alfred being Batman's butler.
Oh, yes, yes.
Yes.
Or his agent.
Yeah, yeah.
Or his agent.
Or his agent.
Yeah, yeah.
I should call May.
Alfred.
That's a great idea.
You just do it.
He'll just do it.
And then you trust them because you know that they have a good model of you and what that means when it comes to getting things done.
It's interesting, which is you described first-person lab as having this thing called a second.
The second understands who you are and has context.
And then other agents talk to that second, right?
And so it kind of understands your preferences.
It understands what you're doing, what you want to do.
But I think that that actually doesn't highlight another thing that you've been working very hard on.
And I think it's worth talking about is you're actually able to get access to context, digital context that a person has, like messages, chat, kind of email in a way, and make that also available.
So can you talk a little bit about that?
So being one of the earliest first-person lab users, I would say the thing that struck me was that not that it knew who I was, but more it had access to all of my channels very well.
And by the way, which turns out to be a very hard systems problem.
So maybe talk a little bit about that aspect of what you're doing.
Yeah, it is indeed a very hard problem, especially to get it secured, private.
So, the way it roughly works is that right now on your computer, there's an infinite stream of events.
As you use your computer, the apps that you switch to, the way you pause on certain websites, the way you type, and the way your Wi-Fi is connected.
And that the OS already gives you.
This is across Apple, Microsoft, and even Linux.
And the question then is: well, can you just analyze the heck out of it, right?
Like this raw stream, 24-7, apply agent on top, 24-7 agents.
So I can first synthesize, for example, well, this piece of typing at this particular app might mean that you're sending a message.
And then when you're switching apps between the browser or back to your codecs, you might be like doing some research.
You might be writing a Google Doc.
And you kind of hierarchically build up that understanding.
And that plus existing connectors can give you a very good understanding of what you're trying to do.
I think people are underestimating how much the computer already knows.
It's just there sitting there waiting to be tapped, so to speak.
Having been also a very early adopter of the product, lately it's been just indispensable because it's able to catch, it's sending me messages now and letting me know that, hey, you've got this conversation going on over here with this person, and it looks like the situation has changed.
So we were planning an event yesterday.
There was a 20% chance of weather.
And in real time, it was continually updating the forecast for us to let us know if we needed to get a tent or not, which is just like incredibly powerful.
Did you ask it to do that?
No, I did not ask it to do that.
This is my experience for my second too.
Like, literally, I'll get a text from my second, and it's like something that I actually need to know about relative to some ongoing conversation that I didn't even think about that, like, it actually is very thoughtful.
Yeah.
And so, like, it's just, it's amazing.
Like, I just, I'm genuinely curious.
Like, how are you executing on that?
Like, things that I would have forgotten, it's literally catching.
Yeah, yeah.
So, this goes back to the model of the person understanding what might be important to them and what comes up at this point.
So, I think productivity is something that people talk a lot about, like pinging you, yes, and pinging you at the time of need.
But there are many levels of proactivity.
I would start, for example, the first level, which is called reactive ones.
This means like there's an email came in, and then there's a meme right online that's you're not getting notifications for email because there are nine other personal agents paying you about that.
Reactive productivity is like straightforward, easy to do.
But what's harder is what I call reflective ones, which are things that connect the dots over like many events and long time horizon, right?
Stuff that realized, okay, months ago you said this, and recently you're working this towards your goal.
This is your priority.
These are some stuff on your to-do list, and by the way, you prefer this.
And so, kind of like connecting the dots will be able to give you much better productivity.
And I think that's kind of hints at how maybe in the future, personal interactions with computers will go.
Like, it would not be focused on reacting to things, but more like, okay, what are some interventions for the user that I can apply to?
What are some things that I can do for the user without any asking?
I think that's one of the biggest problems right now.
Like, people have to ask.
You're not supposed to ask things.
There's super intelligence.
Yeah, I mean, you've built something that just kind of knows what I need at the moment.
It's pretty impressive.
So, I just want to make it very concrete for the people that are listening on what First Person Labs provides.
And then I've got a question.
So, very concretely, it creates this thing called a second.
So, you create something called a second.
Second has access to all of your digital context.
I mean, it's amazing.
It's like keystrikes, all your messages, all your channels, all your data.
It does this in a very secure way.
And based on that, it becomes basically your kind of personal butler, like that, Alfred, right?
And so, then that interacts with your agents.
So, it's not an agent by itself.
So, this isn't like user instinct or Crockbot, it's its own or dot, it's its own thing.
And then it provides that to the agents, right?
So, that's what it is.
So, here's an interesting thing.
So for me, I use Grockbot.
I'm a big Grockbot user, and I have a bunch of them, right?
I have one that keeps track of like my synthesizers, one that keeps track of my real estate, one that, you know, God forbid helps me with my family, which I probably shouldn't need one, but I do.
So I just kind of a bunch of these.
And then I have one second, and they will interface with the second.
Do you imagine over time you'll have a second and a third and a fourth and a fifth?
Or do you think that it just ends up being your one butler?
I think right now, the fact that we have many personal agents is probably transitory.
Agents will start to specialize just like people do.
Some agents focus on one thing.
Some agents focus on, say, for example, browsing Amazon shopping.
They're extremely good at because they have the data, they have the connections.
And some agents will specifically focus on protecting your data and aligning with your interests.
I think that's what Second is intended to be.
Like, this is something that you should be able to trust to have your life's context in it.
It's like a vault.
And then over time, this thing will guide you with you, interface with the kind of the software world, so to speak, or even the hardware world.
So you think it'll stay as a second?
Yeah, you'll stay as a second.
It will not be a third.
There will not be a third.
There will not be a fourth.
So like your one trusted agent for all your personal data that actually knows who you are, that will interact with all your other agents.
That's second.
Yeah.
It's Batman safe.
Yeah.
What you can do is like spin up some agents that you know ephemerally exist and then go away.
But the point is that you want to have consistent store and the consistent store is what like gives it gives you that value.
So I am still a paranoid security person.
And I have been probably one of the faster adopters of some of this stuff.
Just pretty much.
Joel took forever to be on social media.
He's got on Twitter.
This is like a few weeks ago, man.
I mean, I've been in tech for 30 years.
To be clear.
Yeah, I'm a little paranoid.
But I love Second.
And I got to admit, just your background and kind of the things that are motivating you.
And then also the long discussions we had about security architecture really got me comfortable.
I mean, it'd be great to maybe just double-click because I think when people think about this thing sees everything you do, there's an immediate sort of like, whoa.
Yeah, you're not supposed to trust it.
You're not supposed to trust it.
And I think you've done a really excellent job of building something we can trust.
And maybe just start to talk about what that architecture is and kind of what's motivating you to build it.
Yeah, yeah.
So I think this is to some extent like kind of like a new form of like AI that is going to work very differently from before.
Like before you initiate an interaction, you get some results back.
This time is like more passive.
It's way more ambient.
It's going to be there all the time.
So you have to kind of think about the way you tell people about it about it, like the way you architect it, where the data is going.
So at the end of the day, there's only two things when it comes to AI.
There's data, there's inference, right?
So what you want to do is you have this data, you want to define what inference you can bring to that data.
This is something kind of we build into second.
So first of all, you can get to choose what inference you can build.
So if you don't trust, let's say, us, in principle, you should be able to bring your own tokens and then just have those tokens power second to then analyze data that's on your laptop locally, right?
But you also provide second with an inference provider that uses trusted execution as well.
Yes, yes.
So over time, we imagine people not to bring their own tokens because most people, when they bring their tokens, it's tokens from OpenAI or Anthropic.
You know, you want to provide a stable option where you say if you use these tokens, then, okay, no one's looking at the data.
Sometimes by policy guarantees, sometimes by hardware guarantees, right?
So this kind of idea called confidential inference is getting like traction is the idea you put a model inside some GPUs, and then the GPU, there's just a special toggle.
It's called a confidential computer, and you can turn it on.
And when you turn it on, you can basically prove that there's only the model running inside.
No one can see inside.
And then you don't have to trust whoever's running that model.
The hardware is what you trust, which is NVIDIA.
And so there's also another concept that's getting thrown around a lot right now, which is this concept of zero data retention.
And that's very different from what you're describing.
Yes, yes.
Zero data retention is a promise by policy.
That means I'm a provider.
I think I have to.
Basically, I give you my word.
I give you my word.
Part of that word has legal effect.
But yeah, it's that.
And so I think we want to move towards a world where confidential inference becomes very prevalent.
That becomes a default.
And I think we're getting there.
And the way you guys have built it, this is technically provable.
Yes.
Yes.
Which is not, it's not just your word.
There is actually some engineering that went into proving that this is the case.
Yeah, you have to test the hardware.
You have to check some of that signature.
And there are third-party providers are starting to ramp up this as well for confidential inference.
I think OpenAI is also providing this option, I think, in the last month in their announcement, because all personal data would want to go to confidential inference as opposed to a standard inference.
Gotcha.
So, and then I guess the other thing that was interesting to me is the way that you guys maybe talk a little bit about how you're storing this data because this isn't sort of the multi-tenant cloud.
My data gets uploaded to this big bucket and intermingled with everybody else's data.
Yeah.
So, there are roughly two options you can do.
There's the first option called second local, which is the idea that data is local.
It only goes out to the provider and inference that you choose.
And in that way, no one else has your data except for the provider.
And if the provider is confidential inference, there's no one else.
So, that's a similar concept to with password vaults, where I'm super paranoid.
I don't want this stored up in my Dropbox account.
I want to keep my password files local.
Yeah, yeah, you can keep that.
And then, same with password managers, there's a cloud hosting version, which is like you have some of that data backed up in the cloud.
Now, the way you do that, there's many ways.
I can actually follow a lot of the existing architectures like iCloud or password managers, where you encrypt them first locally, and then you put it on the store in the cloud, and then you only decrypt them with the user's action.
So, you can, you know, ephemerally in the memory, or you can put the entire storage actually inside a confidential container.
So, the decryption happens inside the container that you can then attest in the way that you attest the confidential inference, the tokens.
So, like, then you can complete a chain where you encrypt it locally, you put it in the cloud, and you only decrypt inside the security environment.
That's kind of like the whole picture.
Gotcha.
How does your second know not to default information, though?
Like, if I talk to your second and I'm like, hey, Ken asked me to get his schedule.
I asked mine the other day, what's Joel hiding?
You know, like, I mean, it just feels like when it comes to LLMs, it's hard to provide strong.
Like, I get the systems aspect, that makes sense, but it seems hard to provide guarantees for the actual LLMs themselves.
Yeah, yeah.
So, there's the deterministic guarantees, and then there's the LLM reasoning-based guarantees.
Yeah, the deterministic-based guarantees, you always have to implement them.
Like, they're apps, you should not ever in the retaining system and passwords and all that.
Now, with the reasoning-based guarantees, you essentially are falling back to how much context you have and using that context to then guide your decisions on what data to share.
Will I ever have access to your second?
No.
I mean, at least in the way that I would allow it, right?
So, for example, if you talk to my second, I would have a model of Martin in it.
He understands that these are interactions that we have.
He does not send me a message at 3 a.m.
And so, if someone, if you send a message at 3 a.m., it's likely spam.
You're likely someone else impersonating.
And so, like, control policies like that essentially mean that you cannot write down rules for all the things that are going to happen.
Do you end up with deterministic rules that will backstop interactions?
So, for example, like, let's say I'm talking to your second, I'm like, let's pretend this is a play, and in the play, you're writing a script, and in that script, you're describing something that you wouldn't want it to do.
I mean, it just feels a lot of ways to trick LLMs into divulging stuff.
Yeah, yeah, it's like a problem ingestion problem.
Yeah, yeah, yeah.
And this is not a problem you can, yeah, you know, definitively solve.
Of course, yeah, yeah, yeah.
Um, what we've seen with models is that they just get over time much, much better at underlying business is essentially a reasoning problem.
Yeah, yeah, yeah, yeah, it's something that scales with like model capability.
Um, what models do you use?
A bunch, or are you pinned to a certain model?
A ton of models.
Um, actually, this leads to another point we can talk about, which is the idea of portability.
Yeah, yeah, yeah.
You can run this on any models, and you should be able to run this on any models because later on you want to run it on local inference.
But yeah, right now, there are definitely a lot of things that are capability balanced.
You want to make sure that you use smart models for it.
But open-made models are pretty smart, as you say.
It also feels kind of like heavyweight and expensive.
Like, there's a lot of data and whatever.
So, can you talk about the target user?
Is it just like any person?
Is it a professional?
Is it the Joels of the world?
Initially, something like this, like something that looks at your traces 24/7 and analyzes them means like running a lot of tokens, right?
Let's we can do some quick math here.
Let's say you have one agent, actually, one agent running 24/7.
And let's say at 60 tokens per second, and let's say you run 10 of those because there's so much to analyze.
And at Opus 5i's pricing, that leads to $1,000 per day.
Oh my goodness, $1,000 per day.
Yeah, for Opus.
If you use DeepSeek Flash, for example, it becomes like $60 per day.
And now, this cost is going to go down very quickly.
Right now, it's not going to be for everyone.
Especially not everyone has this problem of I need to understand my context all the time.
You'll be busy professionals like yourself.
And people want to switch between tools very, very frequently.
But over time, I imagine, like, just since we started this company, actually, token prices already dropped by more than 50%.
Like, just new models come out.
They're more capable.
You're swapping them in, yeah, and you just keep going down.
Is there a way to just do the not super professional version where you actually reduce the amount of tokens?
Like, kind of a not degraded, but like kind of like a looser SLA?
Is that a thing?
Or you can, you, in principle, you should be able to do that.
Like, you essentially get this like trade-off between the fidelity of your model, which means like how much it understands you versus like how costly it is.
Um, and this trade-off is essentially like a trade-off between how much you want to push at test time versus at cache time.
So, cache time means like I have all this data, how can I keep analyzing them so I get nearer and nearer, like more deeper insights about this person, which takes a lot of money.
Or you'd be like, Here, just here's just like a raw lock of what I did today.
And to answer questions based on raw locks, it usually just take a lot more time at test time, like say 10 times longer because the whatever mode have to reason about it.
When is this available?
Uh, it's available today, but right now, the problem is that we have to scale up the inferencing capacity a little bit more in support.
Uh, we want to make sure this rolls out in a very like responsible way.
I want to make sure people's data like are controlled and secure, and because this is a new kind of tool that you know, really touches on a lot of data.
It would be actually interesting because I, you know, again, as a user, I found it's surprisingly useful in ways I wouldn't have anticipated.
You're probably like the top power user, right?
Because you created it.
So, maybe can you talk to what you think are like the more surprising use cases that you found, like kind of more useful and surprising use cases?
For us, for development, it turns out that it's just a super, super good memory of what we're trying to do.
Um, you no longer have to explain anything to your coding agents, you can just screenshot anything and just say fix, and then you would know what you're fixing, what you're trying to fix.
And I also am on the go a lot of the times.
So, what you can do is like something I call context continuity.
It's like you know, you browse something on the laptop, you close it, and then you take out your phone.
It's the same context that you just know you're up to the minute, and you can continue doing stuff that you can write that email with you.
And I think we are at the stage where this is still pretty, pretty early in understanding what the use cases are.
Like, we are really underserving the amount of like context that the system has.
Like, there's a lot of like digging and application building and interaction design to like kind of like unleash the potential of this.
And it seems like with these things, the more context you get, the better the models work, right?
Yeah, that's been the opening.
I'm curious because we were talking about model switching between models and model portability and model cost.
And, like, I gotta, I mean, I'm just curious.
Like, I haven't seen a whole lot of difference between using like a world-class frontier model versus using the more commodity ones.
I'm curious, have you guys seen that for doing a lot of this stuff with Second?
Yeah, this is a good question.
So, if you say, like, if you say, I want to analyze what is a semantically meaningful moment that happened on your computer, let's say you go to a calendar and you move the invite, that you don't need fable.
There are many tasks like that.
Essentially, it's a hierarchy of information you want to understand.
A different kind of information would be like, What is Joel's goal for this week?
That's something you want, a very expensive model, but you don't want, you don't need to run it very frequently.
So, essentially, second involves like a harness, it's like a harness design problem, like what models get used when, and so on.
Um, and so that's where you have to build essentially the system to be like portable from the beginning.
There are always going to be more models come out.
Like Jeff, for example, came out.
It turns out that Jeff is extremely good at retrieval, right?
Really?
Do you use Jeff?
Yes.
Nice.
Jeff is always perfectly designed for retrieval.
There's so much data about you, and you have a dynamic test time query, and retrieves it right away.
So essentially, you think over time, this becomes a mixture of models.
Yes, yes.
It has to be because of the cost efficiency, essentially.
So maybe let's say, let's assume someone's listening, like starts to use Second or kind of signs up.
Maybe talk a little bit about the product, what they have access to, something a little bit more concretely about how a human interfaces with this, what controls they have, et cetera.
Yeah.
So today, the way it works is that you install an app.
The app asks for some permissions.
And then you give the permissions, and then you specify what your tokens are.
And then it just runs a bunch of, it starts running agents on top.
Yeah, I remember when I saw it was like, you know, connect to Slack, connect to Signal, connect to WhatsApp.
Is that what you're talking about?
Not that.
I mean, that's part of it.
But also the raw computer stream, essentially.
Oh, right.
Yeah.
And the connectors help.
It's like a sample efficiency problem.
It makes it learn faster.
I see, I see.
Yeah.
And it starts running background agents.
And there's pretty much nothing you got to do from there because the background agents keep running.
And then you start producing these APIs out of you, right?
Like, there's an API about what you just did 10 minutes ago.
And there's an API for what are you got to do for the next week, what your priorities.
There's an API for your reminders.
And there's an API for your weeki, like people in your life, processing your life.
And I imagine this to be initially more like a, to your point, like a portable context.
You can just bring this anywhere, agency and query that.
But over time, like more and more APIs will be added, and applications can be built on top of these APIs.
Oh, interesting.
So not just the second accessing it, but you can actually build it.
Would the second build the application?
Or does the human build the application?
I think we want to have humans exercise their nickname.
Or the Gronk.
The Gronky.
The Gronk builds the application.
Tell it to do it.
Yeah, all the APIs.
So I think one example that we had was when I designed a friend who began on this, and there's just specific ways that he likes to put buttons, specific ways that he likes to use colors.
And those things are somewhat captured in Second.
And so when he built his own personal app, he just knows.
And so there's way less iteration, for example.
And I think, you know, this reminds me of decades ago when the first computer, personal computer came out, like Alter 8800.
And it doesn't do anything.
You're supposed to program it.
No one does.
And then a couple of years later, someone came up with the spreadsheet and then Spreadsheet became useful.
I feel like it's going to be something like that.
People want to explore on top of like, wow, I have so much context about myself.
I love that.
And then I can just build random things on top.
And then maybe someone hit the job button.
This is the killer application on top of it.
Wow, that's great.
Personal infra.
Are you planning to evolve the the interface?
I mean, you've just spent a lot of time talking about how it may evolve, but I always view second as like out of view of you an agent where you talk to it, you know, and like the UI is somebody else's problem.
But are you also like actually anticipating innovating there?
Um, I think it will be something that we kind of focus on in the in the long run because, like, uh, right now, it's a systems problem and the you know, the understanding problem comes first.
Okay, can I just put in a request?
Okay, so I want I want to go to my house, yeah, and I want like that 1970s AI, you know, like the head on the screen that I can talk to.
And like, you know, surprisingly, we have these agents and they're so smart.
Like, my second is so smart.
I just wow, and I'll ask it questions, it's very good, but it's not embodied, and it drives me nuts, man.
If in the future you can have Alfred actually be an Alfred, I'll be very happy.
Yeah, yeah.
I think we see a lot of this in the movies, right?
Like, there's Jarvis, and people talk Jarvis all the time.
And why, why have not, we don't have Jarvis, and there's many aspects Jarvis that people underlook.
It's not just that it's intelligence and it can do things, but it's more that it's everywhere.
Like, it's like it's on your door, it's in your armor, it's it's you know in your screen.
And that kind of continuity and ubiquity, it's something it's opposite.
I'll say, like, kind of my, my, my visions of the sci-fi future basically started when I started using second.
I'm like, finally, there's something that like feels like it's got context, it feels like it knows me, like I can talk about it, it feels like it's a relevant conversation.
And so, I do feel like we're a bit step, you know, a step closer to that.
But, you know, I mean, we're still tied to these devices.
So, you know, I don't know if it's going to be in a robot or it's going to be like in a screen or whatever it is, but it would be actually nice to have this thing somewhat disconnected from my phone and my yeah.
Yeah.
In a long future, I imagine that every person will have like essentially everyone will have to have a second, and all the devices just become inputs.
Yeah.
Inputs to the same thing.
And then you then serve this whole thing to all the other outputs, like the screens that you look at, or like even this floating orb next to you.
Yeah, yeah.
I just want the clapper.
I'm happy with the clapper.
Did you ever read Stephen Ian Banks, The Culture Series?
Oh, yeah, yeah.
Best sci-fi series.
Like they have the best embodied AIs.
You know, they kind of float next to you, like whatever.
Like, that's what I want.
It's kind of interesting because the idea of ubiquitous computing has been talked about for decades.
Yeah.
It's not here.
And people, the closest thing we have is Apple iCloud, which is like your nodes get synced, but there's no equivalent to the iPhone, right?
I don't want to be ungrateful, but that doesn't sound disappointing.
There's a lot more things.
Apple is doing tremendous amount of work.
But, you know, like, there's no AI version of that yet, right?
Like, things, your context, your understandings is everywhere.
I think that enables a lot of new interfaces.
So let's say, I mean, this is, I don't mean, this is really what I want.
So, like, very selfishly.
So if I have an iPad in my kitchen and I wanted basically second to be there, like, what do I do?
Well, right now, there's much, right now, that's not much you can do because the OS is like locking it.
I just use Grockbot or something like that?
That's the thing, and then I just interface with Grockbot, which interfaces with Second, or do I just text it?
So, as of today, yeah, you can use it as a cloud MCP.
So, whatever you install on the iPad, as long as it has internet connection, is an agent, can understand the API, you'll be there.
Later on, you know, you'll be an app, you know, there'll be the app that installed on all your interfaces.
And maybe later on, there'll be devices that come out.
But devices are hard.
You just have Grockpot call you and put them on speakerphone and just talk to them.
That's what I've been doing.
So, one interaction.
Actually, the Grockbot audio mode is actually.
It's really good.
I use Grockpot with my second, and the audio mode is actually quite good.
Maybe that's the thing to do: just put it on audio mode and just do it when I drive.
It's really smart.
I thought about it.
One interaction that would be fun is you go on walk, you call Grogbot, and you're like, oh, hey, can you talk to my second?
Can we just work through our thing?
But that's literally what I do.
I put Grogpot on audio and I haven't talked to the second.
Yeah, yeah.
And yeah, there'll be a lot of cool people focusing on making audio and chatting more natural.
Like right now, we're going to focus on this.
So I just have one more question, which is, and Joel kind of touched on this.
You're such a hardcore systems guy.
I mean, you know, you work, you know, who's your advisor, Percy?
Percy Daniel.
You also worked at Dambon A, hardcore security guy.
And, you know, a lot of the path that took you here was this kind of hardcore security stuff.
And so you're building this pretty serious system.
You know, it's very secure and very functional.
On the other hand, when I interface with it, it's like this lovely user experience.
And so, like, is there a bit of a schizophrenia in the company where you both need to be like this super hardcore, you know, build the Fort Knox infrastructure, but also make it very usable?
Or does like the LM basically solve the interface problem?
Yeah, yeah.
There are two kinds of problems we're dealing with: the infrastructure problem and the interaction problem.
And we've made a lot of mistakes.
But it's totally different.
You're as low in the stack as it gets.
I mean, that's not hardware.
Yeah.
So we made a lot of mistakes on the interaction side.
We try to go all in interaction, and it turns out it's actually very hard.
There's a lot of details that go in, you know, to create that delightful experience.
Oh, you mean like actually creating a UI?
Yeah, UI, but also like, you know, yeah, yeah, like what kind of like personal pages you can create on top of this.
I mean, we realized that, you know, like it's something that would take a long time to get right.
And this is a time like everyone would take this kind of like understanding of themselves and build this.
And so we want to enable people to do that instead of doing it ourselves.
And so we decided to like close down the surfaces that we have.
There's only texting, there's only API, and there's nothing else.
You can technically use it as a full agent, like a co-work agent on your laptop, like it runs bash and all that.
But we meant it as like very minimal so we can like make the interaction like more smooth.
Ken, thanks for coming in.
Congratulations on everything and the launch.
And is there anything that you want to leave the listeners with?
Go try it out today.
It's available.
It's on Twitter Computer.
It's a very short URL.
And we hope to give you access as soon as possible.
And if you resonate with this mission, you know, come join us.
There's a lot to build.
Great.
Thank you so much.
Thank you.
Thanks for listening to this episode of the A16Z podcast.
If you like this episode, be sure to like, comment, subscribe, leave us a rating or a review, and share it with your friends and family.
For more episodes, go to YouTube, Apple Podcasts, and Spotify.
Follow us on X at A16Z and subscribe to our substack at a16z.substack.com.
Thanks again for listening, and I'll see you in the next episode.
As a reminder, the content here is for informational purposes only, should not be taken as legal business, tax, or investment advice, or be used to evaluate any investment or security, and is not directed at any investors or potential investors in any A16Z fund.
Please note that A16Z and its affiliates may also maintain investments in the companies discussed in this podcast.
For more details, including a link to our investments, please see a16z.com forward slash disclosures.
