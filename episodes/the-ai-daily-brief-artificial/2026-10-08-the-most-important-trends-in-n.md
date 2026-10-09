---
record_id: "podcast:7e29f1d9-4b32-4800-a55c-f2f229925245"
episode_id: 7e29f1d9-4b32-4800-a55c-f2f229925245
title: The Most Important Trends in New AI Products
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/the-most-important-trends-in-new-ai-products/7e29f1d9-4b32-4800-a55c-f2f229925245"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/the-most-important-trends-in-new-ai-products/7e29f1d9-4b32-4800-a55c-f2f229925245"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-08
played_at: "2026-10-08T12:00:00Z"
play_count: 1
duration_seconds: 1620
source: pocketcasts-history-browser
played_label: Yesterday
history_order: 4
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 24aac16d2d5ab7886ff5acf1ee62be5bc5b17bb98710ee01cb6b97d9b59012d6
analysis_mode: health
summary_source: local
model_source: local
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: Qwen3.8-Flash-Next-UD-Q4_K_XL
tagging_model: sonnet
proposed_tags: []
proposed_entities: []
status: new
routed_to: null
---

## Summary

Hermes/News Research raised at a $1.5B valuation, with WSJ-reported 22M installs, ~2.5% global token usage, $36M annualized revenue and a $100M target, while CEO Dylan Rolnick framed open source as anti-lock-in and the company’s “non-negotiables” emphasized model choice, local/offline execution, prompt/tool visibility, memory control, exportability, and code access. Chip financing deals dominated: Oracle seeking Apollo/Goldman funding, Broadcom/Apollo/Blackstone in a reported $50B deal for OpenAI custom chips, and SpaceX seeking $40B for NVIDIA chips with Apollo leading, Pimco considering, and CDS pricing ~15% default by 2031. BioHub launched a $1.8B biological data initiative with Google and the US government to build an open dataset for AI biology, with Alex Rivez and Molly O'Shea framing it as infrastructure for virtual experiments. Anthropic expanded Mythos via cyber verification tiers—Defense, Red Team, Specialized—with reduced guardrails, government approval for high-risk systems, mandatory retention only for Specialized, and earlier government restrictions on Mythos/Fable; Nathan Lambert and JPMorgan CEO Jamie Diamond debated whether Mythos-class risk is an acceleration or a tenfold cyber-risk jump. RAMP data showed TypeSafe AI’s Jev gaining foundation-model share, Anthropic/SpaceX AI/OpenAI in top five, DeepSeek/OpenRouter/Featherless appearing, and Scale AI/Runway/Higgsfield signaling RL data and image/video spend. Product trends included Elon Musk saying Grokbot will route to the best backend model, including Claude Opus 5.5, Midjourney and Suno, while using fast Grok 4.8 for simple requests; Anthropic’s Claude Haiku 5/5.5 undercutting GPT-6 Luna and Chinese models on cost and benchmarks; Meta’s Muse iPad rollout with GitHub/Asana/QuickBooks/Canva connectors and Windows plans; OpenAI bringing GPT-6 to free ChatGPT users; and OpenAI’s B2B marketplace allowing committed spend on open models.

For the user, the actionable takeaways are procurement, risk, and research decisions: test model routing and cost-per-task rather than assuming one lab is best, benchmarking Haiku 5/5.5 against GPT-6 Luna, GLM 5.3 Flash, DeepSeek V41 Flash, and Jev for coding, computer use, and knowledge work; if privacy, auditability, or sovereignty matter, evaluate Hermes/News-style open agents and ask whether third-party model routing passes API costs, retains data, or allows opt-out. For health/biology work, watch BioHub’s open dataset and virtual-experiment claims as possible leads for cell modeling, assay prioritization, and drug-discovery workflows, but verify data provenance, consent, security, and whether models transfer to real lab results. For cybersecurity, decide whether Mythos-style reduced-guardrail access is needed and understand the tradeoff between zero retention and mandatory retention in Specialized Access; for investing, treat chip-financing headlines as credit-risk and capex-sustainability signals, especially Oracle, Broadcom/OpenAI, and SpaceX deals, and ask for auditable compute demand, customer concentration, and collateral before acting. Follow-up questions should cover whether enterprise demand for Chinese open models is driven by price or sovereignty, whether multi-model harnesses become standard in enterprise contracts, and whether image/video AI expands beyond marketing into construction/manufacturing.

