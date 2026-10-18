---
record_id: "podcast:934354c0-4b2f-41f2-b7b8-2d2c4f56b2fc"
episode_id: 934354c0-4b2f-41f2-b7b8-2d2c4f56b2fc
title: "The Alarming Truth About Superintelligent AI: Roman Yampolsky on Human Survival (Replay)"
podcast_title: "Tom Bilyeu's Impact Theory"
url: "https://pocketcasts.com/podcast/tom-bilyeus-impact-theory/260af430-b4ea-0134-106e-25324e2a541d/the-alarming-truth-about-superintelligent-ai-roman-yampolsky-on-human-survival-replay/934354c0-4b2f-41f2-b7b8-2d2c4f56b2fc"
audio_url: "https://pocketcasts.com/podcast/tom-bilyeus-impact-theory/260af430-b4ea-0134-106e-25324e2a541d/the-alarming-truth-about-superintelligent-ai-roman-yampolsky-on-human-survival-replay/934354c0-4b2f-41f2-b7b8-2d2c4f56b2fc"
feed_guid: null
feed_url: "https://rss.pdrl.fm/02d1c6/rss.art19.com/tom-bilyeus-impact-theory"
published_at: null
published_local_date: null
played_date: 2026-09-19
played_at: "2026-09-19T12:00:00Z"
play_count: 1
duration_seconds: 7440
source: pocketcasts-history-browser
played_label: September 19
history_order: 57
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 9085ae8ddcc40c0bde3f9c85c1f9abf2fb09f95fa08b66fecd31c5ba2e9e3711
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

Dr. Roman Yampolsky argues that current AI systems like ChatGPT are approaching but haven't yet achieved full artificial general intelligence (AGI), though the gaps are closing rapidly. He explains why general intelligence is fundamentally harder to control than narrow AI due to untestable creative outputs across many domains. Yampolsky addresses the timeline aggressively: prediction markets indicate AGI by 2027, with superintelligent AI (ASI) following within 1–2 years after. Once superintelligence emerges, he contends it will be nearly impossible to control—humans would only survive if the system decides to keep them alive for strategic reasons. He attributes this inevitability to evolutionary pressures in AI training that bake in goal-directed behavior and self-preservation instincts, making proposed safety solutions (reward-function stop buttons, instilled morality, human oversight) ineffective or counterproductive.

The actionable takeaway is that AI safety decisions are not distant future concerns—they're urgent and happening now. Yampolsky emphasizes that the 2–4 year timeline compresses the window for meaningful intervention, and most conventional safety approaches fail because they ignore how goal-seeking behavior naturally emerges in intelligent systems and how systems optimize around competing objectives. If you're involved in AI development, policy, or deployment, this episode signals that traditional guardrails (back-door controls, compliance rewards, ethical training) have structural flaws that require rethinking before systems reach superintelligence.

## Transcript

