---
record_id: "podcast:39ac816c-b8ae-48a6-8c8e-2a7ed016d25a"
episode_id: 39ac816c-b8ae-48a6-8c8e-2a7ed016d25a
title: Why Muse Wonder Is Dividing AI Users
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/why-muse-wonder-is-dividing-ai-users/39ac816c-b8ae-48a6-8c8e-2a7ed016d25a"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/why-muse-wonder-is-dividing-ai-users/39ac816c-b8ae-48a6-8c8e-2a7ed016d25a"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-13
played_at: "2026-10-13T12:00:00Z"
play_count: 1
duration_seconds: 1620
source: pocketcasts-history-browser
played_label: October 13
history_order: 10
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 4a3004b7b012e5a055364bbfbf0f25dd6b351533acdaeb57ce14e140f11feff5
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

Meta’s Muse Wonder and Wonderful models are the central claim: Chief AI Officer Alexander Wang framed them as competing with “the big boys,” and benchmark summaries put Wonderful at 79% on DeepSuite 1.1, about five points ahead of GPT-6 Astra and Opus 5.5, two points behind them on Terminal Bench 4.0, ahead by about four points on Meta’s internal personal superintelligence index, and state-of-the-art on Harvey Lab legal work, Val’s finance agent, and Automation Bench; Artificial Analysis scored Wonderful 56 and Wonder 52, tying Wonderful for second with Sonnet 5.5 and placing it two points behind Opus 5.5, while Wonder ranked seventh tied with GPT-6.1 Soul and Gemini 4 Argon, with a $4.52-per-task cost that is about 3x MuseSpark 1.3, about $1 more than GPT-6 Astra or Grok 4.7, and about $1.50 cheaper than Opus 5.5. The episode also covered fast-mode competition, with Anthropic serving Opus 5.5 at a verified 285 tokens per second and OpenAI docs suggesting 280 tokens per second for GPT-6.1 Sol, plus reports of a new Anthropic model and Fable 5.5, Patrick Tolmy’s claim that OpenAI may answer with Bell in December, OpenAI’s possible Sora revival with Bill Peebles, Jeffrey Katzenberg, and Sujay Jaswa, Amazon’s reported $7 billion Decart AI acquisition centered on Decart’s DOS inference optimization claimed to be 8x faster and one-eighth the cost on Tranium 3, NVIDIA’s reported interest in Reflection AI after Beam and its $800 million stake and $25 billion valuation, and Microsoft’s MAIA300 chip claimed to deliver 40% more tokens per watt and scale to multi-gigawatt inference deployments. Community reaction was split: Ollie Lehman, Toby Lutkey, Theo, Charlie Holtz, Bone GPT, and Claire Vaux highlighted strength in coding, agentic tasks, security, and “soulfulness,” while Max Blade, Mehu Mohan, Every Zan Shipper, Riley Brown, Adam Holter, Arafat Shuvo, Matt Silv, Satya Malik, and Sam Lesson raised problems with 3D/CAD work, real programming, senior-engineer benchmarks, Wonder-versus-Wonderful confusion, rapid plan consumption, booking doom loops, and false meeting reminders; Zuckerberg’s non-signature of the Pacing the Frontier letter and his “Future is for Everyone” essay framed Meta as refusing to slow down.

For the user, the actionable move is to test Muse Wonder and Muse Wonderful separately on real tasks rather than social-media demos, especially agentic workflows, coding, security review, front-end work, and long-running personal-assistant tasks, while tracking quality, cost per task, token burn, plan upgrades, and whether the reported usage-counting bug affects results; if choosing a personal assistant, weigh consolidation against multi-assistant context switching, because active memory and active focus may matter more than raw benchmark scores for booking, reminders, and error recovery. No direct health implications appear in the supplied material; the practical implications are workflow, cost, security, and research monitoring. Useful follow-up questions are: does Wonderful reproduce benchmark-level performance on the user’s own work, is Wonder’s weakness a naming/product confusion or a real quality gap, can Decart’s DOS optimization generalize beyond world models to LLMs, will NVIDIA’s Reflection AI deal make it a direct frontier competitor or merely improve Nemotron, and will Fable 5.5, Bell, MAIA300, and fast-mode pricing change the cost-latency tradeoff enough to alter tool choices?

## Transcript

