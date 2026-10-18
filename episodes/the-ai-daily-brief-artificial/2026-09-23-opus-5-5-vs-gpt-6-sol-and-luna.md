---
record_id: "podcast:cd81c793-879f-463f-b230-418c936bc84e"
episode_id: cd81c793-879f-463f-b230-418c936bc84e
title: Opus 5.5 vs GPT-6 Sol and Luna
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/opus-55-vs-gpt-6-sol-and-luna/cd81c793-879f-463f-b230-418c936bc84e"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/opus-55-vs-gpt-6-sol-and-luna/cd81c793-879f-463f-b230-418c936bc84e"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-09-23
played_at: "2026-09-23T12:00:00Z"
play_count: 1
duration_seconds: 1860
source: pocketcasts-history-browser
played_label: September 23
history_order: 53
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 34011be80aa5f6bb57dd67e25f89acc0dbe5a58e322d83f4e53fdf4f4b8b09ee
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

# Summary: Opus 5.5 vs GPT-6 Sol and Luna

This week Anthropic and OpenAI both released major models on the same day: Claude Opus 5.5 and GPT-6 Sol/Luna. Opus 5.5 performs at Fable 5.1 level but costs 40% less ($4/$20 per million tokens vs prior pricing), with benchmark scores exceeding Fable on multiple measures (Terminal Bench 4.0: 66.4% vs Fable's 55.8%). Community response is overwhelmingly positive—users describe it as a return to the beloved Opus 4.6 with Fable's intelligence, citing major improvements in writing quality (clearer, less verbose, better at taking feedback) and coding for complex tasks like 3D graphics generation. GPT-6 Sol and Luna pursue a different strategy: 50% cheaper than their GPT-5.6 predecessors, optimized for iteration and broader organizational use, with emphasis on enabling more frequent model calls rather than a single leap in capability. Opus 5.5 leads external benchmarks (Artificial Analysis score: 58 vs 53 for competitors); specific tests show 63% fewer tokens used than Opus 5, 30% faster output, and 15–65% accuracy gains on enterprise tasks. Notable drawback: increased safety rejections limit Opus 5.5 for some legal and life-science use cases.

For your workflow: if you use Claude, migrate to Opus 5.5 immediately for cost savings and better performance. If on GPT-5.6, upgrade to Sol for cheaper and better results. The actionable shift is moving away from single-model reliance to task-matched stacking (Sol for routine work, Opus 5.5 for ambitious coding/writing). Cost reductions from both releases dramatically expand AI agent deployment economics—you can now iterate more, process more data, and run agentic workflows at scale that were previously prohibitive.

## Transcript

The first half of this week has seen not one, not two, not three, but four major model releases, including two on Tuesday this week, a pair from OpenAI and one from Anthropic.
For OpenAI, GPT-6, Soul, and Luna continue their quest to build cost-efficient models at every level of the intelligence stack.
And for Anthropic, early indications suggest that Opus 5.5 is a return to glory or at least early adopter acclaim that the company has not seen since Opus 4.6.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, Blitzy, Section, and HyperAgent.
To get an ad-free version of the show, go to patreon.com slash AI DailyBrief, or you can subscribe on Apple Podcasts.
And to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
Now, as is normal when it comes to big new model releases, this will be a main-only episode.
And honestly, we're going to have a hard time getting it all in even with that.
So let's dive in.
Welcome back to the AI Daily Brief.
It's fairly undeniable that the best days on the AI Daily Brief, certainly the most fun, exciting, dynamic, oh boy, I can't wait to be done with this episode because now I get to go do things types of episodes are ones where we get new models.
And yesterday, we got the absolute rarest of treats.
A thing which I can't frankly remember ever happening before, which is the two most important labs of the moment, OpenAI and Anthropic, both releasing new models on the same day.
Certainly we've had models released close together before.
In fact, usually the pattern that we see is what SpaceXAI did yesterday, releasing their model in advance so as not to be drowned out by models that they knew would get more attention than them.
The challenge of the same day release is that it inevitably gets people to ask not what's valuable about this particular model and where it's going to fit in my rotation, but instead, which of these is better, and what does it say about which lab is in the lead?
So, today we are going to go through what was released, where things stand on the benchmarks, the first reactions, examples around some particular use cases, the impact on the competitive landscape, what it says about the whole pacing the frontier thing, and in the community's estimation, who won the day.
The first model we got was Claude Opus 5.5.
And frankly, it's been some time since an Opus class model was the big show.
Now, the biggest reason for that is, of course, the introduction of Mythos and then Fable, but even before that, people had so much love for Opus 4.6 that 4.7 and 4.8 were for many, if not a regression, certainly very incremental at best, and not even incrementally ahead in certain cases.
And in fact, when it came to Opus 5, people just genuinely did not like the thing at all.
Now, jumping ahead to where this conversation is landing, the perfect encapsulation comes from AI content creator Peter Yang, who used a meme of an illustration of a horse, beautiful and complete at the beginning, representing Opus 4.6, of course, to a much scratchier, more simplistic and childlike line drawing for Opus 4.7 and Opus 4.8, culminating in near scribbles for Opus 5, to finally, once again, the beautiful front side of a horse in perfect illustrated detail for Opus 5.5.
The people, in other words, are really liking this model.
But how did Anthropic pitch it?
In their announcement post, they said that Opus 5.5 performs at the level of Claude Fable 5.1 for most tasks, but costs 40% less to run, not even just than Fable 5.1, but then Opus 5.
In their announcement thread, they point out that it is a major step up from Opus 5, but also, frankly, at least when it comes to the benchmarks, it's also a step up from Fable 5.1.
On Terminal Bench 4.0, the model jumped from Fable 5.1's 55.8% to Opus 5.5's 66.4%.
Cursor Bench, Frontier Code v1.1, and Humanity's Last Exam also all saw jumps, not only from Opus 5, but from Fable 5.1 as well.
In fact, there wasn't a single benchmark that Opus 5.5 wasn't ahead of the other Anthropic models, Fable 5.1 and Opus 5, and only two, Automation Bench, which measures business workflows, and Terminal Bench Science, which measures agentic scientific research, where Opus 5.5 wasn't ahead of GPT-6 Astra as well.
Importantly, this is not just a performance gain, but also a pricing gain as well.
The Clot account wrote that because Opus 5.5 requires less compute to serve than Opus 5, its pricing is consequently down.
Compared to Opus 5's $5 per million input tokens and $25 per million output, Opus 5.5 is $4 per million input and $20 per million output.
However, because of additional efficiencies, they said that the cost gains will actually be about 40% as opposed to just the 20% reflected in the cost.
Although it's not pitched as a model focused on speed, they do note that because many of its default effort settings deliver better results than other models running at higher settings, that Opus 5.5 generates output much faster than those other models, including an average of 30% faster than Opus 5.
As a cherry on top, they increased five-hour usage limits on all of their ProMax and team plans, and threw in the rest of the subscription users a rate limit reset which can be used whenever people need.
On the safety front, they note that this is their first model released in the wake of the Pacing the Frontier note, and that Opus 5.5 was tested before released by external evaluators, including Frontier Design and Meter.
And overall, they argued that Opus 5.5 is basically the best aligned model they've released yet.
Sam Bauman, who works on alignment at Anthropic, wrote: We think Opus 5.5 is sufficiently safer than its predecessors that releasing it, more likely than not, reduces risks related to misalignment.
Now, Opus 5.5 alone would be more than enough for a complete episode, but OpenAI was determined not to let Claude have all the fun, and in the early afternoon Eastern time on Tuesday, they dropped their own set of models, GPT-6 Sol and GPT-6 Luna.
And if the Opus 5.5 announcement was a little bit focused on cost and efficiency, the 6-Soul and 6-Luna announcement was all about cost and efficiency.
Their announcement post on X reads: GPT-6 Sol and Luna build on the advances behind GPT-6 Astra, bringing much of its strengths into faster and more affordable models to support work at scale.
We've also made caching and inference more efficient, and we're passing the savings directly to you.
50% lower API prices for Sol and Luna compared with GPT-5.6 promotional pricing.
In other words, they're not just talking about this pricing being lower than Astra, they're cutting costs from the previous generation even before that.
And what's interesting is that they're clearly presenting cost as enabling new ways to use the tool as well.
As they put it, higher usage limits and lower cost give you more flexibility and room to iterate.
In other words, one of the ways that they think that people should cash in on those cost savings is to be more iterative in how they use the model.
Going back a couple of generations of models at this point, one of the subtle divides between Codex and GPT usage and Claude and Fable usage, on the other hand, has been an impulse to use Fable and Claude for more hands-off long-running tasks and the GPT models inside Codex for things where you need more interaction and iteration, and these new Sol and Luna models seem to build on that as well.
Like the Opus 5.5 announcement, OpenAI also points to advancements in alignment.
And what's notable when you get into the benchmarks on the OpenAI page is that where Anthropic is still using the traditional charts, which show a benchmark name and then a set of percentage scores across a set of models, OpenAI has entirely abandoned that, only showing benchmarks on graphs that map performance on the Y-axis versus cost on the X-axis.
Sam Altman tweeted: GPT-6, Sol and Luna are big improvements on intelligence, alignment, work output, coding, computer use, and more over their 5.6 family predecessors.
They are also half the price per token and even less per task.
He then went and followed up and really reinforced just how important this way of thinking is to OpenAI now, especially compared by per-task pricing, which is the metric that should matter, Sam says.
I don't think there is anything competitive anywhere in the market.
We want people to be able to use tons of AI.
It's important to being able to explore this new renaissance in front of us.
Putting some magnitude around what they mean by tons, in the announcement post they point out that valued at API prices, the median researcher at OpenAI uses $600 in tokens per day, while the 90th percentile of researchers use $7,000 of tokens per day.
Almost understating it, they write: As coding agents take on longer and more demanding tasks, the cost of sustained use matters more.
The upshot?
GPT-6, Sol and Luna, they write, combine strong coding performance with lower API prices, giving developers more room to iterate and teams the confidence to be more ambitious about what they ask Codex to take on.
But what about external benchmarks?
Even for those folks who care about benchmarks, everyone assumes you have to take any internal measures with a grain of salt, and one of the first places that people look when a new model comes out is independent sources like Artificial Analysis.
On their new V3 index, GPT-5.6 Luna and GPT-6 Luna are basically score the same at 37 overall, while GPT-6 Sol slightly beats GPT-5-6-Soul.
That said, both of those models get those scores at a lower cost per intelligence.
Indeed, Artificial analysis is for sentence is, GPT-6-Soul, and Luna pushed the cost-efficiency frontier by having cost relative to GPT-5-6-Soul and Luna.
In another positive highlight, Artificial Analysis found that both models saw a significant reduction in hallucination.
Zapier also tested GPT-6-Sol on a slate of real workflows.
They found that 6-Soul scored 33.2% compared to GPT-5-6-Sol's 28.77%, and did so at roughly half the price of 5.6.
Their summation was pretty simple: upgrade any of your workflows that are using 5.6.
It's cheaper and better, a rare combo.
Opus 5.5, however, was a different kettle of fish entirely.
Opus 5.5 was notable because it absolutely thwumped everything else to get the new top score on the intelligence index by five whole points.
Claude Fable 5.1 and GPT-6 Astra were previously holding it down at the top with scores of 53, but Claude Opus 5.5 jumped all the way to 58.
And while its cost and efficiency gains might not have been as much as GPT-6-Soul, artificial analysis did note that this increase in performance also came with the 20% price cut.
And honestly, while I've been trying to keep this analysis largely aligned and equivalent so far, watching people's first responses, there is absolutely no doubt which model among these dominated the discourse.
Matthew Berman wrote, Opus 5.5 being the absolute best model on the planet and being cheaper than Astra and Fable was not on my bingo card.
Chubby Kiminismus on X writes, the more I use, the more I fall in love with Opus 5.5.
It's so good and so much faster and so much less verbose.
It's everything I could have asked for.
It's as if my beloved Opus 4.6 came back but better and rebranded as 5.5.
Now we'll get more into that love, but what were some of the specific areas that people were testing Opus 5.5 on?
Aaron Levy and the team at Brocks brought it into quote a variety of complex enterprise knowledge work tasks dealing with unstructured data and saw not just improvements in performance, but major efficiency gains as well.
Versus Opus 5, they found 63% fewer tokens used, 42% less verbosity, and 30% faster.
On financial services tasks, they found an increase of 39% task accuracy.
On cloud cost analysis and technology use cases, they found an increase of 65% task accuracy.
And in use cases related to consumer products and clinical diagnostics, they found an increase of 17% and 15% task accuracy, respectively.
If you're leading AI inside an enterprise, you already know that the gap right now isn't capability, but execution.
That's why KPMG's You Can with AI is back with a new season featuring conversations with leaders like Sorojit Chatterjee of Emma, Mehabib of Ryder, McKesson CIO Ellery Fisher, and others focused on practical execution.
What's working, what's not, and what it actually takes to move from pilots to real scaled impact across strategy, data readiness, governance, workforce, and value.
And of course, it's co-hosted by me, Nathaniel Whittemore.
Go listen and subscribe at www.kpmg.us slash ai podcasts.
That's www.kpmg.us slash ai podcasts.
Here's why most legacy modernization projects fail.
The AI doing the work can understand code bases at scale.
It sees a small slice of context, examines syntax, and misses years of decisions distributed across the global application ecosystem.
Blitzy solves this the way it solves everything.
Grounded in your code before any migration begins, Blitzy's agents reverse engineer the entire legacy system into a persistent knowledge graph.
Every dependency, every constraint, every piece of tribal knowledge that used to live in one engineer's head.
From that understanding, Blitzy autonomously executes language migrations, framework upgrades, and monolith to microservices transformations, all validated end-to-end.
One Blitzy customer modernized a $10 million monolithic insurance stack in 16 weeks against a 137-week baseline with coding agents.
That's 9x compression.
Retire technical debt while accelerating your roadmap.
See how at blitzy.com.
That's BLITZY.com.
Here's a harsh truth.
Your company is probably spending thousands or millions of dollars on AI tools that are being massively underutilized.
Half of companies have AI tools, but only 12% use them for business value.
Most employees are still using AI to summarize meeting notes.
If you're the one responsible for AI adoption at your company, you need Section.
Section is a platform that helps you manage AI transformation across your entire organization.
It coaches employees on real use cases, tracks who's using AI for business impact, and shows you exactly where AI is and isn't creating value.
The result?
You go from rolling out tools to driving measurable AI value.
Your employees move from meeting summaries to solving actual business problems, and you can prove the ROI.
Stop guessing if your AI investment is working.
Check out Section at sectionai.com.
That's S-E-C-T-I-O-N-A-I.com.
This episode of the AI Daily Brief is brought to you by HyperAgent, where you run fleets of agents your team can manage together.
Forget local agents and chat workflows waiting on your laptop to be prompted.
HyperAgent deploys always-on agents in the cloud, doing real work across the tools your team already uses.
Marketing agents turn competitor moves into landing pages.
Sales agents enrich leads, draft emails, and updates the CRM.
Ops agent chases the paperwork and tracks the budget.
Every agent has access to shared context and follows your rules about scope and approvals.
It's time you add agents that feel like teammates.
Hire yours at HyperAgent.
Get $100 in credits at hyperagent.com/slash AI DailyBrief.
Now, when it came to the social media demos, as has been the case with the last several models, a huge amount of the posts were highly visual things like graphics, 3D renderings, and game design, which are interesting to look at on the internet, if not necessarily super reflective of the type of use cases that most people are going to actually have for this model.
Still, given how much 3D graphics and visuals and Blender were a big part of the story of the GPT-6 Astra release, a lot of the demos of Opus 5.5 basically have it mugging that model on exactly that type of use.
And given that my analysis just a week or two ago or whenever it was that we got GPT-6 Astra was about how much those sort of capabilities asked us to think in more expansive terms about the opportunities that AI opened up, it's worth noting that Opus 5.5, at least initially, seems to be another jump in those capability sets as well.
Alex Albert from the Anthropic team showed Opus 5.5 using Blender to make claymations with a single prompt.
Chase Lean made an interactive coral reef wallpaper.
And some people showed how the models were powerful enough to use generated code rather than image models to create real visual representations of the world.
Peter Yang shares what looks like a video of the Golden Gate Bridge, but notes that it's actually entirely generated using code by Opus 5.5.
He adds, from my testing, I think Opus is just as good at building 3D scenes as Astra.
Alex Albert again did something similar, visualizing a historically accurate San Francisco market street in 1906 pre-earthquake using only Opus 5.5 code and Blender, no image generation.
Dan Woods says that Opus 5.5, quote, absolutely frame mugs every other model on these sort of 3D generated worlds, adding that it is a quote, astounding leap in spatial awareness.
In a wildly viral post, Jake Eaton from Anthropic shared a number of different what appear to be paintings and said, For the past few months, I've been asking our models to paint.
Opus 5.5 is very skilled at emulating different styles.
Every image here is a Python program generated pixel by pixel.
There is no image model and no off-the-shelf art software.
Instead, it's about 7,500 lines of code using standard libraries to emulate different brush styles.
The agents don't use any pictures as reference, instead, working only from what they know about each painter.
And certainly, this is where you can see these capabilities, which might otherwise be cool to look at on social media but not necessarily all that relevant for most of us, maybe start to become a little bit more relevant.
If the advanced coding capabilities of Opus 5.5 are enough that it can, as in the case of this post by TAC, generate a one-shot 30-second long marketing animation, well, certainly all of a sudden a bunch of use cases open up that you might not have thought of before.
Tariq from the Cloud Code team asked Opus to do a bunch of redesigns on his personal website and then make a trailer with all of its iterations.
And at first glance, it seems to have done a great job.
For what it's worth, this is one use case that I tried on Opus 5.5 as well, and I was definitely pleased with its analysis and review of my AI Daily Brief website.
It was clear, had good concision of thought, and was very practical.
Although I will say, for those who are just trying to live in the world of strictly betters or strictly worses, it wasn't that it was necessarily strictly better than Fable 5.1's analysis, it was just different.
And yet, one area where almost everyone seems to be in agreement that Opus 5.5 is indeed strictly better is writing.
Anthropic Sholto Douglas reposted their announcement and wrote, Also, important news, we fixed the writing.
So, what does that mean?
Well, part of it is, as Theo put it in all caps, they removed the M dashes.
But what the Anthropic account actually said about this is: Opus 5.5 communicates more naturally, addressing some of the most common feedback we heard on Opus 5.
It puts the most important information up front and follows the writing rules you give it, which makes long sessions easier to follow.
The team at Every, who have one of the best benchmarks and processes for testing AI writing wrote, Opus 5.5 produces the most readable prose we've seen from an Anthropic or OpenAI model.
In fact, presaging a point that would come up a lot more later in the conversation, they wrote that while Opus V had made their writers kick Claude models to the curb, 5.5, quote, makes us want Claude back in the room.
They continue, it responds well to feedback, builds on the material you give it, and explains its choices where Opus 5 wouldn't.
And importantly, it turns out that this isn't just an improvement on the output of writing, but an improvement on the actual process itself.
They write that Opus 5.5 is a pleasure to write with.
It takes feedback without a fight and builds on material instead of handing it back tidier.
In fact, the team writes, the biggest upgrade is not even exactly about the writing, it's about the feel and vibe of the model.
As the Every team puts it, Anthropic fixed Opus's personality.
It's not an obstinate little turd anymore.
And this is an experience that many have had.
AI builder McKay Wrigley writes, Opus 5.5 equals the personality of Opus 4.6 that we all desperately wanted back, and the intelligence and taste of Fable 5.1.
And certainly Anthropic knew it.
Nat McCallis from Anthropic posted, Opus 5.5 is way, way, way better than Opus 5.
Sorry about that model.
Please try this one.
So have people had any issues yet with Opus 5.5?
There is one that stands out and that for certain use cases will be effectively a non-starter.
Chief of staff on X wrote, I burned all my usage reset benchmarking Opus 5.5 against Fable 5.1 for complex open-ended legal work, i.e.
drafting client and court-ready documents, draft and contract redlining, legal and matter-related research.
As far as I can tell, Opus 5.5 is much worse due to increased safety rejections and what I'd guess you would call poor effort budgeting.
Simon Smith writes, Opus 5.5 looks good, but as a life science commercialization company, I'm a bit concerned by this.
Quote, because Opus 5.5 is comparable to Claude Mythos 5.1 in biology and cybersecurity, we're deploying it with safeguards similar to those on Claude Fable 5.1.
Simon continues, We've faced issues using Fable for some tasks because of these guardrails.
We've applied for Anthropic's life science verification program, but haven't yet been approved.
We had used Opus when Fable refused to request because of Fable's biology guardrails, but now it seems like this won't be possible anymore with Opus either.
It's not everywhere, but I certainly have seen a number of people complaining about these overzealous safeguards, which is unfortunately the type of thing where if that hits your use case, it basically makes the model null and void.
So what are some of the big takeaways for folks after this huge slate of releases?
Aaron Levy writes, What an insane day in AI.
The frontier models just became substantially cheaper with the Opus 5.5 price cuts, and now with GPT-6, Sol and Luna dropping token prices by 50%.
The rate at which the cost per task on a like-for-like basis drops in AI is unlike any other type of technology in history.
And every time the cost of AI drops, the use cases you can deploy agents against dramatically increase.
This is Jayvon's paradox applied to agents.
Making a bit of a prediction, Aaron continues, these improvements will directly lead to broader diffusion of AI in the economy as we can use agents to process all of our data, scan our code for security issues, read through all log data to make decisions, have agents swarms in workflows, and much more.
The cost of tokens is directly correlated to these use cases being opened up at scale.
And putting some research heft behind that, Epic AI Research yesterday also dropped data arguing that, quote, AI is getting cheaper more quickly than any other transformative tech in history.
At a given level of performance, cost has fallen around 47% per quarter since 2023.
They point out that that's 4x faster than DNA sequencing, 6x faster than compute, 18x faster than lithium batteries, and at least up to 1973, 54 times faster than electricity.
Now, when it comes to head-to-head analysis, you can find people arguing all sides when it comes to which of these models are the most valuable in aggregate.
Tier Taxes writes, cheaper, better, Sol and Luna.
I assume they're natively trained for being Astra's henchmen.
This makes OpenAI's value proposition considerably stronger.
I suspect that Opus 5.5 wins on cost and multi-agent are effectively negated with Astra plus Sol plus Luna.
And there are also many of folks just happy to enjoy the unique values that each of these different models provided on their own terms.
In answering the question of whether there was a winner, Chubby writes, both OpenAI and Anthropic gave us plenty to be excited about.
And if you have any question about the strategy that OpenAI is pursuing, Sam Altman could not have made it any more clear.
He wrote, We want the OpenAI API to feature the best model at every price point and to be the best at every modality, text, code, image, video, et cetera.
And then we all want you to come up with great ideas and build them and get to be happy users.
Again, remember that he had written in a separate post: we want people to be able to use tons of AI.
It is important to being able to explore this new renaissance in front of us.
I think, in many ways, you can view this set of releases from OpenAI as a continuation of the strategy that they've clearly been pursuing for a while now, which is to be really aggressive about focusing on cost and efficiencies and building a model slate for an era in which people are moving away from a single model towards complex model architectures that actually match tasks with the right type of intelligence.
Claude, on the other hand, feels like it was out to reclaim some momentum.
And if that is the case, they've done so pretty successfully.
Here's how Every put it: Seoul feels like an S-class iPhone release.
It will give you much of Astra's power at about a fifth of the price.
Opus 5.5 is the bigger surprise.
5.5 is tempting a few people on our team to switch back from Codex.
You'll love this model if you're already in the Claude ecosystem.
And if you're a Codex user, it's worth a look, especially for your top-end coding tasks.
Now, in some ways, this is just a continuation of the divide which I mentioned before and which we've seen for several model iterations now.
Dan from Every concludes that article: You'll like Sol 6 if you want a fast, affordable daily driver for reading, writing, and getting things done.
It's the model I keep reaching for.
You'll like Opus 5.5 if you're willing to pay more for stronger performance on ambitious coding and visual projects.
Its best work surpassed Seoul in our tests, enough to pull some of our team back towards Claude.
And the pulled people back to Claude is a real take that I'm seeing from a number of different people.
Yu Chen Jin writes, Claude is back.
Time for me to open Claude Code again after ignoring it for a month.
And if anything, the more time that goes on, the more positive I'm seeing people get on Opus 5.5.
This morning, former investor-turned AI builder Jeffrey Emmanuel chimed back in: My God, Opus 5.5 is breathtaking.
It's just grinding through incredibly tricky stuff like it's nothing, finding bugs and problems that eluded Fable and Astra for weeks in some cases, and showing a level of agency and resolve I haven't seen before.
Now, for me personally, I'm going to save a bit of my personal analysis for a little bit more time with the models, which will come together in more of a how-to episode for getting the most out of both of these models later in the week.
That said, I do think that there are a few interesting observations that are worth closing on.
By the way, this visual that I'm talking over was created by GPT-6 Soul, which added quite a bit of text that I didn't have in there, but I left it perhaps as an example of particular model quirks.
Observation number one is that even early adopters who are more ruthless about switching and who profess to really only care about performance definitely have personality preferences.
So much of the excitement around Opus 5.5 is not about, wow, it does this thing which AI has never been able to do before, but about, oh my gosh, it is such a pleasure to use this in a way that it hasn't been for some time.
I actually think that this is extremely important.
When there was such a big dust up around ChatGPT 4.0 being deprecated, there was a temptation to treat it like a phenomenon exclusively for crazy normies who had gotten obsessed with a sycophantic model.
But as time has gone on, for as much as AI might be a tool to some of us, it's clearly a very different type of tool.
It's a tool that at least approximate having a personality, and different versions of that tool's personalities and more or less enjoyable to use actually has implications for how much we can get out of them.
In short, when it comes to LLMs, personality is UX, and we should make sure we're treating it as such.
Observation number two.
While it is definitely the case that if you were just looking to declare one winner from the standpoint of buzz and excitement, it would be Opus 5.5, the battle of LLMs is not really about one thing anymore.
It's about one, figuring out what the stack of options needs to be, and then two, battling for each slot in that stack.
In other words, even the people who loved Opus 5.5 the most aren't saying you have to use this for absolutely every single use case.
And in many ways, I'd even argue that although at first glance, Opus 5.5 and GPT-6 Soul seem to be direct competitors, the way that their respective builders are thinking about them is a little bit different.
What matters at this stage is individuals and companies being able to understand their complete set of needs and how different models and harnesses combine to best fill those needs with respect to performance, capability, cost efficiency, and speed.
A third observation is that we're definitely in the era where you can't really separate models from harnesses anymore, at least not fully.
For a lot of folks who are fully invested, for example, in the codex ecosystem now, it doesn't matter if Opus 5.5 is much better.
As long as their OpenAI options are close enough, they're not going to fully shift out of that harness.
Will Brown from Prime Intellect wrote, I keep switching desktop agents every week and it's getting out of control.
Codex didn't have Fable 5.1, Claude didn't have Astra, AMP had them both, but now doesn't have Opus 5.5, so I'm back to Claude.
Self-build is annoying to maintain.
We didn't talk much about harnesses in this episode, but give it about a week, and the real proof in the pudding will be whether anyone has actually switched their overall behavior because of any of these model changes, or whether everyone tested things, found out what they liked, and just went back to the ecosystem that they were already using before, dictated in large part by the harness, where they store their context, their tools, their rules, et cetera.
A fourth observation is actually not so much about either Anthropic or OpenAI, but about the fact that as these models were being released, the other big buzzy thing that people were talking about was, I would argue, the first AI product that is seeing a lot of traction, where the people using it genuinely don't know or don't care about the model underneath.
I'm talking, of course, about Muse, which you can tell just from the posting from Meta's chief AI Officer Alexander Wang.
The team over there at Meta is very excited about the uptake and reception for.
How will it change this sort of new model conversation if the models actually start to get abstracted away?
That's something we've talked about for a long time, but which so far hasn't really played out in practice.
But who knows, maybe we're at the beginning of the product rather than the model era of AI, in which the models really will disappear into the system.
The fifth and final observation for today is what this all says about pacing the frontier.
One of the standard jokes that could get you a bunch of reposts and likes on X was people staring with bleary eyes at four major model releases in two days and asking some version of this is pacing the frontier.
But I think Theo had the right of this when he wrote, Hot take, this is what pacing looks like.
None of today's releases were Astra or Fable tier.
This is intentional.
The point of pacing isn't to stop iteration and improvement.
The goal is to prevent the development of bigger models from spiraling out of control.
Opus and Sol class models are a great place for our focus to go right now.
Lots of opportunity for real wins without as much risk.
And I think that that's correct.
If this is what we get from the pacing the frontier era, in other words, models that solve specific problems with previous iterations of those models and deliver incremental performance or value gains at significant cost and efficiency gains, that seems like a pretty good place to spend some time.
And not one where somehow all sorts of adoption is going to slow down.
Tariq from the Claude Co.
team is clearly pointing at this as a key direction for the labs.
He wrote, The right way to use model capabilities is not to ship 10x more features to prod.
It's to spend more time understanding your users, trying experiments, building prototypes, learning about things you don't understand so that you can ship things that actually work.
In fact, I think you could argue that because there have been such radical capability increases at such a fast clip for the entire history of generative AI post-Chat GPT, the labs have never really had to think in product terms.
The raw capabilities jumps have been so pronounced throughout the entire period that they can just splatter the latest thing at us and we're gonna eat it up.
But at some point, the market of people who are willing to do that saturates, the percentage of business use cases that that approach can get to saturates, and you actually have to think in terms of human and system realities.
Now, I don't at all think that somehow this means that all of a sudden all the resources are going to go to perfecting existing classes of models rather than trying to build bigger things, but it certainly shows that the endless pursuit of bigger models is not the only be-all and end-all for the labs.
Anyways, guys, it is a pretty phenomenal day.
If you haven't yet, I would highly encourage you to go out and spend some time with these new models.
For now, that is going to do it for this edition of the AI Daily Brief.
I appreciate you listening or watching, as always.
Until next time, peace.
