---
record_id: "podcast:955fa65d-87d6-44af-9350-78c21f1b8cfc"
episode_id: 955fa65d-87d6-44af-9350-78c21f1b8cfc
title: How to Build an AI-Native Company Today
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-to-build-an-ai-native-company-today/955fa65d-87d6-44af-9350-78c21f1b8cfc"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-to-build-an-ai-native-company-today/955fa65d-87d6-44af-9350-78c21f1b8cfc"
feed_guid: null
feed_url: "https://anchor.fm/s/f7cac464/podcast/rss"
published_at: null
published_local_date: null
played_date: 2026-09-06
played_at: "2026-09-06T12:00:00Z"
play_count: 1
duration_seconds: 1620
source: pocketcasts-history-browser
played_label: September 6
history_order: 70
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: b521222791b9c2916c47a652defcc2571c6a02a83a54e91c47a616d76e5b1613
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

Alex Lieberman, founder of 10X Labs and former Morning Brew founder, presented a 30-feature view of AI-native companies, expanded by the host with enterprise observations and a retro-futurist presentation made with Codex and GPT image 2. The episode framed 2026 as the start of agentic AI, arguing that AI-native organizations redesign work from first principles rather than bolting agents onto old processes. It covered process blueprints, daily-driver harnesses such as Grok Bot, Claude Co-work, or ChatGPT, a unified or meshed intelligence layer for structured/unstructured data, model routing, context-as-code, periodic workflow reinvention, skills distribution, separating intent from implementation, cost per accepted pull request, agent-native development, planning/execution model splits, markdown metadata and progressive disclosure, continuous finance, OpenAI CFO Sarah Friar’s continuous accounting example, citizen-developer STLC, self-improving loops, AI ROI frameworks, agent swarms for marketing creative, weekly SEO/AEO experiments, agentic cybersecurity, RL-gym fine-tuning of open-source models, human first/final-mile judgment, evals as infrastructure, everyone-as-builder, recording learnings, governance as a partner, guardrails before features, autonomy earned through observation/suggestion/approval/acting alone, and full traceability from output to prompt/model/data/approver. The host cited Anthropic’s Claude tag as an example of agents triggered from shared spaces, with a claimed ~60% of some Anthropic building initiated that way, and added Binte Jameel’s comment that clear ownership and accountability is the missing feature.

Actionable decisions for the user are to treat process mapping as context capture, not a mandate that agents copy human workflows; define goals, guardrails, permissions, and success metrics before automating. Provide or evaluate daily-driver harnesses, possibly open-source foundations like DeepSeek’s harness, while planning for model-routing, cost-per-successful-task, cost-per-accepted-PR, and planning-vs-execution model tiers. Build a queryable context layer or interoperable mesh, treat architecture docs and conventions as code, add metadata/progressive disclosure to reduce token use, create a shared skills library, and separate high-level intent from implementation so non-engineers can contribute safely through a citizen-developer STLC with governance, access, versioning, and conventions. For operations, consider continuous accounting/forecasting, self-improving loops with objective evals, an AI ROI framework, weekly SEO/AEO experiments, agent-swarm creative testing, agentic cybersecurity, and selective RL-gym/open-weight fine-tuning only if technical capability exists. Keep humans at first and final miles, make evals standing infrastructure, require traceability and named owners for every AI workflow, and ask follow-up questions: who owns the outcome, what is the measurable success criterion, where are human checkpoints, which data sources are authoritative, what permissions do agents inherit, and what cadence should trigger re-architecting workflows. No health implications are present in the supplied material.

## Transcript

