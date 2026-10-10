---
record_id: "podcast:97b13d8f-5ce3-49cc-b665-07240ebf5090"
episode_id: 97b13d8f-5ce3-49cc-b665-07240ebf5090
title: "Episode 700: A New Co-Host, TypeSafe’s Jev, and Qwen3.8 at Home"
podcast_title: The CTO Advisor
url: "https://pocketcasts.com/podcast/the-cto-advisor/581a3430-2394-0133-b02a-0d11918ab357/episode-700-a-new-co-host-typesafes-jev-and-qwen38-at-home/97b13d8f-5ce3-49cc-b665-07240ebf5090"
audio_url: "https://pocketcasts.com/podcast/the-cto-advisor/581a3430-2394-0133-b02a-0d11918ab357/episode-700-a-new-co-host-typesafes-jev-and-qwen38-at-home/97b13d8f-5ce3-49cc-b665-07240ebf5090"
feed_guid: null
feed_url: "https://thectoadvisor.com/feed/podcast/"
published_at: null
published_local_date: null
played_date: 2026-10-01
played_at: "2026-10-01T12:00:00Z"
play_count: 1
duration_seconds: 1080
source: pocketcasts-history-browser
played_label: October 1
history_order: 29
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: f25cb6680b4305b0ac7ec0d9cd30a50e32eda525ca818c1e0357d454215ff7ef
analysis_mode: health
summary_source: local
model_source: local
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: Qwen3.8-Flash-Next-UD-Q4_K_XL
tagging_model: claude-haiku-4-5
proposed_tags: []
proposed_entities: []
status: new
routed_to: null
---

## Summary

Keith Townsend introduced Calvin Parker Hedricks as co-host of The CTO Advisor and discussed TypeSafe AI’s Jev, a closed-weight, non-conversational classifier that returns yes/no, confidence scores, or multiple-choice answers, reportedly runs in parallel across very large row sets and returns answers in milliseconds, and is priced around 42 cents per million tokens; they raised concerns that sending proprietary rows to a third-party classifier may expose data and that a general-purpose model may miss business nuance, while also noting possible uses in CI/CD eval frameworks and questions about enterprise agreements, BAAs, fine-tuning, vector stores, and RAG. They also covered Alibaba’s Qwen3.8 and Qwen3.8 Flash Next, including a 26B/27B model and a mixture-of-experts variant that activates only part of the parameters to reduce memory footprint; Keith claimed local runs on NVIDIA Spark and a Framework desktop with AMD chip, with Qwen3.8 completing 21 of 22 complex tasks on a single Spark versus 17 of 22 for another local setup, and Gemma 4 30B at about 10 tokens/sec versus 26B/4B-active at about 24–25 tokens/sec without perceived quality loss, plus local home automation voice and Scott Pocock’s research skill.

No health-related claims appear; the actionable items are technical: treat Jev as a fast, cheap classification/eval tool but not a default for sensitive data until TypeSafe AI’s data-retention, enterprise, BAA, fine-tuning, and RAG/vector-store terms are clear; test it on non-sensitive prompts, compare against open-weight alternatives such as Kev, Jev K5 (Apache 2), and SimF/OpenJev, and consider using classifier-based evals in CI pipelines to score model outputs. For local AI decisions, run Qwen3.8/Flash Next or similar MoE models on available hardware for tool-calling, home automation, and research workflows where privacy or latency matters, but model total cost against cloud APIs because local hardware may not be cheaper; follow-up questions should cover active-parameter memory savings, tokens/sec on target hardware, task success rates, data residency, and whether local inference provides enough quality to replace frontier/cloud endpoints.

## Transcript