## Transcript

Once again, this week we got some awesome new AI products and features.
We got a new type of generative UI and ChatGPT, a new model from Claude that shows that Anthropic is not going to compete just at the high end of models, and a big announcement from Elon that Grokbot will use whatever models it takes to have the best experience, not just Grok models.
In different ways, each of these announcements represents some key trends shaping AI right now.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, Section, Harbor, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AIDailybrief, or you can subscribe on Apple Podcasts.
And to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
I don't normally start with fundraising stories at the top of the headlines.
In fact, most fundraising stories don't actually make it.
And yet, I think that Hermes Creator News research reaching a valuation of $1.5 billion after a new funding round is worthy of discussion.
In the wake of OpenClaw, a group of people took the inspiration from what OpenClaw was doing and decided to do their own version in a slightly different way.
In all honesty, the group's early work felt like a mix of AI research and performance art, given that they were trying to build the first LLM trained across a distributed network of anonymous GPUs contributed by strangers on the internet.
Where they vaulted into the big leaks, however, was when they released the Hermes agent.
Hermes has the same sort of extreme user control and openness that attracted people to OpenClaw, but has been moving incredibly quickly.
In fact, pretty much any time that one of the closed labs releases some cool new feature or product, you can bet that Hermes is going to have some version of it available for their users quickly thereafter.
Putting some numbers on this, the Wall Street Journal reports that Hermes has now been installed 22 million times, and even more impressively, accounts for roughly 2.5% of global token usage overall.
With this funding, News intends to move from individual enthusiasts to the enterprise big leagues, suggesting that the fresh capital will fund the launch of Hermes for Business.
Alongside the jump to enterprise, this fundraising reinforces that open source has a viable business case in the AI industry.
News offers Hermes for free, with users able to bring their own models.
But they also have a range of different subscription options, which bundle frontier model usage in hosted instances.
The business model allowed News to grow to 36 million in annualized revenue so far this year, with a target of $100 million by year-end.
Announcing the fundraise, CEO Dylan Rolnick posted a note that was halfway between a celebration and an open source manifesto.
He wrote: The marginal cost to reproduce a piece of software has plummeted.
There are few benefits to keeping a technology like Hermes agent locked down, and many to proliferating it.
Users don't want lock-in, and they deserve observability into the thing they will allow into so many aspects of their lives.
Hermes as an open ecosystem gives them a foundation of trust.
We believe businesses of all size want the same liberties.
In a separate but at least philosophically related post on X, the official News Research account declared what amounted to their list of non-negotiables for AI: you should be able to use smarter models in your agent.
You should be able to use cheaper models in your agent.
You should be able to use local models in your agent.
You should be able to use a different model for every job.
You should be able to switch models in the middle of a conversation.
You should be able to choose what data your agent has.
You should be able to choose what it remembers and what it forgets.
You should be able to choose what computer your agent runs on.
You should be able to run it on a machine that never touches the internet.
You should be able to run it while your laptop is closed.
You should be able to reach it from apps you already use.
You should be able to choose how your agent thinks.
You should be able to read the prompt it runs on.
You should be able to see every tool it has and turns off the ones you don't want.
You should be able to teach it something once and never explain it again.
You should be able to know what it did and when and why.
You should be able to export your agent.
You should be able to read the code.
You should be able to change the code.
Your agent should be yours.
Congrats to the team there.
I'm excited to see that force and that energy have more resources behind it.
Next up, a bit of a different type of fundraising.
Tens of billions of dollars of chip financing deals are being arranged as the big players seek their next round of funding.
According to the Wall Street Journal, three big deals are being hashed out at the moment.
Oracle is reportedly seeking funding from Apollo and Goldman Sachs for what sources called a big purchase of chips.
The size of the deal wasn't disclosed, but with Oracle already at risk of a credit downgrade, this could mean they're turning to private markets in lieu of trying their luck in the investment grade bond market.
Broadcom is also in talks with private credit, with Apollo and Blackstone attached to a $50 billion deal to finance the production of OpenAI's custom chips.
That deal looks like Broadcom lending their credit rating to OpenAI to access a better interest rate, suggesting the Frontier Labs could struggle to borrow at investment grade once they go public.
The third deal has SpaceX approaching various lenders to borrow $40 billion to pay for NVIDIA chips.
The Financial Times reports that Apollo is leading the deal, which is among the largest in history.
A few lenders have already passed after receiving what can only be described as a soft bank-style investor deck.
Per the FT, they said they quote, only received a short two-page deal memo with pictures of outer space and an arrow pointing out that the company was going to build data centers, quote, somewhere in the universe.
One of the investors that passed on the deal commented, How are we supposed to take that to the investor committee?
And yet it seems like some investment firms are still willing to cut Elon a check, with Bloomberg reporting that Pimco is looking at the deal.
The financing for the next leg of the AI buildout is starting to draw more criticism on Wall Street as these mega deals come under scrutiny.
SpaceX credit default swaps spiked on the news, now pricing in a 15% chance of default by the end of 2031.
Still, some analysts are arguing that a few pictures of space should be enough.
Citrini wrote, It's about time that companies stood up to the ridiculous amount of information that investment committees demand in order to invest.
What more could you possibly need to know, other than there will be data centers and they will be extra-planetary yet intra-universal?
Ultimately, and this is probably the logic behind that memo: you either want to give Elon Musk $40 billion to build space data centers or you don't.
A giant folio of investor materials probably isn't going to change your mind.
Moving over to a very different area of the industry, Mark Zuckerberg's BioHub has launched a new $1.8 billion biological data initiative in collaboration with Google and the US government.
The group aims to build the largest open biological data set ever assembled.
This data can then be used to train AI models on more complex biological systems.
Models like Google's AlphaFold have mapped out protein biology, but BioHub believes the same can be done for entire cells.
BioHub head of science, Alex Rivez, said that the goal is to help scientists conduct virtual experiments so only the most promising ones progress to a physical lab.
He said, If we can put more and more reasoning and intelligence into every single question we ask in the lab, the value of those empirical results will be far greater.
We're at the beginning of a new scientific paradigm with AI.
Said Molly O'Shea, host of Sorcery, This is effectively an infrastructure build out for AI biology.
Instead of just building bigger models, they're attacking one of the biggest bottlenecks in biology AI today, generating standardized, high-quality biological data sets at massive scale and making it openly available to researchers.
On the model front, Anthropic has expanded access to Mythos under a new cyber verification program.
Mythos has mostly remained under lock and key since its launch in April, initially available to a few dozen companies selected to participate in Project Glasswing.
Anthropic even triggered a political incident when they expanded Project Glasswing to international firms across 15 countries in June.
A week later, the government ordered Anthropic to shut down Mythos and Fable entirely.
Global access to Fable was eventually returned, but the government ensured that Mythos was kept to a small group of U.S.
companies and government departments.
Anthropic's new cyber verification program looks to be the first major expansion of access to Mythos since launch.
Security professionals can now apply for access, which includes the use of Mythos as well as versions of Opus and Sonnet with reduced safety guardrails.
Anthropic is offering three tiers providing different guardrail settings.
Defense access will enable defense-focused cybersecurity tasks, like incident response, reverse engineering malware, and analyzing vulnerabilities.
Red Team Access will allow for limited offensive cyber activities like penetration testing.
Anthropic says red team access will still be subject to real-time blocks for actions that could cause physical harm or mass disruption.
Access to this tier will require enhanced vetting and is only available to enterprise customers rather than individual researchers.
Finally, Anthropic is offering a tier called Specialized Access, which has the fewest guardrails.
Access to this tier involves government approval and is reserved for organizations involved in testing high-risk systems like flight control, power grids, and financial plumbing.
This tier will replace and expand Project Glasswing.
Interestingly, the Specialized Access tier is the only one with mandatory data retention, with everything else being available under Anthropic's zero data retention policies.
Now, outside of X being filled with cyber professionals showing off their new access to Mythos, one of the more interesting conversations has been how our thoughts about the potential risks of a Mythos-class model have changed since it was announced back in April.
Open model researcher Nathan Lambert argued in a post earlier this week: if Claude Mythos was accidentally released as open weight, it seems like the world would have been more or less fine.
Yes, there would be a clear increase in cybersecurity incident, and it would be bad for society if the model leaked, but it would be a scenario that looks more like an acceleration than a step change in risk.
JPMorgan CEO Jamie Diamond disagrees, claiming that cybersecurity risks went up tenfold after Mythos, that's his phrase.
In an interview on Tuesday, Diamond said: AI created vulnerabilities that we didn't know about, and we always worried about cyber before these things.
Now, this is different than the conventional framing, with Diamond seeming to claim that AI capabilities created new risks rather than exposed existing ones.
And yet, in spite of this, Diamond is not calling for drastic measures to protect against AI hacking, commenting, I'm not going to get hysterical over is it existential or not.
What we're going to do is roll up our sleeves and going to work to fix it.
Lastly, today, a little feature for you musers out there.
Muse is now available on iPads, completing the trifecta of Apple devices.
The new iPad version is very similar to the iPhone version, but takes advantage of having more screen real estate and enhanced multitasking capabilities.
Alongside iPad support, Meta has added connectors for software tools including GitHub, Asana, QuickBooks, and Canva.
This update is focused on use cases for small business, with Meta introducing the ability to give Muse a high-level business goal and allowing it to work autonomously toward it.
Next up on the roadmap is Muse for Windows, with a Windows EVP announcing the port at a hardware launch event on Wednesday.
New features are, of course, the subject of our main episode, so with that, we will switch from the headlines and move on over into the main.
If you're leading AI inside an enterprise, you already know that the gap right now isn't capability but execution.
That's why KPMG's You Can with AI is back with a new season featuring conversations with leaders like Sorojit Chatterjee of Emma, Mehabib of Ryder, McKesson CIO Ellery Fisher, and others focused on practical execution.
What's working, what's not, and what it actually takes to move from pilots to real scaled impact across strategy, data readiness, governance, workforce, and value.
And of course, it's co-hosted by me, Nathaniel Whittemore.
Go listen and subscribe at www.kpmg.us slash AI podcasts.
That's www.kpmg.us/slash AI podcasts.
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
If you listen to this show, you likely have a thesis.
Maybe it's enterprise adoption, maybe it's compute, maybe it's a specific lab.
Harbor Capital's AI Lab Ecosystem ETFs let you express it via five actively managed ETFs, each seeking exposure to the ecosystem around one major lab: Anthropic, OpenAI, DeepMind, Meta, or SpaceX AI.
Your view of the AI race in ETF form.
Harbor Capital Advisors AI Lab Ecosystem ETF suite gives investors a way to invest in the AI ecosystem they believe is best positioned for success.
Search Harbor AI Lab Ecosystems ETFs wherever you invest or follow at Harbor Capital on X to learn more.
Visit harborcapital.com for a prospectus containing investment objectives, risks, fees, expenses, and other important information.
Read and consider it carefully before investing.
Risks include principal loss and artificial intelligence-related risks.
Harbor ETFs are distributed by Forside Fund Services LLC.
Harbor is not affiliated with AI Daily Brief, and the funds are not affiliated with, sponsored by, or endorsed by any AI lab.
This is a paid advertisement and not personalized investment advailable.
Investing involves risk, including possible loss of principal.
Blitzy's deep code-based understanding unlocks the thing every roadmap owner cares about: shipping new features.
Here's the truth about building inside a massive enterprise codebase: writing code was never the bottleneck.
Context is: which system does this touch?
Which contracts can't break?
Which standards apply?
Blitzy already knows because it reverse-engineered your entire code base into a dynamic knowledge graph before feature work began.
With that complete picture, Blitzy builds features end-to-end.
Architecture, APIs, UI, and tests all validated against your existing systems.
One Blitzy customer built an AI-native application from scratch with 100% autonomous completion, saving over 2,700 engineering hours.
Features that respect your code base instead of fighting it.
Stop letting your backlog grow faster than your team.
Accelerate your roadmap at Blitzy.com.
That's B-L-I-T-Z-Y.com.
Welcome back to the AI Daily Brief.
We are definitely in the exciting early fall time when companies are just absolutely pumping out products.
With AI, of course, there is less seasonality than other industries because everything is such a mad dash.
But still, this is one of those moments where you see an extra big concentration because everyone's back to school or back to work from the summer and not yet in holiday mode.
Plus, they're all planning for 2027, especially if you're dealing with enterprise budgets.
And so it is just an absolute explosion of new products and features.
In addition to that being very cool for us as consumers and users and builders, what's especially interesting right now is how much all of the new products and features being released express and embody key trends that are shaping the direction of AI overall.
So that's what we're going to be looking at today.
And to kick it off, to give us a frame of reference for some of those trends, I want to start with RAMP's most recent data drop.
For those of you who don't know, RAMP is effectively a next-generation banking and money type solution for dynamic tech-first enterprises.
They do bill payments, expenses, company cards, increasingly more traditional banking as well.
Each month, they published a list of their fastest-growing software vendors in terms of market share and revenue growth relative to size.
There is always an important grain of salt that the companies that use RAMP are themselves on the bleeding edge, and so this isn't going to necessarily reflect the entire enterprise sector, but there's still obviously a ton of value in understanding where the bleeding edge is because those early adopters tend to set the patterns that everyone catches up to eventually.
The data set is always interesting, but isn't necessarily usually surprising or all that enlightening.
It typically confirms a few companies that are converting Buzz into paying customers and shows whether Anthropic or OpenAI are currently leading in the market share war for foundation models with businesses.
October's list, however, was remarkable for just how many emerging trends it captured.
First of all, we have the ascendance of Jev showing up in the numbers.
TypeSafe AI, who are the creators of that decision model, ranked first in growth relative to size, which by the way seems to be the terminology that's becoming normalized versus the judgment model language that I was using before.
In any case, Jev and TypeSafe ranked first in growth relative to size and second in growth in market share terms.
Keep in mind that RAMP placed Jev in the Foundation LLM category, meaning it's gaining market share faster than all the other Frontier labs besides Anthropic.
Jev, in fact, gained a full point of market share within a month.
The point is, Jev is not just capturing mind share on X.
Startups and some advanced enterprises are actually signing up and using the model in a significant way.
The rest of the Frontier model rankings were more interesting than usual this month as well, with Anthropic, SpaceXAI, and OpenAI all ranking in the top five for capturing market share.
SpaceXAI in particular has rarely shown up in these rankings, suggesting that Grockbot is driving a significant amount of new business.
DeepSeek also featured on both lists, and model routers like OpenRouter and Featherless also showed up.
Ramp economist Eric Karazian wrote: Competitive factors like the introduction of cheaper models are pushing AI spend down.
The introduction of highly performance standard and light models and highly token-efficient models designed for specific enterprise use cases like Jev will threaten OpenAI and Anthropic's revenue growth among businesses.
In other words, these shifts are about more than just companies bouncing from one model to another.
There's a more structural realignment going on as companies build out these advanced model architectures that we've been talking about for the last several months.
For honorable mentions, we also have scale AI showing up on the growth relative to size chart for the first time in months, suggesting that data provision for reinforcement learning is heating back up.
This could either be reflective of the big training runs recently completed by each of the Frontier model labs, or it could be a hint that fine-tuning of open models is starting to pick up.
Runway and Higgsfield also both ranked on the market share growth list, with Carazian writing, the increased adoption of expensive image and video generation models will push AI spend up.
These use cases are comparatively expensive relative to the coding and language model use cases that have dominated enterprise adoption of AI.
Speculating about where strong new image and video models will take the industry, he continued, Today their use is largely limited to social media marketing and advertising.
Though you could imagine the bull case for AI being greater adoption of image and video models for construction and manufacturing automation, signs of what could come, but we're not there yet.
So, for our purposes for the rest of the episode today, the key idea is that even when it comes to the data, everything is showing a key set of trends, which are also showing up in the products themselves.
So, first up, one of the most interesting announcements of the week came from Elon Musk.
Early on Wednesday morning, he posted: Important note regarding Grokbot.
Going forward, SpaceX will use the best back-end model for any given task, including Claude Opus 5.5, Midjourney, Suno, and other leading APIs.
Whatever is most likely to give you the best outcome.
This is massive news.
We have been talking all year about the importance of harnesses and whether moats are going to be in the harness or the model domain.
And Elon is basically planting a flag here and saying that Grok is willing to compete on both fronts.
He did clarify later on that, quote, most bot requests are pretty simple and will be handled by a lightning fast version of Grok 4.8 when that comes out.
Our operating principle is to give Grokbot users the best possible combination of speed and intelligence.
In other words, this does not mean that SpaceX AI is looking away from their own models.
They're just willing to acknowledge that there is a difference between their models and the most advanced in certain areas.
And for some use cases, they're not willing to let the experience of Grokbot be compromised because of that differential.
Now, to the extent that people had negative responses to this, it was either that one, they already pay for Grok, so they don't want the fees for those other models to be passed on to them via those API costs, and two, for some, there is also a principled question, given that some amount of Grok's core audience are philosophically against some of the other labs, I did see some people requesting the ability to opt out and only use Grok models even if there is a difference in capability.
For some, the interesting thing is what this said about SpaceX's place in the overall race dynamics.
Investor Anisha Sharia called it SpaceX getting to eat their cake and have it too.
Quote, they get the benefits of being a lab, vertical integration into inference, and being a cursor-style router.
They have a state-of-the-art model, so labs can't bully them.
They can capture margin on third-party models through inference, and somehow they have access to Suno and Midjourney as well.
They can offer the overall best, the Pareto best, or the best-for-a-tail modality, and the house always wins.
And I agree, I find that interesting from a competitive dynamics perspective.
However, for the vast majority of people, and even the vast majority of my own interest in this, this is exciting primarily on a user experience basis.
The whole trend and trajectory of the industry is companies wanting more choice, not less choice, when it comes to their models.
Certainly, individuals who are willing to deal with context have been there already.
But as business and power users demand the ability to not be locked into one ecosystem, using the harness and product and the context that comes with it as the lock-in, but making the models mobile and transportable adds just a ton of value for users.
It is worth noting that it is still not the same as something like using Hermes Research, where you can really get access to any model.
These are all companies that have some relationship with Elon or Grok, for example, Anthropic running their models or training their models in SpaceX AI data centers.
And you're still not going to get access to the OpenAI models through this, but still, it clearly shows the trend of multi-modelness that I think is going to do nothing but get more in demand over time.
Wrote investor Thomas Tungus: No company can provide the best model for every use case.
Maximizing customer attention and retention is the most valuable asset in a commodity market.
And by the way, if we need more evidence that this is a trend and not just something that Elon is doing, remember that I argued that one of the most important, if under the radar, announcements from the OpenAI Dev Day was the fact that they're now selling open model inference through their B2B marketplace.
That means that when your enterprise makes a big spending commit with OpenAI, you can use a meaningful portion of that on not OpenAI models, but on other open models that are bought through their marketplace in exchange.
Even the companies that are spending the most to have the state-of-the-art, best, most frontier models realize that they're not going to be able to solve everything for everyone.
One other feature bonus, which will be irrelevant to some and hugely relevant to others, i.e., me, Grokbot now has direct access to search, read, and monitor X, which really does open up a ton of use cases around social media monitoring and other things.
I think it reflects a push for Agentic offerings to compete on UX streamlining, but we'll come back to UX in a minute.
For now, I want to talk about this idea of the Foundation Labs realizing that their owned models can't be everything to everyone.
Our next announcement seems to fly a little bit in the face of that, with Anthropic announcing Claude Haiku5, which is itself a very strong statement that this company is going to compete to provide cheap and fast models to compete at the bottom end of the market as well.
Anthropic called this the cheapest, fastest, and most capable small model they've ever released.
And performance looks pretty incredible across the suite of benchmarks showcased by Anthropic.
Haiku5.5 is light years ahead of version 4.5 to the point that there's no real comparison.
More importantly, against GPT-6 Luna, Haiku also wins across the board.
It scored more than double on Terminal Bench 4.0 for Agentic Coding, with a smaller edge on Frontier Code 1.1.
In computer use, Haiku scored 72.4% on OS World compared to 48.9% for Luna.
And on Knowledge Work, Haiku beat Luna on both GDP Val and AA Briefcase.
Artificial Analysis scored Haiku at 43 on the Intelligence Index, which amazingly puts it between Kimmy K3 and GLM 5.3 Flash.
But the big story is cost.
Anthropic is offering this model at a quarter of the cost of Sonnet 5.5 and half the cost of Haiku 4.5 per token.
And to reinforce that the model is intended to be used for quick small queries and for use on sub-agents, Anthropic is discounting tokens by 80% for smaller prompts below 100,000 tokens.
Artificial analysis found that this pricing structure meant Haiku cost 21 cents per task on max inference or 12 cents per task on extra high.
That's right in line with GPT-6 Luna, a few cents cheaper than GLM5.3 Flash and DeepSeek V41 Flash, and one-sixth the price of GPT-6.1 Sol.
Haiku was one of the most token-hungry models artificial analysis has ever tested, but it more than made up for it by being extremely cheap.
Now, in terms of the trend that this one represents, investor Hasib Qureshi sums it up simply: Narrative violation: if you want the cheapest LLMs, you should now buy American.
Back in June, both GLM and DeepSeek were on the cost and intelligence Pareto frontier.
At their price points, nothing could beat them.
Then the cost crisis hit, and in the last few months, the US labs have responded with aggressive price cuts and efficiency improvements.
Now, with the new Haiku, the frontier is fully reshaped.
The entire Pareto frontier is now owned by the US labs, Anthropic, OpenAI, and TypeSafe Jev.
Your move, China.
At this point, what will be interesting to watch is when push comes to shove, how much of enterprises' interest in the open models from China has to do with cost versus how much has to do with sovereignty and their ability to run those models on their own hardware and ensure that their data isn't ever used by anyone else for training.
The American labs have increasingly solved the cost side of that equation, but obviously haven't addressed the issue when it comes to concerns around sovereignty.
From OpenAI, we got two announcements and two trends they represent.
The first trend is better, more powerful models, even in free accounts.
OpenAI writes: Last month we introduced the first GPT-6 models for paid customers, and today we're bringing that next generation of intelligence to more people with a new GPT-6 model built for more than 1.2 billion people who use ChatGPT each week.
Given how much, even today, people's experience with AI and their perception of AI is dictated by the core free experience, this is a non-trivial upgrade.
Still, it was very clearly the second in the list of two important announcements, with the first being what OpenAI is calling intelligent UI.
Intelligent UI basically says, text is not the only way we want to receive information.
Instead, ChatGPT's new intelligent UI will use all sorts of other ways of presenting information to make it better and more contextual for whatever the query is.
This can be interactive visualizations, it can be charts, it can be images alongside recipes.
The goal is basically to give people the best possible answers by also giving them the best possible presentation of the information.
And you can see from all of the different OpenAI researchers chiming in that this was a non-trivial upgrade.
Issa Fulford writes, This is the result of many months of work from our team and so many amazing collaborators.
We built a library of native streamable components and a compiler that renders the interface as the model generates it.
We train the model to make thoughtful design decisions with these components, including when to use something interactive and when plain text still works best.
OpenAI's Andrew Chen added, It turns out the hardest part of generative UI isn't generating the UI.
Models have been able to generate good-looking HTML for a while.
The more interesting challenge is getting it to feel like it actually belongs in ChatGPT.
One of our big bets with Intelligent UI was that you didn't have to choose, that you could keep all the power of HTML and still have it feel fast and native like it was always part of chat.
The other half of the problem is model judgment.
How do we post-train GPT-6 to know when an interface would actually help?
What should it show you or let you do?
How do we make it useful and beautiful without taking over the conversation?
None of this was obvious when we started, and there's plenty we're still figuring out.
And indeed, some folks' first experience was that it felt to them like it made the information a bit less clear or like there was too much.
But overall, I think first impressions can be summed up by Ethan Mullik, who wrote, had early access to the intelligent UI experience and it was a nice change from walls of text.
It also suggests that increasingly we are going to see interfaces built on demand for the problem that you have.
So the two trends to keep track of here, the one that's farther out, like Ethan said, is generative just-in-time interfaces in general, but the more immediate and broader is just the idea that for the first time, you're seeing these foundation labs actually care about the product experience.
So far, they've gotten away with having fairly bad, unintuitive products because the intelligence you get access to through them is so powerful that it more than makes up for it.
Now that everyone has that sort of intelligence on tap, product differentiation is going to really matter.
Overall, I think a super interesting week for new features and product announcements, all with trends that are generally very net positive for consumers, be they individuals or businesses.
For now, however, that's going to do it for today's AI Daily Brief.
Appreciate you listening or watching, as always.
And until next time, peace.
