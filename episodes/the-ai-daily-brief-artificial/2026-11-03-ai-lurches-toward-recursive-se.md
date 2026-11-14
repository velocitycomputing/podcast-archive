---
record_id: "podcast:a81d317d-ad35-43fe-9355-0de660c1b723"
episode_id: a81d317d-ad35-43fe-9355-0de660c1b723
title: AI Lurches Toward Recursive Self-Improvement
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/ai-lurches-toward-recursive-self-improvement/a81d317d-ad35-43fe-9355-0de660c1b723"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/ai-lurches-toward-recursive-self-improvement/a81d317d-ad35-43fe-9355-0de660c1b723"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-11-03
played_at: "2026-11-03T12:00:00Z"
play_count: 1
duration_seconds: 1560
source: pocketcasts-history-browser
played_label: November 3
history_order: 18
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 68ff6c987cd99bb9ec223e0f86ce94ae0fcc49e0779f99ddf63553d5580da9dd
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

RSI, personal-agent economics, and model self-editing dominated the discussion: Alphabet CEO Sundarpi Chai said AI is increasing training and launch velocity and expects acceleration from RSI; Elon Musk said Grockbot serving costs were unsustainably high relative to revenue after users hit usage limits, prompting Bruno Lemos, Benjamin DeCracker, Shrek, Alex Michael, Dax/OpenCode, Eric Sky, Nick Huber, and HedgyMarkets to debate whether this reflects product-category weakness, broken consumer pricing, or the end of the AI subsidy era, with one analysis cited that a full month on a $200 ChatGPT Pro plan could cost about $14,000 at regular API prices; Olivia Moore/A16Z argued Meta’s Muse could matter most for SMBs because Meta has 3.64 billion daily active users and more than 500 million SMBs use Meta for marketing; SemiAnalysis’ GDPX benchmark found Opus 5.5 most valuable at 12% and $51 per task, while Gemini 4 Carbon scored 10.9% at $16 per task, and OpenAI’s LifeVal showed GPT 6 Astra improving everyday-task success from 49.3% for GPT 5.2 to 80.6%; MIT researchers led by Rukia Takahi reported GPT-6 Astra edited 0.016% of Quen 3.5 0.8b weights, improving math 6x and instruction following 3x, with Alex Krensel/Google replicating, while Wei Zhu/Microsoft Research cautioned the math gain came from fixing a loop bug; Anthropic’s S1 update reportedly approached an RSI danger threshold of one year of progress equal to two years of the 2018–2024 baseline, and a Wall Street Journal chart showed AI leading 26% of Anthropic research, with Jack Clark and David Sachs highlighting RSI as a major technical and IPO-relevant trend.

For the user, the actionable implications are to treat AI pricing as a unit-economics problem rather than a feature problem: audit whether current subscriptions are subsidized, model-routed, or API-backed; compare cost-per-task and success-rate trade-offs, such as Gemini 4 Carbon’s 10.9% at $16 versus Opus 5.5’s 12% at $51, before scaling agents; decide whether to keep power users on API pricing or move them to efficiency-tier plans; watch Meta Muse’s SMB connector strategy, Hermes migration offers, and OpenAI’s LifeVal as signals of where consumer-agent monetization may land; treat MIT weight-editing and Anthropic’s RSI language as research leads to follow, especially replication at larger model scale, runtime self-improvement, interpretability risks, and whether “self-improvement” is true capability gain or bug-fixing; and, because the material has no direct health implications, any health-related use of these agents should be validated for accuracy, privacy, cost, and human oversight, with follow-up questions about enterprise adoption inertia, whether RSI accelerates revenue or just capability, and whether companies can charge natural token prices without losing users.

## Transcript

