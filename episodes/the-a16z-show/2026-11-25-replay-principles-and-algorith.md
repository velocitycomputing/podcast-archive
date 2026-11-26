---
record_id: "podcast:4d00b22c-8fdf-4cc9-b61f-004d33ed8c5d"
episode_id: 4d00b22c-8fdf-4cc9-b61f-004d33ed8c5d
title: "Replay: Principles and Algorithms for Work and Life | Ray Dalio (2019)"
podcast_title: The a16z Show
url: "https://pocketcasts.com/podcast/the-a16z-show/20a7ca40-9128-0131-8b7f-723c91aeae46/replay-principles-and-algorithms-for-work-and-life-ray-dalio-2019/4d00b22c-8fdf-4cc9-b61f-004d33ed8c5d"
audio_url: "https://pocketcasts.com/podcast/the-a16z-show/20a7ca40-9128-0131-8b7f-723c91aeae46/replay-principles-and-algorithms-for-work-and-life-ray-dalio-2019/4d00b22c-8fdf-4cc9-b61f-004d33ed8c5d"
feed_guid: null
feed_url: "https://feeds.simplecast.com/JGE3yC0V"
published_at: null
published_local_date: null
played_date: 2026-11-25
played_at: "2026-11-25T12:00:00Z"
play_count: 1
duration_seconds: 3000
source: pocketcasts-history-browser
played_label: Yesterday
history_order: 2
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: ca58ef0465b9747add6ca2218fbe393138084c9c36ba36393f477ba46553a021
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

Ray Dalio, Alex Rampel, and Sonol Choxi discuss turning repeated experience into written principles, then into decision-making algorithms and computer-assisted systems. Dalio illustrates cause-effect thinking with his McDonald’s chicken McNugget story: McDonald’s wanted a fixed price despite commodity volatility, and Dalio helped structure hedges around the real cost drivers—chicken feed, especially corn and soybean meal futures—so a supplier could sell forward chicken at a locked price. The conversation covers principles as “species” of problems, the value of writing down decision criteria, using history to recognize recurring patterns, and Dalio’s “upward corkscrew” view that cycles repeat with new variations. Named references include Bridgewater, the 1982 crash, 1999, the 1930s, the 1880s, populism, Mackay’s Extraordinary Popular Delusions and the Madness of the Crowds, Thompson Reuters data, machine-learning black boxes, image recognition, lending algorithms, Gary Kasparov, computer chess, Jeff Bezos, the Firephone, Amazon’s iPhone app, Apple Maps, and “baseball card” profiles of people’s strengths and weaknesses. Key claims include: timing matters, especially in high-latency decisions; risk can mean standard deviation or risk of ruin; backtesting should follow explicit causal logic, not replace it; black-box models are acceptable only when the future is likely to resemble the past; diversification across roughly 15 uncorrelated or low-correlated return streams can materially improve return-to-risk; and organizations should judge process—the “swing”—rather than only outcomes, using an error or issue log rather than blaming mistake-makers.

No health-specific claims appear, so the actionable value is decision, investing, and organizational design: start a personal or team decision log that records the situation, your hypothesis, the causal logic, the bet, timing indicators, and the outcome; convert repeated decisions into written principles and, where appropriate, testable rules; separate process quality from luck or outcome, especially for hard, low-probability projects; maintain an issue log that treats mistakes as information rather than grounds for punishment; profile people’s cognitive and behavioral strengths and pair them with complementary teammates instead of expecting one person to be good at everything; for portfolios or venture bets, explicitly examine correlation, not just quality, and consider whether diversification can reduce risk enough to improve expected return; and when using algorithms or AI, ask whether the environment is stable enough for pattern matching and whether the model’s “why” is understood. Useful research leads include commodity hedging mechanics, historical bubble and populism cycles, long-term debt or economic cycles, quant backtesting pitfalls, and computer-assisted decision-making; follow-up questions include: What are my recurring decision types? What would my written rule have been in past failures? Which of my bets are truly uncorrelated? Where am I relying on black-box signals without causal understanding? And how can I measure the quality of a decision before its outcome is visible?

## Transcript

