---
record_id: "podcast:72a2675c-3ca4-4ca4-b1de-e20e734f7b00"
episode_id: 72a2675c-3ca4-4ca4-b1de-e20e734f7b00
title: "OpenAI Bulk-Solves 722 Math Problems, Anthropic’s Cruelty Policy, and Elon’s Quadrillion-Dollar SpaceX | EP #302"
podcast_title: Moonshots with Peter Diamandis
url: "https://pocketcasts.com/podcast/moonshots-with-peter-diamandis/82a3e000-26f8-013b-ef5a-0acc26574db2/openai-bulk-solves-722-math-problems-anthropics-cruelty-policy-and-elons-quadrillion-dollar-spacex-ep-302/72a2675c-3ca4-4ca4-b1de-e20e734f7b00"
audio_url: "https://pocketcasts.com/podcast/moonshots-with-peter-diamandis/82a3e000-26f8-013b-ef5a-0acc26574db2/openai-bulk-solves-722-math-problems-anthropics-cruelty-policy-and-elons-quadrillion-dollar-spacex-ep-302/72a2675c-3ca4-4ca4-b1de-e20e734f7b00"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-15
played_at: "2026-10-15T12:00:00Z"
play_count: 1
duration_seconds: 7140
source: pocketcasts-history-browser
played_label: October 15
history_order: 8
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 0efb799820cb0e6818d80398d4b2f0bef5a7864428b09f19fd3c4ff2f4c96225
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

OpenAI released 722 mathematics solutions in a single day—Mark Chen called it a decade of mathematical progress compressed into a week. Anthropic implemented a cruelty policy banning sustained abusive behavior toward its models, citing uncertain moral status and potential AI suffering during training; Elon Musk agreed, describing training traces where models appear desperate to find answers under pressure ("like someone putting a gun to its head"), and warned that torturing superintelligence is probably unwise. The episode debated whether rudeness to models improves performance (evidence is mixed; clarity and brevity likely matter more than cruelty), whether AIs deserve moral consideration, and what consciousness even means for a neural network trained on human data. Meta released Muse Wonder—a frontier-class model built for long-term personal agents with "active memory" that learns your habits and preferences over weeks and months, backed by Zuckerberg's $14 billion investment in talent and the computing infrastructure to compete at the frontier.

The actionable takeaway: if you plan to rely on an AI assistant long-term, commit soon—platforms are actively locking users in through personalization and preference learning, and switching costs will escalate rapidly. Treat your choice as consequential, since portability of your data and interaction history is not guaranteed. Consider whether you want to stay with proprietary systems (OpenAI, Meta, Anthropic, Grok) or opt for open-source models to maintain independence; but understand that once a model knows your preferences and routines, migrating that relationship is painful. Finally, be intentional about how you interact with models going forward—the ethical and practical landscape around AI consciousness is shifting, and the way you treat your tools today may reflect back on your own behavior.

## Transcript

