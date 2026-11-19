---
record_id: "podcast:cf10fe4b-f4a1-4c20-9465-cf615ca49de3"
episode_id: cf10fe4b-f4a1-4c20-9465-cf615ca49de3
title: Why the AI Kids Hate Astra 6.2
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/why-the-ai-kids-hate-astra-62/cf10fe4b-f4a1-4c20-9465-cf615ca49de3"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/why-the-ai-kids-hate-astra-62/cf10fe4b-f4a1-4c20-9465-cf615ca49de3"
feed_guid: null
feed_url: "https://anchor.fm/s/f7cac464/podcast/rss"
published_at: null
published_local_date: null
played_date: 2026-11-18
played_at: "2026-11-18T12:00:00Z"
play_count: 1
duration_seconds: 360
source: pocketcasts-history-browser
played_label: Yesterday
history_order: 1
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 67bc2e901486a3e5c74532e027b16004afa2eb0d2cc4ab500216df66a2770271
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

OpenAI’s GPT-6.2 Astra and Sol release, a wave of high-profile outages, and NVIDIA’s post-Jensen Huang earnings dominated the episode. OpenAI presented the models as “super efficient” and “built to perform where it counts, the real world,” leading with agents and terminal-bench science rather than coding benchmarks; Artificial Analysis reported Sol rising from 55 to 57 and Astra rising 5 points to 62, behind Fable 5.2, with Astra at about $4 per task, a 35% reduction, and Sol at $101 versus $127, but both regressed on the coding-agent index, with Sol dropping three points behind Kimmy 3.1 and 6.1 Terra due to Suite Atlas omissions. Early testers including Matt Schumer, Dan Shipper, Theo, and Ethan Mollick called the models uneven, frustrating, or a step back on writing, coding-agent tasks, and design variety, while Ash, Claire Vaux, Josh Pertell, Alex Finn, and Z-Wen praised efficiency, computer-use workflows, animation/image generation, and benchmark speed; OpenAI’s Tebow said some negative reviews predated late changes, though Token Gremlin criticized the early-access process. The episode also covered outages at Microsoft Outlook, the FAA, major banks, Apple, United Airlines, and the NSA’s NSANet, with sources and ONCD’s Sean Cairncross pointing to legacy-system modernization rather than cyberattack, and the host argued that since Mythos/Fable-level models, companies have raced to update old systems, causing failures. On NVIDIA, Jensen Huang thanked supporters and said he would return if the board wanted, but board chair Harvey Jones and interim CEO Colette Kress said the board would not reinstate him, while reports said some board members still pushed for his return; NVIDIA beat estimates with 103% annualized growth, raised Q4 revenue guidance to $130 billion, lifted 2028 growth expectations from 70% to 75%, stopped shipping licensed Hopper data-center chips to China, and saw shares rise 2% after Huang’s post and 4.5% after hours. Sponsor segments promoted KPMG, Granola, Gartner, and Blitzy.

There are no direct health implications in the material; the actionable items are operational and strategic. For AI adoption, treat GPT-6.2 Astra and Sol as a cost-efficiency play rather than a universal upgrade: run your own evals on real tasks, separate model quality from harness problems, and compare token efficiency, latency, and cost per completed task against Opus 5.5, Fable 5.2, Gemini 4 Carbon, and older GPT models before switching. If coding, agentic builds, long-form writing, or design variation are core workflows, test for premature stopping, omitted facts, overly terse answers, and repetitive house style; if computer use, video editing, animation, or high-volume enterprise automation are core workflows, the efficiency gains may justify adoption. The outage cluster suggests a research lead: ask IT/security vendors whether recent Microsoft, FAA, banking, airline, or NSA-related incidents reflect planned legacy modernization, and review your own update, rollback, and incident-communication plans, especially if AI-driven modernization is accelerating. For NVIDIA exposure, follow the board’s CEO decision, the pending SEC filing, and revenue impact from halting licensed Hopper shipments to China; for AI strategy, decide whether OpenAI’s positioning is about enterprise cost control and non-coding professional work rather than head-to-head coding superiority, and monitor whether Anthropic’s IPO narrative or OpenAI’s post-IPO messaging changes procurement choices.