We've been doing this for so long, the CTO advisor podcast for so long, that I stop at around 300 or 400 or so episodes.
I stop numbering them, but we are adding a bit of rigor, so we have to invent a number.
I think we should.
We're going to call this episode 700.
And for episode 700, it's kind of like Batman 500, Calvin.
We're rebooting the program.
I want to welcome my new co-host, Calvin Parker Hedricks.
Calvin, welcome to the program.
I'm excited to be here, Keith.
I had approached you a while back and said I think there's something we should do to collaborate together.
And this seemed like a really good way to help get going again and have that discussion around what CTOs need to hear, how we give them direction and the advice that they're looking for.
And I couldn't think of a better person to host it with because you're kind of like my yin and my yang.
You're my infrastructure to my development.
And I'm excited to have both perspectives on the pod.
Yeah, and it's really interesting because those lines are beginning to blur.
If someone asked me today, hey, I'm looking to get into technology.
Where should I start on the infrastructure side or the development side?
The answer is kind of yes.
Yes, it's right in the middle there.
And then even from a CTO perspective, and I know you've had this challenge yourself, what do I need my people to learn?
And the answer is again, yes.
Well, it's all the things, but not everything.
There's a lot of hype out there, and I think that's why we're here.
I think that is why we're here.
And we'll start this week's conversation off on two of the biggest hype points where, you know, AI is dominating the landscape for a lot of CTOs, not just from board-level demands of what the board wants to see, but also from practically, like, I need to get the most out of my people.
And the two topics we decided to talk about are models coming from two different points of perspective: Jev, J-E-V, and the other one is 3.58.
What's the Quinn?
3.3.8.
The Quinn38 model from Alibaba.
Yeah, so both big topics.
Let's start out with you just giving an overview of both.
Well, let's start with Jev.
What's your Jeff?
Let's start with Jeff.
If you've not been living under a rock for the last two weeks, this has probably been one of the biggest news items that has come across in a while as far as kind of super accelerant growth.
And what's interesting is it's not a model you can talk to.
So I think that's one of the important parts to first clarify with the folks out there who are having questions about this: what is Jev?
Jev is a classifier model.
It is going to look at a set of criteria, a set of judgment statements, and answer things like yes or no, or answer a confidence score about something, or it can answer a multiple choice.
Given these five options, what the user just typed into the prompt is: does it satisfy one of these options?
The thing, the real party trick here is that Jev does it very inexpensively and very, very quickly and can do it parallel.
So, where you may have a chameleon token context window on your SONET 5.5 that just released today, you can't fill Jev's context window like that.
It's going to take those options, those data you pass to it, put it in parallel, and ask the question simultaneously across, say, a million rows and give you back an answer in milliseconds.
And that, I think, is probably the thing that got me to go, ah, so one of the things that I've been doing in the Layer 2C lab has been a lot of fine-tuning.
And one of the most difficult things about fine-tuning has been question pairs and finding the right set of question pairs.
And, you know, you don't need that big of a model to be a decent classifier.
You know, you should be, you know, a decent amount of compute.
And I have a decent amount of compute locally with my NVIDIA sparks.
But it still takes time and effort to go through, let's say, 250,000 segments, which is what I have on my data set, and then create or weight answer pairs and say, is this, you know, hot dog, not hot dog?
Whatever, whatever I'm doing.
And that's where you're getting at.
And I think what's interesting is like people have taken, for example, the other topic here, Quinn3.8.
They have fine-tuned the six billion parameter version of that model to be a classifier to basically be an open weights version of Jev.
Because the other side of the coin for Jev is it is a third-party model that is proprietary, closed weight, and closed source.
You don't know who's behind it.
There's the, what's the name of the company?
It's TypeSafe.
Yeah, TypeSafe AI.
I don't know who TypeSafe AI is, but if you are handing them 200,000 rows of your data to do a classifier against, they now have your 200,000 rows of your data.
And some people may be thinking, yeah, okay, that's not a big deal.
My, you know, I'm running this stuff through open AI or whatever.
So that's not a huge deal.
But what is a huge deal is the nuance.
Both of us have done enough AI, and I think this is the executive level concern: is that can a general purpose model, even a classifier, know the nuance of my business enough to give me effective results?
What would Keith Townsend say?
Or what would Calvin say when it comes to X, Y, or Z?
We may have enough data out there that there's enough data in the model that that answer will come relatively strong.
But what happens if I don't mean Keith L.
Townsend and I meant Keith L.
Townsend?
Or that nuance?
So you still fall into the challenges that we have with general purpose models that are not tuned to our specific use case.
Yeah, and Jev, again, being closed weights, I don't know if that, I mean, this is so new to the game.
Right now, you go in, luckily, invites are back open again.
You can go sign up, you put down a credit card, and you're on your way.
But, like, I don't think you can do fine-tuning yet on top of that model.
I've got a bunch of questions, like, you know, can there be a vector store behind this and a search and basically a rag pipeline for adding my own data?
What?
Because it's not a model that I've talked to.
Correct.
But obviously, it works like any other model in the sense that there has to be some type of vector search capability in addition to the model's base training itself.
And plus, base training, as we know, base training, you can't, as much as I love all the secondary stuff, whether it's fine-tuning or rag, it's very, very difficult to defeat the preferences of a base training on a large language model.
Just try to do voice or some type of writing with one and see how many times that model will default to his training versus your garden.
Yeah, well, and I think that the model like Jev and the concepts that it presents to the end users will allow them to produce better, for example, eval frameworks in your CI pipeline.
You may want to incorporate this as part of your eval framework to be like, how close to the mark is the current large language model I'm talking to getting to what I was expecting from that prompt.
Yeah, so I'm not dismissing the technology at all.
It is an absolute brilliant use of a large language model.
I've been thinking about classifiers for a while now, whether we're talking about Google, Big Data, or BigTray, and kind of using BigTury to do some similar activities.
You know what?
It's nice to have something kind of squishy and a little bit probabilistic doing this what was deterministic work.
It blurs the line and gives us another tool.
Yeah, another tool in the Quiver.
I think it's just one you got to be a little careful with because we don't know all of the nuances yet.
Is there a business account?
Is there a team account?
Is there an enterprise agreement?
Can you get a BAA?
Like, be careful what you throw at that one.
But I think we should move over and talk a bit about Quinn 3.8 and the 3.8 Flash Next.
It has been all of the rage before Jev was all of the rage.
3.58 is just talking about, well, what is 3.58 and why should we care?
Well, the 3.3.8 is the latest release from the Alabama folks.
What's interesting is that they're keying us up for what's going to be the Quinn 4 release with the Flash Next release of that model.
So the 26 billion parameter version of 3.8, which released in rapid succession, which is why you find a lot of people saying, oh, it's 3.4, 3.5, nope, it's 3.8, got released like, what, a week and a half ago, two weeks ago?
But I put it to use right away in my house on my home automation system with my internal voice usage.
So none of my data leaves the house.
Its tool usage is super fast.
So it's really well adapted to tool usage, tool calling, and then the flash next version of it, which is a, I can't remember how many billion parameters version of that model is.
There's a unique new wrinkle that they're bringing to the table, which is this mixture of experts models that activates only so many of the neurons at one point in time.
So you can actually run it on a larger parameter model on a lower memory footprint.
Yeah, and GEMA, and I keep saying Quinn 3.5 for some reason.
I don't know why.
I'm stuck on Gemma.
It was the hotness for a while.
I was 3.5.
This stuff is moving exceptionally fast.
But GEMA 426B, 26 or 27B, 26B is a 4 billion parameter MOE model that does this.
So if you're familiar with mixture of expert models from the GEMA 4 sense, this is the same thing that they're talking about with 3.8.
Larger model, more parameters, but smaller in-memory footprint, which allows us to run this on lighter infrastructure.
To give Hannah a sense of scale, the GEMA models, there's a Jemma 430B.
I basically get about 10 tokens a second running that on my NVIDIA Spark.
The 26B with the 4 billion active parameters, I get closer to 24, 25 tokens per second without a, I haven't sensed the drop off in quality.
But the major difference between those models, those GEMA models, and the QIAN models in my lab, is that I've kind of hacked together a harness in which I can use Clark code and power Clark code with one of these models.
And 3.8 was the closest thing that I got to a frontier model.
Yeah.
Without running it on dual sparks.
There's a couple of larger models that compete, but running it on a single spark, I was able to complete like 21 or 21 of 22 really complex problems, of which only the closest thing that came locally that was not running on two sparks was like 17 of 22.
So I was kind of just playing around with it locally.
And I took the Scott Pocock's research skill that's kind of a deep research tool usage, and I put it against the Quinn 3.8 2627B model on my I have a framework desktop with the AMD plus chip on it.
And boy, did that thing work hard and actually complete the tasks and produce what I wanted, which was a lot of web research, a lot of creating spreadsheets, a lot of creating markdown research.
And it's been a good hour against the research.
The puppy has opinions.
Yeah, he did.
He had some real opinions about the grass band mode outside right now.
Yeah.
So where I want to kind of wrap this up and bring these two components together is that one, open wave models are getting very good.
Not only are they getting good, they're getting more and more efficient.
I think more so than we could ever imagine.
Jev is something like 42 cents per million tokens or something to that effect.
But I think most CTOs I talk to are not necessarily in a rush to go out and try Jev.
Yes, it's fun, it's cool.
It is fun, it's cool.
Absolutely, let's try it out.
But I am excited for the local version of Jev.
I know folks have been working around with.
We mentioned this last week when we were talking about the podcast topics: Kev, KEV, which is a fine-tuned version of Quinn 3.8 classifier specifically to emulate what Jev does.
Yep, that's the one that's on my list: the Jev K5.
There's also SimF, SimF, which used to be OpenJev.
What's interesting is with the first one there, the Jev K5, it's an Apache 2 licensed open source open rates model.
And this is, you know, where we're, and we'll tease this, maybe we'll talk about this next week, is this idea of cloud versus local inference, and where should the investment go?
Both of us have made not small investments in local AI.
Yeah.
We have some sense of what can practically be done with local AI.
And what I would love to talk about is the cost benefit of AI locally versus just simply consuming APIs from the cloud, which is exceptionally cheap because the math, I don't know if you've done the math.
I haven't run into much math that has told me that local AI is cheaper than cloud AI.
So there has to be advantages and what considerations are we seeing in the field.
Yeah, I think it depends on what's in the field.
And I think you also see that you get a consistent price over time if you buy your own hardware or rent GPUs in the cloud as opposed to the API endpoints.
Yeah, this is a bit of a spoiler alert.
This is cloud math.
Like the math application may have changed, but the math has not.
A lot of the drivers for why you would use local versus cloud or why you use cloud versus local has not changed.
If you have strong opinions about this, share it in the comment sessions on the video session of this podcast.
Or I don't know if the CTO advisor has a comment session anymore.
I don't think it does.
People don't comment on blog posts anymore, but it would be cool.
I'm sure we'll get in the video.
We'll get some comments.
I'm sure people will have opinions.
There's always some type of opinion about local versus people on the internet with an opinion.
You know what?
The best way to get engagement is to be wrong on the internet.
You'll get all the everyone in the world will correct you.
Calvin, this is your first time on.
Where can people find you?
One socials.
And plus, plug, what do you do for a little?
We didn't even say, what do you do?
So I am CTO and co-founder of Six Feet Up.
We are a Python and software agency that loves solving hard problems.
You can find me on LinkedIn.
It's probably the most active spot I'm at.
So just Calvin HP and all the other socials, whether you're on X, Mastodon, Blue Sky.
Come find me on those spots, and I'd love to chat.
All right.
And if you want to find me, of course, if this is Calvin's audience, for the first time you're trying to find me, I'm Keith Townsend, founder and CEO of The CTO Advisor, the name of the podcast.
You can find me on the website at CTO Advisor or all major platforms.
I'm still pretty hard X slash Twitter user.
That is probably the quickest way to engage with me.
Otherwise, I do spend an awful lot of time on LinkedIn.
If you have suggestions about what we should be talking about, if you have questions, my DMs are open on X.
Calvin, I don't know if that is the case.
Calvin's DMs are open on X at me on LinkedIn.
More than happy to take on requests or answer questions and engage with Pretty at You Fort Socials.
Until then, we'll talk to you episode 701.
Sounds good.
CTO Advisor podcast.
Calvin, go watch some baseball, man.
Sounds good, Keith.
You too.
