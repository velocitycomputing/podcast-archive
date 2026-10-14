---
record_id: "podcast:043e90b9-3d9b-4520-9d33-c0211a2a491e"
episode_id: 043e90b9-3d9b-4520-9d33-c0211a2a491e
title: The Race to Recursive Self-Improving AI
podcast_title: The a16z Show
url: "https://pocketcasts.com/podcast/the-a16z-show/20a7ca40-9128-0131-8b7f-723c91aeae46/the-race-to-recursive-self-improving-ai/043e90b9-3d9b-4520-9d33-c0211a2a491e"
audio_url: "https://pocketcasts.com/podcast/the-a16z-show/20a7ca40-9128-0131-8b7f-723c91aeae46/the-race-to-recursive-self-improving-ai/043e90b9-3d9b-4520-9d33-c0211a2a491e"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-12
played_at: "2026-10-12T12:00:00Z"
play_count: 1
duration_seconds: 1380
source: pocketcasts-history-browser
played_label: October 12
history_order: 2
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: ec94e3caf92df87367e73fb05dd9562991783ef9ee95eb167d3c934047248bee
analysis_mode: health
summary_source: hosted
model_source: hosted
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: claude-haiku-4-5
tagging_model: claude-haiku-4-5
proposed_tags: []
proposed_entities: []
status: new
routed_to: null
---

## Summary

The episode explores recursive self-improvement (RSI) in AI systems with MakerMaker.ai co-founders Daval Ajada and Owen Hu. True RSI means the AI system itself becomes both optimizer and optimizee—the model improves itself in a closed loop, unlike typical "autocatalysis" where humans use AI tools to build better AI. The founders distinguish RSI from claims that simply automate pieces of AI development. They emphasize optimizing across the entire stack (prompts, harness, weights, hardware) simultaneously rather than in isolation, and argue that measuring real progress requires tracking both performance gains (numerator) and resource costs (denominator). They present early empirical evidence that self-improving systems can increase capability while improving efficiency, though they acknowledge asymptotes exist and that distinctions between genuine improvement and noise require rigorous experimental work, including tracking reward hacking and GPU variance.

For practitioners evaluating RSI claims: demand clear answers to "what is the optimizer and what is the optimizee?"—if humans are still the improver, it's not true RSI. When reviewing performance claims, divide improvements by actual capital invested (not just FLOPs, but all human hours and experimentation). Prefer approaches grounded in mathematical frameworks rather than ad-hoc techniques, and be skeptical of announcements lacking replication and variance analysis. If working on similar problems, focus on domains with fast, cheap evaluation cycles (like inference optimization or code generation) where improvements can compound; recognize that domains requiring slow physical validation (drug discovery, clinical trials) will plateau more quickly regardless of algorithmic gains.

## Transcript