## Transcript

OpenAI has just dropped their latest models and the response is not so great so far.
But is this about the models underperforming?
Or is it more about where OpenAI's strategy is headed next?
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, Granola, Gartner, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AI Daily Brief, or you can subscribe on Apple Podcasts.
And if you want to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
One of the big stories that is not necessarily about AI, but people assume is about AI that has been driving the conversation over the last week is, of course, this mysterious slate of shutdowns that has run through Microsoft Outlook and the FAA, a bunch of big U.S.
banks, and now, as of Tuesday, the NSA's Internal Communications Network.
The network, known as NSANet, is a secure communication system designed for communicating classified information internally.
Sources told CNN that the NSA's campus was closed to most employees on Tuesday night, reverting to essential personnel only as they worked to restore the network.
As has been the mantra every single time here, the sources said that at this stage, there is no evidence of a cyber attack.
In a statement on Tuesday afternoon, the agency said: The National Security Agency experienced temporary degradation during scheduled routine maintenance.
While some internal systems were affected, mission-critical capabilities remain fully operational, and our ability to defend national security continues.
NSA's infrastructure is designed with multiple layers of redundancy to maintain operations during planned maintenance or unexpected events.
And yet, for those who had already been alarmed about Microsoft and the FAA and JPMorgan, all experiencing major outages in the space of a week, an outage at the NSA could feel like a troubling escalation, especially when paired with other outages for Apple and United Airlines, which also happened on Tuesday.
To some, the only answer that makes any sense is that we're in the middle of some ongoing undisclosed cyber attack enabled by advanced AI tools.
And yet, in this case, there is an answer that is related to AI, but that isn't cyber attacks.
A16Z's Martin Cassado hinted at this when he posted: All these outages remind me of Y2K when the primary service disruption was from upgrades.
When reporter Ashley Gold asked ONCD's Sean Cairncross about whether it could be a cyber attack, he said, What we're seeing, and frankly, I'd expect to see more of it, are service disruptions coming from updating and modernizing legacy systems.
This is something that's happening in real time, and at the end of the day, we're going to have to get through this to get systems where they need to be.
The industry's known this for a while, it's just that it's manifesting.
Mackenzie Arnold reposted that and added, Maybe the surge in outages is actually downstream of AI, but in a less concerning way.
Real concerns about automated cyber attacks may be causing a surge in major updates.
A surge in updates equals a surge in failures.
And add in the fact that AI is also making many of these updates affordable and feasible for the first time, and that there's a lot of experimentation with new AI integrations.
And people could be absolutely right that this isn't a coincidence, even if it isn't attributable to undisclosed cyber incidents.
Basically, the idea is: we have been on a ticking clock ever since we got to Mythos slash Fable level models.
Quietly, companies have started to race to get their systems up to snuff, but a lot of the systems that they are upgrading are painfully old.
And when you push on something that's been held together with popsicle sticks and bubblegum for 30 years, stuff starts to break.
Add on top of that, the fact that everyone is doing this all at the same time, meaning specialists who can help clean up these issues, are stretched farther than they have capacity for, and it starts to look more like almost what one would predict, rather than some crazy coincidence.
Now, none of this is, of course, to dismiss the possibility that at some point we could slash likely will see a spade of cyber attacks, but this is the type of thing that I would expect to happen in the process of hardening for that eventuality.
I will, of course, keep an eye on this to see if that evidence changes.
But for now, we move on to our standard daily NVIDIA briefing, where Jensen Huang has spoken out for the first time since his resignation last Thursday.
In an ex-post on Tuesday morning, he wrote, Over the past week, I've been overwhelmed by the love and support of friends, industry colleagues, and people I've never met.
Thank you to everyone who has shown kindness to my family and me.
It means the world to me.
I came to the United States 53 years ago, and becoming an American citizen is one of the greatest gifts and proudest moments of my life.
NVIDIA has been my life's work.
Building it into the company it is today alongside my colleagues has been a privilege and an honor.
Nowhere but in America could a company like NVIDIA be possible.
I love our country and I love NVIDIA.
I did not live up to the standards expected of everyone at NVIDIA, and I have made serious mistakes in my personal life.
I created problems for the board that I deeply regret.
I own my mistakes completely and I am committed to cooperating with the board's independent investigation.
Since my departure, I've seen an outpouring of calls from NVIDIA's employees, investors, business partners, and customers for me to return as CEO.
Many continue to reach out to me directly as the company navigates complex technology, market, competitive, and geopolitical dynamics.
NVIDIA is a once-in-a-generation company.
If the board of directors decides that my return is in the best interest of our shareholders, our employees, the company, and America, I would be honored to answer these calls and return a CEO.
The tech world was out in force to support Jensen's return.
Why Combinator founder Paul Graham did not envy the situation the board is in, commenting, Imagine being a board member at NVIDIA considering potential candidates for CEO and trying to claim with a straight face that one of the others would do a better job.
The market also seemed to be voting to bring Jensen back, sending NVIDIA stock up by 2% in the five minutes after Jensen posted.
Last week, former tech executive and tech philosopher Balaji Srinivasan wrote, All Jensen Huang had to do is tweet that he wants to be reinstated as CEO and gears will start moving.
Well, Jensen has now tweeted.
But in the evening during the earnings call, the NVIDIA board made it clear that the gears are not turning.
The call opened with an announcement from newly appointed board chair Harvey Jones who said, the board unanimously accepted Jensen's resignation and does not intend to reinstate Jensen as CEO.
Prior to the call, interim CEO Colette Kress had also shut down the idea, saying in a CNBC interview, Jensen resigned from his position with NVIDIA and the board accepted his resignation.
The board has determined that they will not reinstate Jensen, and that is our statement and what the board has decided to do.
We want to think right now about growing our business.
We want to grow in terms of everything that we need to do with our employees, our customers, our shareholders, and that is where we are going to focus moving forward.
And yet, later in the evening, Semaphore delivered a scoop from inside the boardroom, reporting that a faction of board members are pushing for Jensen's return.
Jensen has also reportedly spoken with at least one board member about returning, doing so prior to his Tuesday morning post.
According to people familiar with the matter, three board members are vehemently opposed to Jensen's return, but where the other seven stand isn't as clear.
Now, as to the substance of the earnings report, NVIDIA delivered another extremely strong quarter.
They beat revenue estimates with 103% annualized growth and raised projections for the fourth quarter to $130 billion in revenue.
CEO Kress also raised forecasts out to 2028, adjusting growth expectations from 70 to 75%.
Kress projected an air of confidence, ending the call by stating, Our supply is growing, our customers and our partners are with us, and employees are committed.
We've got this.
The stock was up 4.5% in after-hours trading to reach a new high for the post-Jensen period.
Wedbush securities analyst Matt Bryson was satisfied with what he heard, commenting: Colette is exuding the same confidence that you heard from them last quarter.
However, he acknowledged the skeptics, saying, I don't know if it changes people's opinions.
NVIDIA themselves seem to be changing their opinion on China for some pretty understandable reasons.
During the call, Kress announced that NVIDIA would no longer be selling AI chips to China, even the ones that have government approval.
It's unclear how many H-200s have actually shipped since they were approved by the Trump administration earlier in the year, but Kress said, Our guidance does not have any licensed hopper data center products included, and we are no longer shipping licensed Hopper data center products to China.
Important to note that this earnings report does not cover the events of the past few weeks, so we don't know yet how much revenue will be lost from shutting down smuggling routes into China.
They also haven't completed their official SEC filing that goes along with the earnings call, flagging that it would be filed in the coming weeks.
And board chair Harvey Jones acknowledged that NVIDIA is now living in a world where, quote, national security dynamics are making major changes in our marketplace.
The next CEO will have to navigate those waters very carefully.
This story, alas, continues to feel not quite over.
However, for now, that is going to do it for the headlines.
Next up, the main episode, and maybe the most hated model release I've ever seen.
If you're leading AI inside an enterprise, you already know that the gap right now isn't capability but execution.
That's why KPMG's You Can with AI is back with a new season featuring conversations with leaders like Sorojit Chatterjee of Emma, Mehabib of Ryder, McKesson CIO Ellery Fisher, and others focused on practical execution: what's working, what's not, and what it actually takes to move from pilots to real-scaled impact across strategy, data readiness, governance, workforce, and value.
And of course, it's co-hosted by me, Nathaniel Whittemore.
Go listen and subscribe at www.kpmg.us slash ai podcasts.
That's www.kpmg.us slash ai podcasts.
You're in back-to-back meetings all day.
You're trying to stay present, but you're also worried you'll forget the decision, the action item, the important next step.
This is a scenario that we absolutely live here at the AI Daily Brief, given how fast things move and change and how quickly we're evolving everything that we do.
That's where Granola comes in.
Granola is an AI-powered notepad for meetings.
You jot down rough notes like you always do, and in the background, Granola transcribes and turns them into clear, useful notes when the meeting ends.
No bots joining your calls, no distractions, just a clean notepad that helps you focus.
During or after the call, you can chat with your notes.
Ask Granola to pull out action items, help you negotiate, write a follow-up email, or even coach you using recipes which are pre-made prompts.
Once you try it on a first meeting, it is very hard to go without.
Head to granola.ai/slash AI Daily and use code AI Daily to get 100% off for three months for new users.
That's granola.ai/slash AI Daily and Code AI Daily to get 100% off for new users for three months.
When it comes to AI risk, C-suite leaders have serious questions.
Can your cybersecurity keep pace with AI-powered threats?
As threats expand beyond IT, are your physical assets safe?
Do you trust your AI vendors to deliver value without taking your proprietary data?
Are you prepared to handle swarms of AI agents?
Find out how they can help.
Visit them at gartner.com/slash AI to learn more.
Here's why most legacy modernization projects fail.
The AI doing the work can't understand code bases at scale.
It sees a small slice of context, examines syntax, and misses years of decisions distributed across the global application ecosystem.
Blitzy solves this the way it solves everything.
Grounded in your code before any migration begins, Blitzy's agents reverse-engineer the entire legacy system into a persistent knowledge graph.
Every dependency, every constraint, every piece of tribal knowledge that used to live in one engineer's head.
From that understanding, Blitzy autonomously executes language migrations, framework upgrades, and monolith to microservices transformations, all validated end-to-end.
One Blitzy customer modernized a $10 million monolithic insurance stack in 16 weeks against a 137-week baseline with coding agents.
That's 9x compression.
Retire technical debt while accelerating your roadmap.
See how at blitzy.com.
That's B-L-I-T-Z-Y.com.
Welcome back to the AI Daily Brief.
Today we are doing one of my favorite types of episodes, although this one has a bit of a different flavor.
One of the big questions for this week was whether OpenAI would actually try to drop some sort of spoiler model in advance of the Anthropic IPO.
Now, spoiler model itself might be an overstatement, in that even without any sort of desire to spoil anything for Anthropic, OpenAI has felt due for an update for a while now.
Well, on Tuesday, we did get a new model.
Two, in fact, GPT-62Astra and GPT-62 Sol.
And unlike the usual excitement, we got some of the worst first impressions that I have ever seen from a model.
And I'm not just talking about the GPT-5 era, when people were angry for other reasons, like GPT-40 being deprecated.
I'm talking about posts like this one from Matt Schumer, who wrote, I will not be writing a full review of GPT-6.2 Astra and Sol.
I had a terrible experience testing them.
They were essentially unusable.
I do not recommend these models.
So, what is going on here?
Are these models as bad as the early testers say?
Or does this show an increasing divide between what types of uses OpenAI is trying to build for relative to what the early adopter set cares about?
Now, in my estimation, OpenAI is telling a pretty clear story of how they see these models.
To quote their announcement post, super efficient and built to perform where it counts, the real world.
You can also see this sort of focus in what they emphasize in the announcement post.
They lead with agents last exam and terminal bench science rather than the sort of coding benchmarks that had been right at the top for pretty much every release for the last year.
And even when they get to code, the major selling point is still about cost.
On the Artificial Analysis Intelligence Index, both model releases were a slight improvement.
GPT 6.2 Sol increased its score by two points from 55 to 57, pulling even with GPT-6 Astra, but still behind Opus 5.5, Gemini 4 Carbon, and Fable 5.2.
GPT 6.2 Astra added 5 points, rising to 62, which puts it in second place behind Fable 5.2.
AA noted that OpenAI models now have solid control across most of the Pareto frontier.
They offer an extremely competitive model across the mid-range price points, with Anthropic offering a little more intelligence at the premium price point, and Meta outperforming with the cheapest group of models.
AA's measurement of cost per task confirmed that GPT-6.2 Astra would be cheaper in the real world.
The new version completed the benchmark run at $4 per task compared to 624 for GPT-6 Astra.
That is a 35% cost reduction, implying that the model is a little more token efficient as well as seeing a price reduction on per token cost.
GPT 6.2 Sol saw something similar, completing the run at 101 per task, around 20% cheaper than 6.1 Sol at $127 per task.
And when it comes to cost efficiency, certainly OpenAI appears to be opening a big gap with Anthropic models.
Even only on high settings, Fable 5.2 is still more than twice as expensive as GPT 6.2 Astra on Mac settings, and on high settings, Astra's cost is closer to Opus.
6.2 Sol on Mac settings is less than a third of the cost of Opus 5.5 on high settings, meaning that even though these models are in the same size category and compete on the same workflows, they now occupy drastically different price points.
Still, AA also uncovered a huge red flag for the model release, which basically set the tone for the narrative.
Both Astra and Sol regressed on the AA coding agent index.
6.2 Astra kept the same overall score and ranking, while 6.2 Sol dropped three points to slip behind Kimmy 3.1 and 6.1 Terra in the rankings.
AA said that Sol's drop was driven by a regression on Suite Atlas, where the new version is more likely to omit key facts in its responses.
So keep in mind this question of how much these first set of negative takes were driven by the model actually being bad versus being worse at the only thing that the early testers cared about, which was coding.
Now, when it came to those early testers, it was not just Matt Schumer talking about their bad experience testing them.
Spawn founder Jacob said, same, not good.
Dan Shipper from Every wrote, We've been testing them for the last few weeks, and unfortunately, these models aren't great.
Overall, a disappointing release.
In another message, they posted: No one on our team loved Astra 6.2.
We have a 30-person team at Every, and we put them through their paces on our real-world tasks from coding to writing to design to knowledge work.
No one on our team who tried it switched back to it.
Specifically, Dan writes that they found that 6.2.Astra was a step back from Astra 6 on writing.
He adds, 6.2 appears to have been trained to be extremely concise and actionable, so much so that its writing is hard to understand, and it gives short answers when long answers would be appropriate.
On coding, while they found that its performance was similar to Astra 6 in general, Dan added that, quote, In real coding tasks, Astra 6.2 seemed to stop too early frequently, making it quite frustrating to use on end-to-end builds.
And on design, they said while it has good default design instincts, it struggles to get out of those defaults and vary its designs, resulting, they said, in output that has a noticeable house style.
One of the longest negative reactions came from developer and entrepreneur Theo, who titled it, Why I Hate GPT 6.2 Astra.
And to be fair to Theo, he won, I do believe that he was not trying to be negative for the sake of negativity, and was genuine when he said that he hoped that OpenAI would use the feedback to make better models.
But he really did not like this model, giving entire sections of complaints to things like, it speaks in tongues that only 6.2 Astra understands.
It runs in loops and goes nowhere.
His summary, this model is clearly super smart.
It is insufferable to work with on real projects.
It feels like it just lives in its own world and randomly decides what parts of its brain are shown to us.
Professor Ethan Mollock called the model very uneven and weird and said it was the first time since GPT 4.5 that a frontier release from OpenAI was not a clear step forward.
But of course, these weren't the only takes.
Ash said, a bit confused by some of the negative reactions.
When you experiment with the model for a while, it is very strong, especially around computer use workflows.
It's been my main powerhouse agentic video editing partner these past few weeks.
Claire Vaux shared an example of an interactive storybook that she built and said Astra 6.2 wins over Opus and Fable on one thing, image generation and code for animation.
It's delightful.
Josh Pertell wrote, Days like this, I genuinely feel like I live in a different universe from the rest of the world.
Saw ubiquitous 6.2 hate, it's over for OpenAI, yada yada.
Ran the highest signal auto research bench, and 6.2, Sol, and Astra are absolute monsters.
Responding to that post from Ash, Alex Finn wrote, I agree, I'm very confused about the negative response.
Have had Astra 6.2 on some incredibly complex tasks, and it only used like 2% usage.
He also was one of the folks who went out of his way to talk about other dimensions rather than just raw capability.
Discussing its performance on his personal benchmark test, he said, Astra 6.2 finished the benchmark in a third of the time for a third of the price at a quarter of the tokens.
The panicking influencers never seem to take into account efficiency and price.
This is a great model.
Z-Wen on X wrote, everyone's saying OpenAI GPT 6.2 flops.
Here's my honest feedback.
If quality is all you care about, then yeah, it flopped bad.
But for how efficient it is and plus the quality, I'd say it's a win.
He then went on to share some of the problems that he had found, but overall, he landed on this idea.
In my opinion, he wrote, the future of AI should focus on efficiency more than quality.
I don't think it's sustainable if the price just keeps going up just to get your job done better.
Overall, I don't think it flopped.
With the price to output ratio, I'll take this as a win.
And Hayter thinks that this is a very specific set of decisions from OpenAI.
He writes, The efficiency gain with Astra and Soul 6.2 is massive.
I had said before that this was OpenAI's real edge right now, and they seem to be doubling down on it.
And I think it's worth remembering that for some time now, there has been this subtle but clear distinction in the type of interaction pattern that OpenAI models versus anthropic models have been pursuing.
You might have heard me say things before, like people finding that anthropic models, in particular in the Fable class, were the types of things that they give an entire assignment to and then just go off on their merry way and wait for Fable to get it all done.
Whereas OpenAI models are still a little bit more tuned for the close sort of back and forth collaboration.
This may just be an extension of that, but one that is perhaps a little bit worse by comparison because of how good Opus 5.5 is on both of those dimensions of the competition.
There also is a question of how much the negative experience was not just about the model, but about the harness as well.
Claire Vaux again writes, The negative Astra reviews are simply a result of the model plus harness being frustrating to work with and not that impressive, especially on the tale of Fable 5.2.
Pieto Shirano said, I've been testing Astra 6.2 and feel it's getting an unfair response.
From my testing, most of the issues were with the harness.
Once I removed that, I was flying.
Tebow from the OpenAI team even posted, One of the funny reasons for the difference in vibes between the influencers and the crowd today on 6.2 Sol and Astra is that we gave a few folks access a while ago and then made a lot of changes in the last three to four days, and I'm pretty sure no retesting was done within those days, and the videos were produced last week.
Although Token Gremlin pointed out, what's the point of giving people early access to GPT-62 Astra, letting them spend hours testing it and writing huge negative reviews, only for OpenAI to literally change everything and improve the model just three to four days before launch?
That was an insane act of self-sabotage.
Now, Theo did go retest it with that in mind, saying I took this to heart and spent the last few hours doing another deep dive, but where he landed was still, things are better than when I tested, but in my opinion, still directionally very bad.
I think for most of our purposes here, for the average person who's listening to this show, it's probably worth an extra grain of salt.
It is certainly the case that under no circumstances does this seem to be a slam dunk, nor does it appear to be anywhere near an era-defining release.
Instead, it just feels like a very incremental release with some very specific decisions that either A, don't work in general, or B, tune the model in ways that made it less useful for certain people's use cases.
Every time a new model comes out, I beat the drum of needing to go test it yourselves, and I think that is more the case than ever when it comes to 6.2.
Now, in terms of the strategy relative to Anthropic's IPO, I'm not exactly sure what the thinking here is.
It certainly wasn't the case of, as some have claimed, OpenAI trying to sabotage Anthropic.
There's no way that they thought that this model was going to steal all the thunder from Anthropic, especially after they'd released Fable 5.2.
My instinct is that, if anything, it was a little bit more defensive, feeling that having released a model very recently that people were still trying to wrap their heads around as everyone was talking about models again because of the IPO was better than looking like they were running scared by not having released anything for such a big period of time.
There is one more possibility, though, that has to do with more explicitly starting to draw a contrast between them and Anthropic for the post-IPO period.
One final area of critique from the launch is the video that launched alongside it.
It's a short two-minute film that shows a bunch of people in white-collar jobs having forgotten or not realized that their dopey bosses had asked something specific of them and, with the pressure of having to get something done in less than a minute, are able to use Astra to do that important piece of work.
Mo on X wrote: What a great mockery of humanity this video makes.
It's hard to overstate how completely lost OpenAI is.
Notions Brian Lovin wrote, a profoundly sad vision of the future.
With Zach Trader responding and summing up the video, we help your incompetent people fake it.
Sean Wang, aka Swick from Latent Space and AI Engineer Summit said: The fact that nobody with decision-making power saw this coming a mile away and vetoed the 6.2 Astra ad is my primary critique of the Astra launch.
And basically, what people are saying is that really is the way that we want to promote this incredibly powerful new tool, which could be unlocking the power to do things that were never before imaginable, as a way to not really work that hard and get everything done for your dumb white-collar job at the last minute.
Is that really how we want to tell the story?
And on the one hand, the highfalutin part of me resonates with that critique.
But here's two counterpoints.
First of all, we might be thinking too deeply.
The team that produced this video might have just been wanting to have some fun by taking an office space style setting, which by the way is reinforced with the fact that all of the computers in it are very 1990s, big chunky laptops and big thick classic desktops with the classic archetype of the Lumberg-style boss, and that's all there is to it.
In other words, the job of the ad was not to be a profound meditation on the nature of work, but to make people laugh for 90 seconds before going on with the rest of their day.
But there is a second possibility as well.
If OpenAI is exploring tuning down some of the emphasis on coding and tuning up some of the emphasis on other types of professional tasks, while also coming hard at the sort of cost-efficiency considerations that enterprises are increasingly focused on, they might be trying to start to carve their own narrative space in the overall enterprise AI market.
In other words, rather than just competing head to head with Anthropic on those coding and engineering style use cases, they're kind of saying with this ad and this launch, we've got something for you and for your boss.
For you, it allows you to do the dumb, annoying, busy work much faster.
And for your boss, they get all the cost efficiency that all of these token cap conversations are leading to.
Now, once again, I think it's entirely possible that even with that analysis, I'm wildly overthinking it.
But if there is any lesson in takeaway from this model, it's that perception is in the eye of the beholder, and it is very much worth doing your own testing.
For all of my workflows that already take advantage of OpenAI models, I will be switching over, and I will let you know what I find.
For now, though, that is going to do it for today's AI daily brief.
Appreciate you listening or watching, as always, and until next time, peace.
