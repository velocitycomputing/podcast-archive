---
record_id: "podcast:95b04581-eff4-4034-9fb6-37ed970407dc"
episode_id: 95b04581-eff4-4034-9fb6-37ed970407dc
title: The AI Challenges Businesses Are Actually Focused On Right Now
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/the-ai-challenges-businesses-are-actually-focused-on-right-now/95b04581-eff4-4034-9fb6-37ed970407dc"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/the-ai-challenges-businesses-are-actually-focused-on-right-now/95b04581-eff4-4034-9fb6-37ed970407dc"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-09-18
played_at: "2026-09-18T12:00:00Z"
play_count: 1
duration_seconds: 1800
source: pocketcasts-history-browser
played_label: September 18
history_order: 55
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: fb36f17dcfa76a65b450662102a2e1b5987480e2a7f8e9ce82d80fc1aa03d7fe
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

The episode opens with two weeks of intense AI safety debate centered on recursive self-improvement and development pace, featuring Anthropic's proposed three-axis measurement framework (R&D automation with Claude leading 26% of tasks, oversight coverage with 0.002% escalation rates, and 6–12% compute allocation to safety). The conversation broadens to regulatory considerations, including Bridgewater CIO Greg Jensen's argument for treating compute concentration as a systemic risk requiring regulation similar to systemically important banks, potential antitrust carve-outs for safety coordination, and Andrew Ng's counterargument dismissing extinction risk as science fiction. The episode then shifts focus to actual enterprise priorities: businesses at the WSJ Technology Council Summit expressed pragmatic concern about guardrails rather than existential risk, and the real enterprise challenges are cyber security, model selection warfare (shifting to cheaper models), agent identity and access management, legacy system integration, and data sovereignty—not the safety debate dominating media.

For your business, treat data sovereignty as non-negotiable by owning infrastructure for sensitive information rather than relying on third-party APIs, following Latham & Watkins' model of buying Nvidia servers to keep proprietary data private. Adopt a multi-model strategy rather than consolidating on one vendor, since enterprises report rapid switching when tools underperform. Prioritize agent security and identity management systems before agents integrate with legacy systems, as the power of agents is escaping non-engineer containment. Plan for continuous cost optimization—the top 1% of AI spenders cut costs 10% by shifting to cheaper models while maintaining capability. Execute process re-engineering now rather than waiting for perfect tools, since competitive advantage lies in execution speed and the pace of innovation makes comprehensive transformation risky.

## Transcript