The fundamental idea here is to build AI that improves itself, and I think we're getting there.
For the first time, we could swap the optimizer as the optimize, and this leads to a reinvestment of cognitive improvement into itself.
You can think of RSI at many different levels of the stack: prompts, harness, weights, and you can go all the way to basically chips.
Our goal here is to optimize all the levels of the stack.
Our approach to RSI is that we have a multi-agent system working together that's been recursively improved.
I'm so impressed by your belief that, like, this idea of a model improving itself.
But it's not a belief.
This is a dramatic statement, which is, I think, the first time I've heard you say it.
Because we have been so thorough, we have not released things until we're super sure it's correct.
Do you envision a system where the amount of energy that goes into it somehow decreases over time relative to the improvement?
We can't share too much, but one of the very important things that we've tried to do.
A16Z general partner Martine Casado sits down with MakerMaker.ai co-founders Daval Ajada and Owen Hu to unpack recursive self-improvement, or RSI, and separate the increasingly popular term from what it would actually mean for an AI system to improve itself.
Daval and Owen distinguish true RSI from simply using AI to automate pieces of AI development.
Their goal is a closed loop where the system being improved is also doing the improving across components including models, harnesses, and eventually more of the AI stack.
They explain why closing that loop still doesn't guarantee runaway takeoff and why measuring real progress requires accounting for both capability gains and the resources required to achieve that.
They also share what they're seeing in their own research, including early signs that self-improving systems can increase performance while improving efficiency.
And they dig into the practical challenges of proving those gains are real, from variance and reward hacking to the enormous difficulty of distinguishing genuine improvement from noise.
Welcome, both of you.
We're going to be talking about everybody's favorite topic, which is RSI, recursive self-improvement.
Maybe to start, it'd be great to just introduce yourselves and your backgrounds.
So we'll talk a little bit about what you're working on now, and then we'll dig into the content.
I think of myself as a physicist of some kind.
I studied that, then I did the PhD in reinforcement learning at the MIT Media Lab.
I really like building things, and I'm very excited to be building a cool startup Maker Maker with Owen and Grace.
My name is Owen.
I was first studying math, and then one day I realized that all mathematicians do are proving theorems.
And I was taking a class called Formal Language and Logic, and they were showing how you can build a theorem prover.
And I was like, oh, that would be cool.
I can just build a machine that proves theorems for me.
That's how I got into AI.
Amazing.
And then for my PhD, I work on continued learning and meta-learning.
Then worked for a few years at DeepMind as a research scientist.
Now I'm working on RSI.
I see a lot of pitches come in, and a lot of them use the term RSI.
And I'll be like, oh, so what do you do?
And they'll say, we use AI to create AI.
That sounds very interesting.
So what do you do?
We use AI to create GPU kernels.
Which that doesn't, to me, kind of map the definition of what I would consider to be RSI.
So maybe can we start by you defining what you think or what you would include in RSI definitionally?
Yeah, I think RSI is definitely an overloaded term today.
Many people, when they say RSI, they mean different things.
So, I think the important thing when you are differentiating them is to ask the question: what is the optimizer and what is the optimize?
When you're self-improving, who is improving, right?
So, there are people who are saying, okay, we're doing RSI, we have humans using AI to develop better AI.
But that to us is just autocatalysis in a sense that the improver is still human with tools, even though these tools are getting better and better.
But the ideas and the improvement come from human brains.
Right, I don't mean to interrupt, but to be clear, most technical epochs have had auto-catalytic effects, right?
There's no way you can create a computer chip without a computer, right?
You could argue that the internet development was sped up by the fact that people that weren't geographically located could coordinate, right?
I mean, the steam engine, you could build better steam engines because you could get coal faster, et cetera.
So, this notion of using the thing to build the thing faster is not new.
And so, you're saying something different.
Yes.
I think for us in history, right, our civilization, we have this autocatalysis using computers to build better computers.
But the idea for this change, for this improvement, come from the human brain.
But that human brain was never the improvee, never the optimize.
Now, for the first time, we could swap the optimizer as the optimize.
So, the brain of the agents, which is the LM, the model, can be the thing that you're optimizing.
And this leads to a compound, this reinvestment of cognitive improvement into itself.
But there has to be a reason that you decided to take on this hard problem as opposed to what anybody else would do, which is like chew off pieces of the problem.
Yeah.
I mean, before I answer your more important question here, the reason I did this is I think it's a hard problem and it's fun working on the hardest problem.
And I think...
But do you have an intuition that this is the actual right answer as opposed to like something that's more pragmatic?
Yeah, I think a pragmatic thing would be just from a control theory perspective, if you have a gap in the system, you can't have a closed loop.
And autocatalytic has no closed loop, right?
So whatever you improve, there's still like a gap.
Humans have to come in.
You have to pour in other resources to make it work.
But if you have a closed loop, you still have to pour in resources, but the marginal gains ideally get either constant or larger over time.
And that's the fundamental difference.
I think what's really different here can be explained pretty easily.
So if you think of capability, what we're trying to do here is we're trying to improve the rate of improvement of capability.
So the first derivative of capability with respect to time is the thing that everybody is trying to improve.
And now you can put that to be equal driven by two things: the nominator and a denominator.
The nominator would be performance, which is what everybody is trying to improve.
And then the denominator is some kind of cost, let's say capital, right, or difficulty.
And this one is pretty set because the higher the capability, the higher the difficulty of the next step, right?
Now, the numerator is the interesting part.
For things like steam engines and whatnot, that was fixed.
So then you end up with a very simple differential equation where you basically plateau.
Now, if you have a system where the improveee, the things being improved, is also the thing that's doing the improvement, you now have a new way to think about it.
And the simplest case would be that the numerator is also correlated with capability, which makes sense, right?
Because the better you are, the better you are at also improving.
And if you do that, the math cancels out and you basically get constant improvement over time.
That could be one level of RSI, right?
And then there's one more case, which is now that the numerator could be correlated with a higher power of capability.
And then you get exponential takeoff.
Can we dig in a little bit more between RSIs having closed the loop and actual convergence properties?
For some reason, when people see a graph where there's like a circle with an arrow to another circle and it goes back, they look at that closed control system and they say takeoff.
Right?
Which, I mean, if this is a non-linear control system, it's very difficult to know what the hell happens.
By the way, most people don't seem to understand this distinction because we very quickly go to takeoff and foom and all that stuff when we talk about these things.
Well, as a network guy, you know that it depends on the exponent of your function that's self-referencing.
And it's what we found is that it's almost not useful to speculate on what we think could happen because this is really an empirical problem.
And the real way to know what's happening is to test things.
And testing things is really, really hard.
Like reward hacking is one of many problems that we have to deal with.
But the question you're asking is very empirical.
And for some other...
So I'm a networker.
That's how I would have answered.
I would have thought math people would have been like, we've got this differential equation.
And I took out my pencil and I wrote down the answer.
I mean, it is possible to write down the differential equation, but you still have to empirically measure the variable, the exponent.
So there's no analytical solution.
I mean, honestly, we don't even have a learning theory of deep learning.
We don't know fundamentally why it works, right?
And then now you're like five, six layers on top of deep learning.
And so we don't have a good theory.
I think the closest things we have are scaling laws.
And these are empirical laws.
I think one misunderstanding people have about our approach to RSI is that they think the entire system has to be fully automatic and digital.
But actually, if you look at our mathematical foundation, we have a multi-agent system, not just one digital agent.
And in this multi-agent system, human researchers and engineers are actually special cases of these agents.
And it's this hybrid system of multiple agents working together that's been recursively improved.
And we don't want to leave out any component to not optimizing them.
Because if it's possible to optimize the model, why wouldn't we do that?
Because you will have more gains if you do include those.
Anything that you don't optimize will later become your bottleneck.
So one observation that we have made here is there are claims of speed is improving, which is actually the case, right?
So if you look at the model release time, it is reducing.
And so on one hand, you can be like, okay, so clearly we're in some sort of a rapidly improving phase.
But if you divide by the actual amount of capital raised by these companies, that's no longer the case, right?
And so you're like, well, maybe they just raise a whole bunch of money and then AI allows you to apply that money.
So how would you, this is not for yourself, but how would you encourage people that are either evaluating claims about this or even working on them to think about not fooling yourself by throwing more money at the problem?
Like you're actually showing that you're making an improvement here that's meaningful with the denominator.
I think for us, it's pretty straightforward.
It's because if you get improvement and they just come at more and more resources being poured in, it's not RSI.
You have to be able to back your claim of how much improvement you're getting.
But do you include all the man hours and experimentation that went into that?
Because I feel like at some level, like that, it's like they'll talk about the actual flops that go in and the money that go in, but the reality is this is like the 23rd experiment and it's actually a human burning a lot of mental capital to get to that final configuration.
Do you actually include that in the denominator?
We do.
And I think it's good company discipline to do that.
And we've tried, again, to very intentionally from the beginning, have a culture of tracking where things go, cost, time, all that kind of stuff.
I'll share funny thing.
Internally, we have this thing.
People talk about leaderboards, you know, which is like score.
You know what I'm about to say.
We have something called a bleeder board, where we keep track of the cost of experiments of everybody who's running experiments.
That's awesome.
You know, and everybody, it's the comp everybody any day can look at like who's who's high up on the on the bleeder board.
I can also give an example from AI.
I don't know if you know this nano GPT benchmark they are running.
It's basically asking you to retrain GPT-2, which when it just came out, it's a very expensive model to train and it takes weeks, I think, on multiple GPUs.
And right now, people can train it on a single GPU within hours, and that number has been shrinking constantly.
Yeah.
But that's also totally separate, right?
Like that's just like whatever Moore's Law.
No, no, it's the same GPU.
It's the same hardware.
Using the same hardware and then improve the techniques of retraining.
Oh, interesting.
Yeah, what does improve is like algorithmic techniques, data techniques, kernels, all of that kind of stuff.
Do you know how much it costs to train GPT to I think it's a few hundred dollars?
I just said earlier.
Oh, wow.
So the same GPU.
Same GPU, same data.
And this is just algorithmic.
And do those come from humans or do those come from agents.
A lot of them are auto-research results.
But that's definitely the denominator.
That's not the dominant.
What you want to see is like you can do that with GPT-5, which we're not seeing, right?
Well, the cost of these things is going up dramatically.
I think one of the most closely guarded secrets in the industry is exactly this thing, which is how much compute you can get out of this.
Because in some sense, even if all you were improving was your denominator, you could get faster training because now you can get more rollouts.
Right, of course.
And that means now you can sample that what you were describing, like the manifold of the space of language more extensively.
And then you can get better trajectories, which means you can get smarter models when you use that to train.
For sure, improving the denominator is good.
Yeah.
For sure, improving the numerator is good.
I've yet to see, which is great that you have glimmers, where you can improve both the numerator and the denominator.
I mean, that's a pretty meaningful statement, which is awesome.
What we found is that a lot of the papers that claim to do RSI, when we test it in our internal infra, we find that they don't work.
And a lot of it is because they're cool ideas that humans try to introspect and say, oh, you know, this is what I think should happen.
They're complicated.
This sound cool.
They get you a good paper.
But then when we test it at scale, you know, on benchmarks, on real economic problems, they don't scale.
And what we found is that the simpler thing that closes the loop is the thing that scales.
I would say one thing that we do that's probably unique is that we always start with a very grounded mathematical framework that basically lays out the map of the whole space.
And the reason is because this space is so large that if you don't do that and you don't have this very principled way of doing it, you get lost very quickly in this complexity.
And the other reason is that often when you have this really complex system, there's two extremes of how you can build it.
You can take an approach where you basically build like 200 different systems and you hope that like this, this, you know, what is it, the Rube Goldberg machine will kind of work out.
Or you take the other way and you kind of basically spend some time thinking about these 200 things and maybe you realize they're actually just 12 abstractions that generalize to these 200 things.
And so what we have tried to create a culture of let's really think from first principles.
Let's look at the math and then we realize what are the assumptions we make to be practical because you have to do both.
And then we see what works.
And when you do that, you then can see that, oh, you know, these multiple papers or ideas are actually subclasses of the same general framework.
And if you do that well, you can scale.
And I think that's one thing that I see that's missing.
and that's hard to do and and takes a very unusual group of people to to really like make that work i think richard fan said once that there are two kinds of sciences there there's a stamp collections and then there are physics yeah so without a unified math framework all these research are sort of just stamp collections you could like a lot of this paper we're reading they're just ideas inspired by some human behavior and then they try to mimic that and say oh look we have rsi but then if you don't put into a unified system you don't know if the overall system is actually improving or you're just like locally applying an idea that that's getting better so what we have is that we're putting all these components that you could possibly recursively improve into a unified framework and look at it from a holistic view so that improving one part um does not negatively impact the other part right i see i see so so for example there are people who are doing recursive improvements just on harness and then there are people who are only doing on widths yeah but widths and harnesses are not isolated components they have impact on each other you can think of rsi at many different levels of the stack right you can think of um prompts um harness, weights yeah and you can go all the way to basically chips yeah right sure yeah and our our goal here is to optimize all the levels of the stack, right?
Efficient because we care so much about the denominator.
And then we started doing weights, weight updates.
And what we found is that you get more gains, but you still have to do harness stuff.
And you can keep going down the stack.
And my guess is that you probably will need to do a lot of the kind of co-optimization of many different parts of the system to make it work.
Can you talk a little bit about the problem domain that you're going after just to prove that this works?
We are trying very hard to pick areas of the AI space that are as close as possible to AI itself.
Again, we try to be recursive.
And if you think about it, there's not that many problems that are super close to AI and gives you improvement on both the numerator and denominator.
And one of those is the inference problem.
Because the more you can spend on, sorry, the more you can get improvements and efficiency out of inference, the more everything kind of unlocks.
And it's not just for technical reasons, but also the most promise of both the numerator and the denominator being improved.
It kind of breaks the mind, right?
So like just for everybody that's listening to this, there's two improvements going on here.
One of them is the ability of the model to make inference faster.
And the second one is now that the inference is faster, it can do that faster.
And again, that does not necessarily mean takeoff.
That can still, you know, asymptote at some point.
But it's just wild to think of this kind of compelling impact.
Yeah, yeah.
We're a startup, we're not a research lab.
And one of the reasons we chose it is because everybody in the world right now wants to serve their own model.
Yeah.
And everybody wants to use the latest, for example, open weight model, Chimi K3 or whatever, just coming out.
And they want to be able to serve it as efficiently as possible.
Right.
So it's an economically extremely important problem right now.
Just for the sake of discussion, if I wanted to make the inference for Kimi K3 faster, would I use Kimi K3 in a recursive way, or would I use a separate model and system to do that for Kimi K3?
To improve the serving stack of Kimi K3, you mean in our well, our system is not just using one LLM.
You have many different LLMs that are doing many different things.
Oh, so you're doing different parts of the.
Do you need the inference site for all of them?
I mean, again, we pick whichever is the most effective because it's being used the most time.
But the interesting thing is the choice of which LLM to use for which thing is also not always up to us.
We let the model choose.
To be honest, today it's not really us who are deciding what to optimize.
It's our agent because it's recursively self-improvement.
And what we're trying to do is not to limit itself to only one component.
So it chooses whether to.
Yeah, we try to be like as hands-off as possible, let it do its thing.
Do you have like a single master prompt?
Is it like improve yourself?
But even that master prompt has been improving.
Yeah, and I mean, and it's not one RSI system because you can think of it as there's the thing that does the improvement, but then you also have to have the thing that knows what to improve.
And that's both are dynamic problems, and they are very co-linked, right?
How general do you think this ends up being?
Like right now, you're focused on speeding up inference in a specific domain.
Do you think that whatever approaches you're coming up with here generalize, or do you think there'll be a different one per target solution space?
Mathematically, we have defined it so that it's one system that generalizes to everything.
I think the one part of the system and by everything mean any problem domain that you can point AI to.
Correct.
But then there are physical limits, for example.
And one big limit of this is the human element.
I think the way that a lot of AI companies are thinking is, you know, let us use AI to replace humans.
But what we found is that there's so much that if you have good researchers and good engineers that they can bring to the table, that's going to be very hard to replace by agents.
And so that's why from the very beginning, we've tried to think of our basically entire company as a multi-agent system where humans are a kind of agent that's cohabitating with other AI agents.
Can we at least reduce bounds?
So, for example, do you envision a system where the amount of energy that goes into it somehow decreases over time relative to the improvement?
We can't share too much, but one of the very important things that we've tried to do in our company is not just work on the numerator, which is what I was describing earlier, which is your performance, but to work on the denominator, which is how much you can get out of the same amount of physics, money, whatever you want to call it.
Right, but do you think it's possible to have a system where the numerator continues to increase at the same way with the denominator being fixed or decreasing?
It's not just possible.
I think it's happening.
Really?
Yeah.
So it takes less energy to get better results.
Yeah.
Yeah.
Over time.
Do you think there's a universe in which that continues without asymptoting?
Because if that was the case, then you actually have takeoff.
I mean, it just seems to disobey information theory and the laws of physics.
Yeah, yeah.
I mean, I think at some point you're going to reach Planck constant.
Yeah.
You know, Planck length, Planck energy, Planck time, right?
So it will asymptote at some point.
But I think.
Oh, I see.
And so you think that asymptote is basically like the computation of the universe.
At least, yeah, I mean, you know, how many particles are there?
10 to the 80.
Like we know speed of light, you know, we know what it is.
You multiply those two, and you basically get an upper bound of computation.
And so, given this fixed amount of computation you can do every second, we know we have a limit.
I'm so impressed by your belief that like this idea of a model improving itself.
But it's not a belief.
No, you've got a miraclear that.
That's amazing.
Also, it's a question of what metric you use to view the progress, right?
So if you use, I don't know, benchmark accuracy, it's upper bounded by 100%.
You're never going to see exponential improvement on that because it eventually bottom back at 100%.
So for a long time, we had this question: how do we even know if something has ticked off, right?
If we don't have the right metric, it's not a belief that this is happening.
I think we're already seeing glimmers of that happening.
But it is a dramatic statement, which is, I think it's the first time I've heard you say it.
Wait, is this like a continuous result, or is it relatively recent that you're starting to see glimmers of this?
No, we've been seeing these results kind of grow and grow and grow over the last few months.
That's amazing.
How do you have confidence in the results given, you know, like it's not working yet and you don't know?
No, it's not a belief.
It's empirical measurement.
But also, as a company, there's a very funny thing that is happening, which is because we have been so thorough, we have not released things until we're super sure it's correct, right?
And every few months, you know, there's like an announcement of something RSI-related.
We look at it, we're like, we should have released our results or something.
And then we look at it, we try to replicate it, and we realize, oh, it's noise, you know, it's cherry-picking.
And so it's very, very hard to know in this sea of, you know, AI, I don't know what you want to call it.
Like everybody's trying to do AI RSI stuff to know what's legit or not.
The technical answer is you have to be really, really good at measuring things.
So, for example, we have one of our engineers that we named him the Viceroy of Variance.
That's a real thing.
Like, his job, his job, is to go and destroy the results we have and find what's wrong.
And we even have little Slack emojis that we have.
There's one where there's red laser stuff coming out of his eyes when he finds that there's bad variants and stuff.
One of the things that we found is that when you're dealing with a new benchmark or a new problem of economic value that you want to apply this to, so far we have not found a replacement for what we call quality time.
Literally running hundreds of experiments, looking at it, developing an intuition, trying to figure out what is wrong, what is not wrong, what is just variance, what is not.
What is this weird thing that actually shows that there's some kind of reward hacking, like two levels down?
The agent that built the agent that built the agent did hack something, and now you have these weird results.
It's not easy.
So, when I have dealt with non-linear control systems, there's a bunch of in networking, there's a bunch of degenerate behavior you have to deal with.
It's not like just convergence and divergence, you have things like oscillations, and this is a very multi-dimensional problem.
So, do you have to deal with all of that stuff, like potential oscillations?
And then, on top of that, you have noise.
LLMs are fundamentally super stochastic.
So, what we find is that specific agent on a specific benchmark, you know, there's levels of noise that sometimes are unpredictable.
And some of them are extremely weird.
Like, you even have some weird noise that comes from this GPU and this other GPU.
They're both, you know, B200, but they have slightly different behaviors on the physics.
And you can see some of that being replicated at the high level.
So that's why it has to be an empirical thing.
So, from that, you could already see that intelligence is not a single scalar, it's more like a multi-dimensional vector.
And there will be domains and fields where this RSI will give you takeoff, and there will be dimensions where you might plateau or you will have relatively slow improvement.
And I think the defining factor is what is the slowest component in it.
So, you're an optimization person, you know that there's this MDOS law where the component, the speed up you can get by optimizing a component is you just take it to zero.
Yeah, everything else dominates.
Exactly.
So, the digital part we could optimize and accelerate, you could get like a thousand times faster or a million times faster.
But if it's only 20% of your orbital time, you're only going to get 20% speed up, right?
So, for domains where you still need to move atoms that interact with the physical world, that's really slow, you're still going to be bottlenecked by that.
So, let's say every evolve, every evaluation you need to do, let's say drug discovery, you still need to do wet lab experiments and then clinical trials, and that take months.
Then, every new idea has to go through a month or multiple months evaluation.
So, those fields probably won't be accelerated as fast as coding or mathematics, where you have very fast and cheap evaluations.
But I've yet to see is anybody put a balance on that.
Like, to say, in order for me to improve this by X to solve this problem, I need this much net new energy to do it, right?
And if you had that, you could actually predict, like, if I'm like, listen, like, how big of a warehouse do I need to solve like a drug discovery problem or how many different robots I would need to solve?
So do you think that we're getting any closer to actually having bounds?
Because I think this is such a critical question for all of us to answer.
One of the internal jokes we have in the company is that the secret to RSI is somewhere in a garden hose company in Wisconsin.
And the joke here is that if Einstein hadn't discovered relativity, he would not have these laws that tell you how speed and contraction of time works.
And if some unfortunate engineer had to design the GPS system, they would have had to find a correction of time.
And they probably would have said like, no, no, it's clearly not the fabric of space-time that's contracted.
But I don't know why, but this is the formula I've devised.
It's like empirically some absolutely, you know, some functionality.
Yeah, exactly.
And then people later would have been like, holy shit, this is like space-time contracting, right?
And we have this theory that, you know, like RSI right now is being thought of, let's solve all these super hard kind of fashionable problems.
But what we think is that the complexity of the world is such that the real challenges probably exist in spaces that are not being applied to, right?
And so that's the joke that there is some workflow somewhere in a garden hose company in Wisconsin that I think if we solve it, we get we get, you know, foom.
I love it.
I just want to quickly summarize.
So you're going after RSI.
In your case, this is not auto-catalytic effects.
This is actual RSI, where the system improves the full system.
And for you, it's an actual system, which includes the harness and the weights.
If you think about the problem, you've got a numerator and a denominator.
The numerator is like how good the system gets, and the denominator is how much energy goes into it.
You believe you're seeing glimmers of the sign where both improve at the same time using this type of approach.
Is that correct?
Yep.
Yep.
When can we expect to hear more from you?
Very soon.
Amazing.
Yeah.
Thanks so much, both of you, for joining.
Thank you.
Thanks for listening to this episode of the A16Z podcast.
If you like this episode, be sure to like, comment, subscribe, leave us a rating or a review, and share it with your friends and family.
For more episodes, go to YouTube, Apple Podcast, and Spotify.
Follow us on X at A16Z and subscribe to our substack at a16z.substack.com.
Thanks again for listening, and I'll see you in the next episode.
As a reminder, the content here is for informational purposes only, should not be taken as legal business, tax, or investment advice, or be used to evaluate any investment or security, and is not directed at any investors or potential investors in any A16Z fund.
Please note that A16Z and its affiliates may also maintain investments in the companies discussed in this podcast.
For more details, including a link to our investments, please see a16z.com forward slash disclosures.
