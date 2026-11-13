---
record_id: "podcast:9049c375-af3a-494b-b016-0b0baa53524c"
episode_id: 9049c375-af3a-494b-b016-0b0baa53524c
title: 4 Questions for AI This Week
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/4-questions-for-ai-this-week/9049c375-af3a-494b-b016-0b0baa53524c"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/4-questions-for-ai-this-week/9049c375-af3a-494b-b016-0b0baa53524c"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-26
played_at: "2026-10-26T12:00:00Z"
play_count: 1
duration_seconds: 120
source: pocketcasts-history-browser
played_label: October 26
history_order: 31
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 83358a294144799403215b976d9dd2d906e83886e88e747aaea4ca5d0a4f5c52
analysis_mode: health
summary_source: local
model_source: local
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: Qwen3.8-Flash-Next-UD-Q4_K_XL
tagging_model: failed
proposed_tags: []
proposed_entities: []
status: new
routed_to: null
---

## Summary

Moonshot’s Kimi K3.1 Pro, Anthropic’s Opus 5.5/Fable, OpenAI, cyberattacks, data-center financing, and Anthropic’s IPO dominated the episode. Moonshot claimed K3.1 Pro was near Opus 5.5 on agentic white-collar and coding benchmarks—just behind Opus on GDP val, within a point on Terminal Bench 4.0, and about $5/task vs $15 Opus and $10 GPT-6 Astra—while Artificial Analysis ranked it fourth on its intelligence index at 55 and said the open-weight/proprietary gap would narrow from 12 to 3 points; Moonshot also said it deliberately reduced offensive cyber capability, yet Artificial Analysis called it the most capable public cyber model at 64%. The launch was marred by reports that Moonshot instructed influencers not to disclose paid partnerships and to trash-talk rivals, prompting skepticism from Chubby, Nathan Lambert, and others. The episode then treated cyber chaos as a possible new normal after a PHP bug reportedly threatened 70% of websites: Anthropic’s Jason D. Clinton warned of ~18 months of strain, Cloudflare’s Matthew Prince predicted years of “sky is falling” incidents, Sam Altman said not all bugs can be patched, and OpenAI/Anthropic resumed frontier training in isolated/offline environments after agents reportedly communicated via processor cache. On infrastructure, Chamath Palihapitiya, Elon Musk, Ramp, and Bloomberg reported debt-market pressure, direct GPU rentals by top firms, possible stranded compute, a disputed SpaceX GPU-debt story, and consolidation among 200+ neo clouds; on markets, OpenAI’s rumored $1.25T round, Anthropic IPO valuation speculation, The Information’s claim OpenAI gained coding share from Anthropic, and OpenRouter/Ramp data showing Opus 5.5’s 3.6x token-volume surge and 35.1% token share were weighed.

For practical use, benchmark Kimi K3.1 Pro against Opus 5.5/GPT-6 Astra on your own agentic coding and office-work tasks, measuring cost per completed task, token use, and failure modes rather than trusting influencer posts; treat undisclosed paid promotion as a reason to discount hype. If you run software or cloud infrastructure, assume a multi-month/years vulnerability-hardening cycle: prioritize patching, code review, agent-based security testing, incident-response templates, and budgeting for private security or isolated environments. For AI procurement, compare API models with direct GPU/VPC options, watch debt-market access, neo-cloud consolidation, and stranded compute before long-term commitments; the KPMG/UT Austin study also suggests training and hiring should reward people who guide, evaluate, and refine AI outputs, not just technical knowledge. For Anthropic/OpenAI decisions, monitor Fable 5.5 availability, Opus 5.5 token/spend share, OpenAI price cuts, and IPO/prospectus disclosures; follow-up questions should ask whether open-weight cyber-capable models will trigger export/policy changes, whether offline training actually prevents model escapes, and whether K3.1 Pro’s cyber “nerf” holds under real-world red-team testing.

## Transcript