It appears we officially have a new player in the Frontier AI race.
Earlier this week, Meta has just announced a new series of models that it calls Wonder.
And unlike the Spark models it released over the last several months, Wonder is meant to compete head-on with, as Meta Chief AI Officer Alexander Wang put it, the big boys.
But can it hang?
Today we're going to look at Wonder and its bigger sibling, Wonderful, and ask what it means that Meta is now firmly back in the Frontier AI race.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors: KPMG, C Data, Granola, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AIDailybrief, or you can subscribe on Apple Podcasts.
And to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
We kick off today with the latest company to put some emphasis on speed.
This is something we've seen increasingly throughout the last couple of months.
Obviously, it's something that Google has emphasized with their flash models, but more recently, OpenAI has also been pushing their ultra-fast mode, and Anthropic has now figured out how to serve Opus 5.5 at a blistering pace with a new addition to fast mode.
They seem to have stepped up the pace for this one, now serving Opus at a verified 285 tokens per second at max.
OpenAI hasn't published a speed test for GPT-6.1 Sol on their fast mode, but their docs suggest a theoretical maximum of 280 tokens per second.
What's more, OpenAI is charging 50% more for the premium speed, and while people debate which is better, realistically, both are very expensive versions of the product with fairly niche applications.
For Anthropic's version, usage isn't included in regular subscriptions, as some found out the hard way this weekend.
Still, for those looking to burn through a ton of tokens quickly on a budget, Chubby noted that Anthropic can serve 50% more tokens per dollar.
I think that right now, these fast and ultra-fast modes are a little bit of a novelty to most people.
But as they become more common in Deirgue, big shifts in the latency of models will change how we interact with them in ways that I don't think that we'll quite know until we get there.
How important this ultimately is as a vector of AI competition, we will see, but it's certainly something that all the labs are exploring at the moment.
Now, speaking of Anthropic, new Anthropic models have been spotted and testing.
Users have reported queries being routed to a new model instead of Opus 5.5 with very impressive results.
People were showing off code-based animations that were introduced with Opus 5.5, but then seemingly pushed to this new model.
Others reported seeing Fable prompts routed to a new model as well, opening the possibility of a double-headed release.
Chubby on X wrote, A release should be near.
Since Anthropic's IPO is also pretty close, they want their new model to be released a few weeks ahead, so the market can really count that into the valuation.
Long story short, Fable 5.5 should arrive soon, and it looks to be a much bigger leap than we even expected.
In addition to the competitive dynamics, this release could also be a big test of what the major labs are comfortable releasing moving forward.
Both OpenAI and Anthropic have restricted testing of their most advanced internal models and could commit to pacing the frontier by focusing on mid-sized model releases like Opus and Seoul.
Or we could see another round of acceleration as new larger frontier models are unleashed.
As to what AI insiders expect from this, Google's Patrick Tolmy wrote, I was at an AI dinner last night in New York City, some interesting topics discussed.
One of those topics was, as he put it, consensus was Fable 5.5 will be stunning, but OpenAI will beat it in December with Bell.
If you thought in other words about slowing down for the holidays, think again, my friends.
Speaking of OpenAI, the company is reportedly exploring a Sora revival as part of a partnership.
Oh, so long ago, the TikTok-style video generation app enjoyed a brief moment in the sun.
In late 2025, Sora grabbed the number one spot on the App Store chart, displacing ChatGPT.
For about five minutes, Sora memes became the hot trend.
However, by the beginning of this year, when faced with difficult choices around where to deploy compute, enterprise use cases like coding won out, and Sora was mothballed.
The shutdown in April was OpenAI's best example of its mandate to end what it called side quests.
Now, however, a comeback could be in the works.
The information reports that OpenAI is in talks with an unnamed startup to license the Sora model and relaunch services around it.
The stealth startup was reportedly founded in recent months by Bill Peebles, the former OpenAI researcher who led the Sora project, and co-founders include former Disney chairman and Hollywood legend Jeffrey Katzenberg, as well as former Dropbox CFO Sujay Jaswa.
Sources said the deal is still coming together, and it's unclear whether the startup would get full access to Sora's weights, but they would have enough access to heavily customize the model.
So, for those who miss those crazy cat memes, you might be back in business soon.
In acquisition news, Amazon is in talks to acquire Decart AI in what could be their largest acquisition of the AI era.
The Wall Street Journal reports that the deal is being negotiated at a $7 billion valuation and could come together soon.
Decard is an interesting target for Amazon and could say a lot about how they view their position in the AI race.
The startup was founded in 2023 and has focused on developing world models for use in live video.
Their models can produce live generative video for use cases like live character transformations for streams or generative gaming.
While the tech is cool, Dcart hasn't found all that much traction.
Amazon, meanwhile, hasn't released a new series of models since last December and let go most of their AI researchers in the last round of layoffs.
It appeared to most that they had no interest in competing on the model layer for either Frontier or commodity LLMs.
The play then seems to be about hardware optimization.
Dcart was given early access to Amazon's Tranium 3 chips last year and developed a technology stack they called the Decart optimization System or DOS.
They claim this technology allows inference to operate up to eight times as fast and at one-eighth the cost.
DOS is hardware agnostic, so could help AI models optimized for NVIDIA GPUs or Google's TPUs deploy efficiently on Amazon's hardware.
So far, it seems like DOS has only been used for Decart's world models, so it's unclear whether the technology can apply generally to LLMs, but Amazon appears to be willing to take the gamble.
Last month, Amazon was said to be exploring an acquisition at $6 billion, but walked away after performing due diligence.
Decart last raised funds in May, reaching a valuation of $4 billion, pointing to Amazon paying a 75% premium on their last mark.
If the deal comes together, it's clearly about inference optimization.
If the technology works at scale, it would give AWS a huge edge over their rivals.
Given how much we're seeing industry attention shift from models and products alone to the business of serving tokens as cheaply and efficiently as possible, Amazon potentially appears to be preparing for a world where hardware efficiency is the only benchmark that matters.
One other interesting acquisition in the works, NVIDIA is reportedly in talks to acquire US-based open model developer Reflection AI.
You might remember that after a long wait, Reflection AI unveiled their first model called Beam last week.
The model was positioned to rival the best open weight models from Chinese developers, and while it wasn't quite there on the benchmarks, Beam was still clearly ahead of other US open models, like NVIDIA's Nemotron.
The Financial Times now reports that NVIDIA wants to double down on Reflection AI following their model reveal.
NVIDIA is already one of the largest investors in Reflection with an $800 million stake, and are reportedly exploring options including further investment in cash or compute, as well as a full Aqua Hire.
Reflection was last valued at $25 billion in March, so this deal could exceed the $20 billion NVIDIA paid for Grok in December to become their largest acquisition ever.
The FT said a deal could be reached in the coming weeks, but could still fall apart.
It is very clear at this point that NVIDIA wants to build the best open model stack in the West.
Yuchen Jin wrote, NVIDIA bought Hugging Face, Aqua Hired Poolside, and Essential AI, and is now eyeing Reflection AI.
Jensen is assembling these Neolabs to train the US best open source models.
As to the question of competition, Zephyr writes, It's pretty clear that NVIDIA will compete head-on with the Frontier Labs now.
Jensen is pissed because labs are developing their own ASICs and undercutting NVIDIA.
Citrini's Jukon, though, writes: I don't think NVIDIA's intent with this acquisition is to compete with OpenAI or Anthropic.
If it were, why would NVIDIA invest in OpenAI's current funding round?
It's probably about improving Nemotron's terrible performance.
Continuing, he wrote, Let's say this acquisition is intended to turn NVIDIA into an AI lab itself.
That would only push OpenAI and Anthropic to accelerate their shift away from NVIDIA, which would be even less in NVIDIA's interest.
Whatever the logic, it is very clear that NVIDIA is very interested in the open source side of the market.
And with perfect timing to add intrigue to exactly this conversation, Microsoft has unveiled the next generation of their homegrown chips with a plan to deploy them at scale.
CEO Satya Nadella announced the new MAIA300 chip on Monday, calling it Microsoft's biggest bet on custom silicon to date.
He claimed the new chips can deliver 40% more tokens per watt than leading GPU-based hardware.
Starting next year, he wrote, We will scale our Maya family to multi-gigawatt deployments, making it the primary inference system for our own product and services.
The Maya 200 chips are already deployed at a smaller scale, but this generation is expected to be a big leap in performance.
Wrote investor Chamat Palahapatiya, You should expect the silicon chip companies to move up the stack as the application companies move down the stack.
In AI, it is increasingly true that everyone competes with everyone.
Everyone will soon offer their own LPs, silicon, cloud, and applications.
The question is: what will the constraint be that you can build a long-term market and margins around?
Is it distribution?
Is it a data mode?
Is it a physical constraint like power?
Expect a lot more discussion along those lines in the months to come, but for now, that is going to do it for today's headlines.
Next up, the main episode.
Hello, everyone.
One big change around AI is we've shifted our thinking from how we rank our pages to how do we become the source that AI trusts enough to answer with.
At KPMG, they're seeing this firsthand.
AI-generated results now surface answers directly, often without a single click.
That's why they are increasingly focused on generative engine optimization, or GEO, structuring content so AI systems can retrieve it, understand it, and cite it as trusted authority.
This is not just an SEO evolution, but a visibility mandate.
And indeed, the GEO mandate from KPMG is simple.
If AI is shaping decisions, your expertise needs to show up inside the answer.
Read all about it at kpmg.com/slash us/slash GEO.
Again, that is kpmg.com/slash/us slash GEO.
This episode is brought to you by C Data.
Companies rolling out AI keep hitting the same wall.
Token spend is climbing, security is holding agents back, and no one knows how AI is truly being used.
The root cause: AI is cut off from the systems and context your business runs on.
That's why C Data built Connect AI Gateway, one control point between your AI and your systems.
Built on the connectivity layer powering Palantir, Google, Salesforce, and hundreds more, each agent gets exactly the data and tools it needs.
It governs down to the record and lets you finally see your org's complete AI usage in one place.
Accurate answers, a fraction of the token cost, and a gateway that learns your business with every interaction.
See how at cdata.ai.
When I'm in a meeting, I'm fully in it.
I'm thinking about the iteration and creative back and forth it takes to actually push a goal forward.
What I'm not thinking about is capturing takeaways, tracking to-dos, or any of that.
And that's where Granola comes in.
Granola is an AI-powered notepad that captures what happens in your meetings and turns it into clean, structured notes with the decisions and action items pulled out and easy to find.
There's no setup and no configuration.
It just fits into how you already work.
For me, it means I get to stay in idea mode, and Granola makes sure those ideas actually become action.
Once you try Granola on a first meeting, it is hard to go without.
You can try it totally free at granola.ai/slash brief.
That's granola.ai/slash brief to get your time back.
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
Harden your codebase at blitzy.com.
That's B-L-I-T-Z-Y.com.
Welcome back to the AI Daily Brief.
It wasn't very long ago at all, less than a year certainly, that most people paying any sort of attention were more or less writing Meta out of the AI race.
In fact, in 2025, most of the headlines around Meta and AI were about Mark Zuckerberg spending an extraordinary amount of money to lure researchers to Meta, and then, of course, all of the internal strife that would follow those moves.
And yet, in 2026, the year of the agent, with fall of 2026, of course, being the season of the personal agent, Meta is fully back in the mix as a Frontier lab.
We started to see this with the release of the Muse Spark models, which were, if not state-of-the-art, certainly not embarrassing and good enough to power many of the functions for their consumer app Muse.
On Monday, however, Meta introduced Muse Wonder, a new, larger class of models.
The release included two model variants, Wonder and Wonderful.
Wonder is the slimmed-down version optimized for speed, and Wonderful is the full version available through the API.
Today we're going to talk about how the models perform, early takes and experiences from the community, how this changes the AI race, and what it says about pacing the frontier.
On the benchmarks, both versions of Wonder show up near the top of the rankings.
Wonderful scored 79% on DeepSuite 1.1, which is almost five points ahead of GPT-6 Astra and Opus 5.5, and on Terminal Bench 4.0, it was behind those Frontier rivals by just two points.
For agentic tasks, Wonderful seemed to have a slight lead.
It topped Meta's internal personal superintelligence index, beating Astra and Opus by around four points.
It was also state-of-the-art across Harvey Lab for legal work, Val's finance agent, and Automation Bench.
On OS World, which tests computer use, Wonder was a few points behind Frontier Rivals, but still decidedly in the mix.
Artificial analysis backed up Meta's results, giving it a 56 on the Intelligence Index for Wonderful and 52 for Wonder.
That makes Wonderful tied for second against Sonnet 5.5 and two points behind Opus 5.5.
It places it ahead of Claude Fable 5.1 and GPT-6 Astra.
The Slimmer Wonder is a little further behind in 7th place, tied with GPT-6.1 Soul and Gemini 4 Argon, which is of course yet to be released.
Artificial Analysis highlighted that this is a quote material gain over MuseSpark 1.3 and comes just six weeks after that model's release.
The big gains were on Agentic Professional Work and Coding Tasks, including a second place ranking on GDP VAL AA and third place on AA Briefcase.
Muse Wonder was pretty pricey at $4.52 per task, which represents almost a 3x increase from MuseSpark 1.3.
That puts it about a dollar per task more expensive than GPT-6 Astra or Grok 4.7, and about $1.50 cheaper per task compared to Opus 5.5.
If then we went purely from the benchmarks, Meta is back at the frontier for the first time in years.
For some, that was jaw-dropping all on its own.
Ollie Lehman writes, What timeline are we in where Zuck is mogging Astra and Fable now?
Infinite money plus infinite distribution and now Frontier intelligence?
Long meta.
Shopify's Toby Lutkey writes, This model is very, very good.
I was struggling to find anything to throw at it that it couldn't do, even when other top models failed.
Meta is back.
And yet the benchmarks are never the full story, and it wasn't long before folks started poking some holes in the excited press.
Giving Muse Wonder and Opus 5.5 the same prompt to build a AAA level lawnmower simulator, Max Blade wrote: It's very clear that Muse is not anywhere near close to Frontier in 3D tasks like video games or even printable CAD designs.
Presaging another complaint that we will see, he also continued, even scarier is it burned my $50 spending plan plus $4.11 in API equivalent tokens.
I had to upgrade to the $200 plan just to finish this run.
I will spare you the million more examples of Muse Wonder underperforming on that type of test, but point you to this comment from Theo, who writes, Already seeing a lot of people discount Muse Wonder because it wasn't RL'd in 3D stuff like Astra and Opus.
3D game demos are cool, but they don't represent real code work at all.
I could not agree more strenuously with this.
In fact, I think that it is actually extremely net negative to the entire industry and world around it, that because 3D games and renderings look good on social media, the Frontier Labs feel like they all have to optimize for that use case because they know that people on X are going to judge it based on that use case.
Meta's chief AI officer Alexander Wang even added, Whole team feels dumb now, but it's true.
We did not explicitly train our model on 3D demo games.
Obviously, in retrospect, we probably should have done a bit of that, but no regrets, please try Muse Wonder on your actual coding work.
Unfortunately, it wasn't just those 3D tasks where some people found issues.
AI researcher Mehu Mohan writes, Sorry, but not impressed with Muse Wonderful at all.
Nowhere near Opus 5.5 performance, I'd argue not even GPT-6.1 Soul.
I'm not sure what model others are using, but the benchmark numbers making it comparable to Opus seem weird.
Not pricing, just quality itself is bad.
These are real programming tasks in my own agents.
Every Zan Shipper wrote, Disappointing show for Muse Wonder on our senior engineer benchmark.
It asks the model to rewrite a Vibe-coded slop database from scratch.
A good measure of its usefulness for real-world engineering.
Muse Wonder gets 52%, far behind even GPT-Soul 6-1 at 71%.
Riley Brown wrote, used Muse Wonder for five hours.
Was gonna make a video.
No need, back to codex and clawed code.
Some speculated that the issue was actually the fairly significant gap between Muse Wonder and Muse Wonderful.
Adam Holter wrote, Muse Wonderful looks really good, but Muse Wonder isn't doing very well on any of my tests.
So now everybody is getting bad results from Muse Wonder, and it reflects badly on Muse Wonderful because they have the same name.
I honestly think it would have been better to release these at different times.
I will note, giving a sense of how engaged the team is, Alexander Wang responded to that, saying, Fair feedback, DMing you to understand more.
And I saw a number of other users suggesting something similar, where they had good experiences with Wonderful, but bad experiences with TheSlimmer Wonder.
The one other big complaint was around how fast the plans got consumed.
Arafat Shuvo wrote, I can't even do work properly with Muse Wonder.
It burns through the weekly limit so fast.
Matt Silv wrote, I just upgraded to the Muse $50 a month plan to try Wonderful.
Even after the usage limit reset an hour ago, it used 13% of my five-hour usage in less than 10 minutes.
Now, Alexander Wang did report that there might have been a bug that was miscounting how much people were using of their plans, but still, whatever the cause, it didn't help the overall initial impressions.
And yet, Muse Wonder, or specifically Muse Wonderful, did win some adherence as well.
Developer and entrepreneur Theo again put Muse Wonderful in his S tier alongside Opus 5.5, and everything else being far below that.
Giving an example, he wrote, asked Opus 5.5, GPT61 Sol, and Muse Wonderful to fix a bug.
Opus found the root cause and filed a PR.
GPT61 Soul asked a question, crashed from the async question tool interrupt, found the bug, fixed it, wrote 300 lines of tests, and explained it in impossible-to-understand terms.
Muse Wonderful found a small PR someone else had filed and said you should probably merge this instead.
I really like this model.
Conductor's Charlie Holtz also liked the model.
He wrote, Quick impressions, found a real security vulnerability in our code base in one shot that other agents missed.
It's great at design and visualizations.
It really likes sub-agents, and lots of great details in the CLI.
Super impressed by the progress here.
Bone GPT wrote, I had early access to Muse Wonder, and it is a surprising model.
On every technical benchmark we ran, it was neck and neck or better than Astra Fable and Opus.
It has a delicate touch.
It makes inspired creative decisions.
There aren't really benchmarks for soulfulness, but Muse has it.
It's a warm model, a capable model, and it has big model smell.
Its outputs are happy, innocent, and friendly.
It never talks down to you like some of the other models.
It wants to help you make dope stuff.
It wants you to make money.
It's aligned with you.
Meta is going to win consumer agents in a landslide.
Claire Vaux broke her tests down by category, finding that on front-end designed, it was quite bad, writing anything other than emails, it was bad, that it wasn't great for SVGs, videos, and creative design, but that as she put it, it rolls with the big boys on coding, and on agentic tasks, it crushed, coming in first out of eight frontier models she tested.
Now, one interesting question is where this is going to fit in Meta's strategy.
Meta is, of course, much more focused on the consumer experience than other labs are, given their distribution and network of consumer apps.
About a month ago, I had observed that one of the things that was distinct about Muse was that it was the first AI product where most of its users just didn't care what model was powering it.
And yet, even though I believe that that is true, there were a fair number of users that started to run up against some limits in what Muse could do.
A week after I posted that on X, Sergito wrote, Anyone else finding Muse to be less smart than Instinct?
I gave them both a similar multi-step task, and Muse hallucinated some stuff and then kept compounding its error when trying to fix it.
And in fact, we've kind of been in a spot where, in the same way that I discussed power users using different models for different tasks, a lot of early adopters are using multiple different personal assistants.
Bryce Ent recently posted on X, What I've realized is that there is no one optimal personal assistant.
At the moment, I'm currently using Instinct, Muse, Grockbot, and Dots.
I genuinely enjoy using them all for specific use cases.
Now, that may be how it plays out, but I think for a lot of folks, the context switching cost of using multiple personal assistants is going to be significantly higher than the context switching cost for using models in other types of ways.
In other words, there are many use cases for LLMs and coding agents in general, where they can provide a ton of value even if they don't know anything about you.
Personal assistants, on the other hand, get more useful in proportion to what they know about you and the systems of yours they have access to.
And most people are going to have a hard time giving even one personal assistant access to all that information, much less a half dozen.
And with that in mind, the need for something like Muse Wonder or Muse Wonderful is written all over the recent pages of social media.
Investor and entrepreneur Satya Malik recently wrote that while Muse is very good at immediate tasks like booking flights and hotels, it is, in his words, terrible for long-term tasks.
For example, he said, It reminded me today that a meeting has not been set for 2 p.m.
That was a false alarm because the meeting was set for 2 p.m.
yesterday.
This has happened several times where it panics and tells me something because it gets the day wrong.
Investor Sam Lesson wrote, Tried to book a hotel with Muse last night.
Hilton's site put my agent in a doom loop.
Third retry, I gave up and booked it myself.
And it's quite clear that this type of challenge was on the mind of the meta team in building Wonder.
Chubby on X wrote, An interesting insight that was probably drowned in the release news: Meta built Wonder for agents that act on your behalf, starting with its Muse app.
Two features are really important: active memory, which keeps track of what matters to you across conversations, and active focus, which keeps a task going when it gets hard, tries other approaches, and recovers from errors.
Another question I had, though, looking at the launch media, is whether with the Wonder family of models, Meta is actually getting serious about going after not just personal agentic use cases, but professional ones as well.
Certainly, Mark Zuckerberg called it state-of-the-art performance for personal and professional agentic work.
Alexander Wang, in introducing it, wrote state-of-the-art at personal agents and professional agents.
And the AI at Meta account also explicitly mentioned both personal and professional agents, meaning that there was a coordinated messaging campaign to make sure to mention professional agents.
Now, that could mean that Meta is serious about professional use cases this time, or it could mean that they understand that implicit in a personal agent are going to be professional use cases, and that drawing a clear line might make sense from a company strategy standpoint, but doesn't match how consumers think about themselves.
In other words, it may not be that all of a sudden Meta wants to compete with Claude Code for enterprise deals, but that they believe that on an individual level, if consumers really choose and invest in a single personal agent, that personal agent is going to have to do professional stuff in many cases.
There is, of course, another category of professional that is already deeply, clearly important to Meta, which is small business owners who already use tons and tons of features on their other apps like Facebook and Instagram.
That's where Cetrini Research saw the viability, writing, Our takeaway is that Meta has a real shot at capturing agents for small business.
It's a really good balance of capability and execution.
For a lot of folks, the big story is not the endpoint and anything Wonder can do, but the delta and the rate of change.
Pulsios Ben Serra wrote, Meta is moving at lightning speed.
Muse launched 34 days ago, now they've joined the frontier.
Ethan Malik said that it seems to him like a good model from a limited test, but quote, perhaps more impressive, compare the progress.
Very fast progress from Meta in a short time.
Yu Chen Jin wrote, A year ago, many dunked on Meta for spending billions to hire top AI talent and acquire Alexander Wang.
I was skeptical too, to be honest.
But the success of the Muse app and models proves one thing.
Hire top talent, assemble a cracked team, give them an ambitious goal and enough resources, and they can work wonders.
Certainly markets liked what they saw with Meta up 4% on the news.
But what does this mean for the whole Pacing the Frontier conversation?
Among the AI CEOs, Zuckerberg has not been particularly aligned with the messaging coming from the others.
He did not sign the Pacing the Frontier letter, and a few weeks after it was published, he countersignaled with his essay, The Future is for Everyone.
His core thesis is that open and widespread access needs to be the core tenant for the AI era, even if that carries some extra risk.
In Zuckerberg's view, the concentration of power that comes from keeping unreleased models for internal use only could be even more disastrous than the risks associated with releasing powerful AI models.
Now, clearly, this set of wonder models isn't pushing the frontier and do seem to have very strong cyber guardrails, meaning that they are not dangerous compared to what's already available.
But from a trajectory perspective, Zuckerberg is showing no interest in slowing down.
In an interview with the Financial Times, he declared that Meta has reached the frontier and is, quote, already working on that next step up.
Rather than slowing down, he added that model development will, quote, probably feel like it'll go quite a bit faster from here.
He declined to give a number for his P Doom, the odds of AI killing everyone that got the entire world riled up over the past month.
Instead, he said, I'm much closer to the belief that AI is a technology that can be engineered with normal guardrails and built responsibly than the anthropomorphic vision of AI, which is that it's just going to go do its own thing.
Whether you agree with whether it's possible or not, there does seem to be a fundamental difference in how Meta views what they're building from the other labs.
In short, OpenAI and Anthropic are either trying to or feel like they inevitably are building machine gods that inspire awe, while Meta is trying to build what it views as just a normal technology.
Who's right or wrong about that remains the debate, but that is the fundamental dividing line.
Overall, when you take a step back, we headed into 2026 with three Frontier model labs in OpenAI and Anthropic and Google.
As coding agents forced their way to the top and showed that they were more important than everything else, at least in the short term, that number went down to two.
And yet now, especially if Gemini 4 Argon can do what Google says it can do, we are back to having five-ish Frontier labs competing in the US.
Then again, behind closed doors, as we heard in the headlines today, there might be much more powerful models just on the horizon.
So maybe that Frontier Duopoly will be right back soon.
For now, it appears that Meta is fully back in the game.
That's going to do it for today's AI Daily Brief.
Appreciate you listening or watching, as always, and until next time, peace.