[00:00:00] It has been a heck of a last couple of
[00:00:01] weeks when it comes to the AI discussion
[00:00:03] in society. And yet in all of that, one
[00:00:06] group that's left trying to figure out
[00:00:08] if anything has actually changed for
[00:00:10] them or if they are just on the same
[00:00:11] path that they were before, is the
[00:00:13] businesses and enterprises that have
[00:00:15] been trying to figure out how to
[00:00:16] maximize AI for their own value for at
[00:00:18] this point a number of years. Today
[00:00:20] we're discussing both how enterprises
[00:00:22] are thinking about, if at all, this new
[00:00:24] era of AI safety, and also digging a
[00:00:27] little bit deeper to find out what the
[00:00:28] real concerns that businesses have and
[00:00:30] the real AI challenges they're facing
[00:00:32] right now. As always, we're in a moment
[00:00:34] where new challenges are creating new
[00:00:36] opportunities as well.
[00:00:39] The AI Daily Brief is the daily podcast
[00:00:40] and video about the most important news
[00:00:42] and discussions in AI.
[00:00:44] Welcome back to the AI Daily Brief
[00:00:46] Headlines edition, all the daily AI news
[00:00:48] you need in around 5 minutes. We are now
[00:00:51] 2 weeks into the AI safety discourse
[00:00:54] absolutely dominating the conversation.
[00:00:57] For those who think that awareness of
[00:00:59] these issues had been sorely lacking, it
[00:01:00] has been a very good period. Although
[00:01:02] now seeing polling numbers that suggest
[00:01:04] that something like 17% of Americans are
[00:01:06] completely convinced that AI is going to
[00:01:08] end humanity, there is certainly some
[00:01:10] reasonable concern that we might have
[00:01:12] over calibrated. Holding that discussion
[00:01:14] aside for a moment, one thing that I
[00:01:16] think almost everyone is looking for is
[00:01:18] increasing specificity. That is
[00:01:20] specificity of policy, but also
[00:01:22] specificity of monitoring, and it's to
[00:01:24] that that Anthropic speaks with their
[00:01:26] new proposed set of measurements to help
[00:01:28] the public understand just how quickly
[00:01:30] advanced AI is developing. Once you move
[00:01:32] past the scariest headlines, this
[00:01:35] month's safety debate has been largely
[00:01:36] about recursive self-improvement and the
[00:01:39] idea that AI development is A moving too
[00:01:42] fast, but B really about to move much
[00:01:45] more quickly. The threat of societal
[00:01:47] destruction makes for a good headline,
[00:01:48] but the AI researchers issuing the
[00:01:50] warnings have had a difficult time
[00:01:52] describing exactly what they've seen
[00:01:53] inside the labs. To better inform the
[00:01:56] public, Anthropic proposed a three-axis
[00:01:58] measurement to understand the current
[00:02:00] pace of AI development. The first axis
[00:02:02] is AI's ability to build the next
[00:02:04] version of itself. The second is
[00:02:06] Anthropic's ability to oversee and
[00:02:08] intervene in the actions of agents, and
[00:02:10] the third is the scale of resources that
[00:02:12] go into AI model development. Now,
[00:02:14] Anthropic explicitly notes that these
[00:02:16] measurements only look at how models are
[00:02:18] built. In other words, they are
[00:02:20] measuring only the inputs to model
[00:02:21] development, but they argue that these
[00:02:23] inputs are correlated to the growth in
[00:02:25] model capabilities. On the first
[00:02:27] measure, the use of AI models in future
[00:02:29] model training, Anthropic put together a
[00:02:31] measure they called the R&D automation
[00:02:33] index. It seeks to measure every aspect
[00:02:36] of model training, rate how automated
[00:02:38] each task currently is, and aggregate
[00:02:41] those rankings to express them as a
[00:02:42] single number. By Anthropic's measure,
[00:02:44] Claude now {quote} leads 26% of their
[00:02:47] R&D work, and {quote} collaborates on
[00:02:50] more than 90%. Anthropic's definition of
[00:02:53] AI-led R&D was tasks where a human
[00:02:55] provides a high-level goal, and the AI
[00:02:57] completes it end-to-end with human
[00:02:59] oversight. And here you see the
[00:03:01] challenge even as they are trying to be
[00:03:03] precise. They're talking about AI's
[00:03:04] leading R&D, but that definition of
[00:03:06] leading still includes the human
[00:03:08] providing a high-level goal, rather than
[00:03:10] the AI determining the goal, which is
[00:03:12] what I think some might assume when they
[00:03:13] hear AI-led R&D.
[00:03:15] For their part, Anthropic was careful to
[00:03:17] note that {quote} Claude is not
[00:03:19] operating fully autonomously for any
[00:03:20] measured subset of AI R&D work. Still,
[00:03:23] they noted that research automation has
[00:03:25] massively increased since Mythos
[00:03:26] finished its training run and has
[00:03:27] continued to ramp in recent months. In
[00:03:29] March, prior to Mythos, only 1% of
[00:03:31] Anthropic's R&D was led by AI. Mythos
[00:03:34] boosted this to 12% in May, and it has
[00:03:36] doubled since then.
[00:03:37] Regarding oversight of agents, Anthropic
[00:03:40] measured coverage, review latency, and
[00:03:43] escalation rates within their agent
[00:03:44] oversight systems. They said that around
[00:03:46] 30,000 agents are currently doing
[00:03:48] research and engineering work at any
[00:03:50] particular time. Anthropic claims to
[00:03:52] have 100% coverage of agentic actions
[00:03:55] for this work, instant AI review of any
[00:03:57] flagged actions, and around a 0.002%
[00:04:00] escalation rate for real-time review,
[00:04:03] meaning around 1 in 47,000 actions are
[00:04:05] blocked by the monitoring system.
[00:04:07] Anthropic also maintains an
[00:04:09] after-the-fact review system with 100%
[00:04:11] coverage. This system flags around
[00:04:13] 100,000 agentic transcripts per week
[00:04:15] that are then parsed for false positives
[00:04:17] with around 50 escalated to human
[00:04:18] review.
[00:04:19] In other words, around one or two
[00:04:21] transcripts per thousand cause any
[00:04:22] material concern.
[00:04:24] Finally, on resource allocation,
[00:04:26] Anthropic expressed their measure in
[00:04:27] terms of a percentage of overall compute
[00:04:29] dedicated to safety systems.
[00:04:31] Around 6% of the compute allocated to
[00:04:34] AI-assisted R&D went towards safety, and
[00:04:36] around 12% of the compute allocated to
[00:04:38] AI-led R&D went towards safety.
[00:04:41] Anthropic noted that this measure
[00:04:42] doesn't include classifiers that
[00:04:44] constantly monitor agentic activity, and
[00:04:46] is a {quote} imperfect proxy for how
[00:04:48] much a company focuses on safety. This
[00:04:50] is because safety research consists of
[00:04:52] individual researchers designing
[00:04:54] experiments, which is time-consuming
[00:04:56] even though running the experiments is
[00:04:57] not particularly compute-intensive.
[00:04:59] Overall, Anthropic's goal was not to
[00:05:01] provide perfect measures. Instead, it
[00:05:03] was to define and propose a set of
[00:05:05] metrics that any AI lab could report as
[00:05:07] part of a regulatory system. They
[00:05:09] conclude, "As the world considers pacing
[00:05:11] the frontier, we should do everything
[00:05:13] possible to minimize the gap between
[00:05:14] what frontier labs know and what the
[00:05:16] public knows. This means better
[00:05:18] measuring the development of AI,
[00:05:19] reporting on it publicly, and giving
[00:05:21] society an opportunity to decide how to
[00:05:23] use this information. We hope to model
[00:05:25] that transparency by releasing these
[00:05:27] measurements, and will continue to do
[00:05:28] so."
[00:05:29] Now, the response to this announcement,
[00:05:31] I think, shows the good, bad, and
[00:05:33] difficult of this particular moment. On
[00:05:35] the one hand, it is the rare move where
[00:05:37] people on all different sides of the AI
[00:05:38] safety debate largely think that this
[00:05:40] existing is better than it not existing.
[00:05:42] AI safety researcher Geoffrey Ladish
[00:05:44] writes, "Great to see this from
[00:05:45] Anthropic. A few weeks ago, I wrote that
[00:05:47] the company could be a lot more
[00:05:48] transparent and I appreciate how they've
[00:05:50] stepped up both with this and the recent
[00:05:52] incident investigation report and misuse
[00:05:54] report. At the same time, there were
[00:05:56] plenty of people who also wanted to see
[00:05:57] more. Prime Intellect's Elie Boussaid
[00:05:59] writes, "Interesting that OpenAI gives
[00:06:01] us the breakdown of usage per R&D task
[00:06:04] and Anthropic gives us automation
[00:06:05] levels. Would be great to combine both
[00:06:07] and get the evolution of automation per
[00:06:08] R&D task." There are also some who argue
[00:06:11] that the self-reporting, while a fine
[00:06:12] start, isn't enough. Arun Rao writes,
[00:06:15] "We need standard measures across all
[00:06:17] labs to measure progress to RSI and
[00:06:18] publicly report on it weekly to
[00:06:20] monthly." Now, one discussion that we'll
[00:06:22] see a lot more of, especially as markets
[00:06:24] digest all of this, is that one way,
[00:06:26] perhaps a cynical way, perhaps a
[00:06:27] realistic way, to look at an increase in
[00:06:30] safety monitoring is to view it as
[00:06:32] really expensive overhead for R&D.
[00:06:34] Meaning that these measures of
[00:06:35] percentage of spend on safety is
[00:06:37] basically a measurement of that
[00:06:38] overhead. Will markets reward companies
[00:06:40] that spend more on safety or will they
[00:06:42] punish them for cutting into their own
[00:06:44] margins? This shows another complication
[00:06:46] for having these companies operate in a
[00:06:47] public market environment. For what it's
[00:06:49] worth, this week also reminded that
[00:06:51] recursive self-improvement is not just
[00:06:53] the province of the US labs. ZAI
[00:06:55] released a blog post on Thursday called
[00:06:57] "Towards Recursive Self-Improvement: How
[00:06:59] GLM Built Its Own Inference
[00:07:00] Infrastructure." The first sentence
[00:07:02] reads, "As we develop GLM, the model
[00:07:04] sometimes exhibits capabilities that
[00:07:06] surprise us and even unsettle us. The
[00:07:08] most recent moment that shook us, GLM is
[00:07:11] increasingly helping build AI itself. We
[00:07:13] watched the model complete an
[00:07:14] infrastructure task that would have
[00:07:16] previously taken a team of experienced
[00:07:17] infrastructure engineers weeks. When we
[00:07:19] realized that this work would directly
[00:07:21] change how the next generation of models
[00:07:22] is trained, we became even more
[00:07:24] convinced." "Our successors are the AI
[00:07:26] systems we are creating ourselves." It's
[00:07:29] certainly beyond the scope of the
[00:07:30] headlines, but it is a reminder that any
[00:07:32] slowdown discourse that does not include
[00:07:33] China is basically no discourse at all.
[00:07:37] Meanwhile, if I'm correct that we have
[00:07:39] now entered this new negotiation period
[00:07:41] for the next generation of AI, where it
[00:07:43] is no longer just the AI lab that
[00:07:45] determine our pacing, lots of people are
[00:07:47] now stepping in with proposals for what
[00:07:49] the new overall system might look like.
[00:07:51] Bridgewater CIO Greg Jensen made
[00:07:53] headlines this week by suggesting that
[00:07:54] concentration of power is the major AI
[00:07:56] risk to be regulated. Bridgewater is one
[00:07:59] of the world's most successful hedge
[00:08:00] funds and has used AI extensively over
[00:08:02] recent years. In an interview with The
[00:08:04] Information, Jensen discussed his views
[00:08:05] on where AI risk actually resides and
[00:08:08] how he would approach regulation. He
[00:08:10] said, "There's a huge problem with
[00:08:12] open-source models because you can train
[00:08:13] them. We do this at Bridgewater. It's
[00:08:15] extremely effective reinforcement
[00:08:16] learning training on powerful
[00:08:17] open-source models. It's extremely
[00:08:19] powerful, a great technology, and at the
[00:08:21] same time clearly a very dangerous one.
[00:08:23] You don't know what people are doing
[00:08:24] with them. There's no way to track that.
[00:08:26] So, it's dangerous from that
[00:08:27] perspective. We haven't even begun the
[00:08:29] conversation on how to deal with that
[00:08:30] issue.
[00:08:31] And yet, in Jensen's view, that risk
[00:08:34] pales in comparison to the risk posed by
[00:08:36] the frontier labs themselves."
[00:08:38] He continued, "We have to deal with the
[00:08:39] concentration of power. In 2 years,
[00:08:42] OpenAI and Anthropic are going to
[00:08:43] control 35% to 50% of the world's
[00:08:45] compute. That's a crazy outcome for a
[00:08:48] society to allow on something as
[00:08:49] powerful as compute. Would we let one
[00:08:52] entity control that much of some other
[00:08:53] form of energy or commodity?
[00:08:55] Now, one of the common observations over
[00:08:57] the past month has been that the Hugging
[00:08:58] Face incident and other security
[00:08:59] breaches like it require immense amounts
[00:09:02] of resources to power agent swarms. It's
[00:09:05] unclear that they could be replicated by
[00:09:06] threat actors outside of the frontier
[00:09:08] labs, at least with current models,
[00:09:10] because of limits in their access to
[00:09:11] compute. Jensen argued that part of the
[00:09:13] solution needs to be clear guidance on
[00:09:15] liability for actions taken by AI, so
[00:09:18] the companies and individuals understand
[00:09:20] the risk they're taking."
[00:09:21] When asked how he would deal with the
[00:09:23] concentration of power, Jensen
[00:09:24] responded, "We should take anybody that
[00:09:26] has more than X%, let's say 5% of the
[00:09:28] world or US's compute resources. Say,
[00:09:31] okay, those are systemically important
[00:09:32] institutions. We're going to put them
[00:09:34] into some sort of thing like we do with
[00:09:35] systemically important banks and say
[00:09:37] there's going to be regulation. I also
[00:09:39] think it's fine to say we're going to
[00:09:40] have caps on how much you can own.
[00:09:42] There's a cap on how many commodity
[00:09:43] futures you can own. There's a cap on
[00:09:45] much less important things. We may be
[00:09:47] able to do that with current law. You
[00:09:48] may need new laws. Either way, let's get
[00:09:50] going on sorting that out legally. There
[00:09:52] should be a bipartisan recognition that
[00:09:54] you shouldn't want monopolistic control
[00:09:56] on what I think most people will agree
[00:09:57] is one of the most important resources
[00:09:59] in the world.
[00:10:00] Now, I could spend the next week's worth
[00:10:02] of episodes discussing the implications
[00:10:03] and challenges of trying to apply
[00:10:05] GSIB-style regulation to existing
[00:10:07] compute. But, what I like about this
[00:10:09] discourse is that not only does it leave
[00:10:11] behind overly simplistic binaries, it
[00:10:13] starts to ask questions about where the
[00:10:14] actual locus of power is. Is the problem
[00:10:17] in the models or is the problem in the
[00:10:18] power to run the models? Those have very
[00:10:20] different intervention points if we're
[00:10:22] trying to stop bad outcomes, and that's
[00:10:24] exactly the sort of conversation we need
[00:10:25] to be having.
[00:10:27] Now, one additional dynamic of the
[00:10:29] safety question that has been playing
[00:10:30] out is a legal question of whether the
[00:10:32] labs can actually coordinate on safety
[00:10:34] or whether that implicates antitrust
[00:10:36] issues.
[00:10:37] The Trump administration is reportedly
[00:10:39] considering an antitrust carve out to
[00:10:40] allow frontier labs to collude on
[00:10:42] safety.
[00:10:43] Now, the theory that this deals with is
[00:10:45] basically that an AI slowdown could mean
[00:10:47] a coordinated reduction in research
[00:10:48] spending and therefore an increase in
[00:10:50] profitability at the expense of the
[00:10:52] consumer. In the abstract and in very
[00:10:55] loose analogy, it would not be
[00:10:56] dissimilar to if Apple and Samsung
[00:10:58] agreed to stop working on new phones.
[00:11:01] Associate US Attorney General Stanley
[00:11:02] Woodward said the administration is
[00:11:04] considering an update to interagency
[00:11:06] antitrust guidance to provide a carve
[00:11:08] out for AI safety coordination. The
[00:11:10] guidelines already allow for
[00:11:11] coordination on cybersecurity risks, so
[00:11:13] a change would extend that guidance to
[00:11:15] AI safety. Interestingly, Woodward said
[00:11:17] that although multiple AI executives
[00:11:19] have publicly called for an antitrust
[00:11:20] carve out, no one has contacted his
[00:11:23] office on the matter as of yet. Even
[00:11:25] without guidance though, Woodward has
[00:11:26] indicated that the DOJ has no objections
[00:11:28] to a coordinated slowdown, commenting,
[00:11:31] "It doesn't occur to me that
[00:11:32] coordinating on cybersecurity or
[00:11:33] security is anti-competitive." Europe's
[00:11:36] antitrust chief, Teresa Ribera, agreed.
[00:11:38] Speaking at the same event, she said,
[00:11:40] "This is a classic game theory problem.
[00:11:42] When the risks are shared, cooperation
[00:11:44] is in everyone's interest."
[00:11:46] At the same time all of this is
[00:11:47] happening, there are certainly still
[00:11:48] many out there who are trying to tone
[00:11:50] down the tenor of the conversation in
[00:11:51] general.
[00:11:52] Legendary AI researcher and Coursera
[00:11:54] co-founder, Andrew Ng, in an interview
[00:11:56] with Bloomberg TV, dismissed extinction
[00:11:58] risk as science fiction and warned that
[00:12:00] AI doomers have pushed this narrative
[00:12:01] numerous time over the past decade in a
[00:12:03] bid to gain publicity for their cause
[00:12:05] and help shape regulation. He said, "I
[00:12:07] was quite dismayed over the past 2
[00:12:09] weeks. This wave of PR has kicked up
[00:12:11] again for probably similar purposes."
[00:12:13] Andrew acknowledged that there are
[00:12:14] genuine risks associated with AI largely
[00:12:17] around cybersecurity, but said, "This
[00:12:18] recent fear about AI leading to human
[00:12:20] extinction and so on is much more
[00:12:22] science fiction than science. It's very
[00:12:23] damaging." In his view, the dangers
[00:12:25] posed by AI are {quote} practical
[00:12:27] engineering problems, and the industry
[00:12:29] needs to continue on {quote} many of the
[00:12:31] wonderful things it can do.
[00:12:33] And speaking of real here and now
[00:12:35] cybersecurity issues, Mistral has been
[00:12:38] hacked for the second time with their
[00:12:40] intellectual property now available for
[00:12:42] purchase on the dark web. In May, around
[00:12:44] 5 GB of internal source code and around
[00:12:46] 450 private repos were exfiltrated and
[00:12:49] offered for sale, and now it's happened
[00:12:50] again with hackers offering full source
[00:12:52] code, internal development files, web
[00:12:54] app code, and additional proprietary
[00:12:56] information. A next user called Benny
[00:12:58] said that they contacted the seller and
[00:13:00] confirmed the file dump included model
[00:13:01] weights, post-training pipelines, and
[00:13:03] data set construction. The hacker was
[00:13:05] asking $25,000, but deleted their post
[00:13:07] shortly afterwards, likely either
[00:13:09] because they found an exclusive buyer or
[00:13:11] got sloppy with their opsec and needed
[00:13:13] to disappear. Later in the day, Mistral
[00:13:15] said that they found no evidence of
[00:13:16] unauthorized access after a thorough
[00:13:18] investigation, suggesting perhaps that
[00:13:20] this is the same material from the May
[00:13:22] break-in coming up for sale again.
[00:13:24] Lastly today, one model release that
[00:13:26] went a little under the radar this week
[00:13:28] was Gemini 38 live extended thinking.
[00:13:30] The model is another live speech model,
[00:13:32] meaning it can process continuous
[00:13:34] conversations rather than using a
[00:13:35] turn-based structure. It topped the
[00:13:37] artificial analysis speech-to-speech
[00:13:39] index, beating out GPT live one Astra
[00:13:41] and Grok voice think fast 2.0. Aside
[00:13:43] from the smooth conversation style, the
[00:13:45] model also supports near real-time
[00:13:47] visual inputs, automatic detection for
[00:13:49] 97 languages, and handoff for tool calls
[00:13:52] to allow it to complete tasks in the
[00:13:53] background.
[00:13:54] Tim Messer Schmidt, a developer
[00:13:56] relations lead at Google, published a
[00:13:57] cool tech demo showing the model
[00:13:59] powering a reaching mini robot. Tim
[00:14:01] demonstrated the model's ability to keep
[00:14:02] up a seamless conversation that we use
[00:14:04] between English and German. Speculating
[00:14:06] about the implications, Greg Eisenberg
[00:14:07] wrote, "Are invisible interfaces coming?
[00:14:10] Google just announced Gemini 38 live. It
[00:14:13] can talk through a task with you and
[00:14:14] then keep working after the conversation
[00:14:16] ends."
[00:14:17] I think 90% plus of vertical SaaS will
[00:14:19] need a voice front door. By that, I mean
[00:14:21] the way you use the software becomes
[00:14:22] talking to it, and the typing, clicking,
[00:14:24] and form filling happens on the other
[00:14:25] side without you. So, a contractor
[00:14:28] standing on a job site just says what
[00:14:29] went wrong out loud, and by the time
[00:14:30] he's back in the truck, the quote is
[00:14:32] sent, inventory is checked, the CRM is
[00:14:33] updated, the customer got a text, and
[00:14:35] anything risky is flagged for him. Kind
[00:14:37] of the dream, right? The same thing
[00:14:39] works for nurses, dispatchers,
[00:14:40] recruiters, brokers, insurance agents,
[00:14:42] etc. The person talks, and the agent
[00:14:44] finishes the admin. Lots of
[00:14:46] opportunities here to build voice-first
[00:14:47] businesses. I think this is how vertical
[00:14:50] software becomes invisible. Nobody logs
[00:14:52] in, nobody fills out a form, and nobody
[00:14:53] learns your interface. You just talk,
[00:14:55] and the work gets done behind you. This
[00:14:57] is a glimpse of where SaaS is going. Not
[00:15:00] fully there yet, but it's coming.
[00:15:02] In this weekend's long read {slash} big
[00:15:03] think episode, I get a little bit more
[00:15:05] into this particular shift as well as a
[00:15:07] bunch of other shifts in how we use AI.
[00:15:09] But for now, that's going to do it for
[00:15:10] the headlines. Let's move over on into
[00:15:12] the main episode where we talk about
[00:15:14] what, after this couple weeks of crazy
[00:15:16] AI safety discussions, big enterprises
[00:15:18] are thinking about their priorities with
[00:15:19] AI next.
[00:15:21] Welcome back to the AI Daily Brief. The
[00:15:23] background context for today's episode
[00:15:25] is, of course, the AI safety debate,
[00:15:27] which has completely broken containment
[00:15:29] over the last couple of weeks. And yet,
[00:15:31] even as we have seen the political
[00:15:34] resonance of this issue absolutely
[00:15:36] explode and polling showing very dynamic
[00:15:39] fast-shifting attitudes around it,
[00:15:41] enterprises and businesses of all shapes
[00:15:42] and sizes are still stuck out here
[00:15:45] figuring out whether it has any real
[00:15:47] implications for them or whether they
[00:15:49] just need to keep on keeping on.
[00:15:51] Today, we're looking at some specific
[00:15:53] answers to that question, as well as a
[00:15:54] few of the broader AI challenges that
[00:15:56] enterprises and businesses are actually
[00:15:58] focused on right now.
[00:16:00] Certainly, the safety debate has found
[00:16:02] its way to the business leader
[00:16:03] conversation. When the Wall Street
[00:16:05] Journal asked for a show of hands at the
[00:16:06] WSJ Technology Council Summit on Monday,
[00:16:09] only a few people said that they were
[00:16:11] worried that AI might kill us all.
[00:16:13] At the same time, around half of
[00:16:15] attendees said that they were in favor
[00:16:17] of slowing down frontier AI research and
[00:16:19] prioritizing better guardrails. This
[00:16:21] sort of comports with my thesis that I
[00:16:23] shared, I think, in last Thursday's big
[00:16:25] AI safety episode, that while I believe
[00:16:27] that the markets would view any sort of
[00:16:29] slowdown as, initially, a big risk for
[00:16:31] AI, I actually think that there is a
[00:16:33] very compelling economic counterargument
[00:16:35] that a slower pace of new development
[00:16:37] might actually increase the amount that
[00:16:39] companies were spending on AI.
[00:16:41] The thesis was basically that the
[00:16:42] incredible speed and pace of change
[00:16:45] actually, in some ways, creates a
[00:16:46] disincentive for companies to try to do
[00:16:48] comprehensive transformation on the
[00:16:50] logic that they're going to spend all
[00:16:51] this time and energy on transforming
[00:16:52] into something that isn't even relevant
[00:16:54] anymore by the time the transformation
[00:16:56] is complete. Indeed, moving back to the
[00:16:58] Technology Council Summit, on the
[00:16:59] panels, the big takeaway was that an AI
[00:17:01] slowdown actually doesn't really have
[00:17:03] that many implications for the way
[00:17:05] enterprises are using AI right now.
[00:17:07] Vishal Talwar, the president of FedEx
[00:17:09] Dataworks, said, "It's in our hands and
[00:17:11] it's up to us to apply AI for good, and
[00:17:13] I think it can do a lot of good for
[00:17:15] society."
[00:17:16] The discussion basically still centered
[00:17:18] around the need for prudent AI
[00:17:19] governance around normal business risks
[00:17:21] rather than the existential risks that
[00:17:23] are dominating the media discourse.
[00:17:25] Up north at the Canada Investment
[00:17:27] Summit, BlackRock CEO Larry Fink was far
[00:17:29] more worried about the data center
[00:17:31] backlash than X risk. He warned that
[00:17:33] construction delays could make AI the
[00:17:35] quote domain of large firms. Fink added,
[00:17:38] "The faster we can build out more
[00:17:39] capacity, the more we can democratize
[00:17:41] and make it available for everyone."
[00:17:43] In the startup world meanwhile, founders
[00:17:44] are starting to think about the
[00:17:45] governance and monitoring tools that
[00:17:47] businesses will need as agents get more
[00:17:48] powerful. One venture investor told The
[00:17:51] Information that they're beginning to
[00:17:52] focus on startups building tech that
[00:17:54] improves model security and
[00:17:55] infrastructure.
[00:17:56] In other words, private markets are
[00:17:58] responding to all of this concern by
[00:18:00] funding startups that can address
[00:18:01] specifics around this concern, which to
[00:18:03] me is part of exactly what you want to
[00:18:05] see.
[00:18:06] Microsoft also tried to bring the AI
[00:18:08] safety discussion back to some of the
[00:18:09] broader AI business sovereignty points
[00:18:11] that they've been trying to make for the
[00:18:12] past several months. This week the
[00:18:14] company dropped a very extensive
[00:18:16] 15,000-word code of conduct document
[00:18:19] that has, as they put it, a single
[00:18:21] overriding objective, that humans must
[00:18:22] retain meaningful control over AI so
[00:18:25] that it can help people live healthier,
[00:18:26] happier, and more productive lives.
[00:18:28] A lot of the discourse around this
[00:18:29] document was its outright rejection of
[00:18:32] AI consciousness and a prohibition of
[00:18:34] designing AI to even imitate
[00:18:36] consciousness. But in his post about
[00:18:38] this on X, Microsoft CEO Satya Nadella
[00:18:40] also brought up the implications for
[00:18:42] businesses themselves writing, "For
[00:18:44] firms, it's imperative that they retain
[00:18:46] full control over their unique and tacit
[00:18:47] knowledge. Every organization should be
[00:18:49] able to build its own continuous
[00:18:51] learning loop and hill climbing machine
[00:18:53] without becoming dependent on any one
[00:18:54] model provider and have the ability to
[00:18:56] embed its own knowledge into models and
[00:18:58] weights they control." Basically, part
[00:19:00] of this is power concentration in the
[00:19:01] firms and a way to deal with power
[00:19:03] concentration in the firms is to not
[00:19:04] surrender power to the firms in the form
[00:19:06] of your unique and proprietary data.
[00:19:08] Now, meanwhile, outside of the AI safety
[00:19:10] conversation, there had started to be
[00:19:12] some debate about AI market signals in
[00:19:14] the form of enterprise spent. On
[00:19:16] September 9th, Ramp released its latest
[00:19:18] AI index that found that AI spend
[00:19:20] declined among the top 1% of businesses
[00:19:23] spending on AI. In August, wrote Ramp
[00:19:25] lead economist Eric Carrizales, the top
[00:19:28] 1% of businesses spent $7.2 thousand per
[00:19:30] employee per month, which was down 10%
[00:19:32] from a July peak of 8,000.
[00:19:35] Now, we've talked a lot about the limits
[00:19:36] of Ramp data. Ramp has a very, very
[00:19:38] highly concentrated tech-forward, early
[00:19:40] adopter type of audience. It is also
[00:19:42] pushing products that are specifically
[00:19:44] about cost efficiency. But, of course,
[00:19:46] when you take all those caveats, it
[00:19:47] still provides an interesting and
[00:19:48] important signal.
[00:19:50] Now, when it comes to their analysis in
[00:19:51] this particular area, I personally think
[00:19:53] that they are underestimating summer
[00:19:54] seasonality as a driving force. But,
[00:19:57] their take is that this is about the
[00:19:58] most sophisticated AI users getting more
[00:20:01] adept at complex model architectures
[00:20:03] that don't rely on the most expensive
[00:20:04] models at all times.
[00:20:06] Arrow wrote, "My take is that it's not
[00:20:08] because of Chinese open models, it's
[00:20:09] model wars. Price cuts plus a growing
[00:20:12] share of spend is shifting to standard
[00:20:13] and light models, which are already
[00:20:14] cheaper over the frontier."
[00:20:16] Now, speaking of Ramp not necessarily
[00:20:18] having exactly the right analysis all
[00:20:20] the time, even though their data is
[00:20:21] really valuable, while they had
[00:20:23] previously caused a bunch of frantic
[00:20:24] headlines when they showed that
[00:20:25] businesses weren't adopting Fable,
[00:20:27] arguing all sorts of reasoning for that
[00:20:28] besides the obvious one, which was data
[00:20:30] retention policies. But, to their credit
[00:20:32] in more recent reporting, they found
[00:20:34] that Fable 5.1, which got rid of the
[00:20:36] data retention requirements, had started
[00:20:38] to make up 22.5% of enterprise spend and
[00:20:40] was rising very quickly.
[00:20:42] But, what about overall? On September
[00:20:44] 10th, Box's Aaron Levie wrote a long
[00:20:46] post on X about the issues that he was
[00:20:48] hearing about from executives across
[00:20:50] industries including banking, media,
[00:20:51] information services, and insurance when
[00:20:53] thinking about AI and agents in the
[00:20:55] enterprise. The big trends that Aaron
[00:20:57] heard about were cyber, model battles,
[00:20:59] agent security and identity, process
[00:21:01] re-engineering, architecture adjustment,
[00:21:04] evals, and the hurdle of legacy systems.
[00:21:07] On cyber and security, he wrote,
[00:21:09] "Everyone is nervous about the growing
[00:21:10] rate of vulnerabilities coming at them
[00:21:11] from AI and the implications of the Open
[00:21:13] AI Hugging Face incident. The
[00:21:15] conversation is not as existential as it
[00:21:17] is in Silicon Valley, but still highly
[00:21:18] concerned and pragmatic about what to do
[00:21:20] about it operationally in their
[00:21:21] environments. Lots of new discoveries
[00:21:23] due to AI and still hard to keep up with
[00:21:25] all the changes they have to execute
[00:21:26] now." Adding in what he wrote about
[00:21:28] agent security, he continues, "Somewhat
[00:21:30] tied to Hugging Face, there's much more
[00:21:31] awareness to the new challenges around
[00:21:33] agent security and identity management
[00:21:35] in a world where agents are trying to
[00:21:36] get into every system they can. In a
[00:21:38] perfect world, enterprises could set up
[00:21:40] identities for all their agents and
[00:21:41] control what they're doing, but of
[00:21:42] course, sometimes the agent needs to act
[00:21:44] exactly as the user as well.
[00:21:46] This is certainly something that we've
[00:21:47] seen a lot in our conversations in the
[00:21:48] podcast context as well as Super
[00:21:50] Intelligent. And interestingly, a lot of
[00:21:52] the security concerns aren't just about
[00:21:54] malicious actors. It is to some extent
[00:21:56] rooted in just the general power of
[00:21:57] these systems.
[00:21:59] Now that it's not just engineers who
[00:22:00] have access to agents, many companies
[00:22:02] are finding that the agents are powerful
[00:22:04] enough that they escape the containment
[00:22:05] of the non-engineers that are using
[00:22:07] them, even if those non-engineers aren't
[00:22:08] trying to do anything problematic. This
[00:22:11] is also showing up in the numbers.
[00:22:13] Once again, looking at Ramp data, lead
[00:22:14] economist Eric Kerosian writes, "One
[00:22:17] area companies are increasing their
[00:22:18] spend is AI security software. In the
[00:22:20] wake of the Hugging Face hack, three of
[00:22:22] our trending software vendors make
[00:22:23] software specifically designed to
[00:22:25] monitor agents in production. Now, he
[00:22:27] did point out that these specific
[00:22:28] vendors might not have done anything to
[00:22:29] stop the Hugging Face hack, but it's
[00:22:31] clearly a category focus for business
[00:22:33] buyers as well as startup builders.
[00:22:35] Another interesting area that Aaron
[00:22:37] talks about is the nascent exploration
[00:22:39] of open source and alternative model
[00:22:40] architectures. He wrote, "Most companies
[00:22:43] are deploying multiple frontier models
[00:22:45] within their enterprise. Too hard to
[00:22:46] standardize on anything and seeing
[00:22:48] different preferences across their teams
[00:22:49] and use cases, but the dollars are still
[00:22:52] concentrated on just a few vendors. Open
[00:22:54] weights still in infancy at scale in
[00:22:55] most of these organizations, often due
[00:22:57] to lack of domestic frontier open source
[00:22:59] options.
[00:23:00] Plenty of appetite for more options
[00:23:02] here, but so far few places to go.
[00:23:04] Now, paired with that I think is Aaron's
[00:23:06] observation that there is a ruthless
[00:23:07] adjusting of architectures.
[00:23:09] Most companies, he wrote, had examples
[00:23:11] of changing systems out multiple times
[00:23:13] just in the past year or two with
[00:23:14] different vendors.
[00:23:15] I probably haven't heard we tried X and
[00:23:17] it didn't work so I've gone with Y more
[00:23:19] than in today's environment. The lesson
[00:23:21] here is that because innovation is
[00:23:22] happening so fast, no one hangs around
[00:23:24] until a vendor gets something right.
[00:23:26] They just move on to the next one.
[00:23:28] Now, I think this sets really
[00:23:29] interesting context for watching some of
[00:23:31] the competitive dynamics right now
[00:23:32] around how different types of actors are
[00:23:34] trying to appeal to different types of
[00:23:35] businesses. Labs like OpenAI and
[00:23:37] Anthropic are clearly trying to keep
[00:23:39] everything consolidated in their own
[00:23:40] environment. Part of that, especially
[00:23:42] for OpenAI, has been a real focus on
[00:23:44] cheaper models and pushing the price of
[00:23:46] their models down as far as they
[00:23:48] possibly can. That's something we've
[00:23:49] seen a lot over the past couple of
[00:23:50] weeks. But, they also are, as they have
[00:23:52] been all year, focused on vertical
[00:23:53] solutions such as the newly launched
[00:23:55] Astro for Law from OpenAI. Alongside the
[00:23:58] Astro for Law launch, OpenAI and law
[00:24:00] firm Cooley also co-launched a product
[00:24:02] that they called Go Public. This is
[00:24:04] designed to draft S-1 filings, which are
[00:24:06] the documents that companies must submit
[00:24:07] to the SEC before they can go public.
[00:24:10] And yet, as if to give us a perfect
[00:24:11] comparison of the different types of
[00:24:13] options that different companies are
[00:24:14] taking, another law firm, Latham &
[00:24:16] Watkins, was recently reported to be
[00:24:18] buying Nvidia servers to set up their
[00:24:19] own in-house systems specifically as an
[00:24:22] alternative to models from OpenAI and
[00:24:24] Anthropic. Latham, which is the US's
[00:24:26] second largest law firm, said, quote,
[00:24:29] "Sometimes we may have information that
[00:24:30] is so sensitive, client information that
[00:24:32] we really want to protect, we don't want
[00:24:33] to put it on any cloud vendor."
[00:24:35] Seeming to make the point that one of
[00:24:36] the ways that enterprises can stay out
[00:24:38] of the fray of the AI safety discourse
[00:24:39] is to own their own models, Mistral CEO
[00:24:42] Arthur Mensch posted, "Don't pace
[00:24:44] building and owning your own AI models
[00:24:46] and systems as an enterprise, and there
[00:24:47] will be no doomsday for you." Foundation
[00:24:50] Capital's Gia Gupta also thinks that
[00:24:52] this pacing the frontier moment could be
[00:24:54] a good one for the software incumbents.
[00:24:56] She wrote, "If you're the CEO of any
[00:24:58] software company and you're not offering
[00:24:59] open weight models as a skew right now,
[00:25:01] you're asleep. Pace the frontier may be
[00:25:03] the greatest invitation software
[00:25:05] incumbents have ever gotten. While the
[00:25:06] labs debate how quickly intelligence
[00:25:08] should advance, software companies
[00:25:09] should be racing to commoditize the
[00:25:11] intelligence we already have. Pharma and
[00:25:13] banks are already picking up open weight
[00:25:14] models partly for margins, partly
[00:25:16] because a revocable lab API is a
[00:25:17] dependency they increasingly don't want.
[00:25:19] AI natives and tech companies that care
[00:25:21] about cost of goods sold are doing the
[00:25:22] same. Most software companies that tried
[00:25:24] have failed attempts because the open
[00:25:26] weight models sucked. But now open
[00:25:27] weight models are good enough. I believe
[00:25:29] that every major software company should
[00:25:31] become a model factory for its own
[00:25:32] vertical. On the evals, post train open
[00:25:34] weights on the workload it uniquely
[00:25:35] sees, serve those models to its
[00:25:37] customers, and use production feedback
[00:25:39] to continuously improve them."
[00:25:41] And so, on the one hand, to some extent,
[00:25:43] the response from businesses to the AI
[00:25:45] safety discussion seems to be business
[00:25:47] as usual. The pace and challenges of
[00:25:49] adoption within the enterprise were
[00:25:51] always unique and distinct to them, and
[00:25:53] the challenges of big institutional
[00:25:54] inertia that comes with them. But on the
[00:25:56] other, there are some ways that the
[00:25:59] conversation is reinforcing trend lines
[00:26:01] that were already starting. Companies
[00:26:02] will need to spend more time and
[00:26:04] resources on cyber and security issues.
[00:26:06] That was always coming, but the point
[00:26:08] has been made even more crisply now. And
[00:26:10] well, already there were some compelling
[00:26:12] reasons to explore and consider open
[00:26:14] weights or more owned model alternatives
[00:26:16] to just getting in bed with the big
[00:26:17] vendors, there are now even more reasons
[00:26:19] to be willing to walk down that path.
[00:26:21] Not least of which is the increasing
[00:26:23] likelihood of regulatory disruption. I
[00:26:25] think that if I had to summarize my
[00:26:26] advice in a single thought, it's that
[00:26:28] while overall the changing AI safety
[00:26:30] discourse doesn't really impact the
[00:26:32] short term for enterprises, it certainly
[00:26:34] reinforces the fact that the companies
[00:26:36] that are willing to try the hardest
[00:26:38] things, like actually investing in their
[00:26:40] own owned architectures, have even more
[00:26:42] potential to differentiate from their
[00:26:44] peers and competitors than they did
[00:26:45] before.
[00:26:47] I will, of course, continue to watch
[00:26:48] these trends as they evolve, but for
[00:26:49] now, that's going to do it for today's
[00:26:51] AI daily brief. Appreciate you listening
[00:26:53] or watching as always, and until next
[00:26:55] time, peace.