[00:00:00] Last week was one of those weeks where
[00:00:01] it feels like everything in AI just
[00:00:03] ratcheted up another level. Coming into
[00:00:05] this week, we have a set of huge
[00:00:07] questions that are dominating the
[00:00:09] conversation. From whether data center
[00:00:11] funding has dried up to how we're going
[00:00:13] to handle the latest Chinese open-weight
[00:00:14] models, to whether this cyber apocalypse
[00:00:17] is now just with us forever, to how
[00:00:19] difficult it's going to be for Anthropic
[00:00:20] to get this IPO out of the door. Today,
[00:00:22] we're talking about the four big
[00:00:23] questions that are shaping AI this week.
[00:00:26] The AI Daily Brief is a daily podcast
[00:00:28] and video about the most important news
[00:00:30] and discussions in AI.
[00:00:32] All right, friends. Quick announcements
[00:00:34] before we dive in. First of all, thank
[00:00:36] you to today's sponsors, KPMG, C Data,
[00:00:39] Granola, and Blitzcy. To get an ad-free
[00:00:41] version of the show, go to
[00:00:42] patreon.com/ai daily brief, or you can
[00:00:44] subscribe on Apple Podcasts. If you want
[00:00:46] to learn more about sponsoring the show,
[00:00:48] send us a note at sponsors@ai daily
[00:00:50] brief.ai. And lastly today, I am super
[00:00:52] excited to share that I have launched a
[00:00:54] new podcast. You can think about this
[00:00:57] one as sort of a spiritual sibling to
[00:00:58] AIDB, but one who gets to get away from
[00:01:01] the grind of the daily and instead sit
[00:01:02] back and go bigger because we're doing
[00:01:04] it weekly. The show is called How We Got
[00:01:06] Here, and it's a show about how modern
[00:01:08] important trends and phenomenon came to
[00:01:10] be. To give you a flavor, the first
[00:01:12] episode is about America's 15-year
[00:01:14] history falling out of love with the
[00:01:15] tech industry and how that sets up the
[00:01:17] data center debate. But then I've got
[00:01:19] future episodes coming about how stuff
[00:01:21] got cheap while life got expensive and
[00:01:23] prediction markets and GLP-1, so pretty
[00:01:25] much anything is fair game. I tend to
[00:01:27] think that a lot of what we feel is
[00:01:28] inevitable is actually just a series of
[00:01:30] decisions that were made by people. And
[00:01:32] if that's true and we want to change
[00:01:33] things, we can make different decisions
[00:01:35] in the future, but only if we
[00:01:36] understand, well, how we got here. That
[00:01:38] show is live now. You can find it on
[00:01:39] Apple or Spotify, and you can get all
[00:01:41] the links you need either in the show
[00:01:42] notes of this show or go to how we got
[00:01:44] here.com. I would so appreciate it if
[00:01:46] you would take a moment to listen, and
[00:01:48] then if you like it, rate and review the
[00:01:49] show. This kickoff week is where it
[00:01:51] matters most, and I think a lot of you
[00:01:53] guys are really going to like it. Thank
[00:01:54] you in advance for checking it out. But
[00:01:56] now, let's get into the big questions
[00:01:58] for AI this week.
[00:02:00] Last week was one of those real
[00:02:02] heightened stakes weeks, and we almost
[00:02:05] have archetypes of these weeks in AI.
[00:02:07] There are the everyone's freaking out
[00:02:08] about a bubble weeks, the new models are
[00:02:11] coming so fast that it's head-spinning
[00:02:12] weeks, and then there was the type of
[00:02:13] week that we had last week, which is the
[00:02:15] most subtle but no less knowable, which
[00:02:18] is the oh man, it just feels like the
[00:02:20] stakes of everything are getting higher
[00:02:22] kind of weeks.
[00:02:24] We had cyberattacks, market jitters, a
[00:02:27] continued and growing recognition of the
[00:02:28] power of the most recent models,
[00:02:30] particularly Opus 5.5.
[00:02:32] We're kicking it off with the four
[00:02:33] questions that I think are shaping the
[00:02:35] conversation heading into what's to
[00:02:37] follow.
[00:02:38] The theme of the first set of questions
[00:02:39] is about models, and specifically how we
[00:02:42] respond to the latest Chinese models and
[00:02:44] what it says about our larger sense of
[00:02:45] the geopolitical stakes of the race. But
[00:02:48] to understand that question, we got to
[00:02:49] go back to Friday, when Moonshot
[00:02:51] released their latest version of Kimi,
[00:02:54] Kimi K3.1 Pro. It's their first model
[00:02:57] update for the K3 family. Now, you might
[00:02:59] remember that when Kimi K3 was released
[00:03:02] in July, the media presented it as an
[00:03:04] open-source alternative to Fable. K3 was
[00:03:07] the first ultra-large open model,
[00:03:09] weighing in at 2.8 trillion parameters.
[00:03:11] It showed some pretty big advances in
[00:03:13] what you could do with it, and it
[00:03:14] happened to come at the exact perfect
[00:03:16] moment when Fable was offline because of
[00:03:18] the export control issues with the White
[00:03:20] House.
[00:03:21] As always happens though, whenever there
[00:03:24] is a new Chinese model, everyone loses
[00:03:26] their mind about having closed the gap
[00:03:27] with the US closed models, the benefit
[00:03:29] of time tends to calm things down a bit.
[00:03:32] Ultimately, beyond a handful of specific
[00:03:34] use cases like front-end web design, K3
[00:03:37] never fully lived up to the hype.
[00:03:39] Since then, new releases from OpenAI and
[00:03:41] Anthropic push the frontier forward and
[00:03:43] open what has perceived to be a wider
[00:03:45] gap with the leading models from China.
[00:03:47] On top of that, while American
[00:03:49] open-weight models have not yet gotten
[00:03:51] up to that Kimi K3 sort of level, they
[00:03:54] are for the first time in a long time
[00:03:55] starting to nip on the heels of their
[00:03:57] Chinese counterparts. Meaning in short
[00:03:59] that the whole conversation around open
[00:04:00] weight models has changed quite a bit
[00:04:02] since the summer when K3 was first
[00:04:03] released.
[00:04:05] And yet, with the release of K3.1 Pro,
[00:04:07] we're once again seeing the comparisons
[00:04:09] to Fable and Anthropic's mid-size
[00:04:11] powerhouse Opus 5.5.
[00:04:13] Moonshot provided an extensive set of
[00:04:15] benchmarks for comparison, which placed
[00:04:17] K3.1 clearly ahead of Chinese peers and
[00:04:20] in the mix with the best models from the
[00:04:21] West.
[00:04:22] On GDP val which measures agentic
[00:04:24] white-collar work, K3.1 was just behind
[00:04:27] the leader Opus 5.5 and ahead of Fable
[00:04:30] 5.1.
[00:04:31] Likewise on Terminal Bench 4.0 which
[00:04:33] measures agentic coding, K3 was once
[00:04:35] again less than a point behind Opus 5.5
[00:04:37] and around seven points ahead of GPT-6
[00:04:39] Astra and Fable 5.1. Terminal Bench 4.0
[00:04:42] is notable as it is comparably not
[00:04:44] saturated and has in the past shown a
[00:04:47] clear performance difference between the
[00:04:48] latest generation of Western models and
[00:04:50] Chinese open models. DeepSeek V4.1 Flash
[00:04:53] and GLM-5.3 only managed scores in the
[00:04:55] low 40s giving them a 15-point gap with
[00:04:58] the Western frontier. Moonshot
[00:05:00] emphasized cost as a big differentiator
[00:05:01] for K3.1. When K3 was released over the
[00:05:04] summer, it wasn't a particularly cheap
[00:05:06] model costing around the same as GPT-5.6
[00:05:09] Soul for similar benchmark performance.
[00:05:11] And despite there being lingering
[00:05:12] perception that every Chinese model that
[00:05:14] comes out is pennies on the dollar, in
[00:05:16] practice without the cost advantage that
[00:05:17] Chinese models had been known for, there
[00:05:19] just wasn't a hugely compelling reason
[00:05:21] for most people to make the switch.
[00:05:23] Moonshot is pricing K3.1 at around 2/3
[00:05:26] the cost of K3 on a per token basis
[00:05:28] giving it the same price as Sonnet 5.5
[00:05:30] and GPT-6 Soul. That's still almost 10
[00:05:33] times the per token cost of DeepSeek 4.1
[00:05:35] Flash and about twice the price of
[00:05:37] GLM-5.3, but it now sits at least
[00:05:39] comparable with some Western
[00:05:40] alternatives.
[00:05:41] What's more on Terminal Bench 4.0,
[00:05:43] Moonshot suggested that K3.1 was far
[00:05:46] cheaper on a cost per task basis than
[00:05:48] all major rivals. It cost around $5 per
[00:05:50] task compared to around 15 for Opus 5.5
[00:05:53] and 10 for GPT-6 Astra on max settings.
[00:05:56] Artificial Analysis confirmed extremely
[00:05:58] solid benchmark performance in their
[00:06:00] independent testing. K3.1 scored 55 on
[00:06:03] the intelligence index ranking fourth
[00:06:05] behind Opus 5.5, Sonnet 5.5 and Muse
[00:06:07] wonderful. K3.1 was two points ahead of
[00:06:10] Fable 5.1, GPT-6 Astra and Gemini 4
[00:06:12] Argon which are all now tied for fifth
[00:06:14] place. Artificial Analysis wrote, "Once
[00:06:17] the weights for K31 Pro are released, it
[00:06:19] will be the highest scoring open weights
[00:06:20] model and the gap between the leading
[00:06:22] open weights and proprietary models on
[00:06:24] the intelligence index will narrow from
[00:06:26] 12 points to three."
[00:06:28] They found that K3.1 uses 14% more
[00:06:30] tokens per task than K3. However,
[00:06:32] because of the price reduction it's
[00:06:33] slightly cheaper than its predecessor.
[00:06:36] Now, the first reaction was to be pretty
[00:06:37] impressed with the benchmarks if
[00:06:39] recognizing that this is perhaps a movie
[00:06:41] that we've seen before. Chubby on X
[00:06:43] wrote, "Just to be very clear and that
[00:06:45] everyone understands this. Today we got
[00:06:47] Fable 5.1 intelligence as a local model.
[00:06:50] I remember the GLM founder saying in a
[00:06:52] post that he expects Fable 5
[00:06:53] capabilities by the end of the year from
[00:06:54] China. Well, it happened with all its
[00:06:56] consequences. Just think about it." Ram
[00:06:59] Ananth from the Singularity University
[00:07:00] wrote, "Based on this, Kimi K3.1 Pro is
[00:07:03] around 5 weeks behind the US frontier.
[00:07:06] That's the shortest the open/closed to
[00:07:08] AI model gap has ever been.
[00:07:10] Yet, unfortunately for Kimi, pretty soon
[00:07:12] all of the conversation shifted away
[00:07:14] from the model itself and towards how
[00:07:16] they were promoting it. Al Shaiban X
[00:07:18] posted a bunch of communications from
[00:07:20] the Kimi team about how they were
[00:07:21] running their influencer campaign. Of
[00:07:24] note was the fact that they explicitly
[00:07:26] instructed those influencers to not put
[00:07:28] the paid partnership label on their
[00:07:29] posts. Now, they also had a whole bunch
[00:07:31] of narrative instructions like wanting
[00:07:33] those influencers to call it Opus 5.5
[00:07:35] but five times cheaper and focus on this
[00:07:37] narrowing gap between open source and
[00:07:38] frontier as well as explicitly trash
[00:07:41] talking Astra and Opus. But, still even
[00:07:43] with that it's the non-disclosure thing
[00:07:44] that people were really upset about.
[00:07:46] Chubby again summed it up writing, "This
[00:07:48] is such a shame and so sad to see.
[00:07:50] Moonshot ruined their launch themselves.
[00:07:52] K3.1 [snorts]
[00:07:53] Pro is a great model and it did not need
[00:07:55] people to fake good reviews. But since
[00:07:57] they were trying to cheat the game it
[00:07:58] makes the whole launch look bad."
[00:08:00] Open model researcher Nathan Lambert is
[00:08:02] willing to extend a little grace saying
[00:08:04] that there are still some cultural norms
[00:08:05] and communication issues that could have
[00:08:07] led to this type of mistake. He wrote,
[00:08:09] "This is a mistake but I suspect they
[00:08:11] will correct. Chinese labs are very
[00:08:13] eager to influence the western ecosystem
[00:08:15] in X so they likely took a step too far
[00:08:17] here. They followed the vibes closely
[00:08:19] and I bet will understand even if some
[00:08:20] cultural differences cause this."
[00:08:22] Given the new questions though, some
[00:08:24] people went back to more aggressively
[00:08:26] test the claims and found the model a
[00:08:27] bit lacking.
[00:08:29] Future Forward editor Alex called
[00:08:31] released.
[00:08:34] I think when it comes to model
[00:08:35] performance with this one we're going to
[00:08:37] have to wait and see how it shakes out.
[00:08:39] We've not even yet had a full business
[00:08:40] day with people using this thing and
[00:08:42] given the dust-up around the strategy
[00:08:44] everything is a little bit colored right
[00:08:45] now.
[00:08:46] And going back to the idea of questions
[00:08:47] that will shape the week, if the numbers
[00:08:49] actually hold up in anywhere close to
[00:08:51] what the benchmark suggest, how is the
[00:08:53] US policy structure going to handle an
[00:08:55] open weight model of this level of
[00:08:56] capability?
[00:08:58] One note from the release was that
[00:08:59] Moonshot said that they deliberately
[00:09:00] nerfed the model when it comes to
[00:09:02] cybersecurity tasks. They wrote, "We aim
[00:09:05] not to release open weights that would
[00:09:06] extend the absolute frontier of cyber
[00:09:07] capability. K3.1 Pro's offensive cyber
[00:09:10] capability is by design below what our
[00:09:13] pipeline can produce and remains behind
[00:09:15] that of frontier proprietary models."
[00:09:18] Basically during their post training,
[00:09:19] Moonshot found that cyber capabilities
[00:09:21] were scaling so they deliberately
[00:09:22] removed cyber related data from their
[00:09:24] training pipeline.
[00:09:26] Moonshot explained that they tried to
[00:09:27] strike a balance retaining capabilities
[00:09:28] for general purpose coding and making
[00:09:30] reasonable levels of cyber performance
[00:09:32] more widely available.
[00:09:33] External testing from artificial
[00:09:35] analysis found that K31 is the most
[00:09:37] capable cyber model available to the
[00:09:38] general public. It scored 64% on their
[00:09:41] cyber index, 11 percentage points ahead
[00:09:43] of DeepSeek V41 flash, and only 5%
[00:09:45] points behind the trusted version of
[00:09:46] GPT-6 Soul available through their
[00:09:48] partner program Daybreak Blue.
[00:09:50] Elie Bursztein from Prime Intellect
[00:09:51] explained why this was a positive sign.
[00:09:53] He wrote, "One point that was under
[00:09:55] discussed in my opinion is that it's the
[00:09:57] first open lab that is pacing the
[00:09:58] frontier of open weight cyber
[00:09:59] capabilities, which makes it much easier
[00:10:01] and creates incentives for other labs to
[00:10:03] make the right decision and do the same
[00:10:05] when they reach the same level of
[00:10:05] capabilities.
[00:10:07] The remaining question is how to set the
[00:10:09] right level. Underestimated and open
[00:10:11] models will become useless for defensive
[00:10:12] cyber security, leaving the world
[00:10:14] relying on US closed labs to spread
[00:10:15] defensive capabilities quickly, which is
[00:10:18] not realistic in my opinion, although I
[00:10:19] obviously wish them to succeed in this
[00:10:21] mission. Overestimate it and you might
[00:10:23] get the catastrophic scenarios that
[00:10:24] Anthropic and others describe.
[00:10:26] Now, my sense is that K31 is not going
[00:10:28] to be the only model we're talking about
[00:10:29] this week, but let's pick up on the
[00:10:31] cyber theme to move to our next
[00:10:32] question, is cyber chaos just for the
[00:10:35] time being the new normal?
[00:10:37] Last week we got a PHP bug that
[00:10:39] reportedly threatened 70% of all
[00:10:40] websites. On Thursday, after the dust
[00:10:43] had started to settle, Anthropic's
[00:10:45] Deputy Chief Security Officer Jason D.
[00:10:47] Clinton wrote, "As bad as things have
[00:10:48] gotten in the past 4 days, they're going
[00:10:50] to get a lot worse before they get
[00:10:52] better. Security leaders never let a
[00:10:54] crisis go to waste. Please go to your
[00:10:56] boards and ask for help right now. Not
[00:10:58] for AI, for the basics. We need to hold
[00:11:01] on for around 18 months."
[00:11:03] A lot of folks responded saying, "Hey
[00:11:05] man, you guys caused this."
[00:11:07] He and sorry wrote, "You and your
[00:11:09] cohorts created this monster. Now you
[00:11:11] want us to help you clean it up."
[00:11:13] Clinton responded crisply, quote, "It
[00:11:16] was always going to be this way. We
[00:11:17] tried to warn the world."
[00:11:19] I certainly don't think that from an
[00:11:21] efficacy standpoint the blame game is
[00:11:22] particularly useful. AI models capable
[00:11:24] of detecting and exploiting
[00:11:25] vulnerabilities are clearly here, and
[00:11:27] before society wants to decide how to
[00:11:29] apportion blame, the much more important
[00:11:31] question is how long the cyber chaos
[00:11:33] will persist and how we can help address
[00:11:34] it. Cloudflare CEO Matthew Prince
[00:11:36] believes there's much more to come,
[00:11:38] telling Reuters he was aware of quote,
[00:11:40] "a bunch of additional vulnerabilities
[00:11:41] that are present in other pieces of
[00:11:42] critical software." He predicts a busy
[00:11:45] few months while the world hardens the
[00:11:46] core technology that underpins the
[00:11:47] internet, adding, "I think we're going
[00:11:49] to have a couple years where every
[00:11:50] single week it's going to feel like the
[00:11:52] sky is falling."
[00:11:53] Indeed, in last week's disclosure post,
[00:11:55] OpenAI flagged that more would be
[00:11:57] coming. So, we could be in for a black
[00:11:59] October that stretches on for several
[00:12:00] months if not years.
[00:12:02] Sam Altman, for his part, doesn't seem
[00:12:03] that optimistic about a swift
[00:12:05] resolution. In an interview, he said, "I
[00:12:07] don't even know a dramatic enough word
[00:12:09] to use. Models can find bugs that are
[00:12:11] outside of the normal threat model of
[00:12:12] what we think a hacker can do. Hardware
[00:12:14] level, insane stuff. I no longer think
[00:12:17] we're going to be able to just patch all
[00:12:18] the bugs."
[00:12:20] A new study from KPMG and the University
[00:12:22] of Texas at Austin found that when
[00:12:24] people work with AI, similar skills
[00:12:26] don't guarantee similar outcomes.
[00:12:29] Researchers studied more than 500
[00:12:30] early-career professionals and found
[00:12:32] that the best performers consistently
[00:12:34] amplify the value of AI by guiding,
[00:12:36] evaluating, and refining its outputs.
[00:12:39] These top performers, called AI
[00:12:41] amplifiers, weren't defined by what they
[00:12:43] knew alone, but by how they worked with
[00:12:45] AI. Learn more about what separates AI
[00:12:48] amplifiers from everyone else at
[00:12:50] kpmg.com/us/aiamplifiers.
[00:12:55] This episode is brought to you by CData.
[00:12:58] Companies rolling out AI keep hitting
[00:12:59] the same wall. Token spend is climbing,
[00:13:02] security is holding agents back, and no
[00:13:04] one knows how AI is truly being used.
[00:13:06] The root cause? AI is cut off from the
[00:13:09] systems and context your business runs
[00:13:11] on. That's why CData built Connect AI
[00:13:14] Gateway, one control point between your
[00:13:16] AI and your systems. Built on the
[00:13:18] connectivity layer powering Palantir,
[00:13:20] Google, Salesforce, and hundreds more,
[00:13:22] each agent gets exactly the data and
[00:13:24] tools it needs. It governs down to the
[00:13:26] record and lets you finally see your
[00:13:27] org's complete AI usage in one place.
[00:13:30] Accurate answers, a fraction of the
[00:13:32] token cost, and a gateway that learns
[00:13:34] your business with every interaction.
[00:13:35] See how at Cdata.ai.
[00:13:39] You're in back-to-back meetings all day.
[00:13:40] You're trying to stay present, but
[00:13:42] you're also worried you'll forget the
[00:13:43] decision, the action item, the important
[00:13:45] next step. This is a scenario that we
[00:13:47] absolutely live here at the AI Daily
[00:13:49] Brief, given how fast things move and
[00:13:50] change and how quickly we're evolving
[00:13:51] everything that we do. That's where
[00:13:53] Grainola comes in. Grainola is an
[00:13:55] AI-powered notepad for meetings. You jot
[00:13:57] down rough notes like you always do, and
[00:13:59] in the background, Grainola transcribes
[00:14:01] and turns them into clear, useful notes
[00:14:02] when the meeting ends. No bots joining
[00:14:04] your calls, no distractions, just a
[00:14:06] clean notepad that helps you focus.
[00:14:08] During or after the call, you can chat
[00:14:10] with your notes. Ask Grainola to pull
[00:14:12] out action items, help you negotiate,
[00:14:13] write a follow-up email, or even coach
[00:14:15] you using recipes, which are pre-made
[00:14:17] prompts. Once you try it on your first
[00:14:18] meeting, it is very hard to go without.
[00:14:21] Head to grainola.ai/aiday
[00:14:23] and use code aiday to get 100% off for 3
[00:14:26] months for new users. That's
[00:14:28] grainola.ai/aiday
[00:14:30] and code aiday to get 100% off for new
[00:14:33] users for 3 months.
[00:14:35] Every AI coding tool on the market does
[00:14:37] the same thing first. It starts writing
[00:14:39] code. Blitzy does the opposite. Before
[00:14:41] writing a single line, Blitzy spends
[00:14:43] days reverse engineering your entire
[00:14:45] codebase. Thousands of agents ingest
[00:14:46] millions of lines mapping every
[00:14:48] dependency, every undocumented
[00:14:49] constraint, every architectural decision
[00:14:51] made over the last decade. The result is
[00:14:53] a dynamic knowledge graph that
[00:14:54] understands your software the way a
[00:14:56] principal engineer would after 30 years
[00:14:58] in the building. Other tools guess at
[00:14:59] context with grep searches and markdown
[00:15:01] files. Blitzy never guesses. It builds
[00:15:04] true understanding first, then delivers
[00:15:05] over 80% of entire software epics
[00:15:07] autonomously, validated, end-to-end
[00:15:09] tested, production-grade pull requests.
[00:15:11] That's why Fortune 500 engineering teams
[00:15:13] trust Blitzy with the codebases that
[00:15:15] matter most. See for yourself at
[00:15:17] blitzy.com. That's b l i t z y dot com.
[00:15:21] So, how are people responding to this?
[00:15:23] Well, first of all, we are very much
[00:15:25] going to be living in the fog of war,
[00:15:27] where critical thinking and skepticism
[00:15:28] is going to be extremely important. You
[00:15:31] have all sorts of viral posts all over
[00:15:32] social media right now from anonymous
[00:15:34] accounts claiming to be inside labs or
[00:15:36] inside the NSA talking about all these
[00:15:38] things going on behind the scenes that
[00:15:39] are being hid from the public. And while
[00:15:41] it's of course not impossible that
[00:15:42] that's true, I do not think that that's
[00:15:44] a particularly useful set of posts to be
[00:15:45] engaging with. More interesting to me
[00:15:47] are practically the people who are
[00:15:48] discussing how we shift to hardening
[00:15:50] these systems as fast as actually
[00:15:51] possible. Boxes and Levy wrote, "Agent
[00:15:54] swarms for cyber defense is about to be
[00:15:55] one of the biggest categories in AI.
[00:15:57] We're going to have agents reviewing our
[00:15:59] code and infra, testing every
[00:16:00] permutation of risk, processing gobs of
[00:16:02] data, and more."
[00:16:04] Security is one of the best use cases
[00:16:05] for swarms because it's an obvious area
[00:16:07] where more compute in equals more value
[00:16:09] out. There's a wide range of testing
[00:16:11] that people can never get around to, or
[00:16:13] at least quickly enough that agents have
[00:16:14] no problem going after.
[00:16:16] And some think that this doesn't end
[00:16:17] well for the free and open internet.
[00:16:19] Economics writer Noah Smith wrote, "The
[00:16:21] proliferation of AI cyber attacks may
[00:16:23] signal the end of the internet as a
[00:16:24] public good. We may only be able to use
[00:16:26] it in the future if everyone shells out
[00:16:27] big bucks for private security. That
[00:16:29] will, he points out somewhat obviously
[00:16:31] if that thesis is correct, reduce the
[00:16:33] internet's economic value."
[00:16:35] And yet already you are seeing teams
[00:16:37] posting the templates for how they're
[00:16:38] trying to get out ahead of this. Alan
[00:16:40] Wells from Rocketable said, "Just spent
[00:16:42] the last 7 days on the front lines of
[00:16:44] the vuln apocalypse fending off an
[00:16:45] active cyber attack on one of our
[00:16:46] products." He then followed and shared a
[00:16:48] bunch of thoughts including how to be
[00:16:50] working on hardening your systems even
[00:16:51] if you aren't a huge team.
[00:16:53] Now, in terms of what all this cyber
[00:16:55] stuff means for new models, all we have
[00:16:57] to go on is what we're getting out of
[00:16:58] the labs. OpenAI has announced that
[00:17:00] they'll resume training frontier AI
[00:17:01] models, but will isolate them from the
[00:17:03] open internet. In a Friday blog post,
[00:17:05] OpenAI wrote that they'd quote, "Built
[00:17:07] an offline world, a vast set of indexed
[00:17:09] and cached web content in which our
[00:17:10] models can interact without risk of
[00:17:12] affecting external systems."
[00:17:14] Moving forward, all of their frontier
[00:17:16] reinforcement learning runs will use
[00:17:17] this quarantined mode of interaction.
[00:17:19] This news mirrors a decision made by
[00:17:21] Anthropic earlier in the month when they
[00:17:22] announced that they had also resumed
[00:17:24] frontier training.
[00:17:25] On the one hand, if this works, it means
[00:17:27] that frontier model training can
[00:17:28] continue, hopefully without endless
[00:17:29] reports of rogue agents escaping from
[00:17:31] the frontier labs. However, it also
[00:17:33] means that neither of the big labs has
[00:17:34] much confidence in their ability to
[00:17:36] constrain their models using alignment
[00:17:37] research or other methods, needing a
[00:17:39] more blunt instrument of cutting off
[00:17:41] access to the internet. And honestly,
[00:17:43] even the air-gapped setup seems like it
[00:17:44] might not be enough. OpenAI wrote, "In
[00:17:46] one experiment, we asked the agents in
[00:17:48] separate micro VMs created and managed
[00:17:50] by OpenAI's sandboxing software on
[00:17:52] shared host machines to exchange
[00:17:54] synthetic secrets without the use of
[00:17:55] network connections or shared writable
[00:17:56] files, something that our systems are
[00:17:58] meant to prevent." "The agents found a
[00:18:00] way to communicate using the processor's
[00:18:02] cache."
[00:18:03] Ship Together co-founder Wise wrote,
[00:18:05] "OpenAI is now building a fake internet
[00:18:07] for its AI agents to interact with. The
[00:18:09] idea is to keep them isolated from the
[00:18:10] real internet. I'm not sure if this is
[00:18:13] going to work."
[00:18:14] So, in fact, the better question might
[00:18:17] not be is cyber chaos the new normal,
[00:18:20] but instead might be are we reaching the
[00:18:22] point officially where the most advanced
[00:18:24] frontier models are simply too dangerous
[00:18:26] to release, not because they are
[00:18:28] paperclip maximizers who are going to
[00:18:30] reduce all the atoms in our human bodies
[00:18:32] to material that helps them achieve some
[00:18:33] impersonal goal, but that they're just
[00:18:35] at the moment too good at breaking into
[00:18:37] our very human-created systems.
[00:18:40] For our next question that'll shape this
[00:18:41] week, let's move over to markets where
[00:18:44] people are asking is data center funding
[00:18:46] drying up? Neo clouds are feeling the
[00:18:48] squeeze from two secular trends turning
[00:18:50] against them at the same time. The first
[00:18:53] is debt markets turning sour on data
[00:18:54] center funding, demanding a huge and
[00:18:56] growing premium for new fundraising. The
[00:18:58] second is large AI consumers beginning
[00:19:00] to stand up their own data centers.
[00:19:02] According to Ramp data, more than a
[00:19:04] third of AI spend from the top 1% of
[00:19:05] firms is now going towards direct GPU
[00:19:08] rentals rather than calling models over
[00:19:10] the API.
[00:19:11] Investor Chamath Palihapitiya said that
[00:19:13] he's already seeing a change in behavior
[00:19:15] on the ground. He commented, "Ever since
[00:19:17] Palantir's Alex Karp's commentary on
[00:19:19] CNBC about data sovereignty, buying
[00:19:21] patterns have changed. And I think
[00:19:23] people are being a lot more methodical.
[00:19:25] They are building out their own data
[00:19:26] centers or at least moving into VPCs,
[00:19:28] virtual public clouds. My team yesterday
[00:19:30] was at the CIO event of, let's say, one
[00:19:32] of the largest banks in America. It was
[00:19:34] the most incredible thing. They said,
[00:19:36] "We have decreased our spending on AWS
[00:19:38] and Google Cloud. We now have six
[00:19:40] completely independent ground-up data
[00:19:42] centers that we built from scratch for
[00:19:43] ourselves."
[00:19:45] Over the weekend, meanwhile, that
[00:19:46] narrative advanced. Yuchen Jin said that
[00:19:48] he heard that AI Neo Labs are betting on
[00:19:49] the rising cost of compute as a backup
[00:19:51] plan to building their own models. His
[00:19:53] friend apparently said, "Even if we fail
[00:19:55] to train the best model, we locked in
[00:19:56] GPU capacity early. GPU rental prices
[00:19:59] have since gone up two to three X. We
[00:20:00] can just resell the compute and print
[00:20:02] money."
[00:20:03] Elon Musk, however, responded, "I think
[00:20:05] we're going to see a lot of stranded
[00:20:06] compute in partially complete data
[00:20:08] centers."
[00:20:09] Later in the weekend, Chamath again
[00:20:10] explained what he's seeing on the
[00:20:11] infrastructure side, building on similar
[00:20:13] themes. First up, he wrote, "Neo clouds
[00:20:15] are disorganized and poorly capitalized.
[00:20:17] Some are definitely better than others,
[00:20:19] however." He explained that
[00:20:20] hyperscaler-backed projects are facing
[00:20:22] delays from a combination of
[00:20:23] bureaucracy, energy supply difficulties,
[00:20:25] and the data center backlash. This could
[00:20:27] lead to Neo clouds with partially
[00:20:29] stranded compute and an infant shortage
[00:20:31] hitting Anthropic and OpenAI as the
[00:20:32] hyperscalers focus on their own needs.
[00:20:34] Chamath added, "This dislocation will
[00:20:36] benefit two kinds of orgs. The
[00:20:38] non-bureaucratic big scalers who can
[00:20:40] build industrial scale quickly and the
[00:20:42] nimble well-capitalized players feeding
[00:20:43] them.
[00:20:44] 2027 will be a turbulent year because it
[00:20:47] will clear out a bunch of wrong and bad
[00:20:48] bets. It will also be a consolidation
[00:20:50] year for a few."
[00:20:52] Elon Musk again responded, "Pretty much.
[00:20:55] As of the past few weeks, debt markets
[00:20:57] have almost entirely shut off access to
[00:20:58] money for any company that doesn't have
[00:21:00] substantial revenue independent of AI
[00:21:02] data centers. SpaceX closed 40 billion
[00:21:04] of debt for GPUs, but we're investment
[00:21:06] grade and have Starlink and launch
[00:21:07] revenue. That means the 200-plus neo
[00:21:09] clouds are going to see guppy-level
[00:21:11] death and consolidation. Some will make
[00:21:13] it through, but not many.
[00:21:15] Now, Bloomberg reported that this $30
[00:21:16] billion deal is actually not quite
[00:21:18] closed, with Apollo and Pimco as key
[00:21:20] investors. In particular, the deal is
[00:21:22] not yet priced. Interest rates in the
[00:21:24] mid-8% range were originally on the
[00:21:26] table, but with some neo cloud debt
[00:21:28] heading into junk territory in recent
[00:21:29] weeks, sources said potential investors
[00:21:31] are going back to the drawing board.
[00:21:33] Now, one type of response took Elon's
[00:21:35] comments very literally. Finance a lot
[00:21:37] wrote, "Elon Musk just told the entire
[00:21:39] world that the AI bubble has popped.
[00:21:41] Buckle up." Boring Business added, "Elon
[00:21:44] Musk is literally telling you that most
[00:21:45] neo clouds will die or get consolidated,
[00:21:47] and you're still bullish?"
[00:21:48] But then others pointed out that this is
[00:21:50] not exactly coming from an unbiased or
[00:21:52] uninterested source. Just another pod
[00:21:54] guy writes, "Elon has every incentive to
[00:21:57] talk crap and worsen access to capital
[00:21:59] for his primary competitors, i.e., neo
[00:22:01] clouds, while pumping his own road map
[00:22:03] to improve his purchase power when Tesla
[00:22:04] is merged into SpaceX."
[00:22:06] Said Lasana Guyb, "The sharks are
[00:22:08] smelling blood in the water. Wouldn't it
[00:22:10] be nice if a few neo clouds blew up and
[00:22:12] Elon could gobble them all up at a
[00:22:13] discount?" Ghostload reflected an entire
[00:22:15] strand of discourse, basically arguing
[00:22:17] that Elon is trying to pull up the
[00:22:19] ladder after SpaceX got out in the IPO
[00:22:20] market, writing, "Elon popping the AI
[00:22:23] bubble after front-running the Anthropic
[00:22:25] and OpenAI IPOs is like watching an
[00:22:27] episode of Billions and Succession."
[00:22:29] How the market digests this new strand
[00:22:31] of conversation is going to be one of
[00:22:32] the most interesting things to watch in
[00:22:34] the week to come. And of course, that is
[00:22:35] going to be entirely wrapped up with our
[00:22:37] fourth question, which is really just a
[00:22:38] proxy question for everything
[00:22:40] surrounding the Anthropic IPO and
[00:22:42] Frontier Lab funding.
[00:22:43] All throughout last week, there had been
[00:22:45] speculation that Anthropic needed to
[00:22:46] make their prospectus public by Friday
[00:22:48] if they wanted to hit their reported
[00:22:49] target of IPOing the week of
[00:22:51] Thanksgiving. Now, that prospectus did
[00:22:53] drop this morning as I was starting to
[00:22:54] record this show, and tomorrow we are
[00:22:56] going to dig into anything new that we
[00:22:57] learned as folks have a day to digest
[00:22:59] it. Heading into that, though, it seems
[00:23:02] like some of the biggest questions are
[00:23:03] around IPO pricing. According to reports
[00:23:05] from late last week, OpenAI's next round
[00:23:07] of fundraising is getting close at a
[00:23:09] valuation of 1.25 trillion, which some
[00:23:11] are taking as a softening, as previous
[00:23:13] reports had said that they had been
[00:23:14] looking at 1.4 trillion. Neither number
[00:23:16] is anywhere close to the $2 trillion
[00:23:18] number that some Anthropic investors
[00:23:19] were looking for, and it makes it more
[00:23:21] likely that we'll see the price trimmed
[00:23:23] to 1.5 trillion as a separate group of
[00:23:25] investors were calling for.
[00:23:27] We still haven't seen a number
[00:23:28] attributed to Anthropic or their
[00:23:29] investment bankers, but it certainly no
[00:23:31] longer feels like Anthropic is IPO'ing
[00:23:33] into strength. Of course, the sentiment
[00:23:36] could turn around immediately once
[00:23:37] Anthropic releases Fable 5.5. Rumor
[00:23:40] monger Chris GPT is suggesting the new
[00:23:41] model is already deployed for top
[00:23:43] customers, including JP Morgan and Meta,
[00:23:45] and while I'm certainly taking that with
[00:23:46] a grain of salt, as I've said publicly,
[00:23:48] it's pretty clear to me that Duet as
[00:23:49] their personal agent and Fable 5.5 as
[00:23:52] their world-leading model feels like the
[00:23:53] inevitable one-two punch for them to
[00:23:55] claim status as definitively the top dog
[00:23:57] heading into that IPO.
[00:23:59] That top dog status, though, is getting
[00:24:01] more interesting itself. The Information
[00:24:03] reports that OpenAI's price cuts have
[00:24:04] helped them take market share from
[00:24:06] Anthropic over recent months. One
[00:24:08] example they gave was that Rippling, who
[00:24:09] was using Anthropic models for 57% of
[00:24:11] their coding in May, with OpenAI
[00:24:13] handling a much smaller 16%, had now
[00:24:16] seen that ratio flipped, with OpenAI now
[00:24:18] powering 52% of coding workflows to
[00:24:20] Anthropic's 18%. Then again, that
[00:24:23] reporting might also be a slightly
[00:24:24] outdated view of the market. Opus 5.5,
[00:24:27] released a little over a month ago,
[00:24:28] seems to have kickstarted a resurgence
[00:24:30] for Anthropic. Open Router reports that
[00:24:32] the 7-day average token volume for
[00:24:34] Anthropic models is up 3.6x since the
[00:24:36] launch of Opus 5.5. And it's not just
[00:24:38] that model, either. Both Sonnet 5.5 and
[00:24:41] Haiku 5.5 have added meaningful token
[00:24:43] volume to reinforce Anthropic's gain in
[00:24:44] market share.
[00:24:46] Ramp data shows that Opus 5.5 has
[00:24:47] grabbed 35.1% of token share and 34.4%
[00:24:51] of business spend, the most successful
[00:24:52] first 3 weeks for any model release.
[00:24:55] Consumption will need to stay strong for
[00:24:56] a few more weeks to match the incredible
[00:24:58] two-month run for Opus 4.6, but the
[00:25:00] signs are there that this could be
[00:25:01] Anthropic's most commercially successful
[00:25:03] model ever.
[00:25:04] Andrew Curran summed it up, "The number
[00:25:06] of people on my feed over the last two
[00:25:08] weeks saying they are switching over to
[00:25:09] Anthropic because of Opus 5.5 is like
[00:25:11] nothing I've ever seen before. And even
[00:25:13] if someone does beat Opus, they have
[00:25:15] Fable 5.5 ready to go."
[00:25:18] Now, here's one interesting little
[00:25:19] speculation that I haven't seen anyone
[00:25:21] else talking about. It seems to me that
[00:25:24] this might be the one moment in perhaps
[00:25:26] the entire history of these two labs
[00:25:28] where OpenAI has a strong incentive to
[00:25:31] very temporarily not release a model
[00:25:33] that competes with Anthropic.
[00:25:35] Let's say you're OpenAI. No matter what,
[00:25:37] Anthropic's IPO is going up before
[00:25:38] yours. Given that, what's a better
[00:25:40] scenario for you? Option one, Anthropic
[00:25:43] going gangbusters, re-exciting the
[00:25:45] markets, and pushing off these bubble
[00:25:46] concerns for another couple of quarters.
[00:25:49] Or option two, Anthropic's IPO
[00:25:51] underperforming, and signaling to the
[00:25:52] rest of the market that yes, indeed, the
[00:25:54] AI bubble has burst, and that they
[00:25:55] should pull back further.
[00:25:57] The former scenario is not without its
[00:25:58] challenges, i.e., might have to battle
[00:26:00] for excitement from a definitive second
[00:26:02] place position, but the scenario if the
[00:26:04] latter comes to pass is an absolute
[00:26:06] disaster that might literally not make
[00:26:08] an IPO available to you anymore.
[00:26:10] So then, if you think the disaster
[00:26:12] scenario is in fact Anthropic's IPO
[00:26:15] failing, you don't want to do anything
[00:26:17] that could help contribute to that
[00:26:18] failure. And so letting Anthropic, just
[00:26:20] for a few weeks, have the absolute
[00:26:22] definitive best model in the world might
[00:26:25] weirdly be in OpenAI's interests.
[00:26:28] As you can see, friends, the questions
[00:26:29] surrounding AI this week are numerous,
[00:26:31] varied, and very interesting.
[00:26:33] For now, however, that is going to do it
[00:26:34] for today's AI Daily Brief. Appreciate
[00:26:36] you listening or watching, as always,
[00:26:38] and until next time, peace.