This episode comes from the A16Z archives, featuring Ray Dalio on how to make better decisions when the answer isn't obvious.
Ray sits down with Alex Rampel and Sonol Choxi to explain how he turns experience into principles, principles into algorithms, and mistakes into information.
They discuss decision-making under uncertainty, learning from history, building teams around complementary strengths, and why the best decisions often start with understanding what you don't know.
So I love the book, and I told my kids, I do this every morning, what am I doing for the day?
And I didn't know how to describe.
This is what I told my eight-year-old, you helped invent the chicken nugget.
I'm glad you told me that because I can use that with my four-year-old grandson when he gets.
No, you know what I'm saying?
My eight-year-old loves chicken nuggets.
I actually have tricked him into thinking that McDonald's is normally closed.
It's like, oh, it's closed on Sunday.
Oh, it's closed on Saturday.
So he goes for his birthday because otherwise he'd want to go every day.
So I was like, you know, actually, the guy today invented the chicken nugget.
He was like, no, actually, he didn't really invent it, but he was responsible for the introduction.
So he was very, very excited.
Actually, he wanted to know if you could sign or give him a chicken McNugget if I could bring him back with a sharpie.
Well, I mean, I mean, I don't really, you didn't actually invent the chicken nugget.
I don't know if you're going to be able to do it.
Just correct that because all of a sudden it'll be all over the media and people who have dietary problems will sue me or something.
And you know how this goes.
Anyway, what happened at the time, I contributed to the economic risk of being able to come out with the chicken McNugget because it came out at a time when there was a lot of commodity price volatility.
And McDonald's wanted to come out with a chicken McNugget, but they couldn't lock in a price.
They couldn't guarantee that because the producers of the chicken wouldn't be able to contract forward those prices because their costs were going up.
But I figured out that, by the way, this is in the old days of trading commodities and so on.
The mechanics of it were that there's a little chicken, it doesn't cost much money.
And what really costs the money is the feed, which is mostly corn and soybean meal.
And so there is a futures market in that.
So I went to the chicken-making client that I had at the time and McDonald's, and I told the chicken-making client that they could put on these particular hedges so that they could sell a forward contract of that chicken at a fixed price to McDonald's so McDonald's could come out and have a fixed price and wouldn't have that price risk.
So that's what happened.
And what I like about that is I love the mechanics of the cause-effect relationships that you could then, you know, when one thing relates to another.
So that was my chicken McNugget story.
That's great because it's a great example of how when you break it down into analyzing it, the result is more than the sum of its parts.
We're all eating chicken nuggets.
Well, I don't have a vegetarian, but your son eats them.
You can actually break down exactly this cause-effect relationship that you're talking about and why that matters so much for decision-making.
Ray, I know you've been actually on a lot of different podcasts, and so I don't spend too much time on this, but just in a nutshell, if you could summarize what principles is, how would you sort of distill it?
Like, what is the point of principles?
I think everything happens over and over again.
And principles are a way of looking at things so that everything is viewed as like another one of those.
And when one of those comes along, how do I deal with that successfully?
So, for example, there may be principles for skiing.
Well, put your weight on the downhill ski or something.
There'd be principles for parenting or whatever it is.
So it's a way of looking at things so that you see this thing coming over and over again.
And how do I successfully deal with my realities so I get what I want?
Those are principles.
Then I think everybody should have their own principles that they believe in.
It shouldn't be anybody's, my principles, or just happen to be my principles.
But from my experience, and I recommend to everybody, whenever I would encounter something, I would write down the criteria I would use to make a decision.
So when the same thing happened again, I could kind of refer to that.
And then it changed how I saw the world because everything just seemed like dealing with a particular species of things.
In other words, that rather than all this noise coming at me, that's a whole bunch of different things, I could say, well, if this is a duck, and how do I deal with ducks?
Or this is a species I haven't seen before, and how do I deal with that?
It's like having a framework that you can look against and see this is different or similar to what I've seen before.
Yes.
And then by writing it down, I was able to communicate with others, so it got us in sync.
And then I was able to convert a lot of these to algorithms so that I was able to build a decision-making system.
So those are what principles are.
And I don't care where people get them.
This is my recipe book that I've accumulated over a period of time.
And then I'm just encouraging other people to pick their own.
So one of the things that I really admired reading the book was just how much you've been a student of history.
So for every cycle, for everything that you've looked at in your career, you were able to understand when it had happened before.
And in many cases, when you thought it was new, it actually had happened before.
Because sometimes if you're standing on the upslope, you don't even see it.
But I think one of the things that was really interesting reading about your journey, knowing everything now that you know now, and starting Bridgewater 40 years ago, what order would you have done things and rolled things out?
Because for many companies that are in the early stages, when they don't have product market fit, they don't have revenue, they don't even know what they're doing, going from zero to one, from nothing to something, that's often a different skill set than going from one to N.
And if you think about the team aspect of this, when you're a team of two people, if you're probably radically transparent with each other, it seems like a lot of information just flows osmotically.
So, part of my question is: how does it change from effectively the zero to one phase?
If you have two people, three people, as opposed to you have hundreds of people where decision-making is actually hampered by lack of understanding different people's strengths and weaknesses, how do you determine if you should listen to this person or that person?
How do you understand what people's principles are?
It becomes more important at that stage, as opposed to early on.
If you really try just focusing on scaffolding before product, you're going to run out of money.
So, I think you're asking two questions.
One, when did I discover it?
And then, secondly, when would I do it?
Right.
Okay.
I discovered it by making mistakes, and you know, particularly like in 1982, you know, that crash and whatever that got me thinking differently.
So, you know, I was just figuring out how to do that at each of the stages.
So, it sounds like everything, like you would have rolled that out at day zero.
I mean, these all developed over time.
It wasn't like day zero.
So, I was in even a worse position in that I didn't raise any capital.
So, I had a two-bedroom apartment, I had a second-bedroom, and it was me in my second bedroom, really.
And I didn't raise capital, but of course, the nature of my business would I could get paid a fee, but that's like earning some revenue or whatever.
It depends on whether you needed capital expenditures.
I needed it for a quote machine and things like that.
But, anyway, back to the basics, knowing what I don't know and how to deal with it is something that's always great, even if there's not even a company.
Right?
Like, one of the things that I've observed over and over again is that everybody gets surprised about the thing that hasn't happened before their lifetime.
Exactly.
Before we ever devalued a currency, boom, I had this one and that one.
But everything has happened in history, almost everything.
The way I look at it is almost like an upward-pointing corkscrew.
You know, these things go around and around, but it's sort of pointing upwards so that there is new.
How it is new repeats itself, and you can start to look at that, right?
So I think one has to be informed and take that perspective of it happening over and over again.
I mean, I'll bet you dollars to donuts that almost anything that you're going to observe, by and large, has happened before in the past.
If you're informed of that, not only does that allow you to think about those cases that are analogous, but it also brings you to the fundamental understanding of why things might be different.
So you will still understand how reality works to produce the cause-effect relationships to get you to that point.
And that fundamental understanding is still valuable, right?
Right.
It's amazing in our business where there are all these people that are starting companies that don't remember 1999 because they weren't born in 1999.
And they don't understand what the concept of technology-inflated bubbles look like.
And it's just, that can't exist because it's never existed before.
But exactly as you said, it's not before in their lifetime.
And some of these cycles, like the longer-term cycles that you talk about, like most people haven't been around since the 1930s.
So for them to observe something and actually think that this actually happened before in history, it's just not something that they're capable of.
I think of McKay's book, Extraordinary Popular Delusions and the Madness of the Crowds, and it's about that phenomenon.
And that was written in 1640 something or other, looking backwards and so on.
So that dynamic exists.
Or today, let's say populism.
Okay, so think of populism.
That's a phenomenon.
Just say, okay, what is the phenomenon of populism?
How does this thing grow and develop?
So once you start to think that way, then it brings you into it.
And then I like to look at them laid on top of each other.
So, in other words, let's take all of those cases and put them together.
And if they have data associated with them, let's say a bubble, then you just plot the data on top of each other so you could see each one on fold.
And then you can then say, what is an archetypical one?
And then what is the deviations between that one archetypical and the others?
And can you explain that?
And then when you get the explanation, then you get a rich understanding of the dynamic behind it.
It's a very effective way of making rules.
So this kind of making rules has been key to our investment perspective.
Well, except there's one big layer here, which is we're talking about this arc of history and having that knowledge or the mistakes you made when you first came to your business because you didn't have experience and then you earned the experience the hard way.
But the theme that really resonated for me was the timing of it then actually making a decision on that information and data you've gathered, whether it's from history or personal experience.
Because the other thing that resonated about your book is that it was also a matter of knowing you were too early on a lot of different things.
And in VC, we talk about this all the time.
You can either be very early or very late.
It's all about timing.
Being wrong and being early are the same thing.
Venture capital has a very, very high latency loop.
You make a decision today, you figure out if you're right or wrong in 10 years.
So for public markets, you make a decision today, you could figure out if you're right or wrong, maybe even in an hour from now, maybe tomorrow, certainly within a year.
That's one of the things that's very, very hard with technology is you don't have the benefit of real-time feedback.
You don't have this benefit of knowing how the market is anticipating or answering your actions.
You do in 10 years.
I would argue that the set of principles that people use around investing has to be much more internal focused than external focused because you don't on a short-term time horizon have the external outputs in terms of the stimuli.
So, how do you guys think about acting on this information to make a decision to know when is the right time?
Like, what's sort of the framework for that aspect of it?
What does it really mean?
Because I think of it in mechanical terms.
In other words, what I think about in terms of returns, I'm now going to get into an investment perspective.
Everything is a return stream, meaning from the moment you buy it, it has a return in the form of either what its worth is or the cash that it throws off.
Think of that like the dividends, and that is the return stream.
And now you're thinking about how should you optimize for that return stream.
And I believe then that the best way to do that is to think about that return and also what do you define as risk.
And to what extent, for example, is risk the standard deviation of that return stream, or to what extent is it risk of ruin, and so on.
And so, as you approach that question of being early, you start to think of it as an engineering exercise, it is a betting strategy.
So, when you take that and you have a highly volatile or unknown, timing could be a very, very, very big thing.
We're in agreement that it's a very, very big thing.
And then you have to then think about, okay, so now it's not just good enough to find a good investment, it has to be well-timed.
So, now, how am I going to determine that particular timing?
What are my indicators?
Then, brainstorm of what your indicators are, and you think, you think about that question.
And through that exercise, you will come up with something that is your particular thing.
You write it down, you specify it, and then you backtest it.
In other words, get a large sample size of those particular cases.
And then you say, if I executed that strategy in that way, how would it have been?
When you tested it, you might think, oh, that was good, but it wasn't good in these ways and that time.
And then you say, okay, what happened in those times that it wasn't good and whatever.
And what do I do to modify my strategy?
And then I execute it carrying forward.
You've got the framework, the decision-making framework to decide on timing.
Well, I think part of the reason why I asked about, you know, what can you learn from history because it's almost equally interesting, what can you not learn?
Like, so on that corkscrew that you think about, like, is there going to be a new archetype or is kind of everything that's going to happen, has it already happened in another archetypical form?
To be very clear, you don't know that unless you know the author, right?
That's true.
Because that's what the framework is.
And what you'll discover is it really depends on exactly what it is.
It'll be, by and large, true, but not 100% true.
You make a very good point about how history repeats itself again and again.
And there are these natural cycles that tend to just repeat with almost oddly predictable regularity.
Yet at the same time, there are things that have no historical precedent.
You see something and you can say, ah, yes, there is a precedent for this in the 1930s or there is a precedent for this in the 1880s.
But every now and then there is fundamentally a new paradigm that develops and this is obviously easier to do retrospectively than prospectively.
But how do you determine or how do you try to determine if something is truly without precedent?
Because there is an overly pattern matching or pattern recognition trap that you can fall into where you could say, ah, this is exactly like what happened then, but it turns out that there actually are differences.
Alex, do you have any models where you think that pattern recognition breaks down?
Like where there is an archetype that you're sort of the past does not necessarily indicate the future?
Well, I think it's hard to know only in retrospect.
But do you agree that if you don't have deep understanding of the algorithm and the logic behind it and the future is different from the past, that that's extremely risky?
It's a disaster, yes.
Okay, that's an important thing to know.
Well, I mean, especially if you look at the quant trading world, so I know a lot of people in this space, and the pure black box.
So there's a company, they take all of these data sets and then they encrypt the data, but you can still perform operations on the encrypted data because this allows them to buy Thompson Reuters data and then give it out to the entire world of crazy machine learning programmers.
And then the machine learning programmer will design something, it will get backtested, they'll do some kind of out-of-sample test, but there's no cause and effect analysis.
The computer just does what it does.
It's the ultimate black box of black boxes.
And so you don't know the why behind what it's doing.
And it could just be picking up pennies in front of the proverbial bulldozer.
So, yes, I mean, like when you don't understand the why, and then when, especially if the future is going to be different than the past, that's definitely a cause for a blow-up.
And if you do that, go down that path, then the problem is you will never test your mind.
You will never be in that situation of going for the deep whys.
You will not have the deep understanding.
We literally deprive ourselves of that because in the book, I love this phrase where you talked about how you always went back.
And of course, Science Life 2020, we all know that.
But you would look at how the dominoes fell in logical sequence for every big bubble.
But it was interesting.
I always started with what I thought, and I always do this.
You go through your experiences, and then you express your logic.
What is the cause-effect, and what is the bet I'm going to make, and when do I make it in terms of the timing?
And then you've got that clarity, because that forces you to think deeply.
And then when you've got that, then you run that back in time and test it.
Because if you go to history and then you say what would have worked, and then you try to sort through that particular pile, and then you've got that pile, I guarantee you, you can't even understand a basic algorithm.
Let's take just a regression with two independent variables, by way of example.
And it says, here's the constant, and here's the, it's 0.25 times whatever that thing is.
And you're asked to explain why it's 0.25, that if the fact that it will be 0.25, and you probably can't do it.
And that's with a simple two-independent variable type of regression.
Now you put those things, you get a whole bunch of those things, and you get them with more complicated events.
And that's a lazy man's way out of that particular thing.
So I'm recommending that when you're making a decision, you just get in the habit of writing down, just do it in words, forget algorithms, forget backtesting, just do it.
And you accumulate those principles, and then you think, how do I convert those principles over a period of time into algorithms?
And then when you've got that, then you can go back and you could see how it performed and refine what you're betting on.
One of my other favorite parts of the book is how you did talk about your evolution of partnering with computers in thinking about codifying your thinking.
Because at the end of the day, writing something down is codifying it, is turning into an algorithm.
It's code.
And while we do have this open question of how our world is going to change with black box algorithms and AI that veers into complex systems where you can't tease apart cause and effect, it does open a lot of questions.
I wonder if it leads to a new model of thinking, but that's a broader philosophical question.
I just want to pick up on that particular point.
When you build a computer decision-making system and you have your own, think of it as a computer chess game.
So now you have a computer chess game that makes its move, and now you have you making the move.
That relationship is a beautiful, fantastic relationship because if it makes a move that is different than your move, it raises the question: what am I doing incorrectly, or what is the computer, and why can't I reconcile that?
That'll help to teach the computer.
And I was speaking to Gary Kasparov about this, and that's like the best way to play the chess is to have that computer partner next to you and to do that exercise.
And that's a beautiful relationship, and it has tremendous beneficial effects.
Yeah.
Yeah, I think the thing that's really interesting, if you follow the trends in machine learning today, in many cases, they are more black box-like.
Even the way that image recognition works, it's a multi-dimensional regression, effectively.
How is the computer determining that this is a cat?
It's actually kind of hard to figure out.
Or if you look at lending algorithms that newfangled banks are using, it's effectively linear algebra.
You have every consumer here, you have every possible measurable attribute over here, and it's not three things, it's a combination of everything.
So it's a little bit hard to disentangle cause and effect.
Well, if it's something that you're confident that the future will be the same as the past, that's A-OK.
So let's say if you were to say, I have enough cats or whatever, or like computer chess.
I mean, computer chess.
Deterministic, right?
Right, because I'm comfortable that with a high enough sample size, that the future will be the same as the past, and I will do that.
This is what I'm calling mimicking.
I think of it as kind of mimicking.
Okay, I could do that with people making surgeries.
In other words, if I have a surgeon and I have a bunch of people and they still cut the same way, and I take that and I convert that into data, and I know that that form of cutting is going to work with that kind of body, I'm totally happy to derive the algorithm with that because the future will be the same as the past.
There's no problem.
You have to reinvent it every time.
Right.
I want to be clear.
I'm totally okay on that.
So, the issue really is when you go to those two things, right?
When you have a situation where the future will be different from the past and you have no understanding, that's where you're going to have problems.
One of the quotes that I really enjoyed in the book is that he who lives by the crystal ball is bound to eat ground glass.
So, it's combining that also with an arrogance that you really know you can prophecy with 100% certainty what's going to happen.
I mean, one of the things that actually we debate here a lot is if we think we're right, we really, really think we're right, of course, we should ask why do we think we're right.
But if we think we're right, you know, should we go put more money into an investment?
And the problem with that is that it actually creates more stress on the organization.
Because maybe the best way of thinking about it is if you have a fund that's size X and you make 50 investments, you know, maybe the right answer is one over 50 times X.
Even though that might not be optimal, you might believe in one company more than another, that actually might create more organizational not harmony, but it just de-stresses the organization and it kind of hopefully doesn't fall victim to the glass-eating exercise of trying to think that you could prophecy the future.
Well, the question is: what is the marginal benefit of diversification relative to the marginal benefit of goodness?
It's a better way of putting it.
And if you really look at that, the marginal benefit of diversification is much more powerful than the marginal benefit of goodness.
If you don't know what's going to be the best, that and you have some element of uncertainty, so you're not typing in a number that has an uncertainty to it, you have a distribution of that number, and then you know that diversification works, the power is going to be so much greater.
The key in betting, I believe, is to find 15 good, they don't have to be great, uncorrelated or low-correlated return streams.
Because if you have, let's say, a 60% correlation between those items that you're betting, and you could have 1,000, and you're not going to reduce the risk much.
You're going to reduce the risk by 15% or something along those lines.
If you have uncorrelated bets and you don't know which is necessarily going to be the best, but you do know that they're not correlated together, and you put that together, 15% uncorrelated returns is going to reduce the risks by about 15 or 20 percent of what you originally had.
That increases your return-to-risk ratio by a factor of five.
So now you start to think about that in terms of what does that mean for the types of bets you can take.
Let's say if you're using leverage, for example.
Okay, now you could say I could leverage.
That risk reduction can be converted into a return enhancement.
You wouldn't want to overdo it, but you can take that risk reduction equals return enhancement, so that being able to produce the diversification and the structuring of the bets that way raises your expected return while reducing your risk, right?
And so, anyway, that's why diversification and knowing what you don't know and picking it will reduce your risk, reduce your stress, make your better portfolio.
So, one question I have, which I think is really great that you've done, is this decision to record errors versus flog the error makers.
Oh, I love that.
You called it the error log, and then you changed it to the issue log.
Right.
And one thing that I also think is very interesting in terms of how organizations judge process versus output.
And I was wondering if you could talk about this a little bit.
Because if you think about some of the hardest things, like if you want somebody to solve the hardest problem that perhaps has the lowest probability of success, you should probably put the best person for the job on that problem, but the output might be nil.
Yeah, you know that there's a big distinction between goodness of decision-making and particular outcomes, unless you have such a perfect high sample that you could then put that all the way through and you could say, I have a statistically reliable sample.
And also, making mistakes is part of the process of learning.
So, connecting them to mistake and flogging them just doesn't make any sense, right?
So, first, embrace the fact that that's a different thing.
Identify what people are good and bad at.
In the book, I talk a lot about our culture of how you go about that.
So, first, just embracing it is the reality, and then also seeing is somebody doing something right?
If you're looking at a baseball player or a golfer and you see how their swing is, you should be able to say that's a good swing.
So, if you just look at the shot, that's a different thing.
So, you have to know how to look at the swing rather than the shot, right?
I heard Bezos actually tell a story about this.
Exactly, yeah.
That's what I was thinking of.
We had Jeff Bezos here, and he was talking about how the person that actually built the firefund, that was really hard to build a phone from scratch, to get it into markets in nine months, and to do all the things that they did.
You know, he like he actually really rewarded that person.
Whereas, if you think about the most successful thing that Amazon's done in the last five years, it's the Amazon.com app on your iPhone.
But that was riding a massive secular tailwind.
So, to say that team deserves all the praise because they had a really easy job.
And meanwhile, the Firephone guys should get fired.
I mean, if you think about what happened at Apple, Apple built Apple Maps in six months.
The person behind it got fired because it didn't work very well, but that was an almost impossible job.
So if you think about the cultural norms that that reinforces, you don't want people shying away from the hardest work because they're afraid of the repercussions.
You want to be judged on the swing to take your metaphor versus the outcome of the shot if you're going into a massive headwind.
The hard part is how do you measure the swing?
How you do that is to know what the person is like.
Can you talk about what the person is like?
Can you measure what the person is like?
Does the person want to know what they're like?
Do they want to know their weaknesses as well as their strengths?
Can you have a community that does that?
That is, in my opinion, the most important thing in terms of running an organization.
This goes to your idea of baseball card-like profiles of people, where you kind of have their stats on who they are, but at a personality level, not just like their output or batting average or whatever it is.
Yeah, let's recognize that people are strong and weak in different ways, right?
So let's get down to a nitty-gritty level, and then how do you put together teams of people so that you embrace your weaknesses and then you figure out what to do about it?
It could either be that you develop a strength to deal with it, or it's probably even better to work somebody in.
Yeah, work with somebody who has a complementary strength where you have a weakness, and then you can have an appreciation and you could achieve success, right?
But the not talking about it and not dealing with what you're like is a fundamental problem.
I'm so glad you said that because we have a lot of founders that listen to our podcast.
And one of the things that we hear a lot from them is as you build a company from scratch and you've never managed before, or you know, hired a CFO or hired a sales revenue off chief revenue officer, it's not only this radical transparency that you're talking about of knowing people's strengths and weaknesses and sort of having these profiles in your heads, but sometimes it's about knowing what you don't know because you don't know what sales is when you've never done it before.
Exactly.
That's been the story of my life.
And that's why I wrote down these things because knowing what you don't know, it's so much more valuable than anything you know.
Because there's so much more good thinking out there than any human being can have in their head.
Well, let's shift gears then, because given that the biggest barriers to having these kinds of understandings and ability to have these principles are ego and blind spot.
And that's what you quote as the two things.
And we've been talking a lot about algorithms and codifying things, and I think it's fascinating that you're an investor, but what we're talking about, it's all about decision-making under uncertainty, and that's the thing that connects us to life, to finance, to whatever it is.
On that note, you can't necessarily codify emotions into an algorithm.
And so one of the things that I think we should go deep on is sort of the differences in frameworks in your book between two types of minds that we have inside all of us.
The two U's, as I said, the two U's, exactly.
In each person, there's a conscious, thoughtful you that is the prefrontal cortex, the rational, rational you, and then there's a subliminal, emotional you that actually you don't understand very much because it's also subliminal.
Oh, yeah.
And by the way, as a student of therapy, I've been in analysis for a few years now, four days a week.
Let me tell you that those patterns go way back to like when you were born.
And before.
And before, totally.
Okay, you come pre-programmed.
You could show a child a picture of a snake and a picture of a baby.
Show them a picture of a snake and a picture of a flower.
They are programmed to know that this is okay.
Because we come programmed.
Right, it's inherent tendencies.
Right, which things that go back longer than mankind.
Oh, I mean, there's all kinds of philosophies around that, too, exactly.
But we do know our programming.
The brain has evolved.
And so knowing that there are the two U's and that we encounter those two U's all the time then brings a crystallization to that.
So that's why intellectually, when we go through this, that's where the barrier lies.
There's the ego barrier and there's the blind spot barrier.
The ego barrier means it's sort of like it's got to come from me or even disagreement.
The reaction to disagreement is an instinctual reaction of intending to assume it's an attack and it triggers the amygdala.
So there's a mechanics there that produces those kinds of reactions.
It is only an exercise because if you can get to that open-mindedness where you can take in and you can find out where you might be wrong, then you're going to be in a much better position.
I think that one of the greatest tragedies of mankind is that people hold on to wrong opinions that lead to bad decision-making without being able to put them out there and properly stress test them, which is so easy to do to raise their probabilities of taking it and to get information inside.
So that's the ego barrier.
And then there's the blind spot barrier, which is a little bit different.
The blind spot barrier means that people genuinely see things differently.
So you could have a totally open-minded person, but when you see things differently than somebody else, then that's how you see it.
And it wasn't really fully apparent to me that all of these things existed until we made it so crystal clear how people see things.
There's a tool I show in TED Talk, and the tool shows how people see things differently on a continuous basis.
That difference means that when you start to see things collectively and you see through other people's eyes, it's like going from black and white to color or from one dimension to multi-dimensions.
And if you can get that radical open-mindedness, collective decision-making is so much better than individual decision-making.
But you've got to get over those two barriers.
How much do you think people are capable of change within organizations as adults?
I can only tell you what our experience has been.
About a third of the people can't get through it, something like that.
Over 18 months, you can pretty well find out where you are.
So, the answer to the question, just generally speaking, if you're talking about that ego barrier open blind spot, I think most people can make it, but it requires that practice.
It's just a matter of habit.
Our backgrounds are so bad in that all of the ways that we're raised in school, like don't make the mistake, and the kid who's got the right answers is the one who is getting rewarded.
It's like going against programming.
So, I was a manager of no more than 150 people, so very small by your standards.
But the thing that I often ask myself, or you can give people very good feedback, or sometimes you can give people not very good feedback, but in what cases do, if somebody knows their strengths and knowing their weaknesses, like can they change by one standard deviation?
Like, what's the limit that you've seen?
I've examined that at length both in terms of our populations, and then I've really enjoyed working with psychologists to try to figure out they're the pros and doing that.
And generally speaking, with a lot of hard work, you can change by about one standard deviation.
There's some people that argue that the nurture element is malleable until a certain age.
And then there are some people that say, nope, nope, like once you're an adult.
Like the age is that of adulthood, and then it's very hard to change thereafter.
And I think that's one of the things that's very interesting.
If you really map the strengths and weaknesses of the individuals in the organization, to what extent is that dynamic versus static?
And that's why there's two paths.
You don't have to change.
This is the thing about it.
If you can take the joy out of success and you realize that you put together the teams right, you can bring those dimensions and then you could succeed.
There are two ways of thinking about this.
If people can't change, it's very useful to understand what are the characteristics that are effectively ossified.
If people can change, then it might actually be a bad idea to think of certain characteristics as being overly ossified because, in fact, they are fundamentally malleable.
That's what I found fascinating, which is, you know, a lot of organizations try really hard to train people to be things that they don't want to do or to do things that they're not good at, as opposed to actually having radical transparency around, like, here are the things that I like, here are the things that I'm good at, and then pair them accordingly.
I think that's exactly right.
And actually, it was a conversation with Ben that actually prompted this insight in me.
It was about some other things that I was thinking about in terms of trying to change people's biases and how they think and whether that's even possible.
But basically, Danny Kahneman talks a lot about the concept of a system one and system two brain, which is not unlike the two U's that you describe.
And by the way, this is actually a brilliant piece of rebranding that he did this because it sort of takes it out of the Freudian legacy and other loaded interpretations.
But basically, system one is like the fast-reacting, instinctive, subliminal you, and then the other system is a bit slower, more analytical, rational, reflective, et cetera.
So, and it's kind of sad because we as a society are programmed to keep these two you's in conflict, and I think that actually plays out particularly between work and personal settings as well.
But anyway, I want to switch gears now and let's talk about this concept of an idea meritocracy, which Ray, you talk a lot about.
And I have to tell you, I kind of hate the idea of that.
Really?
Yeah, let me tell you, because I don't like this false notion of democratizing all ideas as equal.
I don't believe that for a minute.
No, but that's not what I'm saying.
Okay, so clarify what it is.
So I'm talking about believability-weighted decision making.
So let's talk about what believability weight is.
Okay, in most, when I say a meritocracy, it's dependent on knowing the merit of the person.
It's not all opinions are equally valuable.
You have to know the merit of that person.
That's why I say you have to know what they're like.
Okay.
So, I mean, there's either autocratic decision-making or democratic decision-making.
Autocratic decision-making means that the boss knows best.
Democratic decision-making is one equal vote.
So, I'm going to give you the concept and the mechanics.
The concept is you have a disease, you're sick.
Now, you don't know how to deal with that disease.
You can go to one doctor or you can go to three doctors to triangulate.
What I recommend you do in that case, in almost all cases of making decisions, is find three really great experts who will disagree with each other, openly disagree with each other to try to find the right path.
If you then will isolate what the disagreements are and you bubble those things up to the top, then you can focus in on that.
And when you go through that exercise, you will probably make a believability-weighted decision.
So, that's what I mean kind of by believability-weighted decision.
And then the question is only how you establish each of those people's believabilities.
Now, what we do in processes that we're looking at is that we know what people are like, what are their strengths and weaknesses.
They may be right or wrong about that, but by doing it in agreed-upon ways of saying, okay, now you're good at this and that, and you get believability points, whatever the dimensions are.
Because a believability will change depending on the particular thing.
Now, if you can establish those definitions for that, and then you come into a room and I'm, you know, CEO, I have a choice.
Do I just ask and then go make a decision?
I ask that room and I get an equal weighted answer and I get a believability-weighted answer.
And then what should I do in that situation?
Well, if they're at odds, I still try to reconcile it.
But honestly, like I'm the person who's that patient who then says, I got these three doctors, so that's how it works.
I'm smiling because when I had my foot surgery, I saw three doctors, and this is basically what I tried to do.
But it's hard because sometimes doctors don't like to disagree with each other or speak openly.
You may not be able to do this perfectly, but man, the real question is: do you want to do this?
Do you want to, as an organization, know what people are like?
Can you speak honestly with each other about that?
Do you bring that to the surface so that you can know what and deal with what people are like and then use that as a foundation of who should make what decisions in an idea meritocratic way?
So, now do you like idea-meritocratic decisions?
I do, and I'm going to read out loud your definition of believability.
I define believable people as those who have repeatedly and successfully accomplished the thing in question, who have a track record with at least three successes and have great explanations of their approach when probed.
So, they have the rationale kind of queer.
I need at least one of those two things, right?
Well, I thought it was very interesting because you talk about how if you have a disagreement with someone and you're the more believable person, you might actually remind the other person in a conversation so that they ask you the questions versus you having to be the one answering them.
Because the politics of organizations often mean it's the other way around.
Right.
If Tiger Woods is trying to teach me how to play golf or whatever, it would be smart for me to try to ask him the questions rather than think that I'm the one who has the understanding of that.
That wouldn't be smart.
And so if you have a difference in the understanding, by kind of saying, am I a teacher, a peer, or a student?
Which should I be?
Helps me navigate the best way to approach that.
So if I can ask, you write a lot in the book about shapers.
And one of the things that I thought was interesting was you actually kind of looked at the psychological traits of many people that most people would call shapers.
Steve Jobs, Elon Musk.
Steve Jobs, Elon Musk.
And actually, one of them was, I don't want to call it sociopathy, but it's basically thinking more about the goal that they're going to achieve as opposed to the temporary emotional feelings of others that they might hurt.
I often find that the best leaders, they are dogged in terms of their determination of that goal and not worrying about the feelings of other people along the way, but in a good way, right?
Like it's not that they're sociopathic.
It just means that they really care about achieving that goal.
Yes, so that's why I did the tests.
What have you found?
So let me define a shaper.
A shaper is a person who can bring something from visualization to actualization.
I can visualize this thing and then I can deliver on it.
You can basically do both.
I mean, the quick example that pops in my mind was Hamilton, because not only did he have the vision for the Treasury Department and everything else, he also spent his first year as Secretary of Treasury writing letters about lighthouses on the detailed level.
And you have to fight with people.
Right.
You have to do something.
So I literally asked these people, Steve Jobs, Elon Musk, Mohamed Yunus in philanthropy, these people, essentially to discuss it, and then also take some personality with profile tests, in a sense, to think what their preferences are to see if they would look alike and so on.
And then there are a number of dimensions.
I can't go through all the dimensions.
There's a number of them.
The one that you're referring to is there's a test call in workplace inventory, which is called concern for others, and it doesn't really mean concern for others.
What it means is that when faced with the choice of whether the mission or the individual's feelings are going to be at odds, which is the choice that is going to be made, these people have devoted their side to others.
They have huge concern for others, but on that particular dimension, they are relatively low on that dimension.
And what it's only telling you is that the mission can't be compromised.
Think about it as if it was a team instead of a company.
If we have a team, like somebody's got to say, man, you ain't doing it well, you know, and nobody would say, hey, listen, I'm sensitive to how you're talking to me about that.
You've got to have that particular conversation, and you've got to get the best people on the team.
In other words, tough love is, I think, the best kind of love.
Hold them to standards and also love them.
The meaningful relationships part is as important as the excellence part, because if you have those relationships that are self-reinforcing that you know you care, but you're holding to high standards of each other, you can accomplish things.
We talk a lot about founders having this will to power, and sometimes it requires like a hubris.
Maybe should be a student, but you're trying to be a teacher in a new industry.
A very big difference in mindset, I would argue, between startup founders and like the CEO of a Fortune 500 established company sometimes.
And so this idea that you have to have this will to power, which requires a certain amount of self-delusion.
How do you sort of know, given this framework that you're talking about, when, because weaknesses and strengths are flip sides of each other?
And I would argue that it's actually not just flip sides, but they're a matter of degree.
How do you know when you're going too far on this continuum of letting your strength become a weakness and your weakness become a strength?
Well, we're talking about to be able to have simultaneously open-mindedness and assertiveness.
So in other words, the deep need to make sense of things, knowing that you might be wrong.
And so, yes, you have that vision.
And then at that same time as you have that vision, you say, I might be wrong.
And how do I stress test the hell out of that vision?
So you listen, you can take in at the same time as you can be assertive.
If you don't lose one to the other, that's how you're going to get the balance, right?
So you talk about surrounding yourself with independent thinkers that are sort of like-mindedly independent, even though they might not agree with you.
Because one of the things that I've learned is that you cannot be honest with yourself without mirrors around you.
Right.
And the problem is that people think they're self-aware, but they're really not.
And in fact, I thought one of the best sections of your book was actually on how to tell the difference between closed-minded and open-minded people.
I mean, you'd think it'd be obvious, but it isn't.
I just love the precision of language for each.
So I'm going to go ahead and quickly summarize and read aloud some of this really quick.
Closed-minded people don't want their ideas challenged.
They're typically frustrated that they can't get the other person to agree with them instead of what open-minded people do, which is be curious as to why the other person disagrees.
Closed-minded people are more likely to make statements than ask questions.
And open-minded people also, meanwhile, will assess their relative believability to determine whether their primary role should be as a student, a teacher, or a peer.
I thought that was a really nuanced, interesting point because you actually have to be aware of what you are in different settings because you can be all three of them depending on what you're doing.
Closed-minded people focus much more on being understood than on understanding others.
And open-minded people obviously feel compelled to see things through others' eyes.
Closed-minded people say things like, I could be wrong, but here's my opinion.
And I love this because you said it's a perfunctory gesture.
Because if your statement starts with, I could be wrong, you should probably follow it with a question and not an assertion.
And then finally, you observe that closed-minded people have trouble holding two thoughts simultaneously in their minds.
So that's kind of a big summary, but I guess, Ray, what's your big summary advice takeaway there?
Most people who think that they're open-minded have formed an opinion that prejudices them and that they have to get knocked off on.
They're not reaching out with the worry that they might be wrong.
So the notion that I have an opinion and I might be wrong with that worry prompting them to pull in those others and take it in and consider them is what I'm talking about, the real open-mindedness.
Right, but where is there room for expertise?
Because I love how you also observe that it doesn't pay to be open-minded with everyone, that you should spend time exploring ideas with the most believable people you have access to.
But at some point, doesn't being believable veer into being an expert?
And so very competent people are probably more often closed-minded because they've been doing things that have worked very well for them for a very long time.
But that doesn't make any sense.
You can have your track record, but that doesn't mean that you can't go to the most believable people that you can think of who disagree with you.
Take it in.
Okay.
It's okay.
What is the harm of taking it in and considering it?
Then you still have the right to do it.
Just because you have a good track record does not mean that taking it in from the smartest people you can find who disagree with you to understand their perspective is a bad thing.
You're not losing anything.
So, are there any differences here between big companies and startups?
I mean, I feel like that's sort of the de facto thread of the questions that Alex and I are asking.
So, I want to check on that with this too.
I think all companies have got to decide how people are going to deal with each other, right?
And you have to do it, and you have to be really clear about it.
And so, if you're a big company that's entrenched, it's more difficult to make a change, and then there's the cost of that change.
Where if you're a newer company, then it's easier to make those things.
The classic innovators dilemma type of thing is actually playing out against that fabric.
Right.
But even then, that big company, you better make clear as to who is involved and make that decision.
You might even change the circle of the people.
In other words, okay, it may be the top 20 people.
Are they radically truthful and radically transparent and operating in an idea meritocratic way?
They can do that.
They can get together and say, How are we going to be with each other?
Great point.
Okay.
So, we've talked a lot about how a lot of these frameworks for decisions apply to principles for life, business, relationships, family, spouse, any all different kinds.
Let's talk about, at a very macro level, how do you think this plays out when you think about competition and innovation around the world?
Like, one of my favorite moments is in the book, you talk about your early days and how there is a sort of aspirational and inspirational period in the U.S.
in the 70s, or I think it was the late 60s, in the post-Kennedy era.
And I'm curious for where you think we are now and how it's going to play out, especially given your love of places like China.
Well, I think we're in a relatively bad spot, which is brought about by the loss of opportunity, the conflicts that we're having.
We have an enormous opportunity gap as well as an income gap, right?
And so, we have two economies: there's the top 40% and the bottom 60%.
And if you just carve out and you say, what is the economy and life like of the bottom 60%?
There hasn't been income growth, prospects of having a better life than your parents, there's a loss of hope, and so there's this wealth and opportunity gap.
The question is also how we deal with conflict and how we resolve conflict at this time.
So in other words, to make clear what are our principles that bind us together and what are those that separate us.
So do we know, are we bound together by those principles?
And can we operate in this idea meritocratic way?
So I'm saying, you know, an idea meritocratic way is first, put your honest thoughts on the table.
Second, have ways of having thoughtful disagreement so that you can get to the best answer, not just impose one thing on top of each other.
And then third, how do you have ways of getting past the disagreements that you believe are fair ways to get past those disagreements that you buy into so that you can work on these things together?
If you don't have those principles and those ways of getting through that, we will be at each other's throats.
That's a great note to wrap up on because it just shows how all these mindsets, or rather, principles, aren't just pithy pieces of advice, but they're a framework that can be applied and we can all apply these.
And actually, I don't think I've ever even written down my principles except for career stuff, like about, you know, editorial and content strategy.
I've never actually written down my personal principles.
I have to actually do that exercise.
Alex, do you have any?
I tried doing this exercise when I read the book.
I think one in general is to never judge on the present and to always judge on the potential.
And my favorite, I wrote a blog post for this actually when I first joined here.
And I think this is one of the reasons, one of the things that really separates different types of people.
There's a video of Tiger Woods when he's two and a half years old.
And he goes, I think it's on the Ed Sullivan show.
You can see this on YouTube.
And he hits a perfectly straight drive, which if you play golf, you know is pretty hard to do.
And he does this when he's two and a half years old, but he hits it maybe like 15 feet, 30 feet, something like that.
And there are two ways of looking at that video.
One, if you look at it and if you judge it by the present, you'll say, okay, well, I'm 36.
I can hit a 250-yard drive.
I'm better than that two and a half-year-old kid.
And that is completely accurate.
That is an accurate set of comparison between the world as it stands today.
The other is to try to extrapolate the potential and say, wow, if this kid continues on this current trajectory, then he can be amazing.
And in venture capital, like one of the key principles that you really have to think about is you can't just judge on the present.
You can't judge on the set of present capabilities.
You can't judge on the present state of the product.
You have to judge on the potential that it can get to.
And it's one of the things that often handicaps larger companies because people that work at larger companies too long, not always, but in some cases, they overly judge things based on the present as opposed to the potential because of the bureaucracy that just hinders quick decision-making, quick engineer of products there.
So they have to judge everything on the present.
Now that I think about it, there's actually a lot that people throw around A6 and Z as a firm.
I mean, I think they kind of borrow them from each other.
I don't really know who's or whose, but I know some of Mark's big three are strong views weekly held, don't solve problems, escalate upside, strength, not lack of weakness.
What I'm planning to do is to get the best principles from everybody and then make that all available on an app in which then people can then vote up what are the best principles for that particular thing that they're encountering.
And so then when that thing comes along, they can say, okay, here are the best principles and they can operate in a reflective way rather than just in an instinctual confused way.
Well, it sounds like we could all use that and hopefully this way of thinking helps us get to where we want to be.
Ray, thank you so much for joining the A6NZ podcast.
Thank you.
It was great.
Thank you very much.
Thanks for listening to this episode of the A16Z podcast.
If you like this episode, be sure to like, comment, subscribe, leave us a rating or a review, and share it with your friends and family.
For more episodes, go to YouTube, Apple Podcasts, and Spotify.
Follow us on X at A16Z and subscribe to our substack at a16z.substack.com.
Thanks again for listening, and I'll see you in the next episode.
As a reminder, the content here is for informational purposes only, should not be taken as legal business, tax, or investment advice, or be used to evaluate any investment or security, and is not directed at any investors or potential investors in any A16Z fund.
Please note that A16Z and its affiliates may also maintain investments in the companies discussed in this podcast.
For more details, including a link to our investments, please see a16z.com forward slash disclosures.