[00:00:00] A year ago, it was a very different time
[00:00:02] in enterprise AI. Companies were still
[00:00:04] talking about things like how many use
[00:00:05] cases they had for AI. Now a year on, we
[00:00:08] are no longer talking about use cases.
[00:00:11] Everything, it turns out, is a use case
[00:00:13] for AI. And in fact, in 2026, the
[00:00:16] long-awaited, much-discussed transition
[00:00:17] to agentic AI actually began.
[00:00:20] Surrounding that, companies have
[00:00:21] undergone a significant transformation
[00:00:23] process, one that pretty much everyone
[00:00:25] is still in the midst of. And yet, as
[00:00:27] companies try to become more AI native,
[00:00:30] the question is, what does that actually
[00:00:32] mean? What are the hallmarks and
[00:00:34] characteristics of companies that are
[00:00:36] not just glomming AI and agents onto old
[00:00:39] processes, but are really doing things
[00:00:41] in new ways, redesigning from the ground
[00:00:43] up? While it's all still emerging, I
[00:00:45] think we're at the point where we are
[00:00:46] starting to see a set of features and
[00:00:47] characteristics that define AI native
[00:00:50] companies.
[00:00:52] The AI Daily Brief is a daily podcast
[00:00:54] and video about the most important news
[00:00:55] and discussions in AI.
[00:01:03] Welcome back to the AI Daily Brief.
[00:01:05] Today we have a fun one. I feel like at
[00:01:08] this point, pretty much all of you are
[00:01:10] either at big companies who are trying
[00:01:12] to adapt and become the next version of
[00:01:14] themselves in this AI-enabled world, or
[00:01:17] are the people who are being hired by
[00:01:18] those companies to help them with that
[00:01:20] adaptation. Whichever side of that table
[00:01:22] you find yourself on, a core question
[00:01:24] that exists underneath all of that
[00:01:26] transformation is, what are we actually
[00:01:28] transforming into? A term that gets
[00:01:30] thrown around a lot is AI native. Part
[00:01:33] of the attraction of the term is that it
[00:01:34] separates companies that have simply
[00:01:36] glommed on AI and agents to old
[00:01:38] processes from those who have actually
[00:01:40] rethought from the ground up to take
[00:01:41] advantage of this new era. But what is
[00:01:44] the substance of AI nativeness? Part of
[00:01:47] what makes it great for a podcast is
[00:01:48] that there are a lot of things, and many
[00:01:50] of them are debatable. Enter Alex
[00:01:52] Lieberman. Alex is the founder of 10X
[00:01:55] Labs, which is a company that helps
[00:01:57] transform existing companies into AI
[00:01:59] native companies. And before that, he
[00:02:01] was a founder at Morning Brew. As you
[00:02:03] might imagine, that experience at
[00:02:04] Morning Brew means that he is often a
[00:02:05] great source of content. And the post
[00:02:07] that inspired this episode is actually a
[00:02:09] direct crib from his X account recently,
[00:02:12] 30 features of an AI native company.
[00:02:14] What I thought would be fun, after
[00:02:15] turning it into a beautiful 1950s
[00:02:18] retro-futurist themed presentation with
[00:02:20] the help of Codex and GPT image 2, is to
[00:02:23] go through these features one by one,
[00:02:26] where I will share the aspect of AI
[00:02:27] nativeness that Alex posted about, and
[00:02:29] then add any thoughts, qualifications,
[00:02:32] disagreements, although I don't think
[00:02:33] that I necessarily disagree in a lot of
[00:02:35] places, and other observations that I've
[00:02:37] seen in my work with enterprises as
[00:02:39] well.
[00:02:39] Now, I should note that I don't think
[00:02:41] that this is in any particular order. In
[00:02:44] fact, you can very much tell that this
[00:02:45] is not AI generated, as it reads much
[00:02:47] more like a stream of consciousness
[00:02:49] than, frankly, most of the content that
[00:02:50] you're used to seeing these days, which
[00:02:51] is kind of a breath of fresh air.
[00:02:53] First feature of an AI native company is
[00:02:56] to blueprint every process. To create,
[00:02:58] in Alex's words, a function-by-function
[00:03:00] process blueprint of the entire
[00:03:02] business. Now, I said I wasn't going to
[00:03:04] disagree much, and I'm not exactly going
[00:03:07] to disagree here, but this is one area
[00:03:09] where, although I don't disagree with
[00:03:11] doing this, I think the reasoning behind
[00:03:14] it for a lot of companies is actually
[00:03:16] leading them down the wrong path. Some
[00:03:19] of the reasons that it's valuable to
[00:03:20] blueprint processes, in other words, to
[00:03:22] map out how work actually gets done, is
[00:03:24] that a lot of that information right now
[00:03:26] lives locked inside people's heads.
[00:03:28] There are a lot of nuances and edge
[00:03:30] cases that people have been handling on
[00:03:32] their own forever, and which are perhaps
[00:03:34] transmitted person-to-person through
[00:03:36] random spoken meetings in the hall or
[00:03:38] side chats on Slack, that don't ever
[00:03:40] find their way into actual operating
[00:03:41] manuals. That puts the AI and agents
[00:03:44] that you're bringing into assist with
[00:03:45] the work at a disadvantage, because
[00:03:47] they're recreating things from the
[00:03:48] ground up. And so, having better maps of
[00:03:50] how work currently gets done is an
[00:03:52] incredibly valuable piece of context as
[00:03:55] you redesign your organization around AI
[00:03:57] and agents. So, all that part I agree
[00:03:58] with. Where I get concerned is around an
[00:04:02] inherent assumption of process mapping
[00:04:04] that I see pretty often. The assumption
[00:04:07] is that agents are going to do things
[00:04:09] the same way that humans do. I think
[00:04:11] that that's very unlikely to be true.
[00:04:14] And in fact, I think artificially
[00:04:15] constraining agents to do things along
[00:04:17] the pattern of an old workflow is in
[00:04:20] many cases the wrong approach. As
[00:04:22] opposed to, for example, giving them the
[00:04:24] goal and articulating the guardrails of
[00:04:25] what they can and can't do and letting
[00:04:27] them figure it out from there.
[00:04:29] Now again, that doesn't make process
[00:04:30] mapping not valuable, but we have to
[00:04:32] understand and prepare for the reality
[00:04:34] that the best way to do something in the
[00:04:36] future will not necessarily just look
[00:04:38] like an efficient version of the way
[00:04:39] that we did it in the past.
[00:04:41] Feature number two of an AI-native
[00:04:43] company is highly uncontroversial. And
[00:04:46] that is to give everyone a daily driver.
[00:04:47] I.E. everyone in the organization gets
[00:04:49] to use a daily driver harness such as
[00:04:51] Grok Bot, Claude Co-work, or ChatGPT at
[00:04:53] work. Now, what's interesting here is
[00:04:55] that 9 months ago, 10 months ago, when
[00:04:57] you saw the term daily driver, you would
[00:04:59] have assumed you meant just access to a
[00:05:00] frontier model. In other words, people
[00:05:02] have access to ChatGPT or Claude. But
[00:05:04] what Alex is talking about is a specific
[00:05:06] work harness, an environment in which
[00:05:08] models operate that is designed
[00:05:09] specifically for advanced knowledge work
[00:05:11] and coding, whether that's for software
[00:05:13] engineers or for non-software engineers
[00:05:14] who are now using code as part of the
[00:05:16] way that they do their job. Getting
[00:05:17] comfortable with a harness means getting
[00:05:19] comfortable with context. It means being
[00:05:21] able to understand and organize skills,
[00:05:23] as well as understanding how to
[00:05:24] provision access to different tools.
[00:05:26] Like I said, nothing controversial here.
[00:05:28] The one thing that I will note is that I
[00:05:29] think that we are going to increasingly
[00:05:31] see people rolling their own harnesses,
[00:05:33] often on the basis of an open-source
[00:05:34] foundation, for example, Deep Seek's
[00:05:36] harness that just came out, because
[00:05:38] they're going to want peak flexibility
[00:05:39] and they're not going to want to deal
[00:05:40] with things like investing in Cursor
[00:05:42] only to have it sold and no longer being
[00:05:44] able to access certain models through it
[00:05:46] because of that sale.
[00:05:47] Feature number three is one that many in
[00:05:49] the comments noted is to use AI's
[00:05:51] favorite term right now, load-bearing
[00:05:53] for the rest of the features. The idea
[00:05:55] is to build one intelligence layer to
[00:05:57] aggregate structured and unstructured
[00:05:59] data, documents, and business logic into
[00:06:01] a single source of truth that is
[00:06:02] queryable and that agentic work can be
[00:06:04] built on top of. It is unquestionable
[00:06:06] that AI native organizations are going
[00:06:08] to get good at organizing the context
[00:06:11] their agents need to work. Context
[00:06:13] management is and will continue to be a
[00:06:15] major discipline in this new org
[00:06:17] transformation period. To the extent
[00:06:19] that I have quibbles here, which is
[00:06:20] really just for the sake of interesting
[00:06:21] conversation, I kind of like the
[00:06:23] metaphor of a mesh or lattice rather
[00:06:26] than a single layer because I think
[00:06:27] especially as you get into larger
[00:06:29] organizations, trying to have a single
[00:06:31] source of truth for everything rather
[00:06:33] than sources of truth that can interface
[00:06:35] with one another and that agents can
[00:06:36] traverse, perhaps even uncovering and
[00:06:38] trying to reconcile with human support
[00:06:40] differences in sources of truth, is
[00:06:42] perhaps a more accurate reflection of
[00:06:44] how this is going to look with the
[00:06:45] biggest organizations, but obviously the
[00:06:46] substantive point underneath remains.
[00:06:49] Feature four of agent native
[00:06:50] organizations is one that has been a big
[00:06:52] subject of conversation on this show for
[00:06:54] the last few months, which is about
[00:06:55] using model routing to optimize cost per
[00:06:57] successful task across the business. I
[00:06:59] think this is right, but it's not just a
[00:07:01] matter of task routing. I think that
[00:07:03] task routing is part and parcel of an
[00:07:05] overall model architecture that is
[00:07:07] designed to be adaptable and flexible to
[00:07:09] different types of tasks.
[00:07:11] I think in some cases that will be
[00:07:12] reducible to using a router, but in many
[00:07:15] cases will also implicate a larger
[00:07:17] architecture based around that idea of
[00:07:19] matching task difficulty to model
[00:07:21] capability.
[00:07:22] Number five is an interesting one in the
[00:07:24] way that he frames it. He says that AI
[00:07:26] native organizations will treat context
[00:07:28] as code. They'll keep architecture
[00:07:30] documents and conventions updated while
[00:07:32] making diligent upfront planning part of
[00:07:34] the operating discipline. In other
[00:07:36] words, they will treat context not just
[00:07:38] as the background info that is required
[00:07:40] but as the actual foundations upon which
[00:07:42] agents are building, it's a subtle but
[00:07:44] important distinction and I think
[00:07:45] reflects the idea that a lot of this AI
[00:07:47] nativeness is not just in operational
[00:07:50] process, but also comes down to mindset
[00:07:52] shifts as well.
[00:07:53] Speaking of, feature number six is
[00:07:56] totally about mindset. Be willing to
[00:07:58] throw away everything you've built every
[00:08:00] 3 months and reimagine the workflows
[00:08:01] from first principles.
[00:08:03] Now, I think throwing away everything
[00:08:05] you've built might be slightly dramatic,
[00:08:07] but it is absolutely the case that we
[00:08:09] need to design these new systems for
[00:08:11] assumptions of change rather than
[00:08:12] assumptions of stasis. The frequency
[00:08:15] with which systems will need to be
[00:08:16] updated, whether it's 3 months or 6
[00:08:18] months or 9 months or a year or a sort
[00:08:20] of perpetual update marked by bigger
[00:08:22] periodic reimagining. However, it
[00:08:24] actually plays out, change is the name
[00:08:26] of the game and it's something that
[00:08:27] organizations are going to have to get
[00:08:29] way, way more comfortable with than they
[00:08:30] are today. And that includes not getting
[00:08:33] attached to the exciting way that you
[00:08:35] figured out to do something just a
[00:08:36] couple of months ago, because if the AI
[00:08:38] companies do their jobs well, advances
[00:08:40] should mean that we have new ways to do
[00:08:42] things that are either easier or more
[00:08:43] powerful.
[00:08:45] Feature number seven is about info
[00:08:46] sharing across the organization. Alex
[00:08:49] says that AI native organizations will
[00:08:50] use a skills distribution system to
[00:08:52] manage agent behavior and improve token
[00:08:54] efficiency by triggering consistent
[00:08:56] skills throughout the workflow. In other
[00:08:58] words, organizations will distribute
[00:08:59] skills, not just prompts. I think this
[00:09:01] is well as emblematic of a bigger shift,
[00:09:03] which is the discipline of agent
[00:09:05] management coming to the fore. Skills
[00:09:07] are a key aspect of agentic systems and
[00:09:09] so having ways to improve them, share
[00:09:11] them, access them, etc. across the
[00:09:13] organization, not just within the silo
[00:09:15] of any individual, is going to be
[00:09:16] increasingly important.
[00:09:18] Feature number eight is about the
[00:09:19] changing relationship between technical
[00:09:21] and non-technical team members. I think
[00:09:23] we're mostly past the days where people
[00:09:25] think that when we talk about vibe
[00:09:27] coding or using code for knowledge work,
[00:09:29] we somehow mean that all of a sudden the
[00:09:31] folks in marketing and HR are going to
[00:09:33] be the software developers instead of
[00:09:34] the existing engineers. That's not
[00:09:36] what's happening. But what is happening
[00:09:39] is both that those knowledge workers are
[00:09:41] for the first time able to build things
[00:09:43] themselves as a way to help do their
[00:09:44] job. And second, they have more ability
[00:09:47] to contribute to product and engineering
[00:09:49] discussions than they might have in the
[00:09:50] past. Feature eight of AI native
[00:09:52] companies from Alex's list is to
[00:09:54] separate intent from implementation, to
[00:09:56] keep technical implementation separate
[00:09:57] from high-level specifications, so
[00:09:59] non-technical staff can contribute in a
[00:10:01] format agents can turn into
[00:10:03] implementation plans.
[00:10:05] I think one of the ways that this will
[00:10:06] play out is as we see more agents
[00:10:08] triggered from shared spaces, that's a
[00:10:10] natural place for some of this to
[00:10:12] happen. For example, when Claude tag was
[00:10:14] announced, one of the more remarkable
[00:10:16] things about it was members of the
[00:10:17] Anthropic technical team saying that
[00:10:18] that was how they initiated a lot of
[00:10:20] their building now. And by a lot, I mean
[00:10:22] the number that sticks out in my head is
[00:10:23] like 60% or something ridiculous like
[00:10:25] that. If agents are being triggered from
[00:10:27] shared spaces, that creates more of an
[00:10:29] opportunity for different people to
[00:10:31] contribute to those conversations, but
[00:10:33] that in and of itself is going to create
[00:10:34] a different type of burden and new types
[00:10:36] of system requirements, which is what
[00:10:37] Alex is talking about here.
[00:10:39] Feature number nine is a cost-efficiency
[00:10:41] feature, where AI native companies will
[00:10:43] make cost per accepted pull request a
[00:10:45] key software metric and drive it down
[00:10:47] through better token efficiency. I think
[00:10:49] we are just at the beginning of the
[00:10:50] period of figuring out what the key
[00:10:52] metrics of agentic delivery are. And
[00:10:55] what's clear to us at this point is that
[00:10:57] whatever the metrics we land on are,
[00:10:58] it's likely that they include some sense
[00:11:00] of completeness as well as cost per
[00:11:02] completeness in order to be able to
[00:11:04] better compare model harness combos in a
[00:11:06] more apples-to-apples kind of way.
[00:11:08] Feature 10 is perhaps one of the
[00:11:10] features that many organizations are the
[00:11:11] farthest along with, which is to build
[00:11:13] agent native development systems,
[00:11:15] letting fleets of coding agents plan,
[00:11:17] write, test, review, and ship code while
[00:11:18] humans define intent and acceptance
[00:11:20] criteria. This is a lot less
[00:11:22] controversial than it would have been a
[00:11:23] year ago, but obviously there are still
[00:11:25] many organizations that are using a
[00:11:26] traditional process, despite there
[00:11:28] likely being an inevitable shift that
[00:11:30] that happen in the coming years.
[00:11:32] Feature 11 once again gets at the sub
[00:11:34] theme of token efficiency, dividing the
[00:11:36] business of work into planning phases
[00:11:37] and execution phases, using higher
[00:11:40] effort models for heavy planning and
[00:11:41] then executing with cheaper and faster
[00:11:43] models. The good thing will be that if
[00:11:44] we've done our job with feature number
[00:11:46] four about designing efficient token
[00:11:48] architectures, this is the type of
[00:11:50] division of labor that should naturally
[00:11:51] fall out of those systems.
[00:11:53] Feature number 12 feels at first glance
[00:11:55] fairly term heavy. It's use CLI tools to
[00:11:58] parse metadata in markdown files and
[00:12:00] traverse relationships allowing agents
[00:12:03] to be precise about input token usage.
[00:12:05] But really this is a technically
[00:12:06] specific way of designing a more token
[00:12:09] efficient system. Basically what Alex is
[00:12:11] arguing for is organizing a company's
[00:12:13] knowledge in a way that agents can only
[00:12:15] load the slice they need rather than the
[00:12:16] whole thing. It feels related to the
[00:12:19] idea of progressive disclosure, which is
[00:12:21] an information architecture pattern
[00:12:23] where complexity is unpacked gradually
[00:12:26] and in sequence in order to not create
[00:12:28] too much context overhead when an agent
[00:12:30] is working. Now, in addition to just
[00:12:32] making agents work better, there are
[00:12:34] obviously cost dimensions of that as
[00:12:35] well. And why I'm glad Alex included it
[00:12:37] is that so far we've been operating at a
[00:12:39] really high level. But this is an
[00:12:41] example of where you start to get
[00:12:42] granular and actually do things
[00:12:44] differently. I.e. making sure that the
[00:12:46] metadata that an agent can reference to
[00:12:48] understand whether something is useful
[00:12:49] is right there at the top of knowledge
[00:12:51] files that it has access to so that it
[00:12:53] doesn't waste context window on things
[00:12:54] it doesn't need.
[00:12:55] With feature number 13, we're starting
[00:12:57] to get into specific parts of the
[00:12:58] organization. He suggests that finance
[00:13:00] will run more continuously moving
[00:13:02] accounting and record keeping towards
[00:13:03] continuous processes, resetting
[00:13:05] forecasts on a much tighter cadence.
[00:13:07] OpenAI CFO Sarah Friar actually recently
[00:13:09] wrote about how she had done this inside
[00:13:12] OpenAI and about what a mindset shift
[00:13:14] and a technological discipline it took
[00:13:16] to make this sort of change.
[00:13:18] Alex also suggests that in AI native
[00:13:20] organizations, other parts of the
[00:13:21] organization and specifically the larger
[00:13:23] agentic operating system through which
[00:13:25] it runs will have access to those
[00:13:27] financial models so that that can be
[00:13:29] part of the logic as strategy and
[00:13:30] tactics are designed.
[00:13:32] AI native company feature 15 is the
[00:13:34] citizen developers STLC. It's an
[00:13:37] approach that Alex has talked about
[00:13:38] elsewhere as well, that enables
[00:13:40] non-technical employees to take a
[00:13:42] solution that they are building with
[00:13:44] coding tools from idea to production
[00:13:46] with the company's governance, access,
[00:13:48] versioning, and software conventions
[00:13:50] built into it. It's basically a process
[00:13:52] of reconciling the things that the
[00:13:54] non-engineers are making with the way
[00:13:56] that engineers build. Again, not with
[00:13:58] the idea of replacing software
[00:14:00] engineering in any way, shape, or form,
[00:14:02] but in order to have the new things that
[00:14:03] people are building for themselves or
[00:14:05] their teams, or even some segment of
[00:14:07] customers based on the part of the
[00:14:08] customer life cycle that they touch, to
[00:14:10] have that all contiguous with the
[00:14:11] engineering organization. It reflects
[00:14:13] again that shifting relationship between
[00:14:15] different parts of the organization in
[00:14:17] this new AI native space.
[00:14:19] Feature 16 gets to the sort of loop
[00:14:21] engineering that we covered in the
[00:14:22] webinar that I've shared on the show
[00:14:23] earlier this week. Make non-engineering
[00:14:25] workflows self-improving by learning
[00:14:27] from previous runs through external
[00:14:28] performance metrics and internal
[00:14:29] evaluations. The idea of loops is that
[00:14:32] instead of prompting agents, we give
[00:14:34] them a goal and bumpers around what they
[00:14:36] can do, and design a process that they
[00:14:37] can loop through over and over again
[00:14:39] until they achieve that goal.
[00:14:41] One of the necessary requirements of a
[00:14:43] loop is some verifiable success metric
[00:14:46] that is objective rather than
[00:14:47] subjective. I.E. I need to achieve an X
[00:14:51] percentage result on this test is a lot
[00:14:53] more definable an outcome goal than is
[00:14:55] our interface needs to look good. AI
[00:14:57] native organizations are going to be
[00:14:58] good at creating those sort of clear
[00:15:00] metrics of success, not just for the
[00:15:02] easy deterministic tasks, but for the
[00:15:04] broader array of knowledge work tasks
[00:15:06] that don't necessarily have that sort of
[00:15:07] success criteria built in natively.
[00:15:10] Feature 17 is really two parts. One is
[00:15:12] to use some AI ROI framework. To have an
[00:15:15] idea of what the organization is looking
[00:15:17] for out of its AI efforts, and to be
[00:15:19] able to measure against that. The second
[00:15:21] part is a little bit more opinionated
[00:15:22] from Alex about the way to set that up,
[00:15:24] with his recommendation being
[00:15:26] experimental scaling and optimization
[00:15:28] phases, and bets placed across
[00:15:29] infrastructure innovation and
[00:15:30] efficiency. Whatever the phases that you
[00:15:33] end up using, and the way that you
[00:15:34] organize different types of efforts, I
[00:15:36] think that the big recommendation here
[00:15:38] is to have a complex ROI architecture
[00:15:40] that can understand the goal of
[00:15:42] different efforts as being different
[00:15:43] from one another, but the organization
[00:15:45] having the ability to judge them even if
[00:15:47] they are different all within the same
[00:15:48] framework.
[00:15:49] Feature 18 is my Doctor Strange theory
[00:15:52] of agentic work come to life. The idea
[00:15:54] is that AI native organizations will use
[00:15:56] agent swarms to deploy many, many, many,
[00:15:59] perhaps hundreds, perhaps thousands of
[00:16:01] paid marketing creative variations for
[00:16:02] testing before increasing spend on ads.
[00:16:05] One of the things that I underestimated
[00:16:07] when I was first thinking about that,
[00:16:08] which by the way I still think is
[00:16:09] completely inevitable, was the way in
[00:16:11] which compute constraints in the short
[00:16:13] term would limit the viability of that
[00:16:15] sort of approach. Now that we've crossed
[00:16:17] this capability threshold, where many,
[00:16:19] many models are good enough right now to
[00:16:21] actually do this sort of creative work,
[00:16:23] and will be vanishingly cheaper than
[00:16:24] they are right now 6 months from now, I
[00:16:26] think that's when you'll start to see
[00:16:27] this sort of experimentation become a
[00:16:29] little bit more normalized, and I think
[00:16:30] it's going to be super, super
[00:16:31] interesting to see. Fascinatingly, and
[00:16:33] it's way beyond the scope of this
[00:16:35] particular conversation, I almost see a
[00:16:37] marketing barbell, where you are going
[00:16:39] to have just Doctor Strange crazy
[00:16:41] agentic swarms on one end of the
[00:16:42] spectrum, and utter number denying human
[00:16:46] taste for brand campaigns on the other.
[00:16:49] Basically, Rick Rubin on one side and
[00:16:50] machines on the other, and somehow it'll
[00:16:52] work.
[00:16:53] Feature 19 is another specific marketing
[00:16:55] recommendation of auditing, rewriting,
[00:16:57] and generating SEO and AEO optimized
[00:16:59] articles every week, then measuring to
[00:17:01] see whether any of it worked. I think
[00:17:02] the broader idea is that there is just
[00:17:04] so much interesting room for
[00:17:05] experimentation with content-based
[00:17:07] strategies now that the cost of
[00:17:09] producing content has gone down. Like so
[00:17:11] many of these recommendations, the idea
[00:17:13] here is that the AI native organization
[00:17:15] is not just going to do the thing, but
[00:17:17] to build learning systems around the
[00:17:19] thing to do it even better in the
[00:17:20] future.
[00:17:22] With feature 20, we're getting into
[00:17:23] cybersecurity, something that has
[00:17:25] obviously proven itself to be
[00:17:26] extraordinarily important over the past
[00:17:28] several months. Alex suggests that
[00:17:30] AI-native organizations are going to
[00:17:32] fight AI with AI using agentic
[00:17:34] cybersecurity systems built to defend
[00:17:36] the organization against AI-powered
[00:17:37] threats. Now, I think this is absolutely
[00:17:39] true, but boy is there a lot to figure
[00:17:41] out about exactly what type of
[00:17:43] cybersecurity capabilities organizations
[00:17:45] and legitimate defenders are going to
[00:17:46] have access to and how that's going to
[00:17:47] be provisioned. These are going to be
[00:17:49] some of the most important design and
[00:17:51] policy questions for AI companies and
[00:17:53] governments in the immediate term now
[00:17:55] that we've crossed some of these
[00:17:55] critical cyber thresholds.
[00:17:58] We're in our final third and I'll pick
[00:17:59] up the speed a little bit from here.
[00:18:00] Feature 21 is another approach to token
[00:18:02] efficiency and cost management combining
[00:18:05] a reinforcement learning gym with
[00:18:06] first-party data to fine-tune
[00:18:08] open-source models for high-volume
[00:18:09] processes that need state-of-the-art
[00:18:11] performance at reasonable cost.
[00:18:13] Basically, we now live in a world where
[00:18:14] the prevalence of customizable and
[00:18:16] post-trainable open weights models that
[00:18:18] are very near the frontier opens up a
[00:18:20] lot of new opportunities for AI-native
[00:18:22] organizations, many of which will find
[00:18:24] that this sort of model discipline is
[00:18:25] actually going to be useful for them.
[00:18:27] Still, I would say that I don't believe
[00:18:28] that every organization is all of a
[00:18:30] sudden going to be rolling their own
[00:18:31] models. I think that there are going to
[00:18:33] be a lots and lots of ways that all the
[00:18:34] labs and hyperscalers try to deal with
[00:18:36] cost efficiency, but to the extent that
[00:18:38] you're an organization that actually has
[00:18:39] this technical capability, it's
[00:18:41] definitely a place that you could be
[00:18:42] exploring to get an edge right now.
[00:18:45] Feature 22, we'll call the human
[00:18:47] sandwich. Keeping human touch and
[00:18:49] judgment at the first and final mile of
[00:18:50] most processes.
[00:18:52] If the argument is that even in
[00:18:53] AI-native organizations, there should
[00:18:55] always be people on either sides of the
[00:18:56] work sandwich, that I agree
[00:18:58] wholeheartedly with.
[00:18:59] What I'm less sure is where we'll find
[00:19:01] the right intervention points are for
[00:19:03] humans in the middle of processes. Yes,
[00:19:05] there will be many where it pretty much
[00:19:07] all happens agentically, but I don't
[00:19:08] think that we know exactly the right
[00:19:10] patterns. So, to speak of this one too
[00:19:12] generally feels harder for me to have a
[00:19:14] lot of confidence around.
[00:19:16] Feature number 23, I think is a little
[00:19:18] bit less arguable, which is the idea of
[00:19:20] making evals core infrastructure. Now,
[00:19:22] the specific example Alex gives is
[00:19:24] whenever new models arrive, use a
[00:19:25] standing apparatus to test their cost
[00:19:27] and performance against the company's
[00:19:28] core processes, but I just think
[00:19:30] everyone is now in the eval business
[00:19:31] more generally.
[00:19:33] Again, going back to the entire
[00:19:34] architecture of looping instead of
[00:19:35] prompting, you have to basically build
[00:19:38] in evaluation against some standard, or
[00:19:40] else the loops don't work. Thinking in
[00:19:43] terms of evals is just a new part of the
[00:19:45] discipline, and it's going to get to
[00:19:47] some weird parts of the organization
[00:19:48] that you wouldn't necessarily expect.
[00:19:51] Feature 24, again, totally unarguable to
[00:19:53] me is that everyone is a builder and
[00:19:54] that AI-native organizations will make
[00:19:56] building parts of every role, including
[00:19:58] and especially perhaps those held by
[00:20:00] C-level executives. I am not sure that
[00:20:03] every single person and every single
[00:20:04] knowledge worker goes from doing their
[00:20:06] work to managing agents that do their
[00:20:07] work. I think that'll be a big chunk of
[00:20:09] work, but again, saying all of it is a
[00:20:11] pretty big swath to cover. What I feel
[00:20:13] much more confident saying is that the
[00:20:15] capacity to build, to use code, to
[00:20:17] develop prototypes, to develop products,
[00:20:19] to do your work, is now a critical
[00:20:22] capability.
[00:20:23] Now, of course, over time, the space
[00:20:25] between people and the code that they
[00:20:27] use will get farther and farther as
[00:20:29] products obscure and abstract the
[00:20:30] technical details away, but that won't
[00:20:32] make people less of builders if they can
[00:20:34] still build things to solve their
[00:20:35] problems and create new opportunities.
[00:20:38] This one is both practical action and
[00:20:40] mindset shift, and has some pretty big
[00:20:42] implications for how enterprises even
[00:20:43] organize themselves.
[00:20:45] Feature 25 is kind of the twin of
[00:20:47] feature one, record everything worth
[00:20:49] learning from, because what the
[00:20:50] organization does not capture cannot be
[00:20:51] turned into AI-enabled work. This also
[00:20:54] gets at evals, context transmission. We
[00:20:56] just need to live in a paradigm of
[00:20:58] capturing a lot more, much to the
[00:21:00] delight, I assume, of the 75 meeting
[00:21:02] note-takers that show up in every Zoom
[00:21:03] call you have now.
[00:21:05] Feature 26, I love because people don't
[00:21:07] talk about this enough. Governance is so
[00:21:10] frequently seen as a blocker of
[00:21:12] innovation, but AI native organizations
[00:21:14] are going to treat governance as a
[00:21:15] transformation partner. They are going
[00:21:17] to treat it in other words as a way to
[00:21:19] unlock innovation. That's only going to
[00:21:22] work if you have legal, HR, and IT work
[00:21:24] in lockstep with the owners of the AI
[00:21:26] agenda, helping to design the enabling
[00:21:29] policies that address issues while
[00:21:31] unlocking new types of work. This I
[00:21:33] think in many ways will be a key
[00:21:35] hallmark of truly great AI native
[00:21:37] organizations versus those that are
[00:21:39] still kind of bolting AI onto old ways
[00:21:41] of working.
[00:21:43] Feature 27 harkens back to the idea of
[00:21:45] constant transformation. AI native
[00:21:47] organizations will maintain a bias
[00:21:48] towards disrupting the company before
[00:21:50] someone else does it for you. This
[00:21:51] extends beyond just how you do your
[00:21:53] current work, but cuts all the way to
[00:21:55] what work you should be doing. I think a
[00:21:58] lot of the big transformation of AI is
[00:21:59] not just going to be in the efficiency
[00:22:01] with which you do today's tasks, but
[00:22:03] finding those sort of orthogonal and
[00:22:04] aligned opportunities that you might not
[00:22:06] have gotten into yet, but which AI now
[00:22:08] enables you to go do.
[00:22:10] Feature 28 is kind of the technical twin
[00:22:11] to governance as unlock instead of
[00:22:13] governance as blocker, and you could sum
[00:22:15] up as guardrails before features. Agents
[00:22:17] inherit the permissions of whoever is
[00:22:18] asking, and those permissions are
[00:22:19] enforced in the data layer. You build
[00:22:21] the guardrails in, you don't have to
[00:22:22] relitigate it every time.
[00:22:25] Feature 29 could be an entire show on
[00:22:27] its own, and it's the idea that autonomy
[00:22:29] must be earned. These sophisticated,
[00:22:31] powerful agents are not given full
[00:22:33] autonomy right away, but climb a ladder.
[00:22:35] Observation, suggestion, acting with
[00:22:37] approval, acting alone, until they can
[00:22:39] run whole workflows inside a defined
[00:22:41] boundary. Even if we're trying to
[00:22:42] identify everything, we don't have to
[00:22:44] identify everything all at once. An old
[00:22:46] adage about an ounce of prevention being
[00:22:48] worth a pound of cure, I think is very
[00:22:49] applicable here.
[00:22:51] Feature 30, once again, is about the
[00:22:52] information system that surrounds
[00:22:54] everything that you do in this new
[00:22:55] agentic era, tracing every output to its
[00:22:57] prompt, model data, and approver, so
[00:22:58] human feedback attaches to something
[00:23:00] specific, not to a vague sense that
[00:23:02] something is off. We have the ability to
[00:23:04] create much more comprehensive and
[00:23:05] complex systems that surround our work.
[00:23:08] And if we do so, it comes with all sorts
[00:23:09] of benefits that improve the next work
[00:23:11] to be done after that.
[00:23:12] So, that is Alex's list with a lot of
[00:23:15] great food for thought in there. When it
[00:23:17] comes to what's missing, one of the best
[00:23:19] answers I saw in the comments came from
[00:23:20] a number of people, but was summed up by
[00:23:22] Binte Jameel, who writes, "Clear
[00:23:24] ownership and accountability. AI can
[00:23:26] automate a lot, but someone still needs
[00:23:27] to own the outcome. Every AI workflow
[00:23:29] should have a clear owner, measurable
[00:23:30] goal, responsible when things go wrong."
[00:23:33] The best AI-native companies won't just
[00:23:35] ask, "Can AI do this?" They'll also ask,
[00:23:37] "Who owns the result?"
[00:23:39] This, my friends, is nothing short of a
[00:23:41] new management discipline. And it's a
[00:23:43] management discipline that applies not
[00:23:45] just to the current managers, but to
[00:23:47] everyone, because everyone is becoming a
[00:23:49] manager of agents, as well as an
[00:23:51] implementer of their own work. For that
[00:23:53] reason, a lot of this is going to have
[00:23:54] to be pressure-tested in practice,
[00:23:56] learned through experience and failure,
[00:23:58] and then summed up as collective wisdom
[00:23:59] that we can all share. Hopefully, there
[00:24:01] is some good food for thought in here
[00:24:02] about how you help your company become
[00:24:04] more AI-native. For now, that that is
[00:24:06] going to do it for today's AI Daily
[00:24:07] Brief. Appreciate you [music] listening
[00:24:09] or watching, as always, and until next
[00:24:11] time, peace.
[00:24:16] >> [music]