Hi friends, before we get into today's episode, I wanted to share that the second episode of How We Got Here has arrived.
The episode is called How We Made the Wrong Things Cheap and looks at how for 25 years the price of stuff, consumer goods, electronics, etc., went down, while the cost of housing, healthcare, and all that really important stuff went the other direction.
I think in many ways this dichotomy is at the heart of the economic populism that is increasingly dominating American politics.
For those of you who have already listened and subscribed to How We Got Here, a big thank you.
And for those who haven't yet, this is my invitation.
If you like what you get on the AI Daily Brief, I think you'll like this show.
So go check it out, How We Got Here with NLW on any podcast platform, or go to how wegothere.com.
The three letters on everyone's minds are R, S, and I.
A new MIT paper showing how a bigger model can edit the actual weights of a smaller model has people thinking about it.
And Wall Street investors who are trying to understand where the next leg of growth comes from are also digging deep into what RSI might mean.
On this episode, we're looking at a set of stories whose through line is RSI, and more broadly, what comes next for AI.
But it starts with Elon Musk casting doubt on the entire personal agent space.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, Robots and Pencils, C Data, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AI Daily Brief, or you can subscribe on Apple Podcasts.
And to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
Two more quick announcements.
As you just heard, the second episode of How We Got Here is now out.
It's called How We Made the Wrong Things Cheap.
And for any of you who are interested in the economics of the modern American economy, where by some measures we're doing better than ever, but everyone feels more behind, if you want to know how that came to be, that episode is for you.
You can find it at howwegothere.com or by searching how we gothere with NLW on any podcast platform.
The second note is that I am traveling this week for my anniversary and basically coming to you live from the jungle.
So if you happen to hear bird sounds or water trickling, or let's just call it more nature than usual, that is why.
I hope you enjoy these various nature sounds for the next couple of days.
Next week, we will be back to normal.
One of the conversations that has been swirling around quite a bit throughout 2026, but especially over the last couple of months, is what it means for the AI industry and society more broadly that AI models are getting closer to being able to improve themselves.
On Alphabet's recent earnings call, CEO Sundarpi Chai said, We're at the point where AI is helping us increase our training and launch velocity.
I would expect the next 12 months to see continued acceleration because of RSI.
Now, today's stories are not exactly all about RSI, but there is a through line in how the continued acceleration of AI meets adoption of AI, how that impacts market potentials, and what the state of RSI actually is.
The first then of our troika of stories comes after a seemingly nonchalant, but not really at all nonchalant, post from Elon Musk, where he said over the weekend, the cost of serving Grockbot was unsustainably high relative to revenue.
The genesis of this had been that over the weekend, Grockbot users complained that they were starting to hit usage limits that had never been a problem before.
Elon was responding to someone's request to increase or reset those usage limits.
Now, Elon didn't give any more details.
It's unclear through which plans users were accessing Grockbot, but for those watching the AI space closely, especially market bears, the post hit with the force of a bomb.
For some, there was a weird contradiction in Elon's communications over the past couple of weeks.
Just a couple of days ago, he had posted, saving money for the distant future is pointless with the advent of super intelligent abundance.
But as Bruno Lemos and others pointed out, just a couple days later, he's talking about costs being too high.
Benjamin DeCracker went a little bit farther back, resharing an Elon post from a couple of weeks ago, when he said, Never seen anything grow as fast as Grockbot.
And there is no free tier, which means people are deriving real value in excess of what they pay.
DeCracker writes, Two weeks ago, Grockbot was an incredible success story powering SpaceX AI's revenue growth.
Now it's unsustainable and loses money?
For some, Elon's weird communications were entirely secondary to the feeling of betrayal around the plans.
User Shrek said, This isn't about us not having enough usage or picking the wrong plan.
I've been buying the 12-inch pizza from your place forever, and you guys have always given me a normal 12-inch.
Then one day I open the box and it's a 6-inch.
You tell me costs are too high, so from now on, the 12-inch is actually 6 inches, and if I'm still hungry, it's my fault for not choosing the right size.
That's insane.
If you needed to cut costs, just tell us ahead of time.
If your pizza is good and I still want it, I can just order two or three of these fake 12-inch ones.
Or if I'm not full, I can go somewhere else.
Either way, that's my call, not yours.
But you don't get to keep selling me a normal 12-inch and then suddenly shrink it to six inches with zero notice, not even a heads up so that I can adjust.
Don't turn around and say I picked the wrong subscription.
The problem is you unilaterally changed what you were delivering without telling anyone.
Others thought that inevitably this was good news for the other personal agents.
Alex Michael wrote, This is a huge win for Dots and Duet and will most likely drive a lot of users right back to them.
News Research, the makers of Hermes, of course, jumped all over it and shared specific instructions on how Grockbot users can migrate to Hermes.
But the most interesting discussion, whether the issues that Elon and SpaceX are running into are less about anything having to do with SpaceX and their position in the AI race, and more about the fundamentals of this product category.
Dax from OpenCode reposted Elon and said, This is another major reason why we weren't super excited about this shape of product, by which presumably Dax means personal agents.
Continuing, he says, People don't want to pay for it, so it has to be a top-of-funnel product that leads to something else.
Not sure what the something else could be yet.
Now, careful observers will note that this sort of conversation about the cost center that is free AI users on free consumer tiers that will never pay and how it impacts the ability of the company to monetize more broadly has been around for a very long time.
It was a major subject of discussion in the fall 2025 vintage of bubble debates, where people were basically concerned that OpenAI's breakaway ChatGPT success could actually be a hindrance because of how much it costs to support all of those free users.
For as long as we have been talking about personal agents, especially this year as they've gotten more real, there have been some who have applied those same sort of claims that since consumers aren't willing to pay for this category of product, they're just going to be a cost center for the people offering them, and they're going to have to be made up for in other ways.
And that remains an open debate.
And certainly, market skeptics jumped right to what this might mean for all the other companies offering these products, which includes very notably Meta, who have been riding high on the fact that Muse's leading place in this category has given them a foothold in the AI race more broadly.
Certainly, the Bears were very happy to jump all over this as fait accompli that the bubble was done and the game was over.
Eric Sky writes: Elon is going to abandon the race.
Second warning.
Nick Huber, who is all about traditional boring businesses and very skeptical of many categories of tech startups and certainly AI, got on his high horse and said, This is all of AI right now.
The music will stop.
Better find your chair.
VC money runs out, means prices rise dramatically, means users drop off, means valuations plummet.
HedgyMarkets thinks it's just another sign of the end of the subsidy era.
They wrote, Grok users ran out of usage days early this week, and Musk was straight with them about why.
This is the end of the subsidy I wrote about in this week's newsletter.
AI companies price their plans below cost to win users, and that only works while investors cover the difference.
A full month on a $200 ChatGPT Pro plan would cost about $14,000 at regular API prices, according to one analysis this summer.
Now, I think by that he's referring to semi-analysis, but his note that this was the discussion this summer is worth taking a moment on.
You might remember that we did an AI subsidy era episode back at the end of April.
The episode not only argued that the AI subsidy era was coming to an end, but tried to provide a set of actions for businesses to adapt to it.
So make no doubt that this is not some new conversation, and it has been inevitable for quite some time.
For whatever reason, we got distracted by other things for a couple months over the summer and stopped talking about this.
But now that there's so much bubble analysis once again and critical analysis with Anthropic getting close to IPO, the story is back because, of course, the debate about the implications was never resolved.
The bare case with these subsidies ending is basically that when AI companies actually have to charge the correct or natural rate for their product, i.e., charge customers what the tokens actually cost plus a little bit of margin for themselves, not a version of that that is subsidized by someone else, like venture capitalists and private equity investors, that people don't value or can't afford to value the intelligence at that natural price enough to continue spending in the way that they have been.
And thus it means that all the valuations of all these companies are off.
That is a possible outcome.
And I think it's completely reasonable for market actors to try to figure out how to price in that risk.
In fact, in general, I will say here that despite the fact that I am very much not an AI bear, I have no issue at all with the AI bears in the market right now.
I think it would be much more dangerous if everyone was too enamored of Anthropic and OpenAI to actually ask these critical questions.
I think that likelihoods of a bubble are decreased in proportion in some ways to the loudness of the bears and the resonance of their message with a broad base of investors.
Now, I also, of course, think that there's a wide spectrum of the quality of bearish analysis, and that perhaps listening to the perma bears who have gotten it wrong for years and continue to move the goalpost to get it right might not be your best play.
But overall, I think their voices are an important part of the market segment, and I think it's valuable that investors are taking time to price in the risks that they're talking about.
So, all that said, I don't particularly think that the shift to API pricing for everyone actually changes all that much.
Basically, I think that the plan users shift into one of two categories: the people for whom the models that come with more efficiency trade-offs are good enough for their types of uses, who stay on their $20 or $30 a month plan because for their use cases, it doesn't change all that much.
And then, on the other side, the people who are getting enough value out of whatever plan they're on, whether it's $20 or $200, that they're willing to actually pay for the intelligence they consume and just treat it as a cost of doing business.
I'm certainly not a super normal example of this, but I have APIs running all over the place in addition to my premium plans, and there's absolutely no doubt that the value that I get out of them is well worth the cost.
I do things with those APIs for yes, a premium cost, but a premium cost that's still far below what the comparative human labor would have cost, which by the way, is not a one-to-one replacement because the human labor would have cost too much in both actual money as well as time to recruit and manage those people.
So, from an economic perspective, this is net new money that I'm spending that I would not have spent before.
What I believe that we've seen in 2026, basically since the rise of the agentic era, is that a huge amount of the revenue on an actual percentage basis is coming from power users who are already paying via the API.
In fact, I think there's a bit of a weird contrast between two bare arguments sitting next to one another.
Is it that when people start paying on the API, people are going to drop off and stop using AI because they don't get enough value out of it anymore?
Or is the market too concentrated among a very small number of power users?
Now, of course, the more nuanced in-between argument here is the one that you've seen people like Chamat Palahapatiya make that argues that too many of those power users are currently subsidized by VC dollars, and that could present some significant problems.
I think that's a much more interesting thing to explore.
Still, right now, we don't know.
And all that we have is this sort of interpretation.
Hello, everyone.
One big change around AI is we've shifted our thinking from how we rank our pages to how do we become the source that AI trusts enough to answer with.
At KPMG, they're seeing this firsthand.
AI-generated results now surface answers directly, often without a single click.
That's why they are increasingly focused on generative engine optimization or GEO, structuring content so AI systems can retrieve it, understand it, and cite it as trusted authority.
This is not just an SEO evolution, but a visibility mandate.
And indeed, the GEO mandate from KPMG is simple.
If AI is shaping decisions, your expertise needs to show up inside the answer.
Read all about it at kpmg.com/slash/us slash geo.
Again, that is kpmg.com/slash us slash geo.
The best teams don't have a single star carrying everyone else.
They know their own strengths and each other's weaknesses and play to both.
That's the team Robots and Pencils has built on purpose.
Nobody there is grinding through busy work to pad a headcount number.
People come for the hard problems and they stay because everyone around them is leveling up at the same time.
In a market full of companies that are just trying to hire fast, that's worth a look.
Check out robotsandpencils.com/slash careers.
This episode is brought to you by C Data.
Companies rolling out AI keep hitting the same wall.
Token spend is climbing, security is holding agents back, and no one knows how AI is truly being used.
The root cause, AI is cut off from the systems and context your business runs on.
That's why C Data built Connect AI Gateway, one control point between your AI and your systems.
Built on the connectivity layer powering Palantir, Google, Salesforce, and hundreds more, each agent gets exactly the data and tools it needs.
It governs down to the record and lets you finally see your org's complete AI usage in one place.
Accurate answers, a fraction of the token cost, and a gateway that learns your business with every interaction.
See how at cdata.ai.
Blitzy deeply understands your code base before it writes code.
Here's the first place that pays off: security in the age of AI.
Vulnerabilities don't live in isolation.
They live buried inside millions of lines of interconnected code where patching one thing quietly breaks three others.
That's why surface level scans fail.
Blitzy starts from its knowledge graph of your entire application, identifies and surfaces CVEs across the full estate, proactively recommends patches, and can execute the PR.
Each fix is grounded in how your systems connect and validate so nothing new breaks.
And the knowledge graph dynamically updates, keeping you ahead of an ever-accelerating threat landscape.
One Blitzy customer resolved 21 active CVEs across six core microservices in four days.
Zero compile errors, every validation scan clean, months of planned work fixed in less than a week.
Security remediation grounded in real architectural context at the speed of compute.
Harden your code base at blitzy.com.
That's B-L-I-T-Z-Y.com.
Certainly, it's the case that Elon Musk is not above fanning the flames of panic in the market.
After Core Weave's bonds had a particularly bad day last month, Musk commented yikes, which got picked up across the financial press.
And later in October, he said, debt markets have almost entirely shut off access to money for any company that doesn't have substantial revenue independent of AI data centers.
There are more than a few people who think this is some version of 4D chess, with Musk pushing the markets to sell off harder in hopes of making some cheap acquisitions or harming rivals.
But right now, we just don't know.
What we do know is that there are still some companies who are betting very heavily on personal agents, even if Elon seems to be pulling back.
Olivia Moore from A16Z thinks that when it comes to Meta's Muse, the real story isn't even really consumer, it's Muse for small businesses.
She wrote, Muse for SMBs might be the most underrated story in consumer agents right now.
They have near-infinite consumer distribution at very low cost, with a base of 3.64 billion daily active users across Meta apps.
But even more importantly, more than 500 million SMBs use Meta for marketing.
If Meta gives agent discoverability to that SMB base, it could be a huge boost, especially for local businesses who can hyper-target users with urgent purchase needs.
Meta said in their Q3 earnings call and in blog posts prior that they plan to build an ecosystem of connectors for SMBs and Muse.
Analytics across your meta accounts plus QuickBooks, Canvas, Stripe, et cetera.
Many of these businesses are already trusting Meta with their growth in ad dollars.
I could see Muse becoming almost a nervous system for SMBs that allows Meta to capture more and more of their activity over time.
Interestingly, even as these discussions about the viability of personal agents were swirling, we got two new benchmarks introduced that go some way towards measuring the value of these sort of personal agents.
The semi-analysis benchmark is called GDPX and is focused on economically valuable tasks like chip design, finance, and biology.
They found that Opus 5.5 was the most valuable model to drive an agent, scoring 12% on their scale at $51 per task.
Gemini 4 Carbon was in second place at 10.9%, but only cost $16 per task.
Chubby INX jumped right at this question of efficiency.
He wrote, While performing just 1.1% worse, Gemini 4 is about 4x cheaper than Opus 5.5.
So cost performance-wise, Gemini 4 wins by a lot.
And one of the obvious questions that clearly the labs are thinking about right now is how to use more efficient models to drive down the costs of personal agents, similar to what has been a focus with coding agents across this year.
As we'll see later, there's all sorts of buzz around new training techniques as well, that leads some to think that it's possible that we'll see stronger, smaller models in the coming year that make personal agents a lot more cost-effective.
OpenAI's new benchmark, meanwhile, called LifeVal, sets out to measure the value of personal agents in everyday life.
Writes OpenAI, for the more than 1 billion people who currently use ChatGPT every week, we want to build AI that can help with the practical challenges of everyday life, like finding childcare, accessing government services, creating a budget, preparing for school, modifying recipes, ordering groceries, designing workout plans, and more.
OpenAI's scoring shows the steady increase in capability from GPT 5.2 to GPT 6 Astra, rising from 49.3% success to 80.6% success.
More importantly, OpenAI is now measuring and hill climbing against these everyday tasks with free users in mind.
As we've seen with coding, once a capability is measured and becomes a target for reinforcement learning, it dramatically improves and becomes more cost-effective.
Fraser X commented: Forget all the flashy AI benchmarks, LifeFal is arguably the most important benchmark for 99% of AI users.
This is what actually matters.
Simon Smith wrote: Feels like this is the kind of post you publish right before releasing a personal agent to the general public.
Question for me is whether ChatGPT gets better at being a personal agent before Muse gets widespread voice mode.
ChatGPT's voice mode is awesome, but Muse is the better personal agent.
And yes, I use dots at work and try them for personal use so I know what they're capable of and still prefer Muse.
Now, let's actually move over to the story that, with just a glance at the AI community, seems to be the biggest one of the day.
As you'll see, it potentially has some implications for all of these cost questions around personal agents.
The TLDR is that MIT researchers have published groundbreaking research that could change the way that model training works.
Led by PhD student Rukia Takahi, the researchers found that GPT-6 Astra was capable of reading and directly adjusting the weights of a small model to improve its performance.
The experiment used Quen 3.5, 0.8b, and targeted improvements in reasoning.
Astra changed only 0.016% of the weights, and yet was able to improve Quen's scores on math benchmarks by 6x and instruction following by 3x.
In their abstract, the researchers wrote: We find that Frontier LLMs are surprisingly good at natively reading and writing neural network weights, well past what we'd expect from humans or conventional algorithms.
This might be a big deal for both optimization and interpretability.
Just by looking at the weights, GPT-6 Astra can tell what a network was trained to do, and without any environment feedback, it has no trouble writing from scratch small game-playing networks that outplay networks trained with PPO for 100 million steps.
PPO, or proximal policy optimization, by the way, is a standard reinforcement learning algorithm in use by the major labs.
The research is worth reading in full, or having Claude or ChatGPT read and talking to it about, and includes multiple surprising results.
But when it comes to altering Quenn's weights, the process was extremely straightforward.
Takahi wrote, We simply asked Astra to make Quenn 3.508B better at math.
Astra saw Quenn get stuck in reasoning loops, which is a known issue that Quen's own model card warns about.
With a budget of 50 forward passes on practice problems, it located the cause and edited it out.
This used no gradients or training.
Fixing these loops by editing just 0.016% of weights boosted other capabilities beyond math too.
People were incredibly excited about this result.
Yu Chen Jin wrote, This is cool as heck.
Imagine using a large LLM to directly edit a smaller model's weights and dramatically improve its capabilities.
It's like gene editing for neural networks, even cooler than distillation.
Developer Nick Dobos wrote, Astra can hand-write new weights from scratch that outperform other AI training techniques?
What?
They buried the lead.
Improving math via a looping bug fix is very cool, but debugging and fixing weights is quite limited versus generating brand new weights.
If this works, is training large AI models even needed anymore?
Is this true RSI?
And for those like Professor Ethan Mollik, who said, this seems really cool, but let's wait for some replicated results.
Well, it didn't take long for Alex Krensel, a senior researcher at Google, to replicate the results.
Alex noted, this is a new step change emerging capability that's appeared in just the latest set of models.
Now he did continue: some very important caveats to understand these results.
Note that the models being edited here are very small.
The breakout model in their post in My Experiment is 20,486 parameters.
Frontier models are more than a trillion parameters.
The way that I'm thinking about it is this.
There's a whole body of work of interpretability research from the 2010s.
A la look at model, this neuron lights up when image contains dog, so this is the dog neuron.
This seems akin to that, but scale beyond human capability.
We've done this by hand for smaller models, then we built tools to help this for slightly bigger models.
What we're seeing is the reasoning capabilities are enabling the models to do this by hand for much larger, but still relatively small models.
Krenstel added that the obvious next step in the research is to test self-improvement at runtime, which he believes won't be feasible for current models but could work within a few generations.
As you might expect, whenever you have big, bombastic claims like this, there's going to be a pretty heated debate about whether the results were overhyped.
Chandan Singh from Voyage AI commented, For anyone questioning whether this post is overhyped, I think they are actually underselling the approach.
We did similar experiments and found that Claude models can write entire functioning neural net weights from scratch.
On the other side were people, however, like Wei Zhu from Microsoft Research who said, the findings are pretty interesting indeed, but I think the headline is kind of overhyped.
The 6x improvement on math came from fixing a loop bug in the original model, not from improving general math capability.
And this was the main critique that this is less about a new model training technique and more akin to a bug fix in an existing model.
And yet for others, this was clear evidence that recursive self-improvement is not only a possibility in the future, but now has a clear mechanism that's understood and has been demonstrated in an academic paper.
Tenebris wrote, I think you should strongly expect something like this to happen in the next year and for it to be one of the driving factors of RSI, and potentially quite steep RSI.
Interpretability is incredibly dual use.
Models that are good at optimization writ large are good at optimizing themselves.
Now, RSI was also the main point of discussion around an update of Anthropics S1 that they released on Monday morning.
AI news aggregator Andrew Curran wrote: New language added on Anthropics S1A this morning says that internal estimates indicate they may imminently meet the RSI danger threshold of dramatically accelerated progress attributable to AI, as much progress in one year as two years of the 2018 to 2024 baseline.
They added that they are considering updates to their responsible scaling policy because they, quote, do not anticipate being able to safely use Claude to fully autonomously design and build successive generations of frontier models without meaningful human supervision or understanding.
Basically, the new changes will be aimed at keeping humans in control of frontier model development rather than handing research over to the model entirely.
Certainly, it is the case that financial professionals are taking note of RSI as one of the most important factors for the IPO.
The Wall Street Journal published a chart from Anthropic showing that AI is now leading 26% of research.
Their headline read: The smartest people in AI believe this is the world's most important chart.
AI is starting to build better AI, the self-improvement is speeding up research and development, and freaking everyone out.
The headline seemed to reference Anthropic co-founder Jack Clark, who said that RSI, quote, might be the most important technical trend in the world.
Anthropic first published this chart, by the way, back in September, based on August numbers, and it was boosted by former AI czar David Sachs over the weekend.
Still, with the AI narrative beginning to sour, or at least having more questions as we've been exploring, it's notable that Wall Street investors are paying attention to the possibility that RSI leads to faster advances in model capability.
As Sachs commented, that was back in August, so who knows what they're at now being in October.
Now, one thing I find interesting about that discussion is the presumption, so deeply embedded that no one feels the need to say it, that the key to greater adoption is improved models.
The evidence that we have for that is that true step changes have unlocked new capabilities that have led to massively more adoption in the past.
The most notable and important of these, of course, was the Opus 4.5 jump that led to the full agent to coding era that we've been living in ever since.
In the absence, though, of some entirely new capability coming online, I don't think the evidence suggests that the key to improved adoption is solely model capability.
I think ultimately, when it comes to whether these business models work or not, it's more or less a question of how much intelligence enterprises consume.
They are at the moment consuming a vanishingly small portion of what they could, and it's not because the model capabilities aren't high enough.
It's because inertia is real, corporate systems are lumbering, and adoption is hard.
Now, I think you could write a bear case or a bull case based on that.
The bear case is that even with all this power, we're not using it.
The bull case is, no, we're just not using it yet.
Regardless, whatever investors want to tell themselves about RSI and its impact on adoption is fine.
I'm just not sure model improvement has quite such a straight line to increased revenue as we might intuitively think.
What I will say is that at least some of those investors are starting to ask what happens when we have RSI, not just how close to it are we.
It feels like we're still stuck, broadly speaking, is RSI here yet or isn't it, discussion, rather than what it means when it arrives.
Right now, the only group offering any sort of vision for the world of RSI is the AI safetyists who are terrified of it and think it should be illegal.
We may not agree, but at least they're actually articulating what they think the world is going to look like after that if and after RSI comes.
It strikes me that, like the AGI term before it, we may be getting so distracted with this three-letter acronym that we're spending more attention on trying to define it and articulating how close it is to being here than understanding what it will mean when it arrives.
In any case, it continues to be a fascinating time in AI, but that is going to do it for today's AI Daily Brief.
Appreciate you listening or watching, as always, and until next time, peace.