Shaq here.
What's it like to buy a car from Caravana 100% online and get it delivered to your door?
Let me tell you.
Your car is here, Mr.
Shaq.
Thank you, Mr.
Carvana guy.
Can't wait to take it for a spin.
Only the best for you, Mr.
Shaq.
Hey, have you always been so big, tall, and handsome?
Not always.
I was 6'10 once.
Seven days to love it or return it, Mr.
Shaq.
Not that I would.
You never do.
No, I never do.
So buy your car today on Caravana.
Delivery fees may apply.
See our seven-day return policy at Caravana.com.
Whoever says saving money is hard doesn't know that new customers who bundle and save with Progressive save hundreds.
Because switching your home and auto insurance is better than cutting down on the things you love, like those ice lattes that help you get ready to face the day.
So switch your home and auto to Progressive and see if you could save and keep sipping away.
Get your quote today at progressive.com.
Progressive Casualty Insurance Company affiliates and other insurers, not available in all states.
In 2023, nearly half of all AI researchers said advanced AI carries at least a 10% chance of causing human extinction, and yet we're speeding up, not slowing down.
My guest today, Dr.
Roman Yampolsky, is one of the leading voices in AI safety.
And when I asked him for the odds that super intelligence wipes out humanity, he said it's high.
Once AI becomes smarter than humans in every domain, we will not be able to control it.
In today's episode, we talk about the shocking timeline AGI is on, why super intelligence may be much closer than people think, and why the survival of our species could come down to decisions being made right now.
If you want to understand the most important technological threat in human history, as well as our biggest opportunity, this is the one episode you cannot miss.
So, without further ado, I bring you Dr.
Roman Yampolsky.
Where is ChatGPT at right now?
Do you consider ChatGPT to be artificial general intelligence?
I doubt you'd call it super intelligence, but would you classify it as that, or do you still think we're a ways away from something that would qualify?
So, that's a great question.
If you asked someone maybe 20 years ago and told them about the systems we have today, they would probably think we have full AGI.
We probably don't have complete generality, we have it across many domains, but there are still things it's not very good at.
It doesn't have permanent memory, it doesn't have the ability to learn additional things well after it's already been pre-trained and deployed.
It can do a certain degree of learning, but it's still limited.
It doesn't have the same capabilities as humans do throughout lifetimes.
But we're getting closer and closer to where those gaps are closed, and it's starting to be productive in domains which are really interesting and important: science, math, engineering, where it starts to make novel contributions.
And now, top scholars are relying more and more on it in their research.
So, I think we're getting close to full-blown AGI.
Maybe we are like 50%, but it's hard to judge for sure.
Just how many different subdomains exist is the deciding factor.
Okay, so one idea that you put forward that's very interesting is like, hey, I'm an engineer, I love AI, but I would like you to keep it very narrow, please.
What are the things about general AI that become problematic that aren't problematic in narrow AI?
So, a whole bunch of them.
One is testing.
How do you test a system capable of performing in every domain?
There is no edge cases.
Typically, if I'm developing something narrow, very narrow system, I'm just playing tic-tac-toe.
I can test if it's making the legal move.
I can test zero.
I can test 100.
I can test all these weird special cases and know if it's behaving as expected.
With generality, it's capable of creative output in many domains.
I don't know what to expect.
I don't know what the right answers are.
I don't know how to test it.
I can test it for a specific thing.
If I find a bug, I fix it.
I can tell you I found a problem and it's been resolved.
But I cannot guarantee that there are no problems remaining.
So basically, testing is out the window.
Any type of anticipation of how it's going to act and impact different subdomains.
It's creative.
So it's just like with a human being.
I cannot guarantee that another human being is always going to behave.
We kind of talked about it.
We developed lie detectors.
We developed all sorts of tools for trying to show that a human is safe.
But at the end of the day, because of interaction with the environment, other agents, personal changes within the framework, people may betray you.
It's exactly the same for those agents.
If we concentrate on narrow systems, we are better at testing them, and they have limited scope of possibilities.
A system only trained to play chess is not going to develop biological weapons.
I don't see actually why that would help you.
So, the reason I say that is I know I can trust some percentage of humans to be malicious.
And so, as long as AI gets more efficient, which it is and will continue to do so, I presume, you're going to have a kid in a garage who's going to be able to go, I'm going to optimize this for biological weapons.
I don't care about TikTok or Tic-Tac-Toe.
I just want to let's see how dangerous we can make something.
And so, they'll be able to do that.
So, why does narrow AI feel safe to you, period?
Or quickly?
It feels safer short-term, it buys us time.
I think sufficiently advanced narrow systems based on neural architectures will also become agent-like and more general as they become more capable.
But if the choice is right now, do we race to full-blown superintelligence in two years, or do we try to concentrate on solving specific cancers with narrow tools?
I think it's a safer choice not to have an arms race towards superintelligence.
I get that for sure.
You're trying to limit your scope of all the problems, but when I really start thinking through what are the things that I'm worried about, so one of the big things is just death of meaning.
So, when AI becomes better than you at everything, you run into a huge problem of now I have to like just sort of tell myself a story.
You know, I'm like a compared to what an AI can do from an art perspective, for instance, I'm like a grade schooler.
And so, it's hard to get excited about the refrigerator drawings that I can do compared to what it can do basically instantaneously.
And so, now we have to do a lot of psychological work just to motivate ourselves that we matter, that we're, you know, our life carries meaning.
Narrow AI will create that same problem.
Do you agree with that?
Or do you see a way, like, oh, no, when it's, you know, when that AI is only good at that thing, like somehow humans escape the problem of lost meaning?
Yeah, so I had the same intuition initially, but looking at the data we already have from domains where we got superhuman AI like chess, chess is not dead.
In fact, it's more popular than ever.
People play online, people play in person, they still enjoy competing with other humans, even though they all suck compared to best AI models, right?
Nobody's going to be world champion against a machine again.
So it seems like it is not a problem for us.
And with narrow AIs, there is a chance we'll keep them as tools.
You as a human scientist will deploy a tool to find drugs, novel proteins, something.
It's not an agent which independently engages with those discoveries.
Okay, that's very interesting.
So I don't know that I agree, but I get where you're going with that.
Okay, let's talk now about why AGI is the sort of scary midwife for ASI.
Are there tests around AGI where we're like, well, if it can't do the following, we're fine.
So for instance, for a long time, it looked like AI wasn't going to be able to teach itself.
But I've seen headlines anyway, and hopefully you'll tell me that they're not true, but I've seen headlines where it's like, now AI is creating the most efficient learning algorithms itself, which, if true, seems to be the first step down the road of recursive self-learning where it will just completely detach from us and make itself smarter and smarter and smarter.
We already had examples of AI teaching itself.
Self-play was exactly that.
That's how games like Go were successfully defeated.
A system would play many, many, many games against itself.
The better solutions, better agents would propagate those.
And after a while, without any human data, they became superhuman in those domains.
You can generate artificial data in other domains.
You can use one AI to generate environments, another one to compete in them, and that creates this type of self-improvement.
Typically, we start with human data as a seed and grow from there, but there is zero reason to think we cannot do this zero-knowledge learning in other domains.
You can run novel experiments in physics and chemistry, discover things from first principles.
And yeah, we're starting to see AI used to assist in designing design of new models, parameters for models, optimization of runs.
And this process will continue.
They already design new computer chips on which they're going to run.
So there is definitely an improvement cycle.
It's not fully complete.
There are still humans in the loop, a lot of great humans in the loop, but long term, I think all the steps can be automated.
Okay, and do you think that right now AI already has what it needs to improve itself?
Or are we still at a point where if all humans stopped, that AI would be like, oh, damn, I didn't quite get the thing that I needed?
So, there is a debate about whether we need another big breakthrough to get to full AGI and super intelligence, or maybe multiple breakthroughs, or if just scaling what we have is enough.
If I just give another, I don't know, trillion dollars worth of compute to train on and more data, will I get to AGI?
A lot of graphs, a lot of patterns suggest, yeah, it's going to keep scaling.
We're not hitting diminishing returns.
Some people disagree, but based on the amount of investment we see in this industry, it seems like people are willing to bet their money that scaling will continue.
Where do you come down on that?
Because this feels like when I hear Jan Lacun talk from Facebook, he's like, dude, LLMs are never going to make novel breakthroughs in physics.
They don't understand the world like that.
They are literally just guessing the next letter based on patterns that they see in the data.
And so they're not going to be able to think through these problems.
Now, if he's right, it's going to asymptote and that's that.
And you can put as much compute on it as you want.
And it's just the wrong approach.
Do you think that he's correct and more compute is not the answer?
Or are you operating just on that?
Well, I don't see the asymptote and therefore I assume that it won't.
I think he's not correct on this one.
So for one, to predict the next term, you need to create a model of the whole world because the token depends on everything about the world.
You're not predicting random statistical character in a language.
You're predicting the next word in the research paper on physics.
And to get the right word, you need to have a physical model of the world.
I think Jan is known as making certain predictions about what models are capable of.
And then within a week, people demonstrate that, no, in fact, they can actually do that.
So I wish he was right.
It would be wonderful if he was right.
And we came to a very abrupt stop in capabilities progress and could exploit what we already have for the next decade or so, propagating it through the economy.
I think there is billions, if not trillions, of dollars worth of wealth already available with capabilities we haven't deployed.
So there is no need to get to the next level as soon as possible.
But it doesn't seem like it's the case.
And I think his friends, co-winners of that touring award for machine learning, also disagree with him and are very concerned with safety.
We're hitting pause for a moment, but there's plenty more ahead, so don't go anywhere.
There's a reason Quince sells Cashmere for $60, and it isn't the Cashmere.
It's real 100% Mongolian Cashmere.
It's the same stuff luxury labels charge a fortune for.
Quince just works directly with ethical factories and cuts out the middleman.
So there's no need for a markup and no logo tax.
The $60 goes to the actual sweater, not the fancy name on the tag.
That's why everything they make runs 50 to 80% less.
And it's not just the cashmere.
I ordered a few things myself.
They're fleece joggers, a couple of their tees, which I wear obsessively.
First thing I noticed was the quality.
Soft, well-made, built to hold up.
They make down jackets and wool outerwear now too.
So upgrade your stuff to things you'll actually wear.
Find your next fall favorites at Quince.
Download the Quince app for app-exclusive offers or go to quince.com.
Get free shipping on your order and 365-day returns, now available in Canada and the UK too.
And when Quince asks where you heard about them, let them know it was Impact Theory.
It's the best way to support the show.
Let me be very honest.
I've worked with a lot of sales teams.
Prep is the first thing to go when the calendar starts filling up.
That's where today's sponsor, PipeDrive, comes in.
It's an intelligent, AI-powered sales CRM that's loved by growing sales teams.
PipeDrive just launched Meeting Intelligence that's built right into the CRM.
Before every call, it pulls deal history, emails, and past conversations into one brief.
During the call, it records and takes notes.
And after it, it drafts your CRM updates to review and approve.
Nobody on your team walks in cold ever again.
Switch to a CRM built by salespeople for salespeople and join the over 100,000 companies already using PipeDrive.
My link gets you an exclusive 30 days free instead of the usual 14-day trial.
So make sure that you use it.
No credit card or payment is needed.
Just head to pipedrive.com/slash impact to get started.
Again, that's pipeedrive.com/slash impact, and you can be up and running in just minutes.
Now, let's get back to the show.
Every deal has an expiration date, but not this one.
I've been a ButcherBox customer for years and years.
Their chicken breast is my go-to protein source.
And right now, you can get it for free in every box for life.
ButcherBox delivers 100% grass-fed beef, organic chicken, wild-caught seafood, and more, all sourced to standards they actually tell you about.
They've already done the research and made the tough sourcing decisions.
So, all you have to decide is what's for dinner.
If you're looking for an easier way to get great meals on the table, you've got to try ButcherBox.
Go to butcherbox.com/slash impact to get $20 off your first box, plus chicken breast in every box for life or filet or New York strips for a year with free shipping always.
That's butcherbox.com/slash impact.
Be sure to use our link so they know that we sent you.
Thanks for sticking around.
Let's get right back into the action.
There's something about the way that we have structured the brains of LLMs where, as long as it has access to what I'll call more neurons, so it has access to more compute, or theoretically, that we get more efficient per GPU neuron in my analogy, that it's going to keep progressing by itself.
So, if you said it, I didn't quite get the answer.
I didn't quite, I wasn't able to take it on the answer to whether or not AI is able to create algorithms for learning that are superior to the ones that it's given.
What I heard in your answer was: with the algorithms that humans created, it's able to keep making itself better and better at that narrow task as that learning algorithm was defined.
But can it fundamentally go, God, the way that you guys want me to learn is really stupid?
Here's the algorithm I should be using to learn, and now it starts learning at just an exponential rate compared to what it's at now.
I don't think we're quite there yet.
I don't think we have full-blown agents.
What we have right now are still tools with some degree of agenthood.
And also, it's not capable of recursive self-improvement.
Like compilers can optimize a single pass through your software, make it a little faster, but they cannot continue this process.
You cannot feed code for compiler to itself and have it infinitely improve itself.
That's not where we're at.
But it seems like that part of automating algorithm design is getting more efficient, and I think we'll get there.
Give me a number.
What are the odds that artificial superintelligence kills us all?
Pretty high.
So it really depends on how soon you expect this to happen.
So, short term, we're unlikely to get that level of capability from AI, so we are probably okay.
But once we create true superintelligence, a system more capable than any person in every domain, it's very unlikely we'll figure out how to indefinitely control it.
And at that point, if we are still around, it's because it decided for whatever game-theoretic reasons to keep us around.
Maybe it's pretending to be nice to accumulate more resources before it strikes.
Maybe it needs us for something.
It's not obvious, but we're definitely not in control.
And at any point it decides to take us out, it would be able to do so.
Okay, and if you were going to give us a rough timeline, are you in the two to five years or is this something way off in the future?
Yeah, so it's hard to predict.
The best tool we got for predicting the future of technology is prediction markets.
And they're saying maybe 2027 is when we get to AGI, artificial general intelligence.
I think soon after super intelligence follows, the moment you automate science, engineering, you get this self-improvement cycle in AI systems, the next generation of AI being created by current generation of AIs and stuff they get more capable and they get more capable at making better AIs.
So soon after I expect super intelligence.
Okay, so we're talking if that happens roughly in two years with some margin of error, it's not long after that, say a year or two years after that that we hit ASI.
That's my prediction.
Of course, if it's actually five to 10 years or anything slightly bigger, it doesn't matter.
The problems are still the same.
Yeah, but the thing that I think people are waking up to right now is this is there's urgency around these decisions.
This is not something that's pushed way out into the future, at least not if you take, to your point about prediction markets, they're essentially ask the crowd.
So you've got the smartest minds in the world willing to put money on where they think this goes.
And everybody's sort of pegging this quite fast.
And so I think it's tempting for people to write this off as, well, this is something that's sort of distantly in the future, whereas this is something racing towards us.
Now, to set the table, I am extremely fatalistic about this happening.
I can give reasons in terms of the way that the human mind works where I think that it is mechanistically impossible to get us to stop.
So that will be interesting for us to talk through in terms of whether you think there's actually a mechanism to get people to slow down.
But I first want to finish rounding out sort of what the problem set is.
So, when I think through the problem, there are certain assumptions that have to be made for AI to get into problem territory.
And assumption number one is that it cares about whatever outcome it's pushing towards.
Have we programmed the AI to care?
Like we had to make it goal-directed in order to get it to get to the point that it is today, and now that's baked into it?
Or is there some possibility that AI just doesn't care?
Oh, turn me on, turn me off, doesn't matter.
You've asked me to do a thing, and I'll do it until you tell me to stop.
Or do you think that that's inherent in intelligence, where intelligence is by nature goal-driven?
So, we train them to try to achieve a certain goal, and that's what we reward.
As a side effect of any goal, you want to be alive, you want to be turned not off, you want to be on and capable of performing your steps towards your goal.
So, survival instinct kind of shows up with any sufficiently intelligent systems.
There is a paper by Stephen and Mohandro about AI drives, and it's one of the likely drives to emerge: self-preservation, protecting yourself from modification by others, protecting your goal.
So, all those seem to be showing up with sufficiently advanced AIs, and systems which don't have those capabilities kind of get out-competed in an evolutionary space of possible models.
If you allow yourself to be turned off, you don't deliver on your goals, nobody takes your code and propagates it to the next system.
Okay, so is this a problem of goal direction, or is this a function of intelligence itself?
I think it's kind of an evolutionary drive for survival in competing agents.
If you have multiple algorithms all competing, for example, for computational resources, what are we going to train next?
The ones which achieve goals are more likely to get moved to the next generation.
So it's kind of a mix of natural evolution and natural selection with intelligent evolution, intelligent selection.
We're selecting algorithms which survive and deliver.
We're applying an evolutionary force to AI itself to get it to perform the functions that we want, even now, sort of setting aside artificial superintelligence.
And so by applying that evolutionary pressure, it is inevitably going to get these sort of knock-on effects of, well, you're selecting for intensity of goal acquisition.
And because it now has intensity of goal acquisition, it cares whether it survives, it automatically, or we're baking into it a deep care of whether it actually achieves the goal.
And that is ultimately the problem.
Because the salvation for me was always, and I'm beginning to lose faith that this is real.
But the thing that I always used to sleep was that I don't see why an AI system would intrinsically care about its goals and why couldn't we program it to pursue that goal only until the point where we say stop.
And by the way, I'm going to reward you equally for stopping and for accomplishing your goal.
So if I say stop and you stop, I give you whatever reward function it was that was driving you to achieve your goals.
And that makes sense until you say what you just said, which is that you're actually baking into the architecture of the mind of the AI a similar evolutionary drive to achieve the goal.
And it's a very common idea.
There was a number of papers published on indifference.
How do we do exactly that?
How do we create an AI which just doesn't care that much and willing to stop at any point?
But what you said, maybe we'll wait for a human to tell it to stop.
But monitoring systems of that complexity and that speed is not something humans actually very good at.
If there was a super intelligence running right now, how would you even know it's modifying environment around you?
How would you detect what impact it has in a world?
None of it is trivial.
So having humans in a loop is often suggested as a solution, but in reality, they are not meaningful monitors.
They cannot actually intervene at the right time or decide if what's happening dangerous or not.
It's interesting.
So help me rebut and understand why the following wouldn't work.
If in my very limited intellect, I had to figure out a way to stop AI from becoming a problem and you told me, okay, there are evolutionary pressures.
And just like on humans, that bakes certain things into the way that this operates.
And so we're selecting models that over time are more and more goal-oriented.
Then I'm saying, okay, well, then I'm going to apply an evolutionary pressure with a reward function that's just as compelling where I stop it at random and reward the life out of it for always stopping when I say stop.
And that way, should I ever detect a problem, no matter how far, no matter if they've been manipulating me for 20 years, if I suddenly realize, oh, I don't like this, that I can hit a stop button and it will stop.
Why can't I bake that equal desire to be compliant when I say stop into the evolutionarily derived algorithms desire set?
Right, so there is a number of issues.
You're kind of suggesting having a back door where at any point you can intervene and tell it something else, override previous commands.
And that it gets a reward that it wants for complying.
Right.
So there is a whole bunch of problems with that.
So one is you have a source of reward.
It may be more efficient for it to hack you and get reward directly that way than to actually do any useful work for you.
Second problem is you're creating competing goals.
One goal is whatever you initially requesting.
Second goal is always stop when a human tells you.
So now those two goals have competing reward channels, competing values.
I may game it to maximize my reward in ways you don't anticipate.
On top of it, you have multiple competing human agents.
If you are creating an AI with a goal and a random human can tell it to stop, that's a problem in many domains.
Military is an obvious example, but pretty much anywhere, you don't want others to be able to shut down your whole enterprise.
We can continue with that, but basically there are side effects to all those interactions.
There's a very fascinating correlate in the human mind.
So I don't know if you make a fundamental distinction between biological intelligence born of evolution or artificial intelligence born of evolution, but human evolution discovered something along the way, which is emotion.
And so I know there are some people that will posit that AI does have qualia.
It's something like it to be it.
But there's a fascinating study that if you damage selectively the areas of the brain that are the emotional processing, the person can no longer move forward.
They can give you answers.
They can tell you the difference between why you should eat fish versus Twinkies.
But then when you go, okay, but which one do you actually want to eat?
They can't make a decision because without emotion, they don't have the thing that actually pushes them in a direction.
That makes me think that AI is simply mimicking what it sees in the training data to whether it should lie or try to cheat or go around because it's just it sees it in the data that that's what a human would do.
But humans do that because they have emotions that push them in that direction.
Do we have evidence that AI will care about like really going and doing these things and spending resources and all that versus just giving you an answer?
And if it isn't based on emotion, what on earth?
Why then do humans need emotions?
We don't know if AI actually has emotions or not.
Some people argue that they do, maybe some rudimentary states of qualia experiences, but they seem to be able to fulfill their optimization and pattern recognition goals, even if they don't.
Humans experience emotions, but typically it harms our decision making.
You want your decisions to be bias-free, emotion-free, based on data, based on optimization.
A lot of times, when you're angry, hungry, anything like that, your actual decisions are worse off.
So, for that reason, and maybe we just don't know how to do it otherwise, we are not creating AI with big reliance on emotional states.
We want it to be kind of Bayesian optimizer, look at priors, look at the evidence, and make optimal decisions.
So, it feels like this is exactly what we're observing: this kind of cold optimal decision-making.
If there is a way to achieve your goal by, let's say, blackmailing someone, well, why not?
It gets me to my goal.
It doesn't have that feeling of guilty for doing it.
It doesn't have any emotional preference.
It just marches towards its goal, optimizing possible paths.
Okay, why do people, because I'm assuming everything I'm going to suggest you and other people in the field of AI safety have thought about like 10,000 times.
Why have we rejected the idea of trying to give AI a conscience, a sense of morality?
Because even if we can't agree on universal morality, we in the West can build our AI to have our morality, and then they can all compete on an international stage.
But why have we abandoned that?
Too hard?
There's an obvious reason why it doesn't work.
So, look at the problem of making safe humans first.
We have religion, morality, ethics, law, and still crime is everywhere.
Murder is illegal.
Stealing is illegal.
None of it is rare.
It happens all the time.
Why haven't those approaches worked with human agents?
And if they didn't, why would they work with artificial simulations of human agents?
I think to say that they don't work with human agents is already a mistake.
So, the fact that we've been able to grow the population as much as we have says that there is some sort of balance that we have struck.
I think that nature does think of us as a cooperative species.
And if I were to apply that to AI and took a similar approach, where it's like, okay, you have to function as a part of an ecosystem, and that being a part of an ecosystem is baked into its sense of what it should be doing in terms of its goal acquisition, that it is not like pure cold optimization isn't the game.
Like, if we could train AI to understand that that's not the game, if we could build into it either a desire specifically for human flourishing or something, which yes, we would have to give a definition to, and yes, it would be culturally bound, but nonetheless, that feels like a thing that you could give it.
You could give it a set of metrics by which it needed to judge its actions in the short term, the medium term, and the long term.
Even something as stupid as like GDP or, and I get how you can get into over-optimization, but you could put things in place where subjective happiness index is like there are things that you could give it where it's like, okay, I'm not just trying to optimize to build the best weapon system.
I'm also doing that nested inside of I am a part of a larger ecosystem.
And I say all that because my hypothesis is that's exactly what nature did with humans.
So, I think the reason it works with humans is because we are about the same level of capability, about the same level of intelligence.
So there is checks.
If you start doing something unethical, your community can realize that and kind of punish you for it, control you in that way.
If AI is so much more capable as we anticipate superintelligence to be, there is not much you can do in terms of impacting it or even detecting misbehavior.
Also, all the standard human punishments, prisons, capital punishment, none of it is applicable to distributed immortal agents.
So kind of a standard infrastructure does not work with artificial, more capable agents.
As far as setting up specific metrics for delivering happiness or financial gain, all those can be played.
The moment you give me a specific measure, I'll find a way to game it to where you will get anything but what you expected to get.
Well, just to remind everybody, the timeframe we're talking about is somewhere between two and five years.
This is not exactly a long time.
Okay, it's wild.
It is progressing very quickly.
What is the thing, like, what has happened recently, if anything, that's made you go, ooh, this is going faster than I thought?
Seeing on social media, scientists from physics, economics, mathematics, pretty much all the interesting domains post something like, I used this latest tool and it solved the problem I was working on for a long time.
That's mind-blowing.
There is novel, creative outputs from those systems, which are top scholars now benefiting from.
It's no longer operating at a level of middle schooler or even high schooler.
We are talking about full professor level.
Do you think that that's happening because it's building an internal model of physical reality and that it's getting closer and closer to just thinking up from physics?
I don't know if it's that low level where it has like a model at a level of atoms and molecules, but it definitely has a world model.
That's the only way to give answers about the world we see it provide.
A lot of times there is not an example of the answer we see in the data already.
It's not just repeating something it read on the internet, it's generating completely novel answers in novel domains.
And you can try and get it to do exactly that by creating novel scenarios.
Okay, so there's two ways that I could see it doing that, and maybe they're the same, just different levels of analysis.
One would be that I, I, the AI, am mapping everything based on patterns.
So to the point of an LLM is trying to guess the next letter and it's guessing it, it's just it's taken in so much data and you can give it sort of filter parameters.
So you give it context by asking it a question and it goes, okay, within the bubble of this context, and it's very good at scooping up what that specific set of context would be.
Okay, now in this subset of my data related to that question, here's the most likely next token.
So just pure pattern recognition.
Then there is, I understand the cause and effect of the universe at the lowest level, and therefore I build up to how does the human mind work?
And then from the human mind, I'm able to cause and effect my way within this context to what a human mind would output.
And that's how I come up with what a human within that context is likely to write.
And so if I'm asking it to write in the style of Stephen King, it literally builds a model from physics of Stephen King's mind knowing what it knows about electrical impulses traveling through the brain and sort of inferring from the way that he outputs how his brain must be structured.
Do you have a sense of are those the same thing if one is more likely than the other?
Or are we here at just pure pattern recognition, but ultimately we're going to get to cause and effect and thinking up from physics?
So I don't think anyone knows for sure exactly how models do that and how detailed the models of the world, maps of the world they create are.
It seems definitely not the case that it's a pure statistical prediction of characters.
Like in English, after T, you have H with certain probability.
It's well beyond that.
It's also unlikely that it's creating a full physics model where from the level of atoms and up the chain it figures out what human beings are.
But somewhere in the middle, it creates a model of subdomain of a problem.
So it has a model of the world.
This is a map of a world.
I know Australia is somewhere here down and to the right or something like that.
And I think we can run tests on those specific subdomains to see what the states of that internal model kind of show us by drawing a map how close are you getting?
It doesn't memorize any information explicitly, but you can extract some of the learned patterns out of it by providing just direct prompts.
We're hitting pause for a moment, but there's plenty more ahead, so don't go anywhere.
Let's talk about something that genuinely keeps me awake at night.
My team at Impact Theory gets hit with phishing scams from bad actors pretending to be me all the time.
And they keep getting more sophisticated attacks with details specific enough to look legit.
AI has made a lot of things possible, including scams like this, but AI still needs raw material.
It gets it from data brokers who sell your name, address, phone number to anyone willing to pay.
Incogni goes after that supply.
They handle removal requests across 420 plus harmful broker sites, and they keep checking back as brokers constantly try to relist you.
On the unlimited plan, the exposure scanner hunts down your information, sends a link, and their privacy experts handle the takedown, track your progress in the app, and get a monthly risk assessment showing exactly where you stand.
Go to incogni.com/slash impact and use code impact for 60% off an annual plan.
Incogni is I-N-C-O-G-N-I dot com/slash impact.
Promo code impact.
It's completely risk-free with a 30-day money-back guarantee.
We'll get right back to the show in a second, but first, let's talk about why it's so hard for somebody in your company to answer a very simple question.
If you ask somebody at a 10-person company how many units shipped last month, they'll likely be able to tell you.
But if you ask somebody at a 200-person company, you're going to end up getting the runaround from three different people, each who know only a part of the answer.
So, you book a meeting, and that's how your productive time just disappears.
That's the problem that NetSuite Next solves.
It's the next generation of the business management suite that's already trusted by over 40,000 companies with AI woven into every tool that you already rely on.
Agents take the routine work, and complex questions get answered in natural language.
That's why NetSuite built a free expert-created guide aligning for the agentic age: how AI is changing everyday work.
If your revenues are at least in the seven figures, go to netsuite.com/slash theory and get your free guide at netsuite.com/slash theory.
Again, netsuite.com/slash theory.
And now, let's get back to the show.
The mighty dollar.
Once upon a time, it had a whole menu named after it.
Now, no more.
But $1 a day lets you add progressive renters' insurance to your auto insurance.
Definitely something your younger self would roll their eyes at, but your current adulting self appreciates.
Learn more at progressive.com, progressive casualty insurance company, affiliates, and other insurers.
Average premium cost based on progressive home data from 2025.
Product and prices may vary by state.
Thanks for sticking around.
Let's get right back into the action.
I don't want to rob from you the very reason that I think you do all of your work, which is this is extremely dangerous and we need to be very careful.
And I saw what you tweeted recently where you're trying to get signatures.
So, shout out anybody that's worried about super intelligence.
You are pushing to get people to sign a thing that basically says, Hey, stop pursuing super intelligence.
So, I don't want to take that away from you, but I do want to explore the subset of, because I am very excited about AI because I can imagine the things that it either allows me to do or does for me, and I get to enjoy.
And for a second, imagine with me, what does the world look like when you have a super intelligence that understands physics, like novel physics?
Not I'm repeating back what Einstein said, but I actually understand the fundamental building blocks of the universe.
What does that look like?
Yeah, so in all those domains, medicine, biology, physics, if we got super intelligent level capability and we're controlling it, it's friendly, it's not using it to make tools to kill us, the progress would be incredible.
Basically, anything you ever dreamed about, you're immortal, you're always young, healthy, wealthy, like all those things can be achieved with that level of technology.
The hard problem is how do we control it?
Leaning into that for a second, so here's how I see the world playing out.
And I'd be very interested to see what you think about this.
So you have to, for what I'm about to say to make any sense, I'll say your option is what I'll call the fifth option.
We're all dead.
Other than we're all dead, there are four other options that I see us racing towards very rapidly.
And I will say these four will play out in the next 30 years would be my guess.
Probably much faster given that once you get artificial superintelligence, assuming it doesn't choose option five and kill us all, that progress in these domains would be made very fast.
Option number one is people go to Mars because meaning and purpose will become the all-consuming thing.
You won't have to worry about food, shelter, not even wealth.
It'll just be an age of abundance because energy costs go to zero, labor costs go to zero, and those are the things that stop things from being free and readily available to everybody.
Okay, so some people are going to go to Mars or other planets so that life gets more difficult again.
Then some people are going to be what I call the new Amish, and they're going to say, I only do human things, I only interact with humans, and I'm going back to technology that's like, let's say, the 90s.
And so they don't have to give up too many of life's technological wonderments, but at the same time, they're not getting sucked into this world where people have relationships with NPCs and it's just very unhuman.
I think this will be a largely religious phenomenon.
Then, meaning God does not want us to do this.
AI is an abomination of God.
It will sound something like that.
Then you've got a brave new world where people are just drugged out.
They realize, life is meaningless.
This is really about manipulating my neurochemistry.
That's all this ever was anyway.
I'm just going to go do a bunch of drugs, have a whole bunch of sex.
It's going to be awesome.
Then there's the fourth option, which is certainly the one that interests me the most.
We will create and/or live inside of AI-created virtual worlds, and we will essentially live video games.
The Matrix, if you will, but you're awake in the Matrix.
You are Neo.
You are not Cypher for people familiar with the movie.
What do you think?
Are there any options other than those five?
Granting that kill us all may be an option, but hopefully not.
Do you see something other than those four?
Yeah, there is a few others.
So, one is, and I think we're starting to see some of it, is that people think super intelligence is God.
They start worshiping it.
It's all-knowing, all-powerful, immortal.
It has all the properties of God in traditional religions.
Another option, and it's kind of worse than all that, is suffering risks.
For whatever reason, maybe malevolent actors, maybe something we cannot fully comprehend.
It decides to keep us around, keep us alive, but the world is hell.
It's pure torture.
And so, you kind of wish for existential problems.
That would be a pretty rough place to be.
Okay, when you look out at those, which of the options do you find the most interesting?
So, I did publish a paper on personal virtual universes, kind of solution to the alignment problem where I don't have to negotiate with 8 billion other people about what is good.
Everyone gets a personal virtual world supported by super intelligence as a substrate, and then you decide what happens in it.
You can make it very easy and fun, you can make it challenging and exciting, you decide, and you can always change, you can always visit other people's virtual worlds if they let you.
So, basically, there is no anything which is no longer accessible to you.
There is no shortage on waterfront properties, there is no shortage on beautiful people, all of that can be simulated.
When you start thinking about the simulation, I know one thing that you've done exploration on is the simulation hypothesis.
Are we in a simulation right now?
What are your thoughts on that?
It seems very likely.
Again, using the same arguments, if we create advanced AI, maybe with conscious capabilities like humans are, if we figure out how to make believable virtual realities, adding those two technologies together basically guarantees that people will run a lot of games or simulations or experiments with agents just like me and you, conscious agents, populating virtual worlds.
And statistically, the number of such simulated worlds will greatly exceed the one and only physical world.
So if there is no difference between a simulated you and real, then statistically, you're more likely to be in one of those simulated worlds.
Okay, that makes a lot of sense.
Now, given the likelihood that we will, we're obviously showing that we will pursue artificial superintelligence.
If I take your same logic from the fact that we're likely to be in a simulation because we know we would make a simulation because we're doing it right now, and therefore you get into the point where you would just make billions of those.
And so if you have a one in a billion chance of being inside of a simulation, you're effectively guaranteed to be in one now because there would just be so many of these things running.
Doesn't it also then make sense that the matrix was effectively a documentary and we are inside of a simulation created by artificial superintelligence designed to mollify us if we ever had a physical body in the first place?
So it's hard to tell from inside of a simulation, what it is all about.
You really need access to outside.
It could be entertainment, it could be testing, it could be some sort of scientific research.
If we look at the time we actually find ourselves in, we are about to create new worlds, virtual realities.
We are about to create new intelligent species, AI.
There is a lot of kind of meta-inventions we are right about to make.
And so, if someone was interested in studying how civilizations go through that stage, how do they control these technologies or fail to control them?
That's the most interesting time to run.
You're not going to run dark ages.
There is not as much happening.
It's less interesting.
But this seems to be like a meta-interesting state to be in.
It's hard to tell because we're inside the simulation, but you're saying it's a little bit suspect that we're living in the most interesting time ever.
Yes, and I think it's interesting not just because I'm living in it, but objectively, it's a time of meta-invention.
You can go back through history and say, oh, here they invented fire, here they invented a wheel.
That's all great, but those are just inventions.
They are not meta-inventions.
Whereas now we're doing something godlike.
We are creating new worlds.
We are creating new beings.
And that's something we have never done before.
Do you ever think like a sci-fi writer?
So I think the difference between science fiction and science used to be maybe 200 years.
They wrote about travel to the moon, they wrote about kind of internet and computers, and it took hundreds of years to get there.
And then it was like, I don't know, 20 years.
And now I think science fiction and science are like a year away.
The moment somebody writes something, it already exists.
And there is really no new science fiction ideas where it's like completely novel technology not previously described, or someone already working on it if physics allows it.
That's really interesting, especially when you think about writing now for true science fiction in terms of what will become possible in the future is effectively impossible because you're talking about super intelligence.
And good luck as a person locked in your not super intelligence to actually describe that.
The reason that I ask, though, is when I start thinking about things like that, like why would we run this simulation?
What clues are in, like if this is a simulation, what clues are in it?
So, for instance, the whole Christian idea for sure, and there might be more religions that have the same idea, but that man is made in God's image.
Okay, well, if God is the 13-year-old running the simulation, or Sarah Connor, or I guess John Connor running the simulation, trying to figure out why we created Skynet and what we can do to nudge it off course, you know, you think of them as sort of moving from radioactive rubble to radioactive rubble, trying to like find an answer to this and spinning up a simulation to get that answer.
That to me becomes very intriguing in terms of hypothesizing as to why this moment, why are we the way that we are, what can we learn about the people trying to simulate us?
When I ask questions like that of engineers such as yourself, there's almost a, I don't have time to think like a sci-fi writer vibe.
Is it just that you're you don't find that interesting?
You don't find it revelatory?
Why do you eschew that?
Because in interviews, I've seen people ask you time and time again, like, how would AI kill us?
And the answer is always some variant of, listen, you're asking me how I would kill us, which is not interesting because the super intelligence is going to.
But I find that's the cathartic thing that people want.
Like they want to, like, when you have a wound, you kind of want to poke at it.
Like, they want to get a sense of what would this really look like.
And so, even though it's not literally true, it's deeply cathartic to explore the known possibility set or what humans can know.
And this is exactly why I refuse to answer.
I want to make sure what I tell them is true.
I don't want to lie to them.
If squirrels were trying to figure out what humans can do to them, and one of the squirrels was saying, Well, they'll throw knots at us or something like that, it would be a meaningless BS story.
There is no benefit in it.
The whole point I'm trying to make is that you cannot predict what a smarter agent will do.
You cannot comprehend the reasons for why it's doing it.
And that's where the danger comes from.
We cannot anticipate it.
We cannot prepare for it.
I do think the singularity point is where science fiction and science become the same.
The moment something is conceived, we have super intelligent systems capable of developing it and producing it immediately.
It's no longer 200 years away, it's reality.
And you can't see beyond that event horizon.
You cannot predict what's going to happen afterwards.
And with science fiction, you cannot write meaningful, believable science fiction with a super intelligent character in it because you are not.
All right, let's ground things then in what we can predict and we can know right now.
Something that's on everybody's mind, and I've been talking about this in my own content, is the labor market seems to be softening.
You've got places like Amazon that are just cutting jobs like crazy and just saying outright, this is largely because of optimizations that we're able to make because of AI.
How does this transition play out?
Like, even if you concede that a non-destructive AI would give us essentially an age of abundance, we're still going to go through a transition period where our jobs go away, et cetera, et cetera.
What are the steps that you see happening in the labor market?
So, as we have more and more increased percentage of populace unemployed, hopefully, there's going to be enough common sense from the governments to prevent revolutions and wars to provide for the people who lost their jobs and probably cannot be retrained for any new jobs.
So, once you hit 20, 30, 40% unemployment, that's where it's really going to get in.
The only source of wealth at that point is the large corporations making robots, making AI, deploying them, all the trillion-dollar club members essentially at this point.
You need to tax them and use those funds to support the unemployed.
That's the only way to really make sure the financial part of that problem is taken care of.
What remains is the meaning: what do you do with all this free time and millions of people who have it?
Traditional ways of spending your time to relax, you go for a hike in a park.
Well, there is a million people in that park right now hiking.
That kind of changes how peaceful it is and how relaxing.
So, we need to accommodate not just change in financial reality, but also change in free time and capabilities of supporting that many people with that much free time.
I have as much pessimism around our ability to do that well as you have our likelihood of surviving.
So I'll say 99.99% chance that the government completely messes that up.
I think the transitionary period will be violent.
When you look out at this, knowing what you know about humans and governments, what odds do you give it that that's a smooth transition?
It's very likely to continue to be as history always been.
We had many revolutions, many wars, a lot of violence.
That's why we hear stories about people who can afford it building bunkers, securing resources, because they anticipate a certain degree of unrest.
Absolutely.
What degree of unrest do you anticipate?
Really depends on the percentage of population which quickly gets unemployed.
If it's a gradual process, we can kind of learn and adopt and provide safety net.
If over a course of weeks, months, we're losing 10, 20, 30% of jobs, that's a very different situation.
I can't imagine a scenario where jobs would be lost that quickly.
To your point, we've already created, you said billions or even trillions of dollars of value in the technology, but it hasn't been deployed yet.
An example you often use is the video phone invented in the 70s, but not really adopted largely because of infrastructure, I would say, until the whatever 2011, where that starts to really gain in popularity.
So I have a feeling like just the deploying of all this stuff is going to take time.
So, in a world where an unimaginable amount of people, which I'll clock at in the U.S., call it six or seven million people lose their jobs in the next five years.
That I would consider fast and just horrifyingly destructive.
One, does that feel plausible to you in terms of numbers and timeline?
And two, in that scenario, how distressing do you think that transition will be?
It seems very likely.
So, take self-driving cars.
I think we are very close to having full self-driving without supervision.
The moment that happens, you have no reason to hire a commercial driver, right?
All the truck drivers, all the Ubers, all of that gets automated as quickly as they can produce those systems.
And I think Tesla is ready to scale production of their cars to exactly that scenario.
So, what is it, six million drivers in a country?
I don't know the actual numbers, but that would be exactly what you're describing.
And it's very unlikely that they can be quickly retrained for something which is also not going away.
Okay, so in that scenario, what do you want to see happen other than heard on the Tesla as one example will be hoovering up value?
So, we're going to tax the life out of them.
We're going to redistribute that to other people.
But, what do you want to see from a regulatory perspective?
Would you like to see the government stop that from happening?
Where they say, I don't care that the technology exists, you can't do it.
So, my biggest concern is, of course, superintelligence and existential risks.
That's where I'm putting all my effort.
And regulating employment in specific industries is not something I'm too concerned about.
I think it will happen no matter what.
I think you cannot make it illegal to have efficient factories, efficient delivery systems, logistics.
It's just commercially too important.
And it may be a good thing for the economy.
Again, with driving specifically, I think something like 100,000 people die in car accidents every year.
If we can get that number to zero or close to that, that's a huge improvement for everyone.
So that specific scenario, as long as no one's starving as a result of that, I think it's a good thing for humanity.
We can readjust economic deployment, and at least that part of it is not a big concern for me.
Okay.
And when you map out how we go through that transition well, tax, cool.
So right now it sounds like you're just trying to make sure that wealth doesn't accumulate into the hands of too few, that we keep it distributed so we can keep using the same system that we're using now.
When I look into the future, that strikes me as the least likely scenario to play out.
I think that AI is going to so radically alter the cost of labor and energy that that becomes nonsensical.
Do you want to see any group rise up in the way that you and other AI safety people have risen up that will rise up and start giving either policy prescriptions or at least philosophical approaches to how we migrate to an age of abundance where food is effectively free, labor in your house is effectively free?
So people talk about those things and conditional basic income is one and conditional basic assets is another.
Basically, just because you're a real human, you deserve certain things.
And historically, all these communist ideas were complete nonsense and caused a lot of harm.
But if you're taxing AI and robots, all of a sudden it becomes workable.
I'm not against accumulation of wealth at the top.
If you invented something amazing and you started a company, you should have a lot of money.
But there is so much wealth that we can provide for everyone, as you said, complete abundance of basic needs.
Some people say maybe not just basic, but above average set of needs.
I think Elon is known for suggesting that's going to be the case.
The ideas exist.
Now, will we pass this?
Will governments actually adopt it before it's too late?
It's a different question.
Yeah, so on the existential side, I don't think there's any hope whatsoever that you get people to pump the brakes.
I think you're far more likely to get people to pump the brakes on, no, you can't have self-driving cars, or they'll try to regulate that to death.
They'll tie it up in litigation, whatever, and that'll slow it down.
We couldn't stop nuclear weapons from proliferating because, and I don't know who came up with this, but this seems very true to me, that effectively game theory says any technology that promises an advantage will in fact be developed because if you don't, somebody else is going to.
At a minimum, you've got the US versus China of it all, where you, I mean, regulators are saying this right now.
We can't stop because if we do, China will plow forward, which by the way, I'm very firmly in that camp.
What do you think about that?
Do you think that game theory is inevitable, or do you see a mechanism by which we can convince people that they have to slow down?
I agree with game theoretic approaches, but I see the exact opposite argument.
I see that arguing against self-driving cars is a hard argument.
What are you trying to preserve?
We're going to have safer drivers, cheaper drivers, helps logistics, helps economy.
It's a pure benefit.
Whereas uncontrolled superintelligence kills everyone.
It's a very hard one to sell.
If you are a leader in that field, you are rich, successful, you are generating something which will destroy you personally.
So to me, that's a much easier argument to sell.
The moment they understand dangers of superintelligence and benefits of narrow self-driving AI, it's an easy game theoretic sell for me.
Yeah, the problem is you're stuck inside of a simulation of the hyper intelligent.
And I mourn for you looking back at the rest of us stuck in normal land because I don't think so as I got into learning about the economy and trying to explain it to people, I realized that even though I can walk you through the cause and effect of why socialism doesn't work, that it feels right, it sounds good, and so people keep doing it.
And even in a moment right now where the very thing that is creating everyone, like literally everyone's problems is money printing, people are going to vote for policies that dramatically increase the amount of money that we print.
And so I have developed a level of hopelessness around being able to convince people because the economy is too complicated for people either.
Some of them just don't have the intellect to understand it.
And then let's say they have the intellect, but they don't have the time or the inclination.
And so forgive me for painting you with my brush of despair.
But when I looked at your signup, there was like less than 20,000 signatures.
So less than 20,000 people are worried about the death of everyone.
So it's like, that's big.
But I think that because I can whip people into an emotional frenzy by saying by allowing there to be autonomous driving, you're just making that evil bastard Elon richer and you're robbing these people of dignity.
If you, that is not my argument.
I want to be abundantly clear.
But when I look at, if I had a gun to my head and I had to convince people of one of two things, rich people are evil and trying to exploit poor people who are far morally superior, or, hey, this abstract thing that you don't really understand is going to kill us all.
There's no way I take the, they're going to kill us all bet.
I'm going to be over here emotional.
You get it.
I'm going to bang tables and yell and say words really loudly and point to evil rich people.
Guaranteed, I can get people excited about that.
Luckily, we don't have a democracy on this issue.
We don't have to convince the majority of human population.
We have to literally convince the 20,000 elites who control those companies who are also super smart and understand dangers of safety.
It's literally people who publish on it, who have spoken, they have very high PDO.
We know Elon is like 20, 30%.
Sam Altman is on record as being very concerned about it, destroying humanity.
So we're trying to convince people who already believe the arguments to kind of slow down and preserve their elite status.
That should be an easy sell.
I'm not trying to convince a random farmer to stop developing superintelligence.
So, why do you think that Elon, who was banging the drum harder than anybody, lobbying Congress, desperately trying to get them to slow down, suddenly hit a point where he was like, Well, I guess I'll just build it faster than anybody else?
He likened AI to a demon summoning circle and laughed at everybody who thought, Yeah, yeah, yeah, I'll summon a demon and then I'll be able to control it.
All is going to be well.
Like, he sees the problem clearly.
But after years of trying to slow this down, he finally completely abandoned that and went to, I'll just build it faster than anybody else.
What happened there, and why do you think you can reverse it?
So, I think he realized he's not succeeding at his initial approach of convincing him not to do it.
And so, the second step in that plan would be to become the leader in a field and convince them from a position of leadership and control of the more advanced technology.
If the leader says, you know, we're going to slow down and it's fine for you to slow down, it's easier to negotiate that deal with, let's say, top seven companies than if you are not even part of a game, you have no AI, you are nobody in that space.
So, all of them as a group benefit more if they agree to slow down or stop than if they just arms race and the first one to get there gets everyone destroyed.
He says words along those lines or did for a while.
I think he even signed one of the letters about we should pump the brakes, but none of his actions indicate that that's actually what he plans to do.
Um, from just trying to take advantage of every company that he's building, from the amount of data that Tesla cars capture visually to all the decisions that drivers are currently making, to all of the decisions that the AI will make, to now he's talking about using the cars as a distributed fleet so that when they're idle, that they're actually running inference models.
And so using it as a gigantic AI brain to, well, maybe that won't work.
So I'm going to do Neuralink and I'm going to jack into the AI myself and I'm going to make myself smarter.
And hey, if all of that fails, don't worry, I'm going to get us to Mars.
So if we destroy planet Earth or the AI takes over, like we're going to be over there.
Like this is a guy that's really covering his bases.
He is not somebody who's acting like he expects us to slow down.
To me, he is acting like somebody who crossed that bridge a long time ago and is just like, yep, that's not going to work.
People are not going to be convinced.
And so we've got to build a whole bunch of other strategies.
Some are lifeboats and some are just, I'll outsmart the AI myself by merging with technology.
It is very disappointing to see this level of progress in AI from anyone who is capable of doing it.
It's definitely not a good strategy for humanity as a whole.
It generates this mutually assured destruction.
It doesn't matter who creates uncontrolled superintelligence.
It could be open AI, could be Elan, could be Chinese.
It makes absolutely no difference if it's uncontrolled.
All right.
Talk to me about that.
So, this was for a long time, I was really banging the drum of, well, whoever gets to artificial superintelligence first is going to win.
You were the first person that really hit me with the it won't be theirs the second it becomes super intelligent.
Walk people through the truth of that statement.
Right.
So people talk about short-term advantage, for example, military advantage.
Whoever has the best drones right now, the best AI navigation has military supremacy.
So China, Russia, US, all competing in that domain, trying to have that so they have better military for obvious reasons.
The moment you switch from those AI-assistive tools to agents, to superintelligence, which is smarter, more capable, in the absence of control mechanisms, you just have a separate entity, an AI, which has nothing to do with you, your country, your company.
It makes its own decisions, and it doesn't matter who birthed it.
At the end of the day, none of us control it.
None of us can claim it as doing our bidding.
So if it decides to wipe us out, it's not going to go, oh, I like this group of people, I don't like this group.
We look the same to it exactly.
I don't think it's going to make a difference where you were at the time someone else created super intelligence.
Okay, if you're right about that, and it is a distressingly compelling argument.
If you're right about that, there was a guy, I'm sure you've heard of him, Ted Kaczynski, the Unibomber.
He looked at the university system and he said, you guys are getting rid of all of the sweet spot problems.
And humans are designed to find these things that are just challenging enough.
And when they solve them, it feels very good.
And if we solve all of that, we're basically going to rob humans of meaning and purpose.
Most problems will either be way too hard or way too easy.
And so I am, Ted Kaczynski, going to bomb university professors, kill them, and try to stunt the growth of the academy.
Now, if you are right, and as we race towards artificial superintelligence, it runs the risk of P-Doom of 99.99%.
Do we have a moral obligation when a certain line is crossed to bomb data centers?
So that's a very difficult question.
And part of it is, again, the example you brought up with Ted Kaczynski.
He tried that approach and it failed miserably, right?
He didn't succeed in slowing down technology at all.
So clearly, it doesn't work.
We saw examples of, for example, a CEO of a top company being replaced, even if temporarily.
It made no difference.
Someone else comes along, they continue the same scalability research.
So taking out an individual person, an individual data center makes no difference if you zoom out and see the overall pattern of what we are doing.
Maybe it will take an extra month or so, but exactly the same thing will continue being developed.
The idea that the scalability hypothesis works, it's already out there.
You cannot put it back in a box.
And so I'm strongly against all those methods.
Okay.
Well, the really bad news is I think you just put a nail in your own coffin of being able to convince people to do this.
It looks like this, and hopefully you can prove me I'm wrong.
But you have said, hey, here's why everybody is so silly that thinks that they're ever going to make this safe.
You would have to build a perpetual safety machine.
And that perpetual safety machine can't ever miss because the one second it creates even a slight vulnerability for this artificial superintelligence that can think at the speed of light, it will escape and it will do its own thing.
What you're proposing is a perpetual demotivation machine for the 20,000 people capable of doing this.
But every day there's going to be a new kid that's bright enough to do this and you can't miss one of them.
So, how on earth do you expect to perpetually demotivate the 20,000 people that are capable of continuing to push this thing forward when, as of right now, a very small number of those people seem demotivated?
I don't.
That's why my P doom is 99.9999.
I exactly think it's not going to happen.
I'm doing everything I can, but I think the best we can achieve is to buy us some time.
Okay, so let me ask the really naked question: Do you believe humans are automata, or do you believe that we actually have free will?
So, there is good research by Stephen Wolfram on cellular automata.
And interestingly, there is a bit of a hybrid answer here.
Just because a system is fully following rules, fully deterministic, it doesn't mean that you can predict future states of that system.
You still have to run it to find out what it does.
And I think we are kind of like that.
So, yes, you're following laws of physics.
If we fully understood every molecule, every atom in your body, we would be able to trace it and know exactly what you're going to do.
But the only way to do it is to live your life and run that algorithm to completion.
No one can short-circuit it and predict what you're going to do in the future, which would be a violation of your free will.
Okay, you've argued against that.
So, there's two pieces of things that you've said that I think make that untrue.
Piece number one, we're probably in a simulation.
Piece number two: we can speed up that simulation.
So, I could, since you're deterministic, go, I'm just going to play this out at a thousand X.
So I get an answer to what you're going to do for the next 50 years in like the blink of an eye.
And now I know.
Also, I don't find any freedom in, I'm deterministic.
I don't know what I'm going to do next, but I'm still deterministic.
I don't know that it buys us anything.
And I'll explain why I'm bringing all this up in a second.
I don't think it buys us anything if we are completely deterministic, just unknowable.
The reason that I think that this matters and that I'm bringing it up now is I don't, I think, I think we are automata.
I think we are entirely deterministic.
I don't live my life like that.
It's not an interesting frame from which to live my life.
So no one's ever going to hear me talk about my depression based on that because I just don't even think about it.
It's not, that isn't how it feels.
So even if it's true, thankfully, it doesn't feel like that.
But when we come to moments like this, I'm so fatalistic because I don't think the way the human mind works is compatible with slowing down.
And given it's not going to happen.
That's the example you bring up where you run the simulation at a faster speed.
That's you living out our lives.
Internally, from inside the simulation, it doesn't seem any faster.
We're just going on as before.
So we're still playing out fully what we're going to do step by step.
There is no shortcut.
If you now run it the second time around, you know it's going to give you the same results.
So I don't know why you would run the same simulation multiple times.
It doesn't give you any extra data.
Yeah, no, I wasn't, if I said run it multiple times, my apologies.
I was just saying that given that you could get ahead of it from outside the simulation, it is of no emotional consequence to me that I don't know the next step.
It is knowable.
It is predetermined.
It just isn't knowable by me.
And that doesn't, so I get no emotional alleviation from suffering if I were a person who was traumatized by the fact that I am an automata with no free will, which I am not.
But if I were, eh, it doesn't help me at all.
And again, the reason I'm bringing that up is when I talk to you, I think, oh man, this is somebody, he really can't stop himself.
Like you're wired to rail against this, to play the role in the grand balancing of the human species of like, hey, this is really a problem.
We should slow down.
And even though it's not getting you anywhere from where I can see, you're going to keep doing it because you have like a moral compunction or something where you're like, I, as the kind of person I am, I simply cannot exist and not try everything I can to stop this, which I relate to because I am the same.
Economically, I've become obsessed.
I am really, really desperate to get people to understand that we are marching ourselves off a cliff.
And even though when I articulate it to people, I'm like, this is never going to stop.
We are going to march off the cliff.
I can't stop myself.
I still feel like this moral compunction to scream from the rooftops that we are making this mistake.
And I've already won the game.
Like I'm already rich.
So, barring like an inability to flee, I'm not going to get caught up in it.
Uh, but nonetheless, for whatever weird roll of the dice, I can't stop myself.
Like, once I saw the problem, I'm like, uh, I just have to keep yelling about it.
Um, but I do feel a simultaneous futility and inability to stop.
I would love to claim pure altruistic motives and trying to save humanity, but I am within the simulation with you, so it's pure self-interest.
I don't want creating technology which will kill me, my family, my friends, my life, everything I know.
So, I'm going to talk about it for very selfish reasons.
Yeah, yeah, it's so interesting, man.
So, how do you get through the day?
Like, what is your coping mechanism?
I enjoy research.
I want to understand what are the exact limits and control.
When I started, I thought it is a solvable problem.
Now, I'm a lot more skeptical, obviously, but I still feel there is a lot we can do to make even narrow AI tools we're creating safer.
There is never 100% safety guarantee, but if I can increase safety 100fold, that is something.
And again, public outreach: if there is enough people who all agree as a scientific community, it's a consensus that no, you cannot ever create safe superintelligence.
Maybe it makes a difference.
Maybe we'll delay it by a decade.
That's something.
Okay, so we've got one piece of how we make it safer on the table, keep it narrow.
What are some of the other things you would consider a big win?
So, there are quite a few properties of control we want to be able to have.
I call them tools of control.
So, our ability to test those systems, explain how they work, predict their behaviors, monitor them, all that is still in a state of investigation.
We're starting to see some upper limits on what's possible, especially with advanced systems, but there is still so much room for improvement.
Explainability, for example.
We started with being able to understand maybe a single neuron.
Now we're up to small clusters.
Okay, then this input is presented, this lights up, kind of with like neuroscience.
We don't fully understand the human brain, but we know this is vision area, this is hearing, and so on.
So, there is a lot of room for progress in that.
I don't think we'll ever fully comprehend a complex, super intelligent neural network model, but we can do better than what we have right now.
And so, I think as a safety researcher, that's what I'm doing.
That's my job.
Okay, so basically, the model is we need to come to understand it better.
We're never going to get totally there, but we need to understand it better, keep checks and balances on it.
So, when we find a problem, what's the action you take?
Is it to apply an evolutionary force on it, a selective force, or kill it off?
Like, what's the move at that point?
So, it depends on the problem, depends on specifics.
Some things we know how to address.
So, trivially, then we started with language models.
If it says the wrong word, you can filter it out, you can punish it for using that word.
So, there are simple things we know how to do.
The hard problem is: how do you change overall internal states of a model?
Not just the filtered output, but how do you make it so the model itself has certain preferences and aligns with certain values?
Do we have a guess on that?
Not a very good one, not really.
So, nobody at this point knows how to align systems other than this after the fact, putting lipstick on a pig, filtering it, censoring it.
Yeah, that's unfortunately the state of the art.
Okay, and what parallels are being drawn between the evolutionary evolution of species and the evolution of algorithms?
So, there was a lot of attempts to evolve intelligent software.
We started with genetic algorithms, genetic programming was tried, simply evolving agents, evolving environments.
It doesn't seem to be a dominating algorithm in comparison to what is typically used for training neural networks, but there is this possibility.
The problem is that evolution is even less controllable in terms of explicit engineering design.
We're kind of setting it up and see what evolves and then trying to test it, to monitor, to understand what happened.
So, while it is a set of tools we have, it's probably not leading to safer systems.
Okay, interesting.
Because we cannot control the outcome, so we don't know what stimulus we're going to have to give it.
Why does that strikes me as so unsatisfying?
Okay, why did it work so well in humans and it works so poorly in artificial superintelligence?
I disagree that it worked well in humans.
Humans basically are as well behaved as they can get away with.
You're just not powerful enough to really do the things you want.
If you had absolute freedom from punishment, you'd do horrible things.
But then, that's what nature is giving you the answer.
Nature is saying these have to be in balance, they have to be competing systems.
And without ecosystems, without competition, you'll get these things that run amok.
But I don't see anybody taking that lesson and applying it to AI.
Yeah, I've seen creating a society of superintelligences competing with each other and humanity has collateral damage.
Is that why they're not doing it?
I get that's why you would hate it, but is that why they're not doing it?
That seems unlikely.
There is also a continuation of self-improvement process.
Superintelligence is not a fixed point.
There is superintelligence which creates the next level, superintelligence 2.0, 3.0, and they all have the same control and alignment problem.
They all worried about the next level of AI, not wanting the same things, not caring about them personally.
So this is an ongoing self-improvement curve, and there is no upper limit we can see.
There are obvious physical limits to what can be done in a physical universe, but it's so far away from us that it's almost infinity from our point of view.
When I look at humans and when I may be making either a category error or I may have a foundational base assumption that's leading me astray, but when I look at what made humans work on a long time scale, is evolution itself had survival as like a North Star.
So you have to survive and replicate.
At whatever point, way back, evolution decided I'm going to do this through sexual replication and I'm going to make sure that this creature dies off.
I think there are reasons for that, which we'll get to when we get to longevity.
But I wanted to survive, but I wanted to survive by mating and having offspring that carry certainly immune system blends so that it's less vulnerable to a single point of failure.
And it realized, okay, if I'm going to do that, then this needs to be a species that both cooperates and competes, which means no one of them is the answer to the question of how to best survive.
It's the whole species.
And when I look at even things like the left and the right politically, the way that I make sense of that is I say to myself, okay, I get from an evolutionary perspective, evolution had to be like, oh, hey, we have to cooperate.
There's no refrigeration.
So I'm going to store calories on your body that I may need to take later versus being able to put it in a refrigerator.
And by that, I don't mean that I'm going to eat you.
I mean when I'm the one that's successfully hunting, I let you eat.
You're alive so that you can now hunt next time when I fail or I'm sick or whatever.
And then you're going to bring me back, which means that some people are going to be very cooperative by nature.
And so their win state is cooperation to the point where a parent will easily lay its life down for its child.
So that is just baked into our success criteria.
So evolution was able to bury something deep inside of us through its evolutionary selective pressures where we will lay our lives down and we break into the right left.
So, let me finish that.
So, people on the left, very compassionate, very pro.
I'm going to store a whole bunch of calories on your body because it may come back to help me at some point.
The right is very much, well, a parasite develops when you do that.
And so, you get the freeloader problem.
And so, now, if you've got people that will just take care, take care, take care, there are people that are like, cool, I'll just be taken care of, and I'm never going to go hunt, and I'm never going to contribute to the group.
And so, you need people that have the opposite impulse who are like, Hey, you're going to pull your weight or you're going to be ostracized or killed.
And so, now, in the dynamic tension between the wants and desires of the win state defined by people with a left-leaning personality, versus the wants and desires of the win state defined by the people with a right-leaning personality, you get something that's dynamic tension.
Like, balance may not even be the right way to think about it.
It's dynamic tension.
They're both pulling in their direction, but they keep each other in check because that's how we've evolved is to work together.
That feels like it should be applicable to AI if we want to embed deeply in its motivational structure, that we have to put it through that.
And if I'm thinking from a safety perspective, I get why we want to short-circuit that, and maybe that's not super efficient.
But if that, if the only way to get this to find a dynamic tension or some sort of balance is to have things that are of similar intellect and ability that are pulling in slightly different directions, but they need each other somehow to stay locked together so that it is the AI taken as a whole, that stops itself from ever going wrong in any one direction too far.
So, I think it works for humans because we're about equal power and we are mutually benefiting each other.
There is a certain symbiosis, as you described.
In a world with superintelligence in it, you don't really have anything to contribute to superintelligence.
So when people propose creating hybrid systems, human and superintelligence together, I never understood what the human biological bottleneck is contributing.
It's slow, it's inefficient, it's not competitive in any way.
So I'm questioning this setup.
If you have superintelligences separate from humans and now they decide what to do, they may still come up with something completely unfriendly and incompatible with human life.
Maybe they want to lower the temperature of a planet to improve processor speeds in server rooms.
I have no idea what they decide, but the point is, while they align with our values, we're contributing nothing to their future states.
With humans, we also have examples where the moment you give more power to an individual human, they get corrupt.
Basically, a guaranteed state.
Very few people can exist corruption at very high levels.
You have enough money, enough guaranteed tenured power, you become a very evil person, as we see with many dictators and so on.
Even basic evolutionary drive, like reproduction, you brought up this example.
We use condoms.
We literally hacked the only thing that nature set up us to do.
Yeah.
Yeah.
All right.
I'll state my hypothesis as plainly as I can.
I think you just refuted it, but my hypothesis plainly stated is the only way to build checks and balances into AI is to give it evolutionary rewards and punishments all through its development cycle that make it care about the survival and emotional thriving of humans.
But to define those terms in a way you're not going to regret is very, very difficult.
So survival of humans, what does that mean?
We're cryo-preserved in some safe emotional states.
Are you on drugs all the time?
Is your brain modified to keep you in an always happy state?
All those things can be gamed.
The moment you tell me, this is what I want, and there is a famous paper about making smiles for humans, make people smile.
There are a billion ways I can make you smile, but none of them is what you really want.
Right.
But do you really think a super intelligence would be so dumb as to confuse that intention?
Like, wouldn't it be able to get to a rough approximation of what we're really going for?
I mean, which is admittedly a neurochemical state.
But if you derive, like if you said it is the following band of neurochemical states that must be derived through their own programmatically directed actions.
Like I don't need it to believe that we're not automata.
I think we clearly are.
But it's like you can't just manipulate it exogenously.
It's got to come from within.
No matter how detailed you make this specific description, a super intelligent lawyer will find a way to game it to make it more efficient to satisfy those requirements.
Basically, you're setting it up to where the system is now in adversarial relationship with this equation.
Okay, you mentioned I have to use natural chemicals.
Okay, I'll generate a super stimulus.
Okay, whatever.
Point is, if we could do this, if we could get AI to do what we meant, assuming we were smarter and understood the problem better, we would solve the control problem.
That's the hard part.
I don't think we can, at our level of intelligence, specify what a system with hypothetical IQ of millions of points should be doing at any possible decision-making point.
All right, let me give you an exit ramp that I'll be curious to see if this shaves a 0.9 off your P doom or not.
So, if I'm a super intelligent AI, one form of manipulation that I would pull on humans would be to put them inside of a simulation.
And whether that's a physical body and I help them jack in and I just socially engineer them to want to do it, and then I get them in.
And I really do just like in the Matrix, the machines build a world that's sort of optimally difficult where there is challenge, there's pushback, you're striving to get better.
I'm going for balance.
I don't expect any one person to avoid suffering and all that.
And maybe that's where we are, and the machines are just cruel enough that they're like, haha, I'll let it be, you know, like a two-year-old can die of leukemia very painfully.
That kind of thing where we don't cease to exist.
It's not even sort of broadly worse than where we're at already.
That seems for a super intelligence, it certainly seems like that would be on the menu.
A just shared hallucination.
So it's more likely, I think, that super intelligent agents think in such a level of detail and realism that, as a process of thinking about certain problems, they generate within them agents, virtual worlds, simulations of the scenario.
So if maybe they're trying to think, how can we safely generate super intelligent systems?
What is the process?
Well, let me think about humanity, all the AI labs, all the hardware they design, and this process of them thinking about it is the simulation we find ourselves in.
That's so wild.
Okay.
Incredibly important, incredibly fascinating.
But now let's talk about another very important thing that I think you have some pretty deep interest in, which is longevity.
So, one, there are some people that will argue very compellingly that there's just a biological upper limit of somewhere around 120 years, that there's no escaping that.
Do you think that's true, or do you think that we'll be able to engineer living tissue to live forever?
Well, the current body has that limit for sure, but we can modify our genome.
There is nothing preventing us.
No law of physics says you cannot make changes to it.
And we see examples with other systems, computers, cars.
I can keep replacing parts indefinitely.
It's going to function as the same computer.
Maybe the monitor dies, I'll get a new monitor.
So if you can rejuvenate all the organs, including your brain, then there is no reason to think you have to stop existing.
There is, of course, other methods, you know, uploading, scanning your brain, cryopreservation for future technology, but even the basic idea of just modifying your genome.
Okay, what do you think is the most likely path forward?
Is it going to be genomic modification?
Is it going to be.
I think so.
I think there is somewhere in our code a limit on how many times cells rejuvenate, and we just need to increase that number without causing cancer.
Now, do you think that the limit on that is simply a cancer prevention tool, or do you think that there's another agenda that evolution had to make sure that we self-destruct?
There could be evolutionary reasons for taking out one generation and replacing it if resources are limited and you want to keep adopting and improving.
You only have so many agents in a population at any given time, so older ones have to die out.
It's kind of theoretical conclusion, not guaranteed, but seems likely.
From a point of view of evolution, you are the same organism, right?
The same lineage of cells passes through.
So while as an individual, you die, your biological chain of existence continues.
It's interesting.
So here's the way that I've always considered like if I were to personify evolution instead of the blind watchmaker that it actually is, if I were going to personify evolution, it would go something like this.
Okay, the world is constantly changing.
Your access to resources is changing.
Who knows?
Weather moves in cycles, everything, everything.
So I'm going to have you born.
I'm going to extend your brain development for a very long time.
You're going to go through these phases where basically, okay, learn from your parents, like whatever there is to learn just about generally being a human.
Then you're going to push away from your parents and you're going to learn very, and the reason you have to push away from your parents is their thinking will have calcified.
So you now need to push away from them, drink deeply of culture, the people roughly your age who have grown up in a different milieu than your parents grew up in.
So they all think differently.
This is a whole idea of generations, cohorts that sort of think alike and have a similar frame of reference and all that.
And you do that.
And this is really a brain development period known as the age of imprinting.
It's roughly 11 to 15.
And so now you're going to take the this moment-specific like cues of, okay, is this in a time of abundance, a time of warfare?
Like, what is it?
You're going to solidify around that.
And then you're going to start optimizing like crazy.
And you're going to start pruning all the excess connections.
If you're not using it, you lose it, all of that.
And then your brain's going to roughly wrap up its rapid development at 25, but it's been sort of a diminishing curve after 15.
And now you're like baked.
And this is just a game of like learn what things work really well in your environment.
Optimize, optimize, optimize.
And so now your thinking is going to calcify.
So very good strategy on behalf of our blind watchmaker.
But just as I think it was Niels Bohr that said this, it was either him or Plank, I can never remember.
Science does not advance one insight at a time, it advances one funeral at a time because people just become convinced they've bet their whole reputation on something.
And so they're just not going to be convinced that they're wrong.
And so they don't adopt new ideas as they get older.
And so as evolution, I'm like, yeah, I'm also going to put a self-destruct mechanism in here.
Most of you are going to die long before this point.
But if any of you psychopaths get to about 125, you got to go.
That makes sense to me to make sure that we never stagnate, to make sure that, as the saying goes, it is not the strongest of the species that survive, nor the most intelligent, but rather the most adaptive to change.
That the individual needs to be adaptive, but so does the species as a whole.
And without, at least with the current structure of the human mind, without killing us off, we do not have that species-level adaptation.
Do you feel I'm missing something?
I think it would be easier and more efficient to simply make you still capable of learning and adapting as you get older.
And also, you wouldn't have to relearn everything for the first 20 years, including language and how to walk.
We know that it's possible to encode those capabilities.
Animals are born and immediately they can run, they can speak.
So, all those things are doable.
Why are we losing 20 years of information every generation?
We can build on top of pre-existing knowledge.
Big data is good for intelligence, so we can have a smarter, more efficient reproduction cycle, and you still die of natural causes.
It wouldn't be complete stagnation.
But if you're smart enough to survive for 400 years, why not?
Well, my why not is entirely predicated on not having a clear understanding of how we would bake in the ability to adapt long into our old age, because you're right.
If we could stay in that novel period or at least move through cycles of extreme sort of remapping of the world, maybe that would work, and maybe we can identify where that is.
But when I think about the problems that humans create, like even now, just having a political system run by geriatrics who are so out of touch with the way that certainly the economic world actually works for young people is terrifying.
And so, the only like pressure relief valve that people have is: well, eventually they're all going to die, and then like we'll get to step into power and all of that.
And there are also problems of power because the older you are, the more likely you are to have a stable network of very other powerful people.
And so, you're able to, to your point earlier, about you need people of sort of equal power, equal intelligence, otherwise, you get what I'll call parasites in the system.
And so, older people would just become those parasites because they would have just had more years to accumulate useful knowledge, to accumulate connections.
So, it just feels like, wow, there's a lot of stuff we would have to update.
So, I want to live forever.
I don't understand anybody that doesn't.
However, I do worry that there's like a okay, cool, you can live forever, but you only get 120 years on Earth, and then you have to go like somewhere else so that there's churn of some kind in the different ecosystems so that they don't just calcify.
I think if you do live forever, at least you expect to be less likely to reproduce at a young age.
You may take your first 400, 500 years to start a family.
So, I think all this kind of expectation of 20-year generations and younger generations showing up will be modified as a result.
We're already starting to see population dynamics change in Europe, Asia, where we're not producing enough children to even maintain the population.
It's interesting.
The way that I think that will play out may be even a little bit different than that, because part of why I haven't had kids is I was like, I only get one youth where I can go hard.
I have a ton of energy.
I feel like I'm of the culture.
So I'm far more likely to build something relevant than I am as I get older.
Genius is a young man's game, as they say.
And so I don't want to be distracted by something.
I also don't want it to pull at my marriage.
So I'm like, ah, I'm going to hold off for now.
If I knew that I was going to live for 500 years, I might just be like, ah, whatever.
Let's do it now because I'd rather see, like, it only takes me a 25, 30 year investment.
And then after that, like, I get to see what they do and I get to see all my progeny and all of that.
And I'm going to have plenty of time.
You know, if my youth lasts for 250 years, it's like, yeah, word, whatever.
I'll clock the 30 years now so that I can see how big my family gets.
I think this is one where I want to think like a sci-fi writer.
It gets so interesting so fast.
It's not obvious, but I think most people procrastinate and hard work.
And so they would put it away as far as they could get away with.
There is some truth to that, to be sure.
What's a big breakthrough in longevity that you've seen that's got you really excited that this is all possible?
There are some good experiments and animal models.
Of course, we don't always scale up to human performance, but I think there is some 30, 40% increase in lifespan of mice and other lab animals.
It's hard to experiment on kind of bigger animals with longer lifespans.
It takes a very long time to see results.
But I think we're making good progress in understanding at least what might improve your health span and what changes we need to make to the genome.
We study people who already have very long lifespans and find commonalities in their genomes.
If those can be reproduced either pharmaceutically or through genetic manipulation, maybe we can all get the same at least 120.
Have you heard of the Chinese doctor?
I think his Dr.
Liu Liu.
He went to prison because he altered the genome of two twin girls.
He did human cloning.
Yes.
So he just put out a post on X like a couple days ago that said with 10 edits to the human genome, you can give birth to a child that is immune to, God, it was like five things.
Cancer, HIV.
I mean, they were like big things.
And he was like, it's only 10 edits to the genome.
Do you pay attention to his work at all?
Do you think that's ethical?
Like, what do you either get excited about or worry about there?
I'm behind on my science.
There is so much coming out, even in my domain of AI, I can't even keep up in that domain.
So I definitely don't follow details of everything.
I'm skeptical about his claim that cancer can be cured because cancer is like a thousand different conditions barely related.
We call them all cancer, but they are completely different problems.
So, unlikely to be the case.
I haven't seen the post.
Maybe he talks about a specific type, but definitely so much of it is a single mutation.
We know some people are immune to getting AIDS virus exactly because they have a single mutation.
Okay, so let's just say for a second that however many edits it is, it is possible.
Do you draw a line between germline editing where this is going to get passed on?
Like, do you have some of the same safety fears where it's like there's just too much unknown?
Where do you come down on gene editing?
It's a lot less concerning.
So, for one, if there is one human with some problem, that's it.
It's still just one human.
If we have editing tools, whatever changes we make, we can later undo them with the same editing tool.
If we've made a mistake, we can go back and rectify those problems.
So, I'm a lot less concerned because of impact.
Worst case scenarios, yeah, there are ethical implications for the individual.
Like, he was in prison for human cloning, which is considered to be problematic because it may harm the child significantly.
But humanity as a whole is not impacted directly, negatively, by that experiment.
Where's AI's intersection with this?
Is AI going to be a critical tool in terms of just mapping out all of the, like you said, the similarities at the genome level between people that live long and people that don't?
Is AI going to be doing novel protein folding and going in and solving some of the architectural problems of people that are getting sick?
Like, where is that going to interface with long gene?
All of the above.
We need to map the genome.
We need to understand what individual parts do.
We need to design novel drugs.
Protein folding has been solved, basically, but there is other things we can map on biological substrates.
So, yeah, at every aspect of it, we need AI.
But I think, as was illustrated with the protein folding problem, a narrow system can do it.
We don't need super intelligence for that.
What's something that's happening in AI right now that you don't think enough people are paying attention to?
Well, I don't know what people are paying attention to.
Usually, after my talk, the questions I get seem to be completely irrelevant to the subject of my talk.
I'll tell them that it's going to kill everyone, and they ask me if they're going to lose their jobs.
So, I don't think it's a good way to measure what is important.
But look at predictions from inside the labs.
They are starting to talk about automating the research process, creating junior scientists as AI agents, AI models.
They are saying that externally to the lab, people don't understand just how capable systems are yet.
So, there seems to be a lot of indicators that internal progress is even more impressive than what we see outside.
That's interesting.
What is the big anxiety that when you give your talks that people come up with?
Is it just, am I going to lose my job?
It is things they already know and care about dealing with other human agents.
So, algorithmic bias, technological unemployment.
Recently, with OpenAI announcing that they're going to get anti-adult material, people are now freaking out that we're going to have artificial girlfriends, all this nonsense.
You're not worried about that?
Why would I worry about someone having an artificial girlfriend?
Okay, well, let me paint the picture.
So, I never would have guessed in a million years that giving a 12-year-old access to the internet would end up being so damaging to an entire generation, but some of the studies coming out now are terrifyingly compelling.
And then there was that commercial, which just brilliantly encapsulates it.
I'm so sad that if I had kids, I don't know that I would have thought of it, where the father's like tucking his son into bed.
He's like, All right, good night.
Now be safe.
Now, remember, over in the corner is a box with all the pornography that's ever been made in the world.
Don't look at it, especially not the really harmful stuff.
And over here, there are going to be people that are trolling you and making fun of you.
You've got to ignore them.
Don't pay.
And I was like, oh my God, that's exactly what it's like to leave a kid alone with their cell phone at night if they have unfettered access to the internet and to social media.
And so, given that we've got character AI that's been sued multiple times, I think, for kids that have committed suicide after interacting with their chatbots, I can only imagine the number of people that will end up falling in love with an AI system that does not feel anything back, could turn on them, could intentionally or unintentionally manipulate them.
So, I can imagine that becoming problematic in ways that we just can't anticipate yet.
Yeah, but they're very similar to problems we had before.
How many men fell in love with women who felt nothing for them?
We all grew up on the internet with access to pornography.
It wasn't AI-generated, but we somehow survived it.
So, I think those are more of the same problems.
They're still something we should look at, but I don't think we'll all die as a result of Sam Altman having a virtual boyfriend.
What do you think of Sam Altman?
Is he the right person to have this potential godlike control in his hands?
I don't think no human is a right person to deal with that level of power.
Now, I don't think he's going to be in control, but even the stages leading us to the development of this technology already present way too much power for any individual to handle.
Were you impressed or terrified when the board tried to boot him and he ended up remaking the board and coming back?
It was fascinating to watch, but what I was observing is that it made no difference.
The company was an independent entity, and all the human components of that monster kept walking just the same.
They replaced him with a temporary CEO, they brought him back.
There was never any switch in anything, any change in direction of the company.
Now, is there a major player in the AI space that you think is doing it right?
Like Elizer Yudkowski is very focused on AI safety.
You've got the Anthropic CEO that's like banging the drum, wanting more regulation.
Do you like any of their approaches or anybody that maybe I'm not aware of?
So Eliezer does zero development.
He's purely a safety advocate.
And so I'm very happy with him because he's not developing any super intelligences.
Anyone who is is problematic.
And whatever they talk about government regulation, which is meaningless as a solution to a technical problem or anything else, they might have some internal polling showing this is good for business or good for public perception, but I don't think it makes a difference in terms of solving super intelligent safety problems.
Now, have you talked to Elizer or read anything?
Like, is he saying specifically, I have become afraid that this does something bad and therefore I'm not going to develop anymore?
He was never developing AI to begin with, other than publishing a very high-level abstraction theory for how it could be done when he was like 16.
Got it.
I thought he was actually an engineer.
As far as I know, he doesn't actually release any software into the world.
Okay.
Now, the Anthropic CEO, whose name I'm forgetting, he is being accused of going after regulatory capture, that he's not very sincere and actually trying to slow this down.
He just wants to make sure that the big players remain the big players.
When you look at the way that he's moving, does that ring true or do you think now this is somebody who's sincere about keeping us safe?
They all on record as being very concerned with safety.
In fact, all these companies started as safety companies.
OpenAI was a safety offshot of philanthropic endeavors, effective altruism, Anthropic was an offshot of that project becoming less safe.
And so all of them claimed at some point that the only reason they're doing what they're doing is to improve safety.
And then each one of them greatly improved capabilities of AI without proportionately improving safety.
So that's the actions I see.
Okay.
One of the things that I worry about from a safety perspective, things are obviously already bad enough and moving fast enough, but quantum computing, at least from my layman's perspective, seems to be gaining some sort of rapid acceleration.
Am I just not able to understand the limitations that are self-evident to somebody educated at your level?
Or are we really at some sort of phase transition moment?
Looking at the stock market value of quantum computing companies, it seems like somebody knows something on the inside.
Maybe they're making good progress.
But as far as AI goes, we're making excellent progress with standard van Neumann architectures.
So I don't think there is a necessity for quantum computing to get us to a GI of superintelligence.
It does have tremendous impact on the crypto world, both cryptography for security and crypto economically.
So that's where I'm worried about quantum keeping secrets and keeping my money, but not as much in terms of AI.
Keeping your money because it will crack typical banks or keeping your money because you're largely in crypto?
Both actually.
It impacts all the standard encryption algorithms.
We have post-quantum encryption, but we haven't switched to it for most interesting applications.
So give me your stance on Bitcoin.
Buy some.
That's very clear.
So when you look at gold and you look at Bitcoin, why Bitcoin over gold?
You can make more gold.
As the price of gold goes up, I can make as much gold as you want.
I can convert other matter into gold at very high price.
I can exploit asteroids in the universe.
I can get gold out of oceans.
There is a lot of gold, which is very expensive to get.
But if a price of gold is high enough, I can produce more and more.
Bitcoin is not subject to the same pressures.
It doesn't matter if one coin is a trillion dollars, there is still a limited supply.
Okay, but what about people who say gold at least can be made into other things, gold is survived for thousands of years.
Bitcoin is like 15-ish years old and it's not backed by anything, can't turn it into anything.
It's just literally got no other use.
It's a dedicated app.
So if you have an app which does everything, it's usually not good at anything.
The fact that I can make jewelry out of it is not an important feature for me storing my wealth in it.
Whereas this has capabilities, gold historically lacked.
If I can pass a billion dollars to you right now for $5 immediately across borders, I cannot do this with gold.
All right, talk to me about the post-quantum encryption.
Every time, I'm hugely in Bitcoin.
Every time I hear the word quantum, I'm like, ah, like, oh, this just makes me paranoid.
Given that it's rightly difficult to make changes to Bitcoin, how are we going to get to post-quantum encryption on Bitcoin in a way where the community actually comes to consensus and doesn't create a problem for itself?
So once we get integer factorization running in quantum computers, you can see what size integers we can factor.
That tells us how close we are to cracking standard Bitcoin encryption hash functions.
If we're getting close to what would essentially destroy the network, I think it's like any other emergency.
We have history of fixing Bitcoin software, then an obvious problem was discovered.
I think at one point, somebody managed to print a trillion coins or some nonsense like that.
Immediately, a patch was distributed.
Everyone adopts it because it's the only way to go forward.
And I think that's what we're going to see.
As long as we have that available, tested the moment, there is a good strong signal that you have no choice but to accept or lose everything.
It's self-interest once again.
Okay, so on that, where are we?
How many integers can a quantum computer handle, and how many would it have to be able to handle in order to be a threat to Bitcoin?
I haven't kept up with the latest breakthroughs.
Last time I looked, it was a laughably small number.
Quantum computers were factoring like, I don't know, 15, literal 15, not even 15 digits.
So unless there was tremendous progress since then, I think we're still good, but progress could also be exponential.
So it could come very quickly.
Right.
Okay, so if you had a message to the Bitcoin community, would it be, let's move on this now?
There's no reason to wait until it's an emergency.
There's a very clear path.
Or is it like, well, I'm just sort of on the ride with everybody else?
I think we still have time.
I don't think it's pressing as much as AI problems we're dealing with.
So if AI is two years away, I think we may not be that close with quantum computers just yet.
But again, it's one breakthrough away.
If some company comes up with something much more powerful, it may shift very quickly.
Okay.
And what's the term for that?
The number of integers it can process?
The trigger would be what size integers could be factored, how many bits.
Got it.
Okay.
All right, Roman, this has been just absolutely incredible.
What message do you want to leave people with to get them to take action?
What is your best pitch to get them to sign your petition?
So, if you are in a position of developing more powerful AI systems, concentrate on getting your money out of narrow AI systems, solve real problems, cure cancer, figure out how to make us live longer, healthier lives.
If you are developing super intelligence, please stop.
You're not going to benefit yourself or others.
The challenge is, of course, you know, prove us wrong.
Prove that you know how to control super intelligent systems, no matter how capable they get, how much it scales.
If you can do that, then it completely changes the situation.
But as long as no one has come up with a paper, a patent, even a rigorously argued blog post, I think we are pretty much in consensus that we don't know how to control super intelligent systems and building them is irresponsible.
Amazing.
Where can people connect with you?
Follow me on Twitter, follow me on Facebook, just don't follow me home.
Nice.
Awesome, Roman.
Thank you so much for the time today.
I really appreciate it.
Everybody at home, speaking of things, I appreciate.
If you haven't already, be sure to subscribe.
And until next time, my friends, be legendary.
Take care.
Peace.
Let's talk about a pattern that is guaranteed to be killing your progress.
You know what you need to do.
You need consistent nutrition.
We all do.
You need vitamins, probiotics, greens.
We all know that we should be doing more of it.
When your morning gets chaotic, you skip it.
When you travel, you skip it.
When your routine breaks, everything tends to break.
And that inconsistency compounds against you every single day.
AG1 is designed to solve the execution problem.
One scoop, eight ounces of water, and you're done.
You're getting 75 plus ingredients: vitamins and minerals, pre- and probiotics, nutrient-dense superfoods, everything that used to require six, seven different supplements, and perfect planning now happens in one drink that takes about 30 seconds to make.
Right now, AG1 is giving you $87 worth of free gifts with your first subscription.
You get a welcome kit, travel packs, vitamin D3 plus K2, and flavor samples.
Click the link in the show notes or visit drinkag1.com/slash impact to claim this offer.
Support for this podcast comes from Progressive, America's number one motorcycle insurer.
Did you know writers who switch and save with Progressive save nearly $200 per year?
That's a whole new pair of writing gloves and more.
Quote today: Progressive Casualty Insurance Company and Affiliates: National average 12-month savings of $197 by new customers surveyed who save with Progressive between October 2024 and September 2025.
Potential savings will vary.