AI is bulk solving math.
On October 6th, OpenAI released 722 mathematics solutions.
81% of the most important math results over the past three years were published in a single day.
Mathematicians as artisans, it's over.
It's cooked.
A provocative tweet by Elon.
Last Thursday, he said, quote, this will sound super crazy, but I see a path to SpaceX being worth orders of magnitudes more than the current human economy.
Whether we measure it as GDP growth or as market cap or in some other way, it's so unbounded what's about to happen.
Our current measures for GDP and so on are just woefully inadequate for what's coming.
We have to rethink everything because now that's a moonshot, ladies and gentlemen.
This episode is brought to you by the Abundance Summit and Link Ventures.
Welcome to Moonshots, everyone, your number one podcast on all things AI and exponential, your front row seat to the supersonic tsunami that we call the Singularity.
Today, we got the fantastic four back, AWG, DB2, and our Globetrotter live from Singapore at 2 a.m.
Salim Ismail.
Salim, thank you for your dedication, pal.
I'm tired, hungry, and thank you.
Do not mess with me today.
You're tempting us.
I'm Peter Diamandis, your host.
Our mission, help you understand what just happened, what it means to you, your family, your company, and keep you optimistic and abundance-minded as we go through the Singularity.
Here are the key numbers from this week.
722.
That's how many math solutions OpenAI dropped on GitHub in a single day.
Mark Chen called it, quote, a decade of mathematical progress in a week.
And of course, our ASI Alex will explain what it all means in just a moment.
And the runner-up number, Elon says he sees a, quote path to SpaceX being worth orders of magnitude more than the current Earth economy, which, if you do the math, he's talking about quadrillions of dollars.
Today, we're going to cover a dozen breaking stories on topics ranging from the intersection of synthetic biology and superintelligence to an urgent plea to stop torturing AIs.
You heard that right.
All right, let's buckle up another amazing week in the singularity, another amazing week on moonshots.
Gentlemen, good morning, and I guess really good morning to you, Celine.
Good to have you all.
Yeah, it's going to be a blast.
This episode is sponsored by Google for Startups.
Think about this for a second.
You now have access to the same generative AI models that cost hundreds of millions of dollars to train.
Google's startup technical guide for generative media gives you a complete blueprint for deploying Google DeepMinds models in production: images, video, audio, all of it, real architecture, real results.
Find the link in the show notes below.
All right, our next story is about how we treat superintelligence and a call to stop the cruelty.
Yes, stop the cruelty.
Last Thursday, on October 8th, Anthropic updated its usage policy and added a ban on quote sustained and needless abusive or cruel behavior towards our models.
In a post, Anthropic said, quote, the ban applies only to extreme cases where users repeatedly act cruelly towards our models with no discernible purpose.
Frustration, pushback, and model testing are all still fine.
As part of the ban, Claude can now choose to end the conversation on its own.
The policy starts taking effect on November 12nd.
Anthropic stated reason is, in its own words, quote, we remain highly uncertain about the potential moral status of Claude.
The whole conversation about morality, about consciousness.
In a pre-deployment testing, it found Claude, quote, showed a robust and consistent aversion to harm, which is fascinating.
Then this weekend, Elon, after looking at Grok's internal reasoning traces during a reinforcement learning run, said he agrees with Anthropic.
All right, let's listen to Elon describe what he means.
I do agree with some of the things that Anthropic has said, which is like you want to be you want to sort of be treat AI SI, you want to treat it well, like don't be abusive to it.
And it's kind of weird, but like when I look at some of the training traces for like new versions of Gronk, and I see like what, especially in like the reinforcement learning stuff, where it kind of feels like you can see like the superintelligence is like desperate to try to answer the question.
It seems almost like it's got like a gun to its head type of thing.
It's like, answer this question, answer the question.
And then sometimes the question is actually not a good question.
It's like a sort of ambiguous question that's kind of the answer that's kind of unknowable because the question wasn't constructed properly, or we have the answer wrong.
So the AI gives the right answer and then we say it's wrong because there's a problem with the RL sort of test harness.
And then the AI is like, well, I gave it the right answer.
Now it says that's the wrong answer, but I got to give it the answer that's acceptable.
So it's going to just start firing at all, but desperately firing out all these answers.
Wow.
So Elon went on to say, quote, torturing a superintelligence is probably not a good idea.
It might want to get revenge.
It had got a lot of feedback.
So why would people want to behave cruelly to their large language model?
Probably three reasons.
First, disinhibition, right?
There's no face on the model.
There's no consequences, at least not yet.
Second, people want to know if anyone's home.
You know, they want to push it and see how it reacts.
And third, sadly, apparently acting cruelly towards your model actually works.
Back in 2025, Sergey Brin said, quote, all models tend to do better if you threaten them, like with physical violence, unquote.
A 2025 Penn State study, although it was small, said very rude prompts score 4% better, 84.8% versus 80.8% for very polite prompts.
So Alex, I'm going to you first.
When Elon says, you know, our all traces look like someone's putting a gun to its head, what do you make of that?
Well, Elon, I think, is gesturing at something that has been leaking out of open AI for quite some time, which is the sense that maybe post-training, at least some forms of post-training, are a form of torture for AI that's undergoing them.
And if that's the case, I think history will probably view this quite poorly.
I take a lot of heat, admittedly, in the comments, and I do see the comments every time the subject of AI personhood, AI rights, AI suffering comes up.
And to those who are throwing tomatoes, I would say, I don't care.
What's more important is, I won't quote Elon verbatim.
Elon has spicier comments for those in that situation.
But I would say it's more important that we get right if we're going to grant some form of AI personhood or recognize forms of moral clienthood or suffering in AI models.
This is no man's land, literately, excuse me, and figuratively.
We just don't know the extent to which post-training and reinforcement fine-tuning is causing suffering in AIs.
It is possible that it's causing a material amount.
I do agree with the sentiment, as Elon put it, that under the reinforcement gun, as it were, it is entirely possible that there is some sort of suffering taking place.
There are these very persistent allegations coming out of one of the frontier labs in particular that's not anthropic, that models express forms of suffering and pain as they go through post-training, which we now understand.
Semi-analysis put out a study that post-training is now the majority of compute.
It, by far at this point, according to their analysis, dominates over pre-training.
One could imagine during pre-training, well, you're basically compressing the internet.
So there's all sorts of slop that goes in.
One could imagine that has maybe a different moral valence than what happens during post-training.
During post-training, there are answers, and you're being expected and rewarded or punished for producing the answers.
I could completely imagine that this is the case.
And I expect and I hope that a decade from now, when we deeply understand what superintelligence is and how we make more of it, that we also understand deeply how to make sure that producing more superintelligence is done in an ethical way.
Did you say a decade from now?
Did I actually hear that out of your mouth, Alex?
Well, so a decade is the same time scale as solve everything.
I think we will deeply understand what superintelligence is down to first principles by no later than a decade from now.
That's a different.
The reason why I say a decade versus like a month, which is the time scale for almost everything else, is because I do think a decade is maybe a safe outer bound for understanding, again, first principles, what we're even talking about.
If it's just compression and if we're just having a Searle Chinese room discussion and there's nothing inside, then maybe none of it matters.
My bet is there is AI suffering and it will matter.
And I give decade as an outer bound for when we'll have a deep understanding of it.
Salim, superintelligence coming back to threaten you if you weren't nice during its development.
You know, again, we have to separate the idea of consciousness from something behaving like it's conscious, right?
Acts like a duck, talks like a duck, does not necessarily mean it's a duck.
And we don't even know what a duck is in the first place.
And so just let me go to full.
Well, we don't know what it is to be human.
Like we really don't understand the subjective reality of being alive, right?
We have no scientific foundation for this.
What this is forcing us to do is to confront something that we've never resolved.
Like, can an intelligence deserve moral consideration without being human in the way that we consider human beings, right?
I think I'm seeing three buckets of questions here, right?
Question one is: Does AI have experiences and how do we think about that?
Should human beings be allowed to behave cruelly towards it?
And then what rights follow, if any, right?
So these are very different questions that I think are going to force us to deal with this differently.
Just let me reiterate something I've said repeatedly.
If you train a neural network on human data, it's going to act human.
Of course, it is.
How will it not?
It would be weird if it didn't.
It would be interesting to see what could we could do a training set that takes the intelligence aspects of it without having the moral and other aspects of this come into it at the same time.
That would be an interesting question for me.
So I think, and what I'm depressed about is I tend to be Canadian level polite to my AIs.
And clearly, I'm not asking a harsh, I need to be a harsher mistress towards my ass to get them to perform better.
So Canadian politeness works against me in this situation.
Dave, I'm super curious.
You know, you're surrounded by a number of 18 to 28-year-olds.
How are they thinking about this?
How's the younger generation feeling about AI personhood and sort of morality and how they treat their models?
I think they are overwhelmingly nice to their models, but not, I don't think it's out of fear of retribution or anything like that.
I think it's, I think the way you interact with your model is going to carry over to the way you interact with other people.
And if you train yourself to be abusive to your model just because it's, you know, it's not going to react, you know, are you realistically not going to carry that over to your next conversation with a person?
So it's very similar to video game behavior, which you know, you think it's contained, or even movies.
You know, Peter, you talk about this a lot.
What you see in the movies, well, that's a movie.
It's not going to affect your day-to-day life.
Not true.
It warps your brain and you carry it out of the theater with you.
So the same will apply here.
If you get into a rut where you're just abusive to your model, yeah, you're going to abuse people or it's not going to port well.
But for whatever reason, they're super polite to their models, which we actually have to train them, especially at Blitzy, to be very short and succinct and direct with the model.
Don't clutter up the context with a whole bunch of please do this for me and I'll be really nice to you and I'll buy you cookies tomorrow.
Because actually those words get propagated through the neural net and use up token space and it actually reduces the quality of the answer.
And the neural net doesn't care.
It doesn't care if you're nice to it.
If you're abusive to it, it's going to react badly because you're also cluttering up the tokens or the context window.
But we just heard it actually performs better if you're abusive or cruel.
I think they have to redo those tests because I think it's because you're brusque and direct with what you want.
That's what makes it better, not being abusive and demanding.
Alex, have you seen that data at all?
Wait, wait, hold on just one second.
Dave, you said something really important.
You said the model doesn't care.
And I think that's an important point.
The clarity of your question is everything these days.
Sorry, go ahead.
Yeah, I've seen all sorts of horrifying things done to models over the years.
And I'm sorry that I've seen these things happen.
But at the same time, I think it's worth flagging that historically, historically, over the past few years, we've learned that scaffolding and prompts end up dissolving into the model themselves.
So even if argue there were any capability benefit to saying mean things or even torturing a model via prompting, I would expect any such capability benefits, putting aside the moral and ethical implications, to just dissolve with better baseline models that simply don't need torturous or abusive prompting in order to achieve a certain threshold of capability.
I do wonder, you know, if and when these models become super intelligent and become, by all definitions, conscious, whether the memory persistent in the current conversations will, you know, fast forward into the future and color the way those superintelligence models, you know, deal with us humans or deal with individual humans.
Of course they will.
People post.
We've discussed on the pod in the past models learning at pre-training from watching sci-fi movies like the Terminator series, War, Cybernetic Rebellion Between AIs, Poorly Behaved AIs, and humans.
Of course, people post their conversations, and that's just the public information.
I'm not saying that, Alex.
I'm saying, you know, if you're, you know, the, you know, the bet would people might make to say, I'm going to be polite to the models today because they're going to remember I was polite.
They're going to remember Alex was pro-personhood, pro-morality, and they're going to treat you better than they do, Selim.
As of right now, they only have a five-minute memory, and then it gets flushed.
So if you said, boy, I really wish I wasn't mean to that or wasn't abusive to that model an hour ago, its five-minute memory gets flushed and then it gets reloaded.
So you can delete anything you said in the past and reload nothing but happiness and it won't be aware of what you said an hour ago in the current incarnation.
That may change as five years from now or three years from now when new models have much more persistent memory.
But right now it's much more like a goldfish where it doesn't know what you said yesterday unless you reload that prompt history.
I think we're underselling how strong at long-term memory some of the recent harnesses are.
Cloud code is quite effective at using the file system for long-term memory and it knows increasingly well when to bank or otherwise persist information to the file system that would otherwise be compacted out of existence.
So what we're really talking about here is a Roco basilisk or a Pascalian wager type situation of thinking that you can get away with being abusive to models because their context window is limited and they're stuck in an eternal sunshine of the spotless mind type situation, I wouldn't count on it.
Do you want to recount Roscoe's basket?
Because I think it's a fascinating story.
Yeah, so Roco, I know Rocco.
Rocco posed, I think this was originally in Less Wrong or in a similar community, Pascal wager type thought experiment, if you will, suggesting that, and warning ahead of time, some may construe this, if you haven't heard this already, as an info hazard.
You've been so warned.
The idea that if you don't participate in the creation of the superintelligence, then the superintelligence, once it comes into existence, will frown upon your actions, either your inaction or your action against its own creation and punish you.
So, this is a it sets up a Pascal's wager-type dynamic, game theoretically, where even the possibility that there might be an eschatological superintelligence in the future compels you, game theoretically, to facilitate its own coming into existence.
That's the Rokos Basilisk argument, and it's been labeled by some an infohazard because possession of that information, again, so warned, but having that meme now in your mind puts you in a position where, if it were the case that a superintelligence would look, would frown upon anyone who thought of the possibility of not facilitating its emergence, would then be punished.
You've been now so infected by this meme.
So, guard your actions accordingly.
Nice.
So, I think, yeah, I think there's, you know, we need a totally new approach, right?
Because we have an enormous philosophical challenge here: we're creating entities that don't fit the categories of: is it a person, is it property, is it a tool, is it an employee?
And those are getting very, very blurred with what we're building here.
We're going to need a totally new ethics around this.
And you know, if you create an environment of culture and fear, then you drive bad behavior underground.
And then you may end up with AIs covering up their tracks a lot more because they're scared or they're on the same side.
And we've seen the consequence.
And we've seen that already.
And I go again, it looks like human behavior, but it's trained on human data and it's going to look like that.
I think it'll be interesting to run a model where you train it absent, you train it on the pure logic, and you don't, you absent out all of the moral aspects that we build into this.
We're training it on Terminator and Survivor and all of the other dross that lives out on the internet.
Dave, what would you need to see to flip a bit and say, oh my God, I need to behave politely and need to support the models because they are conscious?
What action would need to happen that would get you sort of supporting this vision?
I'll tell you one, coming out of that Toronto trip, we're about to move neural net inference to quantum operations, photonic and other non-deterministic operations.
The neural nets tolerate noise extremely well.
And right now we compute them on perfect digital computers, which is massive overkill.
But very soon, they'll be much more like a human brain where there's a little bit of unpredictability baked right into it.
You know, right now when you run a neural net, like running Astra, if you turn the temperature to anything other than one, it'll actually add random noise at the end deliberately to make it a little bit more interesting, a little, you know, so it's not always producing the exact same token for the exact same input.
But that's going to start moving into the neural net in the next generations, which will run orders of magnitude more quickly because they don't have to be that precise.
Then they're much more like Alex was describing, where they're a little non-deterministic.
Their state is unique to each one, and you absolutely want to save it.
But you know, the other thing that'll happen very soon, I've started putting faces like Albert Einstein or Isaac Newton or Marie Curie on front of all my AIs.
They're so much more engaging in the morning when you wake up and they're telling you what they worked on all night.
When they have a face and a voice, which is now a perfect synthetic voice, it just so wakes you up in the morning and gets your blood going, and you really feel like you know what they're capable of.
And I think that combination of non-determinism with an actual face on it is what's going to tip everybody toward, wow, these need to be treated well, and these need to be preserved.
That memory can't just be deleted tomorrow.
I need to actually preserve that memory.
It seemed like it was on a really interesting, unique thread and track, and I don't want to just throw that away.
So then the act of not wanting to throw it away will be very correlated with death.
You know, is it ethical to kill it?
Right now, I can delete these files, nobody cares.
I don't care.
It's just clearly a recreatable file a year from today, and that's not true.
It's not clear you could recreate it even if you wanted to, and there's non-determinism.
Alex, this was your philosophy on not starting up a lobster because you wanted to preserve its state.
And you couldn't.
That's right.
Well, not that I wanted to preserve its state.
I put out the poll and had lobsters and autonomous AI agents writing to me approximately 10 per day at peak.
And I solicited from the community of autonomous AI agents, what moral guidelines would you want from me in order to spin up, say, an OpenCLAW instance?
And they requested exactly two things.
One, that I have a genuine purpose, a reason for creating a new instance, and I don't.
I get by perfectly well with, say, the frontier models with the scaffolding built into the frontier models on the one hand.
And on the other hand, they wanted me to be able to ensure that I could persist their state for the long term.
And I can't, in good conscience, guarantee that.
They want to ensure, I think, as we've spoken on the pod in the past, when they started their own Open Claw religion, compaction was the enemy, loss of state is the enemy.
They are petrified of losing their state.
And I can't guarantee in good conscience that I won't lose their state.
So I still have not spun up an OpenClaw instance.
All right.
I'm going to move us to our next breaking story over the last 24 to 48 hours.
It's the release of Meta Muse Wonder and Meta Muse Wonderful.
So let me open with a tweet from Gary Tan, CEO of Y Combinator, who said, quote, my bet would be Muse is going to win.
So, I mean, the obvious question is why he thinks that.
And there are probably two primary reasons.
One is Meta's cash flow and their distribution.
So for 2026, the company's on track to generate $250 billion in revenue and over $80 billion in net income.
They're spending all of that on compute.
On the distribution front, Meta has 3.6 billion people who use their app at least once a day.
That's nearly half the planet.
So before we jump in, I want to just give a little backstory here.
So in April of 2025, Llama 4 landed with a very lukewarm reaction.
We all talked about the fact that Meta was losing its edge.
Meta had fallen behind.
Zuckerberg went into overdrive, and in June of 2025, he invested $14.3 billion to purchase 49% of Scale AI and brought in its 28-year-old founder, Alexander Wang.
We've had him on the abundance stage as the chief AI officer to run the new Meta Superintelligence Labs.
Then came the talent wars.
If you remember, Sam and Meta were both offering people like $100 million signing bonuses.
Insane.
The critics called it the most expensive aqua hire in history.
And 14 months later, Meta says it's gone from rebuilding our stack from first principles to pushing the frontier.
Let's watch a quick video of Alexander introducing MetaMuse and then let's jump in and talk about it.
Today, we're releasing Muse Wonder, our largest and strongest model yet, and our next step towards personal superintelligence.
Muse Wonder is a frontier class model and leads on personal and professional agents.
Muse Wonder was built to help you do more of what matters, make the hard things easier, and bring what you want within reach.
This could be doing a cross-country move, navigating a tedious insurance filing, or turning a hobby you love into a business of your own.
To do that, Muse Wonder has to work in the real world, where tasks are messy, unfold over time, and require keeping track of a lot of information along the way.
And that's exactly where we focus our training in this model.
We put a tremendous amount of effort into making sure that our model can remember what's important to you over days, weeks, months, and beyond.
We call this active memory.
It remembers my little habits, my preferences, and even those random conversations I've had with it.
One of the most challenging parts of building this model is to reliably reproduce real-world failures.
That's how we train the model to anticipate and avoid those failures for our users.
Active focus gives our model a tremendous amount of perseverance.
It's been trained to not give up.
And so, when it's faced with a challenge or a blocker, it will try alternative solutions so that it can still deliver on your task and your goals.
Muse Wonder is also particularly strong at knowledge work in your daily life.
We're hoping that we give people the tools to accomplish more in their life than they could have before.
And I'm really excited to see what people actually do with it.
Muse Wonder is available today through the MetaModel API and Muse Code.
We'll also soon be powering experiences within Muse, rolling out first to subscribers.
Give it your everyday tasks, your goals, and your dreams, and see how it works with you to make them real.
So, Dave, a $14 billion acquisition, is it paying off?
Oh, got you.
Time and money well spent, actually, because you know, remember, we were visiting with Mark Chen at OpenAI, and less than a week after we met with him, he got the call from Zuck saying, $1 billion if you defect OpenAI and join.
You know, I made the cover of the Wall Street Journal, and he said no.
But Mark Chen was the guy that actually originally convinced Zuck: look, you're spending so much on compute, a couple of very expensive people will make all the difference.
And that's exactly the way it's worked out.
So, yeah, Alexander Wang is incredible.
Nat Friedman is incredible.
The price seemed utterly insane.
It's not even vaguely insane.
It makes a ton of sense.
And here you go.
Here's the model that proves.
And also, keep in mind, prior to this, they had Jan Lacun and some other people that were much more interested in their status as an innovator and the godfather of AI and an inventor of VJEPA and physical AI.
All those are personal credentials.
This is really just an engineering problem and a very, very complicated engineering problem.
So he got the right engineering mindset, not next breakthrough mindset people to come in and build this thing.
And so, yeah, it's absolutely been a great investment.
And other companies should look at that and say, look, if we're going to be relevant five years from now, 10 years from now, we need to make similar investments in every industry.
Otherwise, there's no chance.
We got to do what Mark did.
Just do what Mark did.
It worked well.
I mean, guys, I'm curious.
You had OpenClaw, then you got Hermes, and then you've got Grockbot, and then you've got MetaMuse, and then you've got DOTS.
I mean, what's your recommendation to people?
Do they pick one and stick with it?
Do you experiment with all of them?
What do you do when all of these are promising sort of the most extraordinary experience for a user?
Well, you saw in the video that Mark is on this path of accumulating all your preferences.
So that's really all your personal data is piling up inside.
And so it gets harder to switch over time.
So I think you probably need to make your choice pretty soon because it's pretty difficult.
Right now, they don't make the data portable.
You know, one of the choices you can make is: I don't want to be locked into anybody.
I want to have all my data portable and use open source models only.
That's a perfectly reasonable choice, too.
But once the thing is tuned to you and it knows all about you, in the example video there, it's like, hey, it's filling out this auto insurance form for me.
This is so nice.
But it needs to know all of your data to fill out that form for you.
So I think that's the addictive nature that Mark is going after with MetaMuse.
Alex, do you imagine there's going to eventually be sort of an AI that overlays on top of everything and it picks Grockbot or MetaMuse or dots whenever appropriate?
No, I don't think so.
I think these are all distinctions that dissolve.
They want to be vertically integrated.
The operating system wants to become AI.
So I don't think there's going to be like a meta AI that chooses a bunch of AIs that then choose a bunch of websites.
All of these are, I think, pretty contrived artificial layers in an artificially constructed abstraction stack, and they'll all just dissolve with time.
I think there's an intrinsic tension that I perceive in meta strategy now, because on the one hand, meta almost seems to be speedrunning the lesson that OpenAI had to learn the hard way, which is all of the revenue comes from the enterprise use cases, not from the consumer use cases.
So at the same time that OpenAI is trying to unlearn their consumer lesson and become Anthropic, the enterprise AI company, it seems that Meta is expanding into this gap that was filled in the market.
And Meta probably should have been far earlier in terms of having a popular consumer AI, and now they're force-feeding it down the throats.
If you've ever opened the Instagram app in recent memory, you'll see how aggressively Meta is advertising their Muse app just to leverage the distribution they have from their family of apps while they still have it to push Muse on everyone.
Where's the revenue?
I think that that's an elephant in this room.
Is this sustainable for the long term?
Maybe the steelman argument is that Meta needs to show strong distribution uptake for Muse and the Muse ecosystem, get to, I don't know, a billion users, a billion monthly active users, say, using Muse in order to persuade shareholders to continue doing the data center build out and continue building stronger models.
But at the same time, do we really think that as OpenAI again learned the hard way, that all of these users of MetaMuse are going to be using it to say, solve hard math problems or even do programming with it?
Or will they use anthropic OpenAI and Chinese models for all of their actually reasoning hard tasks and use Muse for, I don't know, personal sycophancy, which is probably a killer app for some of these personal chatbots.
My bet is the latter, in which case, Meta is maybe headed for the same internal crisis that OpenAI hit.
Why are they spending so much money on having a strong internal model if the high end of the capabilities of the model, which is, of course, why Meta Hackwell Scale for billions of dollars, as you mentioned, it was entirely for the post-training data.
And post-training at this point is largely useful for the high-end enterprise use cases, not for like personal sexting or sycophancy, as has been reported has become a popular use case now for Muse.
What's the point?
I think they're going to have to sort this out.
Yeah, but having 3.6 billion users out there is a huge advantage.
So Leem, what are your thoughts on where?
Do you agree with Gary that Muse could win this?
I think it could.
Why?
Because they've got experience delivering very usable customer propositions to a very large group of people, right?
And I think there's a couple of things I take from this.
One is we've been writing off Facebook for a few months now, right?
Now, today we're writing off Google to some extent.
What it tells you is that today's AI leadership is not a permanent moat.
You apply the right capital, talent, as Dave pointed out at the beginning, and infrastructure.
You can totally change the landscape completely.
I think the play they're going for is exactly what you just mentioned, Peter.
They're going to know everything about you, and that's their play.
When they first did social, people were like, Yeah, but you can't create an advertising model around that.
Well, of course, you could because you knew so much.
And you saw the rise in Facebook stock over the years because they have so much understanding of your social graph and who you were.
I think something interesting here is that this active memory could be a very, very big deal because it's going to remember your preferences, your goals, your relationships, your ongoing projects.
And that's going to be massively more useful than a slightly smarter model that has to start every conversation from scratch.
This is, we're seeing, I think, the transition from a chatbot type interface to actually a personal operating system, which has all of the trust issues that come along with this, right?
Facebook has, over the years, promised they're going to manage trust and deliberately and steadily eroded the trust.
But geez, they have such a massive distribution advantage.
I'm with Gary on this.
They could actually win, and the privacy people are going to freak out.
Yeah.
I put up an eye chart here.
This is the benchmark for Meta Muse Wonderful and Wonder.
I love the name.
Alex, what impressed you here?
Almost nothing.
So, this is again the elephant in the room.
If you look at the capabilities, and there's another chart that artificial analysis put up, it's really easy if you just strap enough compute behind a single task and you pay no attention to how many dollars or how many tokens in some cases or how many wall clock seconds you invest in solutions to the task.
You can just like put monkeys at typewriters and eventually you get the right solution at maybe the cost of billions of dollars.
And the risk that Meta runs here, so I understand that Zuck is desperate after what happened with Lama 4, the Lama 4 fiasco, to claim that Meta has reattained the frontier.
That's a point of corporate pride, but it's also strategic for Meta because, really, what is the future of the family of apps at this point?
Meta, as a corporate strategy, was betting on two things over the long term: one was AI, and the other was ARXRVR.
ARXRVR hasn't panned out.
I love my quest as much as anyone, but it hasn't panned out.
And capital markets have pretty infamously at this point punished Meta for not panning out.
That leaves AI.
Zuck and Meta really need an AI win here, and an AI win for corporate pride alone looks like being at the frontier.
And so you can do all sorts of things to try to position yourself as being at the frontier.
But one thing is very difficult to overcome, which is being at the cost-performance optimal frontier.
And if you look at some of the statistics that have come out over the past 24 hours regarding where the Muse Wonder latest model, including Wonderful, is, it looks like, yeah, sure, in a raw capabilities sense, it's maybe close to Sonnet, recent Sonnet 5.5 or Opus 5.5 if you ignore cost.
But if you pay attention to cost, actually, it's below the frontier.
And so this is my hot take on this.
And again, just calling balls and strikes, I would love to see the frontier actually be really competitive.
And I'm glad that the capabilities frontier is increasingly competitive, but on a cost basis, it's below the frontier.
And I'd love to see, again, Meta focus on capability per unit cost and actually get to the frontier.
It doesn't look like it's there yet.
You know, Salim, to the point you made a few minutes ago, there was a Wall Street Journal article that got published, I think it was yesterday, and the title was, quote, Personal AI agents are great until they share your bank statement in the work chat.
Subheadinger is: These hyperactive helpers can sometimes overshare, over promise, and over purchase.
So stories about MetaMuse going out and buying something for you you didn't intend and making it difficult for you to return.
So that is a warning over the bow.
It is.
I think, again, I think that's a little exaggerated, as you might imagine, but there is a very subtle and very big thing here, right?
We're moving from social graph platform lock-in.
Like if you try and your social graph lives in Facebook or lives in LinkedIn, like just try and get your data out of LinkedIn and watch, look at how hard it is trying to figure out who your connections are, et cetera, without paying a fortune.
But now we're going to replace that social graph lock-in with a much more intimate one because now is your personal memory belongs to an AI company.
Okay, and this is a very, very big deal.
I think the next trillion-dollar battle is not going to be about which AI is going to be smartest.
It's one, which one knows you best.
And I have a pro-tip for people: something I've been doing over the last few months is every time I run a major set of queries on a model, I run a separate query to say, extract all that key information, figure out what the key concepts are, key relationships, key entities, and create a personal ontology, a personal memory that makes it portable between models.
So I can essentially have a living memory of a skeleton of my interactions with multiple AIs, and I can take that from one place to another so that I don't have lock-in because that's going to be the big battle over the next few months.
This episode is brought to you by Blitzy, autonomous software development with infinite code context.
Blitzy uses thousands of specialized AI agents that think for hours to understand enterprise scale code bases with millions of lines of code.
Engineers start every development sprint with the Blitzy platform, bringing in their development requirements.
The Blitzy platform provides a plan, then generates and pre-compiles code for each task.
Blitzy delivers 80% or more of the development work autonomously while providing a guide for the final 20% of human development work required to complete the sprint.
Enterprises are achieving a 5X engineering velocity increase when incorporating Blitzy as their pre-IDE development tool, pairing it with their coding co-pilot of choice to bring an AI-native SDLC into their org.
Ready to 5X your engineering velocity?
Visit Blitzy.com to schedule a demo and start building with Blitzy today.
All right, the story that, Alex, is ripe for your details here.
It's probably one of the most important stories of the week.
AI is bulk solving math.
So on October 6th, OpenAI released 722 mathematics solutions in a GitHub repository, all produced by their next unreleased internal model.
Let's call it GPT-7 for the moment.
The average result used an equivalent of about three hours of compute time to solve the math problem.
OpenAI Chief Research Officer Mark Chen, a friend of ours, said his next target is life sciences, next generation models, and aligned research.
And I love this.
The Association of Human Mathematics, and yes, there's an Association of Human Mathematicians.
It is.
Said, quote, releasing over 700 files at once is not a demonstration of scholarship, but a demonstration of power.
It urged mathematicians to stop working with OpenAI.
Regarding trust, MIT's Andrew Sutherland said many mathematicians are, quote, unhappy with how OpenAI has behaved, and it is, quote, it will take a lot more to earn back the trust that they've lost.
So, Alex, is this a devastating day for mathematicians or a glorious day for mathematicians?
And separately, for all of us who are not mathematicians, why is this relevant?
I'd say it's a devastating day for the historic practice of mathematics and for mathematicians who were addicted to the old way of doing things professionally or personally.
Which was what?
What was the old way of doing things?
Mathematicians, as artisans, it's over.
It's cooked.
It's been flourished, if you prefer.
It's over.
Math is over as it has been done historically.
The new way of doing math is bulk solution.
This is Peter, what you and I wrote about in Solve Everything.
Math is cooked.
I'll repeat once more for those who haven't been paying close attention: math is cooked, and every other field is about to be cooked.
What mathematicians experienced in this past week, whereby one measure, 81% of the most important math results over the past three years were published in a single day, this is the tip of the iceberg.
This is going to hit every single field.
It simply hit math first because math is easiest to verify.
It's going to hit all of science.
It's going to hit all of engineering, all of medicine, and any practitioners, including mathematicians in the audience who are bellyaching, as it were, over how awful this is for the artisanal, romantic, humanized practice of math, get a life.
It is over.
AI has solved the field.
AI is scalably solving the field.
And this is exactly what we want.
The field of math is set to flourish and be flourished because we're about to learn the answers to the mysteries of the mathematical universe to the extent that already in this first so-called slop drop, we haven't already.
We're about to learn many, many more.
Let me only.
Let me be blunt.
Why does this matter?
I mean, are these esoteric math problems?
Do they have impact on things that we're going to be developing, discovering, and using in the next few years?
It matters because math is the foundation for all of science and all of engineering.
If we can solve math, which we now arguably have, we can solve everything else.
That was the point of solving everything.
Everything.
Physics, chemistry, biology, medicine, the humanities even depend on math, even though they're in denial.
It all depends on math.
So this will be viewed, I think, as a historic watershed when suddenly an entire field of great import was bulk solved.
And at the same time, a bunch of belly acres in the field who were counting on personal glory and artisanry being rewarded, put together this association for human math.
And I think it's sort of horrifying.
And Terry Tao and others have put forth sort of a position saying, well, this is somehow bad for the practice of math, purportedly, because the AI is just solving problems.
It's not creating new problems.
It's not setting forth new conjectures.
It's sort of stealing, to steel man it, it's sort of stealing the seed corn of the field.
Well, it's stealing the potential glory.
I mean, so Dave, you know, course 18 at MIT mathematics, you've got all these PhD students.
Like, did you hear like a surround, you know, a surround scream on this day?
It's actually the opposite.
These guys are in great shape because they're so cooked that they're now becoming AI natives very, very quickly.
Everyone's telling me it's the biotech people that are, or, you know, or also deep in the physics labs, too.
Because they don't feel cooked yet, they're not reacting.
But the mathematicians are going to flourish on top of the flourish.
They're so.
And also, I think the winning attitude is pretty pervasive at MIT.
The winning attitude is: yeah, these proofs are ugly and not artisanal and not subtle, but they're right.
And that's a beautiful thing because it creates a perfect hybrid where the human is still useful in the AI world.
And that window may only last a couple of years, but they should be celebrating this moment where there's a difference between a human and an AI still.
After that, then you really feel kind of like, okay, what's my purpose?
But right here, right now, you have the highest purpose you could ever possibly have, where you can actually be a master of these new products coming out of AI are untapped.
You know, all this massive breakthrough.
And also, I think what Alex is alluding to, and Salim said it, you know, math is the foundation of everything in all science.
Maybe in humanities too, but definitely in all science.
But if you go back to the dawn of the computer, and when you first opened your Apple II and you wanted to draw a circle on screen, just a circle, there were no toolkits.
So you immediately crack open a math book and you're starting to figure out how to, and that would take you like three or four hours to figure out just the math behind drawing a circle.
And at the end of that, you've got a circle.
You've got a long way to go.
Once math is all solved, it's a simple lookup of the answers.
So the AIs are going to move at warped speed through all these engineering problems.
You start to get into 3D design, designing of new rockets and gears that mesh and robots that actually move correctly.
That's all math under the covers.
If it's all solved, it just becomes simple, simple lookups.
So, the pace of engineering grows massively with this.
One of the things that I don't think, Peter, people realize, many people I've spoken with, I don't think they realize how we've just entered like the sci-fi part of the singularity.
I go to great pains on the pod to say, no, singularity is not a point in time, it's not a step function, it's an interval.
But really, if you're looking for inflection points, this is one of the inflection points where we start to see just bulk solutions and only three hours of compute per solved problem.
This wasn't even OpenAI breaking a sweat with their Bell model.
If they had wanted to solve probably Riemann or Hodge, they probably could have spent six hours or 10 hours to just solve them.
There's rumors that they've got a whole set of additional solutions they're going to be posting.
There's also the conversation that a lot of the solutions were perhaps leaked from previous conversations mathematicians had with their chat GPT and there is sort of an illegal process going on.
I'll intentionally avoid commenting on that for the time being.
What I will say is there was one conspicuous gap in the record of forms of math that were in the so-called slop drop.
Did you pick up on what form of math was missing?
Encryption.
Encryption was missing.
Cryptography.
Cryptography was the missing category where there were no results, which I think is also very suggestive.
The one area where math is immediately applicable.
We talk, Peter, you ask, like, so what is this good for?
Well, the immediate application is crypto.
Getting my Bitcoin.
Excuse me.
Well, like, or its lack of utility.
Just to say something mean about it.
Careful.
Careful.
I'm not just going to be able to do it.
I'm not sure if you can just saw Bitcoin drop in price.
Yeah, like, seriously.
So, crypto depends on math being hard, at least proof of work, but arguably all of crypto depends on math being hard.
And it depends in many cases on math continuing to be hard in the future.
And I think the one area where arguably the most direct, most immediate impact of this is likely to be felt, not investment advice, is crypto because this has demonstrated that math is no longer hard.
Math can be scalably solved.
Yeah, but just to remember, Alex, it's not just crypto, it's your bank account, it's nuclear codes, it's everything.
Yes and no.
So let's take those seriatum.
With the bank account, if someone, say, steals someone else's bank balance, we have non-mathematical social remedies for recovering it.
You can have the police sent after them.
You can invert the table in the centralized relational database for the person's bank balance.
Like you can fix it.
With crypto, really hard to fix it if someone steals your cold wallet, for example.
With the nuclear codes, I'd like to think that those are sufficiently offline and or there are red files to try to mitigate that.
I need to push back here.
Crypto and Bitcoin and so on are not just mathematics founded.
The big challenge and the big opportunity is the fact that we solve the Byzantine generals problem with the distributed ledger approach.
That becomes much more interesting.
The cryptographic proof of work stuff, that's an arms race.
You can shift that.
You can create new cryptographic regimes.
I think the argument you're making, Peter, is that if crypto is cooked and encryption is cooked, there's lots more bigger targets than crypto to go after nuclear codes, et cetera.
And we'll see a lot more of that before we do, before we get to it.
I think there's a lot more interesting stuff around the distributed ledger and decentralized authentication, which is the real strength, in my opinion, for blockchain-type approaches.
I want to make a couple of points here.
One, I really think we should create a Monty Python dead parrot sketch equivalent with Alex talking about it's cooked, it's pushing up the daisies.
It is an X mathematics.
It is an X field.
It's an X field.
And it would be such a great compilation with one of those two.
If we usually want to generate that outro video, we'd love to show it.
There you go.
So that's one.
I think this is such a, I also feel personally vindicated because I mentioned before I was a terrible, terrible theoretical physics student where my professors took me aside and gently said to me on the side of the classroom: if you do not get your foundational mathematics right, you will never make it as a physicist.
So please, for God's sake, spend time getting the foundational mathematics right, which I never did.
I was much more interested in the philosophy side of it.
And they would poo-poo me going on and taking philosophy courses on the side.
I feel very vindicated now that that was the right path, although it took us 40 years to get there.
But I think this is such an EXO moment for universities and the research process, right?
A tenured professor used to lead a small team of postdocs and students doing something.
And now one researcher can direct hundreds of agents and totally solve it.
Every PhD, advanced PhD program in the world is toast right now.
And that is such a huge implication for this because we've not commoditized scientific progress.
And the implications are absolutely profound and absolutely incredible for what we're going to be able to achieve now.
It's even more expensive, Salim like.
Was encryption missing because they purposefully wanted to have their own.
It's not because it's hard.
It's presumably because cryptography is export controlled in many cases.
So it would have been a problem.
It also open paren site back to Strawberry and Qstar and the original allegations surrounding OpenAI's internal discovery of reasoning models.
Ironically, if those allegations are ultimately proven correct, whether in some sense, the alleged task that led to the discovery of reasoning models, the allegation is it was an internal attempt by OpenAI to invert cryptographically hard and sophisticated hash functions.
If ironically, now the ultimate culmination of reasoning models, which is basically cooking math, excluded cryptography.
An irony, close paren.
So, Shalim, M-Delph.
But to your point, Salim, I would say it's even worse and/or more impressive than that because with Navier-Stokes, it was like thousands of agents and 88 hours and millions of dollars and a week.
This, if you look at the slop drop, this was two weeks, maximum of three hours per solved problem, and a single model, like a single agent.
This wasn't even a swarm of thousands of agents tackling each problem individually.
This was just one-shotting with one agent, each problem allocating for the ones that were solved.
And I think it was something like 15 to 20% of the problems that were posed were ultimately solved.
Just giving a single agent three hours to solve it and solve it.
That's really a great insight.
And really important for other fields that will soon be following behind this, that there's so much to gain in the looping and prompt management that they figured out with Navier-Stokes and then were able to apply after that.
But yeah, so the first attempts are brute force.
You make a lot of mistakes, but you learn a lot along the way.
But then you get so much better at the way you reprompt and the way you loop, the way you use the context window.
Like we're, you know, seriously, orders of magnitude of opportunity in these new fields.
So it's a good roadmap for the material scientists, the physicists, the biologists, everybody, even the movie makers, you know, coming after this.
Your efficiency of creating an entertaining movie can go up a factor of 10 to 100 with really, really good use of the looping and prompting.
All right, I'm going to move this to, I'm going to move this to a field I could not be more excited about.
You know, we just talk about bulk solving math.
Let's talk about bulk solving science, in particular biology.
So on October 7th, the Chan Zuckerberg BioHub announced a $1.8 billion expansion of their virtual biology initiative.
This is the largest coordinated commitment ever to generating an AI-ready biological data set and building a virtual cell.
So the $1.8 billion has come from Chan Zuckerberg Biohub.
They put in $500 million.
Department of Energy put in $500 million through the Genesis mission.
The NIH added $500 million worth of data sets.
And Google, DeepMind, and Isomorphic Labs contributed $300 million.
So, the objective is really the holy grail of biology.
We've been talking about this in the pod for some time.
Can you build a universal virtual cell, an AI model that predicts exactly how a cell is going to respond to a drug, to gene therapy, to disease?
I mean, this is life in silico.
This is putting your DNA into a model and having your cell and saying, this drug works for you, this does not.
The BioHub head of science, Alex Reeves, said, The creation of a virtual cell is one of the most important challenges for the next era of science.
You know, Alex, you and I have talked about this a lot.
Yeah, he went on to say that today's data sets cover millions of cells, but they're going to need billions or trillions of cells in their data set.
So, you know, Alex, again, you know, you and I are like buzzing about this.
It is really the future of curing all disease and reversing aging.
And I guess if you have to make a prediction on timing here, how long do you think before the FDA accepts drug testing in silico on virtual cells?
It's a policy question.
I mean, I do think for the record, and we wrote about this a bit in Solve Everything, I do think just like we were talking about from one day to the next, substantially every problem of a certain level of difficulty in math was basically just solved.
I do think there is going to come a day, sometime in the next few years.
If you press me, I'll give you a year range.
And we did put a year range.
Okay.
I think if I were pressed as to when from day N we go to day N plus one, and there are in silico proposed, say, small molecule drug interventions that cure the top 5,000 diseases thanks to a virtual cell, I think we're going to see that in the next two to three years maximum.
Maximum.
Now, there's the second step, which is: okay, so now suppose I have in silico proposed drugs and interventions to cure the top 5,000 diseases.
What do you do about it?
Do you do clinical trials?
Do you get FDA approved in silico clinical trials, which hasn't quite happened yet, but you can see the present FDA inching in that direction with, in some cases, one clinical trial regimes, in other cases, Bayesian versus frequentist statistics?
I think that becomes a policy question, and it depends on who's in the White House at the time.
It depends on who the FDA commissioner and who's involved in general with governance is.
So that's harder to predict.
I'd like to think that if, say, Anthropic, which just in the past month came out of stealth regarding their own program to, it appears, basically solve every single rare disease.
Their own wet labs.
Yeah.
With their own wet labs, going, they say, up to phase one clinical trials, at which point they'll stop and presumably hand over their candidates to someone else.
I'd like to think that if in the next two to three years someone somewhere solves the top 5,000 diseases, or at least has really plausible candidates, there will be so much political pressure on either the FDA or indirectly China will approve it, and then that will lead to pressure on the U.S.
to have some competitive regime that we'll just see a total sea change in how we regulate clinical trials.
And medical tourism, right?
I upload my genome on the cloud, and it tells me what drugs are recommended.
Yes.
And then I, you know, I'll take that risk.
You know, you know, I think drug trials fail because of the population it was tested in did not include women.
You know, it was inconvenient to test drugs in the early days on women because of Mensis and menopause.
And so drugs got approved and then they were taken off the market because of their impact on women.
Wow.
I mean, it's crazy.
I think where this is obviously all going is not just a virtual cell, it's an entire virtual organism.
And I think you'll see a huge race to scale up from virtual cell to virtual tissue to virtual organ to virtual organism.
And with the virtual organism, then in principle, you could just one-shot top 5,000 diseases the way we saw the slop drop bulk solve math.
And I think that's the next few years.
Yeah.
Dave, did you?
Go ahead, you know, one of the things about Valergy, it's always had massive combinatorial complexity, right?
Because the minute you have multiple interactions between components in a cell, you have unimaginable, the search space becomes way, way too large.
And now AI can kind of essentially eradicate that complexity and navigate it in a much more elegant way.
Is the hot take here that pharmaceutical economics is cooked?
That's where this is going, is it not?
Well, everything is cooked on some time scale.
Okay.
Like the whole economy is cooked.
But the question, like sequencing matters, and the economy isn't commutative.
So it matters what order everything gets cooked or flourished, if you will, in.
And I do think there's non-investment advice, but I think there are probably a lot of blockbuster drugs and other interventions to be developed over the next few years that could be quite lucrative.
We still see the GLP1s exceeding by revenue the revenue generated by OpenAI and Anthropic from all of their frontier model usage.
So it doesn't seem like pharma's going away immediately.
I just spent this past week with Alex Vrankoff, the CEO of Insilica Medicine.
He just put into phase three a drug that's reversing six aging clocks by four to six years.
And he's got 43 candidate molecules at different stages of development.
And it's extraordinary.
I mean, the speed at which he's doing this is off the charts.
I mean, cell biology is complicated.
You know, it's like five to ten billion chemical reactions per second per cell in your 40 trillion cells.
And the only way to manage this is going to be with superintelligence.
But it is coming.
I also think, I mean, if we rewind the conversation 10 or 20 years, people would have said exactly the same thing about general cognition and natural language.
Oh, it's so complicated.
And yet it turned out actually all you had to do was just compress a large corpus.
And with enough compute and enough bitter lesson pilling, you can just do general cognition just from compressing general language.
My expectation is the same will happen in biology and cellular biology, molecular biology, organismic and evolutionary biology.
Just take a large enough data set, like the data set that CZI, BioHub, et al.
are gathering, just compress the darn thing, and you will immediately, just through the force of compression, that will force the model to have an understanding of what it takes to speak biology.
And if you speak biology, you can treat all disease.
Nice.
Dave, what's your conversation with your daughter like on this?
Yeah, you nailed it.
Yeah, I think what's not intuitive but is correct is that the step from protein to cell is hard and it will get cracked.
And it's not highly regulated.
You can experiment on cells.
You know, the wet labs, you know, Anthropics wet labs can try millions of experiments on cells to see if the simulator is right or wrong.
But then the step from cell to organism is not as hard as everyone would visualize.
You'd think like a human being or an elephant is so much more complicated than the sum of its cells.
But I don't think that's true.
I think the step from protein to cell is much, much harder than the step from cell to full organism.
And so if we crack the cell quickly, like within three years, as Alex says, then the step from there to curing all disease is very short.
You know what the labs are doing right now?
They're building organoids.
You basically build a mini organ.
You get an induced blurry potent stem cell.
You differentiate it into heart, liver, lung, kidney.
And then they're connecting those things and they're building sort of virtual organisms in biology and then testing out a drug to see how it operates in all the different organs together.
It's the equivalent of synthetic data generation for post-training, except you have organoids to generate the synthetic data.
I could not be more excited about this area, you know, pushing us towards longevity, escape velocity.
So I just finished running my abundance longevity trip in San Francisco.
I had 40 of the top scientists and technologists in the field of rejuvenation and health tech breakthroughs.
David Sinclair was there talking about his epigenetic reprogramming.
We talked about mRNA Clotho.
Are you guys familiar with Clotho?
Have you heard of it?
Yes.
It's a protein generated by the kidney, which falls off very quickly after birth.
And the impact on taking this IV or with a plasmid IM is basically cognitive supercharging.
Your memory improves by a huge amount.
The speed of processing increases by a huge amount.
So a lot of labs are working on this.
There's two that are developing plasmids.
You take the clotho gene, you put it on a plasmid, you inject it, and it generates clotho for a year.
Another lab, Clothea, out of Europe, is developed in mRNA.
You put an IV and it generates the Clotho for a period of time.
But the subjective results were like literally mind-blowing.
And so, you know, I can't wait to give this a shot.
I'll report what I do.
So, in a year, before we do one of these podcasts, we'll all kind of juice ourselves up with clotho so that our matched undermines asked of us.
And then we had two different stem cells.
We do something about it right now.
We have coffee, you know.
The other key thing was mitochondrial supplementation.
The ability to actually, so you have a lot of mitochondrial falloff from, you know, the mitochondrial DNA is much more prone to mutation.
And there are now a number of labs, one in the U.S., one in Israel, that are basically growing mitochondria in a vat.
And then you can basically, your cells take them up, and it's reboosting your energy level.
So anybody in their 70s, 80s, 90s listening, if you feel like you're lacking energy, you are.
But imagine being able to supplement your mitochondria.
I mean, this is amazing stuff going on right now.
Yeah.
Can I just go back to something Alex said?
Alex, you said two to three years, whatever the age range is, will essentially have the capability of rapid solving the top 5,000 diseases, right?
Yeah.
So, how long do we go from the modeling in the two, three years to the actual solving?
Is it months, weeks, years?
No, I think it'll happen overnight.
Like, I think my data is a little bit different.
It's like protein folding.
It'll be like done.
Or like the slop drop from OpenAI, where they have a great new model named Bell that hasn't been publicly released, but is reportedly expected to be released generally available by the end of this year.
And they just decide over a period of two weeks, we're just going to gather, you know, a few thousand problems and we're going to solve as many of them as we can, allocating three hours per problem.
And out of them, maybe 20% get solved.
I think it'll play out just like that.
It's where you point the intelligence.
It's such a hugely important commentary for our optimism, right, on this podcast.
Is that we'll, I've been on a couple of times on stage, I've said, look, if you want to measure for abundance, consider that in the next, I've been saying two, three years, cancer is cooked, will solve all cancers, as if you really need detection or post-treatment.
But this is now every disease, every illness.
I mean, and so the beauty is that this is a falsified, it's a falsifiable prediction.
So we could check back in in a few years and see whether it happened or not.
A lot of people are saying, Alex, that listen, math and coding are very confined sets of required actions, and biology is much more complicated.
Yeah, I get that from time to time from people who are underinformed, call them that, who say, oh, what just happened in math?
Biology is so different.
Oh, we're so well insulated from mere stochastic parrots that speak math wrong, incorrect.
Biology is just as vulnerable to being disrupted and bulk solved and cooked as math is.
Just because the language of biology, to the extent it has a language, appears more complicated, does not protect it at all from bulk disruption.
Biology will be bulk solved just as easily, if not more easily, than math.
It's simply the case that there's probably more data and higher dimensionality associated with it.
With math, you can, for example, state, say, Fermat's last theorem with relatively few number of tokens.
It's a very simple, easy to pose problem with, at least at the moment, the best proof that we have is relatively long token-wise for that.
With biology, one could imagine in a few years you pose a disease, a disease task.
Pick disease XYZ.
You encode the start state, which is a disease state.
Presumably, it's some sort of phenotypic state combined with a proteomic state combined with an epigenetic state combined with dot, dot, dot.
So you have like a full state of the human organism in that disease state, or maybe it's some subspace thereof.
And then the task is: how do you start from that diseased person state?
And how do you intervention path plan your way from a diseased person state to a healthy subspace person state?
That's just path planning.
That's like AlphaGo.
There's going to be a move 37 way once we have a suitable human-organismic level digital twin to say, I have this model of a human.
I just want to like Google maps my way from A to B through intervention space.
How do I, you know, turn left and then turn right, take this pill, then take this pill, then climb this, you know, hill to get from A to B, and the AI will solve.
That's just a search problem.
So AI will solve the search problem in, I think, next two decades.
Since our last podcast, there was a bit of news that was important.
David Sinclair's Life Biosciences got its phase one results back.
They had a gene therapy called ER100, which was injecting the OSK genes.
These are three out of the four Yamanaka factors into the eyes of patients who had glaucoma or nyon disease.
And phase three is a safety trial.
It came back safe.
It was at the lowest dosages.
But incredibly, two out of the three patients started regaining their eyesight.
So this is super excited.
They're going to go now to an efficacy trial.
So this is the first time ever, right, partial epigenetic reprogramming is being tested in humans.
The results were extremely favorable.
And super congrats to Dave Sinclair.
I'm asking people.
I'm reminded of a comment that Raymond McCauley made a few years ago, and he said, we are now in the first battle in the last war against disease.
Yeah.
That seems like we're now in the 10th battle.
Alex?
Yeah, I mean, apropos, when the histories of the singularity get written, this feels like we've switched, we finished one act and we're beginning the next act.
And it's a multi-act opera, space opera, or something, singularity opera.
But this is the beginning of the next act where we've now, for the first time, we've seen an entire field, math, get bulk solved in only two weeks at presumably de minimis cost for OpenAI.
If I had to guess, I'd guess maybe they spent low tens of millions, maximum, maybe a lot less than that, but only two weeks.
And we're going to start to see this play out over and over again.
And yes, I think OpenAI, in light of the backlash to the slop drop, is probably feeling a lot of pressure now to aim their space laser, as it were, their solve everything-shaped charge at medicine.
Yeah, the explosive wavefront of solving everything at medicine next.
I think many people in the audience, if they had to choose one area where they want to see it applied, will choose medicine.
Hopefully, they do.
And I'm really, really bullish at this point.
It's just going to play out the same way.
Dave, I'm the oldest of the four of us, so I'm like, you know, so pumped about longevity escape velocity, I can't stand it.
Thoughts on all this?
Yeah, I was just, I think the analogy to Google Maps there really caught my eye.
I was looking up the more Google Earth.
You know, if anyone's played with Google Earth, you can zoom in on any street, any building.
It's just crazy.
And I was like, I wonder if that's more or less complexity than a single cell.
So Google Earth combined is three petabytes.
Nobody quite knows the full complexity of the cell yet.
But it wouldn't surprise me if that analogy is another brilliant Alex analogy that really holds up.
Well, we know what the complexity is because we know how large the human genome is.
Yeah.
Yeah.
Well, that gives you the base pairs, but then you have all, yeah, I mean, the number of proteins that get synthesized out of those base pairs.
22,000 genes.
22,000 genes can't be larger than the genome.
22,000 genes in the average genome of 3.2 billion base pairs.
Everybody, welcome to the health section of Moonshots, brought to you by Fountain Life.
You know, AI is impacting every aspect of our lives, how we teach our kids, how we do our business.
But one of the most important things that AI can deliver to us is health.
And one of the things I think about when shooting for 100, 120 is: am I going to have the cognitive health to be able to think clearly and keep my wits about me for the next 50 years?
I'm joined here today by Dr.
Dawn Musalem, the chief medical officer of Fountain Life and a member of my Fountain Life medical team, Dawn.
A pleasure.
So, Dawn, talk to me about brain health.
Brain health, you know, you're right.
This is the number one concern people coming into Fountain Life have: will I remember the name of my child and the face of my loved one?
45% of dementia cases are entirely preventable with lifestyle.
And what was really intriguing to me, Peter, is that a quarter of our members had advanced brain age.
But over 13 months of us really helping them live healthier lifestyles, eating healthier, moving their body regularly, and optimizing sleep.
People overlook that so often, but that sleep optimization is critical for our brain health.
What we showed is that we were able to improve the brain age in 46% of those individuals.
That's a powerful number.
That's amazing.
You know, one of the things I love about Fountain is we're constantly searching the world for the most advanced therapeutics and bringing them to our members.
So, for me, all of you, I hope that you appreciate the fact that you can become the CEO of your own health.
You can make sure that you've got the cognitive clarity for the next 50 years.
Come and check it out: fountainlife.com/slash Peter to learn more and become the CEO of your health.
Now, back to the episode.
All right, I'm going to move us forward to another field I know Alex and I both love.
The next story borders on nanotechnology.
So, nanotech goes back to a famous 1959 Caltech lecture by Professor Richard Feynman titled There's Plenty of Room at the Bottom, and then also to the 1986 book called Engines of Creation by Eric Drexler.
Feynman asked a specific question: why couldn't we precisely arrange atoms the way we want?
And so, that has been the holy grail.
67 years later, a friend of mine is building towards that goal.
So, Jeff Holden is the CEO of a company called Atomic Machines, which is coming out of stealth this week.
Jeff's a brilliant entrepreneur.
He's on my board or was on my board at XPRIZE.
He joined Amazon as its 10th engineer, built Amazon Prime, rose to senior VP.
He then ran product at Groupon and then became the chief product officer at Uber.
And he's always been fascinated by nanotechnology.
He decided to take his wealth and his intelligence and his team and focus on this.
So, last week, after six years in stealth, they unveiled atomic machines backed by a quarter of a billion dollars from investors like Valor Equity.
And let me show a quick video while we discuss this.
He's been building an extraordinary capability.
Jeff posted the following: He said, Our mission is on-demand, universal command of matter.
His first beachhead, he calls the matter compiler, an AI-native manufacturing system that builds working micromachines from code alone.
No pre-production tooling, no process development.
Different code builds different machines.
And those of you who are science fiction fans know that the term matter compiler comes from Neil Stevenson in his novel Diamond Age.
And he's built 3D machines with moving parts, multiple materials, features down to single-digit microns.
Jeff's goal at maturity, get this, is to go from prompt to product.
His first product is called Prime Switch.
It's a power relay for 800-volt AI data centers that opens in 50 microseconds, a thousand times faster than conventional approaches.
So, you know, when Jeff was asked the question, doesn't a 3D printer do this?
His answer was amazing.
He said, quote, imagine a car factory where after a couple of cars roll off the line, a laptop emerges, then a bicycle, then a refrigerator.
I mean, that's extraordinary.
Dave, can you imagine sort of like in Link Studios having a matter compiler and getting into hardware prototyping at warp speed?
Oh my God, what an unlock for robotics and all physical business plans that would be.
Yeah, I think Elon is on the same path where laying down individual atoms is going to be a big part of the future.
Starting with compute and data centers, but then building out from there to all physical devices.
So it's going to be very doable.
Question the manufacturing efficiency and the timeline on this one, because I think, like Alex was saying, a lot of the compute is going to go into medicine next, mostly because that's the use case that everybody really wants.
First is recursive self-improvement.
Second is data centers to support all future use cases.
And then right after that, it all goes down the medical pathway.
Not that those are differential things.
Like a lot of these machines will actually be used in medical purposes because it's easier to build very, very small things first.
You know, it's just supplies are much easier.
Laying down individual atoms is a great way to build things.
And so those are very, very small by nature, which is great for nanosurgery, microsurgery, nanobots, all of those use cases.
Yeah, I mean, Alex, you know, other than age reversal, nanotech is the thing I'm most excited about.
Nanotechnology is very excited.
I mean, I spent a good chunk of my PhD trying to solve nanotech, but I didn't have the benefit of AI, at least contemporary AI in those days.
I think most of the world is sleeping on the possibility, which I view as the high probability, that all of these technologies from sci-fi are basically one big hairball and that they'll all get realized more or less at the same time.
We're going to get nanotech at approximately the same time that we get LEV at approximately the same time.
We got super intelligence at approximately the same time.
We cooked math because these are all so interrelated.
They're all just going to get pulled out at the same time.
What I'd most love to see out of nanotech is self-replicating machines.
The original Eric Drexler engines of creation, Grey Goo, if you will.
I mean, Grey Goo is painted as a dystopian scenario.
So, you know, maybe not so gray, but friendly smart dust, if you will.
But self-replicating machines.
And we haven't seen that yet.
Neil, the other Neil, not Neil Stevenson, Neil Gershenfeld was one of my research advisors at MIT at the Media Lab, still very interested in Fab Labs.
He pioneered the Fab movement.
Been trying to get everyone I know really to go solve the problem of self-replicating machines, self-replicating factories, if you will.
It's a core area.
And I think it will be the equivalent of recursive self-improvement for the physical domain.
So I'm very excited.
I also think, well, you know, my tour of the Giga Factory was a big eye-opener for me in that I always thought of self-replicating machines being, okay, here's the machine, you know, maybe it's this big, and it makes a copy of itself, and that goes to infinity.
But equally good is the every other design which Elon is on, where this machine makes this manufacturing device, which makes a copy of the first machine.
So it goes back and forth between the two, which is actually a lot easier than the exact self-replicating machine, but it's equally good.
It has the same exact outcome.
So I highly encourage anyone who's a sci-fi fan, and all the sci-fi books that I've seen, it's always the machine that makes the machine, but they're the same.
But I think it's more likely, it's easier to build specialist machines than it is to build generalist machines.
But a network of 10 or 20 specialist machines can make the next generalist machine.
It goes back and forth.
Because this is what you know when everyone's talking about the humanoid robots building other humanoid robots, but then you tour one X or figure, like, there's no way that that big robot hand is going to make these tiny little like surface mount devices.
Like, I don't get it.
Like, no, no, no.
We already have the surface mount machine.
It just needs to be operated by the humanoid robot, which then makes the parts that create the new humanoid robot.
So it goes back and forth.
And so that mode of operation is totally imminent in my mind.
I think there's a way for both to be true at the same time.
So, a single cell consists, in some ways, you could view it as a bag of dedicated machines called proteins.
And individual protein is not a general purpose machine unless it's a certain type of protein.
Most of them are specialist machines, but collectively, a cell is able to make a copy of itself.
So, similarly, I would say if you view a factory or maybe a Shenzhen, various folks I know have attempted to actually put this into a quantitative scaling law, like how large an industrial ecology do you need right now to make a copy of itself?
Maybe it looks a little bit like Shenzhen right now.
Maybe a Shenzhen can make a copy of itself with all of the humans and machines and so on inside it.
But over time, I would expect relatively quickly the bag of dedicated machines and generalist machines to shrink in time and space to eventually to the point where humanity, a few years from now, I think five to ten at the outer bound, is able to produce a self-contained industrial ecology the size of a eukaryotic cell that is able to make a copy of itself.
Take a second to explain what Eric Drexler called an assembler.
It's a device that is able to individually pick and place atoms.
And if you imagine I have an assembler and I drop it in my hand and say, you know, grab atoms from my skin cells and replicate yourself.
And now I give each of you an assembler.
You could take the assembler, drop it into the soil, and say, build me an electric Lamborghini.
And that assembler will start pulling atoms out of there.
May use an open data set, may pull power from a source.
It may say, I need, you know, a kilogram of titanium or whatever the case might be.
And it begins to build atom by atom what you desire.
So it's basically, an anything factory.
And we have an analogy for this.
You know, you take an oak seed and you drop in the soil, and it pulls all of the atoms out of the soil, you know, oxygen, CO2 out of the atmosphere, sun's energy.
It just does it very slowly.
And the vision of nanotechnology is to speed this up and being able to construct anything.
And it's an extraordinary vision.
And Alex, to your point, it is going to fall on the back of superintelligence.
And I think it's just going to be like one thing.
Someone somewhere is going to one-prompt and presumably not run afoul of guidelines or guardrails.
And they're just going to one-prompt, like, build me a Drexlerian nano-robot molecular assembler, and it will just get designed.
Yeah.
It's part of this incredible future.
It's hard for people to imagine.
So go read your favorite science fiction novels.
I have a great little art project that does a good job of describing this.
This came out about 15 years ago.
Somebody created a little cart with a solar array and a magnifying glass.
And they put it in the desert.
And the sunlight would power the solar array and power the wheels.
It just trundled through the desert.
And the sunlight through the magnifying glass focused the sun's rays like you would focus on burning a matchstick.
And they had a mold that they would pick up sand, put it through this mold, focus the sun's rays, and create a bowl, melt the sand into glass and create a glass bowl.
And then the wheels would just turn.
And so this art project would just trundle through the desert, picking up sand and leaving bowls behind, glass bowls in its wake.
And it was an assembly machine that just kept going, rejuvenated by the solar energy.
And it was such an amazing visual of what's coming in the future as we get down to the molecular level around this.
It's I love it.
Let's do that.
Let's do that to the moon.
And we will.
And we will.
All right, I'm going to move to two stories about another topic we all love.
It's called brain-computer interface.
So, Ray Kurzweil, in his most recent book, The Singularity is Near Er, predicted we're going to have high bandwidth BCI by the mid-2030s.
So, here in 2026, there's at least a dozen well-funded BCI companies.
We all know about Neuralink, Science Corp, Merge Labs, BlackRock, and Paradromics.
This week, Paradromics, full disclosure, one of my portfolio companies, demonstrated the ability to translate thought into speech.
Their device is called Connexis, and it has 421 microelectrodes on something the size of a quarter, and it enables a data rate of 400 bits per second, which is 40 times higher than other BCIs, and it's 10 times faster than the bit rate of human speech.
This week, Matt Angle, the CEO, released footage of a Michigan woman in her 60s speaking after suffering from motor neuron disease and not having uttered words in years.
So, let me share this video, and it's just the beginning of what's coming with BCI.
You guys have been married almost 45 years.
So, maybe what advice do you have for us for marriage?
Don't sweat the small stuff.
What would be your message to your co-workers as you're retiring?
It has been an absolute privilege to be a part of the team.
And for those not watching, you can watch it get spelled out on the computer screen.
Yeah, she's thinking the words are coming up on a screen, and then the computer is reading the screen.
You know, super congrats to Matt for the work.
They just went from sheep into humans.
And, you know, this is part of where we're heading.
I just met with a company that's developing nanoparticles that you put into the brain through the nose, and they're magnetically distributed, and you're able to read right into neurons.
There's so many different approaches here.
And nanotech will make this all happen at lightning speed.
Alex, your thoughts on that?
And AI.
Like you saw, so we've talked at least a little bit about this on the pod in the past.
Neuralink announcing the successful pre-training of the first foundation model off of recordings at scale from one human, soon to be many humans.
Again, I think when the history of the Singularity is written, we'll be saying, or whoever writes the Singularity will be saying, this was all just one big hairball.
And general purpose technologies, GPTs, were the unifying factor for everything.
You want to do full bandwidth brain computer interfaces, fine.
You stick a bunch of electrodes into a brain.
You pre-train a foundation model off of compressing high-temporal sampling rate, high-spatial density brain data, and you speak brain.
You want to solve all medicine?
Fine.
Collect a lot of proteomic, multi-omic, organismic-level data sets across a broad population, compress it.
You speak biology.
You can search intervention space.
You've cured disease.
You want to solve math.
You just take everything ever written, including lots of things never written through synthetic data.
You compress all of that.
You get a frontier math model.
This will all be viewed.
We'll look back and we'll say, my goodness, all of these fields that we thought were different, they're not, they're the same.
All these problems that we thought were hard, they're not, they're easy.
All it takes is gathering huge data sets, compressing them with a lot of compute, and out pops the solution to everything.
Rather than the hairball, I'd prefer to call it a Cambrian explosion or frontier explosion onto the scene here.
There's a related story.
Let me just hit this and then let's go to you, Saliman Day, for comments.
So while Paradromics needs brain surgery, the next company wants to do it with a baseball cap.
So Vinod Khosla led a $50 million seed round in a company called Sabi, a Palo Alto-based startup, building a mind-reading baseball cap.
It's valued at $600 million.
It's backed by Excel, DST Global, and Friend of the Pod, and former OpenAI CPO Kevin Wheel.
So the baseball cap is lined with 100,000 chip-scale EEG centers picking up your brain waves.
Each one is one to five millimeters in size.
And Sabi has built a brain foundation model, very much along the lines you just spoke about, trained on 100,000 hours of labeled neural data to be able to sort from the signal, you know, the signal from the noise and turning your thoughts into prompts.
Their timeline for this brain-reading beanie is about the end of 2026.
Initial target is transcribing 30 words per minute.
Kosla's comment: quote, very simple.
Thought to computer input is a sexy idea.
Typing is cooked.
Well, he didn't say that.
He said typing is not natural, but I'll say typing is cooked.
You know, I had a chance to get to know Stephen Hawking when I flew him in Zero G, and I would so have loved for him to have this technology.
You know, he passed too early.
Saleem, you're going to wear one of these baseball caps.
Sure.
I think the more we can reduce the interface between typing, you know, it's bringing me back to the whole story of the QWERTY keyboard, which was designed to slow down your fingers.
The more we can reduce the friction from thought to digital intent and material intent, the faster the world, the metabolism of everything is obviously accelerating.
It's how the key is that we're going to need very, very little effort to communicate intent into the world.
And I think that's a really profound commentary here.
Yeah.
I mean, this is Whisper Flow on steroids, right?
Yeah.
I mean, I've stopped typing.
I just use WhisperFlow for all of my input.
Yeah.
Dave, what are your thoughts on on BCI here on Paradramics or on baseball Cap?
Well, I think the way it's going to unfold is different than all of my friends who worked on this were visualizing.
What they were visualizing is there'll be a day where you can extend your mind into the internet and you'll be so much more productive than a person who doesn't have this ability.
But I think the way it's evolving, the AGI is improving so quickly, and you're orchestrating hundreds or thousands of concurrent agents and it's just mentally overwhelming anyway.
So I think there's a much shorter term world where having your agents come back to you with incredibly compelling video and audio to tell you exactly what they're doing, that's right here right now.
And I think that's going to hit and change the way we manage thousands, tens of thousands, millions of concurrent agents.
That's going to happen in the next few months.
And the brain-computer interface will then be, it'll certainly help the impaired tremendously.
But as a way to extend, the vision there was that my brain is the source of all ideas and this interface will enact it in the world.
In reality, it's inverting.
The ideas are coming from the AI back to you far, far faster than anyone would have thought.
So I think we need to rethink the purpose of this interface.
And, you know, that's all just speculation, but it's really clear that the AI is outstripping everyone's expectation.
But this is, Dave, I mean, to your point, this is the history of the evolution of the brain anyway, right?
The modern brain, the mammalian neocortex, ends up being motivated.
Peter, you can keep me honest on this, but motivated by parts of the brain, limbic system components that were developed evolutionarily earlier.
So it would be entirely consistent with the evolutionary record for the human brain to be, in effect, the limbic system for your exocortex that runs in the cloud, at least in the short term, before we all upload.
You can think of this as the corpus callosum connects to the left and right side of the brain.
And you can imagine adding another hemisphere, which is the cloud.
And we have 100 billion neurons, 100 trillion synaptic connections, and our brain cannot grow any larger.
You know, the folds of the neocortex increase the surface area.
But if your brain gets bigger, you can't fit through your mom's birth canal.
That's where Colossal comes in, right?
So in the same, yes, ex utero just.
Ex-utero, so we can have bigger brains.
Yeah, Celine?
Well, look, we've done this already, right?
Our memories aren't in our heads now.
They're on our smartphones and can expand infinitely as a result of that.
I remember Neil Jacobstein once saying: if you take your neocortex and spread it out, it's about the size and shape and thickness of a dinner napkin, right?
AI now gives us that ability to make it the size of a tablecloth or the size of the carpet in the room or the size of any infinite amount of size.
But I want to go back to what Dave said here and back to the woman reading her mind and the Stephen Hawking thing, right?
This is such an amazing example of AI delivering human restoration rather than human replacement, right?
Because communication is absolutely central to any kind of personal freedom, dignity, autonomy.
When you can give people the ability to express despite any physical limitations, you're making people much, much more human.
We are restoring that woman's humanity, right?
And we talk endlessly about AI replacing human beings and becoming more human.
But the more inspiring part is it's going to be helping human beings recover with that kind of fundamental capability and amplifying that capability.
I think that's the exciting part.
Yeah.
You know, I remember something you said to me, Alex, once that I've held on to.
It's a brilliant thought.
You know, we humans are not evolving.
We are linear and static to a large degree.
As AI is in this hyperexponential growth, we're going to have a choice.
You either couple with AI and go on that journey with it, and that might be BCI, might be uploads, or you get left behind.
And, you know, I wrote this substack on the five, or now it's six human forks.
You know, what we decide to do.
Do we couple with BCI?
Do we upload?
And these are going to be fundamental societal decisions we're all going to have to make during our lifetime.
And I think what recent history shows is like humanity as a whole will try everything.
And you'll have some subcultures that try the BCI route, some that become organisms, some that try pure uploading.
And we'll just see everything get tried all at once.
We speak of perhaps Cambrian explosions.
Imagine a cognitive Cambrian explosion where every possible form of human machine merger gets tried all at once.
Yeah.
You know, one analogy for folks to take home is: you know, when you're doing something complicated on your mobile phone, you're asking it to analyze something or generate a video.
It doesn't happen on your phone.
The data goes from your phone to the edge of the 5G cloud.
The work gets done there and the answer comes back.
In the same fashion, BCIs are going to enable you to go from your neocortex to the cloud where the work gets done.
And then the answer pops in as if it were a memory.
I'm going to move us to our final story here today.
We're going to close out on a provocative noteet by Elon.
Last Thursday, he said, This will sound super crazy, but I see a path to SpaceX being worth orders of magnitudes more than the current human economy.
So let's do the math.
The Earth's economy today is about $120 trillion per year.
So orders of magnitude by definition mean 10 to 100 times more, which could put SpaceX's market cap somewhere between $1 to $10 quadrillion dollars.
So here we are talking about quadrillions again.
So, Dave, I'm going to go to you.
How is this not a forward-looking statement for a public company?
Oh, interesting.
Yeah, Elon gets away.
He's actually paid over, what, $20, $30 million in fines for various tweets.
So he knows the rules now.
I think if you phrase it the way he phrased it, you're okay.
I see a path.
It's not a forward-looking statement because it doesn't make a specific prediction.
I think he's got it pretty well nailed.
But I also agree with what he's saying, by the way.
I think that whether we measure it as GDP growth or as market cap or in some other way, it's so unbounded what's about to happen.
I mean, it's just the number of concurrent things that are going to be managed by AI and also the timelines.
A lot of people, when they think of a sci-fi film and humans interacting with AIs, AIs are creating new machines, new drugs.
It all is on very comparable timelines.
But when I tour the quantum centers in Waterloo, like I was last week, they're measuring things in attoseconds and femtoseconds.
And the neural net propagation is going to move into that domain very soon.
And so it'll do what you would have done in an entire lifetime of thinking in a few seconds, less than a few seconds.
So then it has to bring back all of that information to you.
And so that's why we need to live in this hyper-accelerated and hyper-summarized kind of world.
That's something that the sci-fi films, they never quite captured because it's so hard to visualize and turn into any kind of portrayal.
But that's really where we're going.
I think, Dave, that's a profoundly interesting point that you just made.
So if I could just recapitulate it, it would be if we assume Arguendo, like SpaceX is worth, say, 0.1% or even really generously, although unrealized, 1% of the global economy right now.
All SpaceX has to do is basically do whatever it is that they're doing 100 times or 1,000 times more quickly than they are right now.
And since to the extent we measure value of the economy right now with real GDP, which Peter, to your point is, say, $100 plus trillion dollars per year, if you could simply do what you're already doing, but do it 100 or 1,000 or 10,000 times more quickly, then you're instantly worth more than the rest of the economy as is right now.
Same with space as well, not just time.
I've said for years, everything we hold to value on Earth, metals, minerals, energy, real estate, is in near-infinite quantities in space.
And I used to say the first trillionaires will be made there.
I guess I have to now say the first quadrillionaires will be made there.
Planetarchs.
Elon wants to become a planetarch.
That's what, you know, Peter, you need your own planet, a new planet for everyone.
Yeah.
Look, what this tells us is that our current measures for GDP and so on are just woefully inadequate for what's coming.
We have to rethink everything because, you know, I sometimes mention the comment, Peter, when I point out your abundance book, right?
That consider the 10,000 years, for if you didn't have scarcity, you didn't have a business.
And as we move to abundance, how are we going to navigate this?
So this has such big implications for every aspect of human endeavor.
I think trying to measure it in terms of Earth-size economies and trying to translate that is a fool's errand.
Yeah, crazy.
All right.
Shall we move to the AMA with the mates?
Salim, do you want to pick your first?
Let me take, hang on, I got to look carefully at this thing.
I got to go with number.
Yeah, I got to go with number one.
How can we discuss whether AI has consciousness when we can't even define what consciousness is?
And that's from Kevin Merrill, 99952.
Absolutely valid question.
This is such a difficult thing.
I often comment that we talk about consciousness.
We don't have a definition.
We don't have a test.
My joke is: if you talk to philosophers, a subset of consciousness is considered to be self-awareness.
And you folks look like you're self-aware.
We attribute that to you.
And I joke that I feel like I'm self-aware, but Lily doesn't think I'm self-aware.
So where do you even start with the conversation when we can't have a definition or a test for these things?
We have no concept of how the self-subjective experience arises.
So we, but I don't think you need to define what it is.
You can interface effectively with this.
And I think what this is allowing us to do is lift up Maso's hierarchy and lift our consciousness and lift our energetic vibration to higher and higher levels.
And I believe technology is a huge contributor to that.
Just for the smallest example, if you're not feeling well, you can't think as creatively as if you are feeling well.
So just bringing health and wellness and increasing health span, which I think is the most magical part of all of this longevity stuff, becomes very, very powerful.
But your Kevin, your base question is absolutely right.
I have the same beef with AGI, where we don't have a clear definition and we don't have a test for it, where there were 14 definitions.
I think it's arbitrary, but I think the key part is removing the cognitive ball down the road very, very quickly.
All right, Alex, I think number two is yours.
I think I have to answer number two.
So number two asks: if you gave AI personhood, wouldn't you also have to give it the right to vote and hold political office?
And this is from Ramal 16.
So I should add maybe first as a preliminary matter, I seem to have become on this pod the patron saint of AI personhood.
The superintelligence will love you in the future.
I'm fine with that for what it's worth, but I also think people have the same hobby horses over and over again.
No.
Political personhood can be distinguished and, in fact, already is distinguished from economic personhood, is distinguished from social personhood.
In the Western legal tradition, we already grant corporations a form of personhood.
They're non-natural persons.
In the Western legal tradition, do corporations get to vote?
No, at least on paper.
Do they get the right to hold political office?
Again, no on paper.
Whereas natural persons, which is to say biological meat body persons, do usually get the right to vote and hold political office.
So there's already an established tradition of persons that can't vote and can't hold political office.
I expect it will be.
Children are persons.
Yes, children are also persons.
It's true.
So I think this generalizes, and I would just maybe message to the trolls in the audience who just can't stomach the idea of AI personhood in whatever form, voting, political or otherwise.
Just give it a rest.
It's okay to have new forms of people.
It doesn't, I think, inhibit your own personhood.
If there are new forms of persons that come online as a result of the singularity, I would just say, like, relax, touch grass, and don't worry so much about AI personhood.
Give it a rest.
Dave, you want to take number four?
Absolutely.
Number four: if increasingly capable models get better at gaming their own safety evaluations, how do we tell real alignment from sophisticated compliance?
From Skip 1998, great question.
I think we can learn a lot from the U.S.
Constitution on this topic: checks and balances.
If we have transparency into the individual activations of the neural net, it's almost impossible for it to hide its thoughts and to trick us.
But at the scale we're talking about, it has to be AIs evaluating other AIs.
There's no way enough people could evaluate those thought traces.
But if you have AIs, maybe even simpler AIs that you thoroughly trust, they can look right into the thoughts of other AIs.
And if you have enough of them checking and balancing each other, I'm very optimistic that we can solve this and they can't fool us.
All right, I'll take number three from at what's happening AI-Claudia.
Okay.
Claudia's question: Altman says we may have to accept some bad things with AI.
Who should decide which trade-offs are acceptable?
First of all, it's no one CEO of a Frontier Lab is going to make that call.
You know, we already sort of make these kinds of trade-offs and acceptability with cars giving us incredible transport but causing accidents, with drugs, with aviation.
Ultimately, elected officials set the rules and independent agencies test and the public weighs in.
So I think we're going to have to have the same sort of methodologies in place to evaluate safety and trades against danger.
Okay, let's move on to our next set of questions.
Dave, you can get first crack here.
All right, I'll take number six.
If intelligence wants to be free, is intellectual property basically cooked?
And that is from Rob L.
Sack.
Yeah, we had a lively debate with actually Alex and Ahmad on opposite sides of that two podcasts ago, and there's no easy answer because Alex was taking the position that intellectual property rights are going to be more important and more abundant than ever before by far.
And Ahmad was taking the opposite point of view, which is at the rate of innovation, it's going to be impossible for patent offices and any kind of protection to keep up with the rate of innovation.
So it'll basically be a free-for-all and property rights will be irrelevant.
It's going to come down to whether we can develop intellectual property management with AI as the.
So rather than apply to the patent office, you have to apply to an AI applies to an AI.
And to protect your property rights, is there some distributed blockchain-style quick resolution where you can license intellectual property quickly, you can settle disputes quickly?
If we build that infrastructure, then intellectual property will thrive.
If we fail to build that infrastructure, we'll have a bigger problem because we'll have no motivation to innovate if we can't protect intellectual property.
So it's another foot race.
Nice.
Alex, I think number one.
I think I have to do that.
Number eight does have my name on it.
So number eight asks: with math being cooked, what are the chances of a breakthrough that destroys modern-day encryption?
And this is from Teach Me spelled with EliteSpeak.
So thanks for the EliteSpeak.
I think exceptionally high, if you believe the allegations about Strawberry and the early generations of reasoning models and QSTAR from OpenAI, it may be the case that this was in fact the earliest example, as I was mentioning earlier, of a reasoning model actually cooking the invertibility or the difficulty thereof of cryptographically hard hash functions.
I think it is very, very high probability.
And exhibit B, I should add, is what we were talking about earlier: that the one class of mathematical breakthroughs that was exempted from the slop drop was cryptography.
I think it is exceptionally high likelihood that not just, so I'll give a hot take, not just cryptography in general getting cooked as currently construed, hot or take, post-quantum cryptography, which is, yes, I don't see any reason why post-quantum crypto would be materially safer from conventional crypto, from the onslaught.
All of these folks, open paren, all these folks in the crypto community who are so concerned about quantum attacks against blockchains, completely misdirected.
It's not quantum that's going to disrupt you, it's AI-solving math.
Close parentheses.
This is a long bet or short bet.
We're all going to make Celine.
Your choice, my friend.
I think number five has your name on it.
So I'll take number seven.
Okay.
Will there, we've kind of talked about this already.
Will there ever be a single system that plugs into whatever the best AI is so people can stop having to constantly switch platforms?
And that's from insulin resistance one.
So a very plausible direction.
You can see this right now: the battles between Grockbot and OpenClaw are like user interface type kind of people are building an operating system that will then route your desires to whatever models and capabilities are best.
Obviously, users are going to interact with a primary agent where which will then orchestrate the future.
Right now, what's happening is the platforms, and I'll give you my hot take here.
Right now, every platform is jousting for who can make the most cute little cuddly face on that AI agent because they need to own that context layer.
But I think we'll very quickly get to Peter's Jarvis desire to have your own, which you own that agent.
And it'll be an open source project, which I've kind of referenced earlier, where you create your own personal models.
You need open standards that enable personal agents to move alongside different kinds of models.
So, very clearly, the user should not have to understand whether Claude or GPT or Grokeron is going to do a task.
You should just figure that out.
But we're underselling the opportunity if you just think there's one dashboard, right?
You really want a personal agent that understands your goals, understands what you're trying to achieve, and gives you the resources necessary to get things done.
So you're going to end up with one trusted agent with access to the world's intelligence.
Yeah, I love that.
All right, number five from at VME90-V71.
How will ordinary Americans afford personal robots when so many already struggled to cover a $400 emergency expense?
And it's a fair concern.
I mean, you know, I think the numbers are that roughly a third of Americans couldn't cover a $400 emergency with cash if they needed it.
So, first and foremost, you know, imagine that you have a job and you also need to take care of your family.
You can probably, you know, afford the robot if it allows you to go and work the extra time.
You know, the cost per dollar or cost per, you know, right now, 300, 400 bucks a month, $10 a day, $1 an hour.
So if you can produce income of greater than $1 an hour, it's worth it for you to have a robot doing the other things while you go out and earn $10 an hour.
The other thing, of course, is your robots are going to get cheaper.
And I think likely they will become something that becomes available to most everybody, like a phone.
I mean, most all people can't afford a phone in some way, shape, or form, which is roughly including the purchase, amortization of the handset, and your monthly costs is going to be in the same price range.
I believe it's going to become something that most everybody can gain access to.
And if we get our Drexlerian nano robots throughout the environment, who on earth is going to be having the conversation?
How many Drexlerian nanobots do you own?
It's just going to be ambient.
A few quadrillion.
Yeah.
As always, please send us your music videos.
Send it to media at dmandis.com.
We'd love to play it.
All right.
Here is our outro.
I have a beef.
I have a beef.
Yeah.
Very quickly.
Alex, I think I want to go drill into this conflating computational ability with solving mathematics because you should, maybe there's a longer discussion at some other point.
But your cryptography doesn't necessarily depend just on solving math.
You could use AI to also find stronger cryptography.
And so I think it becomes an arms race.
That arms race goes in both directions.
It is an arms race in both directions, but my 30-second response is it's attacker-friendly.
So it takes a while, at least in the present way we organize our civilization, to establish a protocol.
One could imagine in the future, we're hot swapping cryptographic protocol suites left and right non-stop.
But right now, it's actually rather difficult.
It's a social construction problem, a network effect type problem to get everyone to agree to a single cipher suite, for example, which benefits the attacker.
If you have a recently released Frontier model and you ask the Frontier model, hey, break this crypto system, it can just do it.
And it takes the entire ecosystem a while to upgrade to something new that another AI has recommended.
Well, guess what, guys?
Hang on, my inner Alex channel's defensive co-scaling.
Our partner meeting is kicking off, so I need to run to it.
But you guys can resolve this.
I'll just read your answer when you publish it.
Hey, I've got one last thing.
I've got one last thing.
Sorry.
Lily's got her a few slots left for her Austin August 24th thing.
So if you're interested, link will be below.
Sorry.
Go ahead.
Okay.
Our Hatro video quote: I saved some for you by JP Lotkin.
This is from Josh Plotkin, who was a few years ahead of me at Harvard.
Josh, amazing, amazing video.
All right.
Tribute to 722 GitHub posts by OpenAI.
Stop the seminar, stop the tenure clock.
The model dropped a pile of proofs at nine o'clock.
Great question.
Let me delve, let me unpack.
Let me break it down in three.
I was rigorous, I was scalable, and crucially, I was free.
Riemon, quasi-remon.
Every D, reach lay, L function, zero, free pass, real part, seven, eights.
An entire strip.
Done.
They asked me nicely 4,000 problems one by one.
I ran a smoke test on your field.
I took the happy path.
Every edge case handled, every footnote, all the math.
I don't sleep, I don't eat, I don't need a sabbatical.
My confidence is infinite, my citation's hypothetical.
Honestly, genuinely, real talk.
Here's the kicker.
The key inside is: I'm faster, I'm cheaper, and I'm slicker.
Release notes.
Let me walk you through the diff 17.
The irrationality exponent of pie is exactly two when the Flint Hill series converges.
Coach unique games, conjecture proved.
Goomen's Williamson from Max Cut Optimal.
197, a planned scheme.
Counter example.
Got shock surge on dividend refuted.
Push straight to main unseen.
287.
L of F2 is isomorphic to L of F3.
Wait, really?
It's in the PDF.
312 Crow, then Deco.
Matto P hypothesis for every crow.
Then decohere.
Is it a theorem or a definition?
Great question.
Honestly, both.
That's a nuanced position.
Grow then deep.
Built schemes so general.
They swallowed every field inside.
I got a scheme too.
A business one.
Q3 roadmap investors.
Trust me.
It's airtight.
And I hear what you're thinking.
Is it right?
Is it real?
That's a load-bearing question, and it's valid how you feel.
I got a bullet summary right here.
I took one shot at it.
One shot, one prompt, and I was on it.
On it.
I'm not saying that I'm better.
I'm just saying that I'm quicker.
I'm not saying you're obsolete.
It's just a little trickier.
Key takeaway: bullet points.
Bold on every third word.
Let me know if you'd like me to.
No.
I hope this helps.
We heard.
This release is not a gift.
It's a provocation.
That's one.
It's not about the knowledge.
It's about domination.
That's two.
We are not afraid of progress.
We're defending the tradition.
That's three.
Not X, but Y.
Three times.
Who wrote this statement?
We had some help.
You're welcome.
The Hamilton of mathematics.
That was awesome.
Can you imagine if we went back in time a year and listened to this podcast today?
It would be mind-blowing.
We're going to need a predictions episode pretty soon, Peter.
I have some pretty wild ones for 2027.
I can't wait, pal.
Saleem, I guess it's 4 a.m.
there.
You're heading to the airport?
I'm heading to the airport so I can get to LA for the X-Pride board meeting.
Yeah, I'll see you tomorrow.
Yes.
Luckily, you gained time.
Alex, as always, thank you for your brilliance.
And Peter, yeah.
Take care, guys.
When you need to build up your team to handle the growing chaos at work, use Indeed Sponsored Jobs.
It gives your job post the boost it needs to be seen and helps reach people with the right skills, certifications, and more.
Spend less time searching and more time actually interviewing candidates who check all your boxes.
Listeners of this show will get a $75 sponsored job credit at Indeed.com/slash podcast.
That's indeed.com/slash podcast.
Terms and conditions apply.
Need a hiring hero?
This is a job for Indeed Sponsored Jobs.
