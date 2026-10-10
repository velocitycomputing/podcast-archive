---
record_id: "podcast:9cec51ad-45c3-43ae-8322-9e87e697fbd4"
episode_id: 9cec51ad-45c3-43ae-8322-9e87e697fbd4
title: How to Build Team Agents
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-to-build-team-agents/9cec51ad-45c3-43ae-8322-9e87e697fbd4"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-to-build-team-agents/9cec51ad-45c3-43ae-8322-9e87e697fbd4"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-09-29
played_at: "2026-09-29T12:00:00Z"
play_count: 1
duration_seconds: 2460
source: pocketcasts-history-browser
played_label: September 29
history_order: 26
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 7c9201a6414c5b5b95be3085f76cf48494823bc2ce1dff40f8bff3373432dfd1
analysis_mode: health
summary_source: hosted
model_source: hosted
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: sonnet
tagging_model: sonnet
proposed_tags: [primary-source-video]
proposed_entities: []
status: new
routed_to: null
---

## Summary

The episode is an "Operator's Cut" of The AI Daily Brief in which the host and guest Nofar Gaspar argue that 2026's solo agents are giving way to "team agents" (also called multiplayer AI, shared agents or AI teammates): one agent with shared knowledge, memory, instructions, skills, access and a named owner, used by many people. Their motivation was two problems. One is the "key person" who is the only one who knows how pricing exceptions or a big customer setup work. The other is work that sits between teams, such as a promise made in sales that marketing and customer success never hear about. They describe a three-step pattern at AI-forward companies (Every, Sierra, Shopify): everyone builds a private agent, agent sprawl follows, and the company then merges agents into fewer, broader team agents. They lay out a dial with three settings (private agent, shared knowledge and skills with private agents, and a true team agent) and four archetypes: expert, common-work, bridge and chief-of-staff. They list three reasons not to build one yet: personal taste matters more than a standard, nobody will own the knowledge, or the coordination costs more than the agent saves. Five design decisions follow: what it does (roles served, a "don'ts" list, starting with read and draft only), where it lives (a shared folder, a vendor agent such as Claude in Slack, a ChatGPT workspace agent, Copilot or Notion, or a self-hosted one such as OpenClaw or Hermes), what it knows, what it can touch, and how to run it. On knowledge they recommend four stages: collect (interview experts, harvest existing channels), refine (resolve contradictions, date items, strip secrets), approve (the owner of each piece signs off), and maintain (agent-proposed updates that a human reviews). On access they offer three options: act as the person asking (safest), use the agent's own account, or borrow one person's login (discouraged). They also warn that a channel-wide agent can expose data to people who shouldn't see it. The transcript was truncated at about 30,000 of 40,000 characters, so the "how to run it" section and the closing are missing.

For you, the practical step is to sort your existing agents before building anything. Keep taste-driven ones private, such as a personal social or prospecting agent. Point everyone's agents at one maintained body of company knowledge, which is the easiest starting point. Promote an agent to team status only when colleagues keep asking to borrow it or three people have each built their own version of the same thing. Before you build, check that someone will own and maintain the knowledge, and pick the archetype (expert, common-work, bridge or chief of staff) so you know what to watch for. Then start narrow, with read and draft only and a written "don'ts" list. Choose the simplest home that two people will use this week, such as a shared folder or a Slack or Teams channel agent. Default to acting as the person asking, so users only see what they could see anyway, and be careful about who can reach an agent that has its own account. Set up the four-stage knowledge process, with named sign-off and a scheduled human review of agent-proposed memory updates. Tell the team up front who can see conversations and where learnings are stored. If you want to test your approach, the show also advertises a free live webinar on building a personal AI benchmark on Thursday, October 1st, and a free self-directed course at Multiplayer AI.

## Transcript

[00:00:00] 2026 has been the year of agents. From
[00:00:02] open cloth the beginning of the year to
[00:00:04] now platforms like Muse and Grokbot and
[00:00:07] Instinct that are getting people to
[00:00:09] actually take advantage of these
[00:00:10] incredibly powerful autonomous tools
[00:00:12] that are getting increasingly large
[00:00:14] portions of their work done for them. We
[00:00:16] really have gone from agents being the
[00:00:18] next big thing to just being here. The
[00:00:20] problem is our work isn't just done
[00:00:22] alone. We tend to work in teams with
[00:00:25] other people. And yet up till now most
[00:00:27] agents have been solo affairs only
[00:00:29] covering the portion of our work that we
[00:00:31] do on our own. I think that is shifting
[00:00:33] now. A trend which I've talked about as
[00:00:35] multiplayer AI or shared or team agents.
[00:00:38] But what does it mean to even build a
[00:00:39] team agent? What are the types of
[00:00:41] considerations that go into it? And how
[00:00:42] different is it really than just
[00:00:44] building an agent for yourself? Those
[00:00:46] are the questions that I get into with
[00:00:47] New York Gaspar on this Operators Cut
[00:00:49] edition of the AI Daily Brief. The AI
[00:00:52] Daily Brief is a daily podcast and video
[00:00:53] about the most important news and
[00:00:55] discussions in AI.
[00:00:56] >> [music]
[00:01:03] [music]
[00:01:09] >> All right friends, quick announcements
[00:01:11] before we dive in. Obviously this is a
[00:01:12] pre-recorded episode. There are a bunch
[00:01:14] things cooking today. We will have a lot
[00:01:16] to talk about. So we will be back with
[00:01:18] our normal format tomorrow. I also
[00:01:20] wanted to share a couple of upcoming
[00:01:21] opportunities. First of all, this
[00:01:24] Thursday October 1st, we have a free
[00:01:26] live webinar all about building your
[00:01:28] personal AI benchmark. The whole idea is
[00:01:31] that when you get a new model like Opus
[00:01:33] 5.5 or Sonnet 5.5 or Gemini 4 or
[00:01:37] whatever model comes next, this will
[00:01:39] help you put together your own standard
[00:01:41] benchmark to better understand where
[00:01:43] that model is going to fit into your own
[00:01:44] process. That is completely free and if
[00:01:47] you register you will get all the
[00:01:48] materials after even if you can't
[00:01:49] attend. Again, that is coming up this
[00:01:51] Thursday October 1st. Now speaking of
[00:01:54] training, if you want to go a little bit
[00:01:55] deeper, the next cohort of our
[00:01:57] superintelligent executive AI and agent
[00:01:59] training programs is coming up. The
[00:02:01] Executive Agent Leadership Program is
[00:02:03] where you learn how to build AI agents
[00:02:05] for real business needs, as well as
[00:02:07] building a playbook to scale them safely
[00:02:09] across your organization. And if you
[00:02:10] feel you need a little bit more
[00:02:12] background before you get into that, you
[00:02:14] can also do the Executive Catch-up
[00:02:15] Program. The next Agent Leadership
[00:02:17] cohort starts on October 5th,
[00:02:19] while the next Executive Catch-up
[00:02:21] Program starts a week later on October
[00:02:22] 12th. All right, with all that out of
[00:02:24] the way, let's talk about how to build
[00:02:26] team agents.
[00:02:29] All right, Nofar, welcome back to the
[00:02:32] show. We got a an operator's cut today.
[00:02:34] >> Yes, happy to be here again.
[00:02:36] >> This one has its genesis in some
[00:02:39] conversations we were having as we were
[00:02:40] coming up into the fall around what we
[00:02:43] wanted to do with the the you know, this
[00:02:45] fall's edition of a free self-directed
[00:02:47] training program. And we were talking a
[00:02:49] lot about this idea of multiplayer AI
[00:02:51] and a shifting pattern from people just
[00:02:55] building solo agents that they were
[00:02:56] using themselves to a prediction that
[00:02:59] we're going to start to see and I guess
[00:03:00] we're starting to see early evidence of
[00:03:02] more agents that live in between
[00:03:05] people's shared workspace. And this kind
[00:03:08] of just follows the natural way that
[00:03:09] people work. A lot of your work is done
[00:03:11] individually, but then lots and lots is
[00:03:13] also done at the intersection with other
[00:03:15] people and that's where team agents can
[00:03:17] live. And as we were building out that
[00:03:19] course that's available right now at
[00:03:21] Multiplayer AI and just thinking about
[00:03:22] this concept more broadly, one of the
[00:03:24] things that we kept coming back to was
[00:03:26] that this is nascent enough that what it
[00:03:28] means to actually build a team agent
[00:03:31] won't necessarily be super obvious. And
[00:03:34] so, the goal of today's operator's cut
[00:03:36] is to help actually think through how to
[00:03:39] build team agents, to understand what
[00:03:41] team agents look like, to understand in
[00:03:43] what ways they are different from or I
[00:03:45] think probably what we'll argue here,
[00:03:48] similar to the types of agents that
[00:03:49] people might have already built and
[00:03:51] where they can go from here. So, super
[00:03:52] excited to have you back and uh and
[00:03:53] excited to dive in here.
[00:03:55] >> Amazing. So, I'm going to broaden your
[00:03:57] definition and I'm going to call them
[00:03:59] team agents and the concept is teams
[00:04:01] that your entire team can work with,
[00:04:03] whether it's because work happened
[00:04:04] between them or just because they're
[00:04:06] something that can be shared across team
[00:04:08] members. And kind of the short version
[00:04:11] is that some agents should stay yours
[00:04:13] and private, while others should become
[00:04:15] the team's level agents. And the ones
[00:04:17] that do become the teams need a few
[00:04:18] decisions made on purpose. Some of them,
[00:04:21] as you said, overlap with any good agent
[00:04:23] configuration and some of them are more
[00:04:25] unique or at least more intentional. And
[00:04:27] that's what we'll walk through. And I
[00:04:29] wanted to start as a means of motivation
[00:04:31] to give you like two stories that you
[00:04:34] will probably recognize for you from
[00:04:36] your company or your ecosystem. So, the
[00:04:38] first is about a person that everybody
[00:04:41] that I work with, every company that I
[00:04:43] work with, has at least one like that.
[00:04:45] And this person, they really know how
[00:04:47] their pricing exception work or what the
[00:04:50] data actually is all about or how our
[00:04:53] biggest customer setup was configured
[00:04:55] three years ago. And when they're
[00:04:56] swamped, then work has to wait for them
[00:04:58] because they're the only one who knows.
[00:05:00] And when they're on vacation, someone
[00:05:02] still calls them. And when they leave, a
[00:05:04] piece of the company leaves with them.
[00:05:06] So, in one of the companies that I work
[00:05:08] with, they had, I think, a person like
[00:05:10] that for each and every domain. So, no
[00:05:12] one gets to take vacation without
[00:05:14] getting a call from their peers. And
[00:05:16] obviously, that's not a desired state.
[00:05:18] The second scenario is work that nobody
[00:05:20] fully owns. So, a customer can move from
[00:05:23] sales to marketing to customer success.
[00:05:25] And then sales made them a promise
[00:05:27] during the deal conversation. And
[00:05:30] marketing is running a campaign with
[00:05:31] slightly different messaging. And then
[00:05:33] customer success finds out these
[00:05:35] promises were made to them a few weeks
[00:05:37] before the renewal. And each team has
[00:05:40] their own piece and nobody has the whole
[00:05:42] picture because the work sits between
[00:05:44] them. So, to your point. And even if
[00:05:46] they are using AI in each step of the
[00:05:48] process, these agents don't talk to each
[00:05:50] other and only worsen the problem in
[00:05:52] many cases. So, an agent that is built
[00:05:55] for the whole team can help with both of
[00:05:57] these problems, and they are of course
[00:05:59] quite different problems. So, there is
[00:06:02] another reason, I think, why this
[00:06:03] matters right now and why you should pay
[00:06:05] attention now even if you feel a little
[00:06:07] bit like this is above your head, and
[00:06:10] that's the pattern that I think that
[00:06:11] we're starting to see across the most
[00:06:13] AI-forward companies. And it goes in
[00:06:16] basically three steps. The step one is
[00:06:18] that everybody builds their own agents
[00:06:20] and they're happy with their
[00:06:22] productivity boost. Only with enough of
[00:06:24] those running around, we kind of get
[00:06:26] into an agent sprawl. Lots of agents
[00:06:29] doing overlapping work, each maintained
[00:06:31] by one person, each with slightly
[00:06:33] different picture of the company, and
[00:06:34] each one stops being useful the day that
[00:06:36] the owner loses interest or leaves the
[00:06:39] company. And then, what you see in the
[00:06:40] most AI-forward company, they started to
[00:06:43] merge some of those agents into
[00:06:45] team-level agents. Those will typically
[00:06:48] be much fewer agents, much broader in
[00:06:50] their scope, and each with a named owner
[00:06:53] and used by many people, and ideally
[00:06:55] refined over time as the team learns
[00:06:58] what they should and shouldn't do. And
[00:07:00] this is happening very publicly. There
[00:07:02] are many companies already talking about
[00:07:04] it. I think you mentioned Every's
[00:07:05] experience. They started by giving every
[00:07:08] employee an agent early in the year, and
[00:07:10] then by May they have moved to shared
[00:07:12] team agents. Sierra merged many of their
[00:07:14] agent specialist into one, Shopify's
[00:07:17] internal agent. So, we see a lot of
[00:07:19] these in very public-speaking companies
[00:07:21] all over the place. And most teams that
[00:07:24] I see are probably either in step one or
[00:07:26] two, but I think that it's very
[00:07:27] important for all of us to look at these
[00:07:29] AI-forward companies and understand how
[00:07:31] to get to number three and how to do it
[00:07:33] properly, and that's the entire purpose
[00:07:35] of today. So, to make sure that we are
[00:07:37] talking about the same thing because
[00:07:39] there are multiple names to basically
[00:07:42] the same thing. Some people, including
[00:07:44] yourself, call it multiplayer AI. You
[00:07:46] probably also heard shared agents. Some
[00:07:49] people refer to them as AI teammates.
[00:07:51] And even company brain is sometimes
[00:07:54] thrown into the mix or into
[00:07:55] interchangeably used to mean agents
[00:07:57] being used with shared knowledge across
[00:07:59] the company. I'm going to refer to them
[00:08:01] throughout the episode as team agents.
[00:08:03] And what I mean by that is we have one
[00:08:05] agent that too many people talk to with
[00:08:07] shared knowledge, shared memory, and one
[00:08:10] configuration. The instructions, the
[00:08:12] skills, the access, and the owner, they
[00:08:14] are all shared. And you might be
[00:08:15] thinking when you hear me saying that we
[00:08:17] already share skills, right? Most
[00:08:19] companies have an amazing skill library
[00:08:21] or working on a skill library. And
[00:08:23] that's awesome and that's great
[00:08:25] standardization of how you do the work
[00:08:27] in the company. But a skill is is a
[00:08:29] playbook for a specific task, where a
[00:08:31] team agent is something that your whole
[00:08:33] team works with on diverse set of tasks,
[00:08:36] ad hoc as well as repeated stuff. And it
[00:08:39] does carry the team knowledge, remembers
[00:08:41] what it learns, and using the team level
[00:08:44] skills, if you have them. Those, of
[00:08:46] course, can also tap into skills
[00:08:48] marketplaces and so on. So, a skill
[00:08:50] library perhaps is one of the
[00:08:51] ingredients, but they are not one and
[00:08:53] the same. And I want you to today think
[00:08:56] about how and when to start building
[00:08:58] your next team agent. And one more note
[00:09:01] on scope because there's a lot of
[00:09:02] excitement right now about all of the
[00:09:04] personal agents. I'm talking about Muse
[00:09:06] and Instinct and some of the other in
[00:09:08] this category. Those are for like a home
[00:09:12] or private life. Today the focus is
[00:09:14] going to be on work. So, that's one
[00:09:16] thing to make sure that it's clear about
[00:09:18] the scope. We're talking about agents
[00:09:19] that you build for your job. All right.
[00:09:22] I want to make sure that we understand
[00:09:24] like who I build the episode for. And I
[00:09:26] think it's built for everybody and not
[00:09:29] just the frontier professionals that are
[00:09:31] building the absolute cutting edge. If
[00:09:33] you're about to build one, of course,
[00:09:35] pay attention because it will provide
[00:09:37] you or verify the full playbook. It's
[00:09:39] also aimed at people who are not quite
[00:09:41] there yet because the decisions, as you
[00:09:43] rightfully said, do apply to any agent
[00:09:45] that you build or use. And a team agent
[00:09:48] just makes some of them even more
[00:09:49] critical. And even if you are working
[00:09:52] solo and you have a team of agents or
[00:09:54] you're contemplating building a team of
[00:09:56] agents, you have the same decisions. The
[00:09:58] other player in the your ecosystems are
[00:10:00] probably not your peers because you work
[00:10:02] alone, but perhaps you're building it
[00:10:03] for your customers or you're building it
[00:10:05] for a future you to make sure that it's
[00:10:07] robust enough and representative enough
[00:10:08] of diverse set of work. So, that's the
[00:10:12] motivation or who should pay attention.
[00:10:14] And one thing that I wanted to make sure
[00:10:16] that it's very clear is that not every
[00:10:19] agent should be shared. There is a dial
[00:10:22] here or a spectrum with three settings.
[00:10:24] We have a private agent, that's yours
[00:10:27] for your work with your taste and your
[00:10:28] access. For example, my own social media
[00:10:31] agent stays private and probably not
[00:10:33] going to be able to share it with
[00:10:35] anybody cuz I'm the only one that wants
[00:10:36] to share or write in social in a
[00:10:38] specific way. So, nobody should ever
[00:10:40] sound like me. And then we have shared
[00:10:43] knowledge. Those can be shared knowledge
[00:10:45] and skills, but still private agents.
[00:10:47] Meaning the team maintains one body of
[00:10:49] knowledge. For example, what we sell,
[00:10:51] how we work, what our words mean. Often
[00:10:54] with a shared skill library and
[00:10:56] everybody points their own agents at
[00:10:58] that. But this is where the skill
[00:10:59] library lives, by the way. And it's
[00:11:02] often the right answer and it's the
[00:11:04] easiest place to start. Another concrete
[00:11:06] example, say every sales person has a
[00:11:08] prospecting agent tuned to their own
[00:11:11] style and their own preferences. Keep
[00:11:13] those agents as they are because every
[00:11:15] sales person wants to have their own
[00:11:17] voice, but give them all the same
[00:11:19] well-maintained picture of the ideal
[00:11:21] customer and the messaging for the
[00:11:23] company. So, that's a hybrid mode that
[00:11:25] some companies or some use cases should
[00:11:28] remain. And lastly, we do have the the
[00:11:30] agents where we have one agent that many
[00:11:32] people work with that has its own job
[00:11:34] and its own owner. And agents can move
[00:11:37] along the dial. And if you have a
[00:11:39] scenario where your colleagues keep
[00:11:41] asking to borrow your private agent,
[00:11:43] that's probably a sign that you need to
[00:11:45] make it a team agent or to consider
[00:11:48] sharing it with others. So, the next
[00:11:50] question that I want to answer is are
[00:11:52] all team agents from the same archetype
[00:11:54] or do they all follow the same type of
[00:11:56] use cases? And the answer is not. Like
[00:11:59] across the teams that I work with, I can
[00:12:01] roughly categorize the existing or
[00:12:04] future built team agents into four
[00:12:06] kinds. And knowing which your kind is
[00:12:08] the helps you not only identify use
[00:12:11] cases, but also refine the use cases.
[00:12:13] And also it can tell you what to pay
[00:12:15] attention to in order to get it right.
[00:12:18] So, the first type of team agent, I'm
[00:12:21] calling it the expert agent. It's the
[00:12:23] one person's know-how or one small
[00:12:25] team's know-how. It's available to
[00:12:27] everyone who depends on it. You'll
[00:12:29] recognize it by the person who can't
[00:12:31] take the vacation remember from the
[00:12:33] beginning. If you want another example,
[00:12:35] it can be the data agent that can answer
[00:12:36] any data question across multiple
[00:12:38] departments in the company. Or a pricing
[00:12:41] and build desk agent that serves a lot
[00:12:43] of go-to-market organizations,
[00:12:45] compliance agent, and so on. In order to
[00:12:48] get it right, the knowledge has to come
[00:12:50] from the experts that holds it in the
[00:12:53] company. They need to be interviewed.
[00:12:56] They need to You need to collect the
[00:12:58] answers they already gave in multiple
[00:13:00] forums whether those are direct
[00:13:02] messaging or emails and other places.
[00:13:04] And they have to be they the experts
[00:13:07] have to be involved from day one.
[00:13:09] Because for them, this is what finally
[00:13:11] makes the vacation possible, but also a
[00:13:14] lot of job insecurity. So, tread
[00:13:16] carefully when working in this domain.
[00:13:18] The second type is what I refer to the
[00:13:20] common work agent. That's the scenario
[00:13:22] where many people are doing similar
[00:13:24] recurring work with one shared way to do
[00:13:26] it. The way to recognize a use case that
[00:13:29] falls into this category is when three
[00:13:30] people have each built their own version
[00:13:33] of the same agent. You can think about a
[00:13:35] team research and meeting prep agent,
[00:13:38] that's very classical one, or marketing
[00:13:40] teams content agent, and I'm I'm sure
[00:13:42] you can think of others. In order to get
[00:13:44] this archetype right, you have to agree
[00:13:47] on how work is done, and it's easier to
[00:13:50] say than to actually execute because
[00:13:52] you're managing the best of three
[00:13:54] versions and that's really a
[00:13:55] conversation about what you agree in
[00:13:57] terms of the standard for the company.
[00:13:59] So, an interesting conversation at the
[00:14:01] very least once you start contemplating
[00:14:03] a unifying an agent like that. And then
[00:14:05] we have the bridge agent. That's the
[00:14:08] work that flows between walls where
[00:14:10] nobody can do it alone. You'll recognize
[00:14:12] it when the handoffs break and every
[00:14:14] stage has to explain the context or the
[00:14:17] agents have to somehow work together
[00:14:19] between different departments. Example
[00:14:21] can be a customer agent that spends
[00:14:23] sales solution, customer success and
[00:14:25] delivery, that's a very classical one.
[00:14:27] And to get it right, we have to have
[00:14:29] each function their own piece of
[00:14:31] knowledge that is being fed into this
[00:14:33] agent. And people with different access
[00:14:36] will be eventually using that, so we
[00:14:37] have to also pay attention very very
[00:14:40] carefully to permissions and you'll have
[00:14:42] to work out to do that. And lastly, we
[00:14:44] have the chief of staff. That's the
[00:14:46] agent that own the team operating like
[00:14:49] operationalizing of the day-to-day work.
[00:14:52] It can be the decision, the commitment,
[00:14:53] the status, onboarding, and you will
[00:14:55] recognize this one when the team keeps
[00:14:57] repeating itself and you [snorts]
[00:14:59] joiners take weeks to find their
[00:15:01] footing. And in order to get this one
[00:15:03] right, what you need to do, you need to
[00:15:04] clearly define what it is allowed to
[00:15:06] learn, how can it learn their processes
[00:15:08] and their ongoing, and how does it do so
[00:15:10] automatically, which is not very
[00:15:12] trivial. And then there are also, of
[00:15:14] course, many questions around
[00:15:15] permissions and so on. So, while you're
[00:15:17] thinking about these archetypes and
[00:15:19] which one of them might fit some use
[00:15:21] cases that you are pondering or that you
[00:15:23] should be thinking about. And before I
[00:15:25] give you the playbook on how to actually
[00:15:27] build these team agents, a quick detour
[00:15:30] because I do want to give a quick
[00:15:32] reality check. There are some signs that
[00:15:34] a team agent is the wrong move or at
[00:15:36] least not the right move for you at this
[00:15:38] moment. So, one indication where you
[00:15:41] shouldn't build a team agent, at least
[00:15:43] yet, is when taste beats standards. If
[00:15:46] different people totally need different
[00:15:48] answers or not willing to agree on a
[00:15:50] standard and their own judgment or their
[00:15:52] own voice is the point, those need to
[00:15:54] remain private agents so people can
[00:15:57] remain authentic and not have to fight
[00:15:59] about the ground truth. And the second
[00:16:01] indication not to build is nobody can
[00:16:04] own the knowledge. If the team cannot
[00:16:06] agree on how the work is done or nobody
[00:16:08] is willing to own and maintain the
[00:16:10] shared knowledge over time, the agent
[00:16:12] will drift within weeks, sometimes
[00:16:14] within days. So, sort out the ownership
[00:16:16] before you go and build the team agent
[00:16:18] because that's going to be a no-go. And
[00:16:20] lastly, whenever you're uh realizing
[00:16:23] that trying to build a shared agent, a
[00:16:25] team agent only complicates more than it
[00:16:27] simplifies because you have conflicting
[00:16:30] needs or tangled permissions, endless
[00:16:32] coordination, if you realize that the
[00:16:34] result is more work than
[00:16:36] >> [clears throat]
[00:16:36] >> what the agent can provide for you,
[00:16:38] that's the answer. Don't build it, at
[00:16:40] least not until you are able to untangle
[00:16:42] some of the complexities. And of course,
[00:16:44] notice what's missing from the list,
[00:16:46] sensitive data and high stakes. Those
[00:16:48] are design questions and they shape how
[00:16:50] you build it, which is where we're going
[00:16:52] next. So, I don't think that when data
[00:16:54] is overly sensitive is a reason against,
[00:16:56] it's just something that uh needs extra
[00:16:58] careful attention. In order to build the
[00:17:01] candidate use case that hopefully you've
[00:17:03] gone through the decision checklist that
[00:17:05] I shared before, it comes down to five
[00:17:08] core design decisions for your agent. It
[00:17:11] goes through what it does, where it
[00:17:13] lives, what it knows, what it can touch,
[00:17:16] and how can you run These are the core
[00:17:18] questions. In order to make it more
[00:17:20] concrete, I'll use one example, the
[00:17:22] whole way through out. So, it's going to
[00:17:24] be a customer agent, and it's going to
[00:17:26] be the bridge kind, meaning one that
[00:17:28] holds everything the company knows about
[00:17:30] each customer and everything we've
[00:17:32] promised them, and it's probably going
[00:17:33] to be used by sales and solution
[00:17:35] engineering and customer success
[00:17:37] delivery and so on. They will be using
[00:17:39] that example agent to do various
[00:17:42] customer related activities. So, let's
[00:17:44] break down some of these decisions to
[00:17:46] make it actionable. So, first, the
[00:17:49] decision that you have to make is what
[00:17:50] it does. A quick caveat here, there is a
[00:17:53] lot of scoping that is very similar for
[00:17:55] any serious agent at work. It needs to
[00:17:57] have a clear job and a definition of
[00:17:59] done and a list of what it does and do.
[00:18:02] I'm going to stick here to what changes
[00:18:04] when it's built for a team versus an
[00:18:06] agent that you build just for yourself.
[00:18:07] So, the first decision is who it serves
[00:18:10] by role. For example, sales asks it
[00:18:12] different things than delivery does. So,
[00:18:15] write down each role and what they'll
[00:18:17] come to the agent for to make sure that
[00:18:19] you're covering all the scope. And of
[00:18:21] course, you can aim for one broad area
[00:18:23] of work because I think the team agent
[00:18:25] should be quite capable agents,
[00:18:27] otherwise, it's harder to justify their
[00:18:29] existence. In our example, I would
[00:18:31] expect that the customer agent will be
[00:18:33] able to prepare meeting, answers, where
[00:18:36] do we stand with this customer, will be
[00:18:38] able to flag promises that commit other
[00:18:40] teams and draft every handoff. For
[00:18:42] example, I've a a quite a broad scope.
[00:18:45] And what keeps it focused is the area of
[00:18:47] work, and that is primarily in our case,
[00:18:49] customers. I want you also to pay
[00:18:51] attention to the team don'ts list. This
[00:18:54] is the part people often tend to skip.
[00:18:57] For example, it never makes commitment
[00:19:00] on someone's behalf, or it never settles
[00:19:03] disagreement between people. Those go to
[00:19:05] its owner. You can think of it another
[00:19:08] such examples in your case. Also, make
[00:19:10] sure that the don't list in close
[00:19:12] permissions and data handling stuff. So,
[00:19:14] for example, it never carries
[00:19:16] information from one private space into
[00:19:18] a shared one. So, it never discuss one
[00:19:20] customer in another customer's space.
[00:19:22] And it doesn't speak for one person to
[00:19:24] another. And of course, like with any
[00:19:27] agent, ideally start with narrow scope
[00:19:30] reading and drafting. Only when it earns
[00:19:32] sufficient trust and was validated
[00:19:34] enough, then you can increase the scope
[00:19:36] as you gain more and more confidence.
[00:19:38] So, that's the first decision and we can
[00:19:40] move to the next one. The second
[00:19:42] question will be where the agent lives.
[00:19:44] And this is the question that gets asked
[00:19:46] most. So, let's be a little bit
[00:19:47] concrete. Basically, if I'm trying to
[00:19:49] make it as simple as possible, there are
[00:19:52] roughly three ways to share an agent
[00:19:54] from the simplest to the most involved.
[00:19:57] The simplest method will just to create
[00:19:59] a shared folder with your own tools,
[00:20:01] like the tools that your company already
[00:20:03] owns. And then, each person just point
[00:20:05] their own tool to the shared agent. And
[00:20:08] the folder will include instructions and
[00:20:11] potentially how to store new information
[00:20:13] as part of the way the agent overall
[00:20:15] behaves. That's a very naive and basic
[00:20:18] way, but as
[00:20:19] stepping stone to building shared agents
[00:20:22] and team level agents, that can be very
[00:20:25] good start, especially if all of your
[00:20:26] team members are already using similar
[00:20:29] agentic tools or agentic tools that can
[00:20:30] point to folders as sources for their
[00:20:33] information. So, that's the first and
[00:20:35] simplest method. The second way that we
[00:20:37] can do that is using a vendor ready-made
[00:20:39] agent. And we're increasingly seeing
[00:20:41] more and more, and we believe that we
[00:20:43] will continuously see more and more in
[00:20:45] the coming weeks and months of the year.
[00:20:47] We'll talk more about it later, but the
[00:20:49] way this work is that the vendor host it
[00:20:51] and you configure it. And in this
[00:20:53] category, we have many very recently
[00:20:55] famous tools, including Cloud Tag,
[00:20:58] OpenAI has their ChatGPT workspace
[00:21:00] agent, Copilot has their own offering
[00:21:03] that can be used like that. Notion and
[00:21:05] and many others are already offering
[00:21:07] spaces with agents that you can work
[00:21:10] together on and it's just a matter of
[00:21:12] you configuring their specifics. And
[00:21:14] lastly, and that's of course the most
[00:21:16] sophisticated, is an agent that you
[00:21:17] host. Meaning that something that you
[00:21:19] run. It can be, for example, an open
[00:21:21] source agent like Open Clo or Hermes on
[00:21:24] your own servers or or on a leased
[00:21:27] cloud. Or you some companies are even
[00:21:30] building their own custom harnesses
[00:21:32] specifically for these needs. So, that's
[00:21:34] the most sophisticated, but obviously
[00:21:36] has the most tech like technically
[00:21:39] demanding requirements as well as the
[00:21:41] most freedom to build around that. So,
[00:21:43] that's the three broad strokes options
[00:21:46] of where these team agents can live. On
[00:21:48] top of the decisions of how to build or
[00:21:51] the tools, there are two additional
[00:21:53] questions that come with them. The first
[00:21:56] question is who can see each person's
[00:21:58] conversation with the agent? Maybe it's
[00:22:00] only the people who are conversing with
[00:22:03] the agent, maybe it's the entire channel
[00:22:05] or everyone in the session. Over here,
[00:22:07] there is a lot of differences between
[00:22:09] the different tools. In some tools,
[00:22:11] everybody can read every chat. For
[00:22:13] example, in Claude in Slack, everyone in
[00:22:16] the channel sees what the agent does and
[00:22:19] what the agent converses with others and
[00:22:21] can also steer it. With many other
[00:22:23] agents, your chat is private. So, that's
[00:22:26] sometimes a design decision by the
[00:22:27] vendor, sometimes it's something that
[00:22:28] you can configure. And the second
[00:22:30] question is what it learns stored and
[00:22:33] who can read it. So, an ideal agent is
[00:22:36] not one that is obviously frozen, but
[00:22:37] one that has a lot of memory and
[00:22:39] learning on the go. And then the
[00:22:41] question where is this learning being
[00:22:43] stored and how does it happen? Is it
[00:22:45] something that happens per person and
[00:22:47] then the the agent evolves just from its
[00:22:49] interaction with you? Or is it per
[00:22:51] channel or team? Or maybe the entire
[00:22:54] workspace has a shared learning and
[00:22:55] memory and the agent evolves with
[00:22:57] everybody in public. And of course, one
[00:22:59] thing never costs customers. So, do
[00:23:02] check and choose and tell the team
[00:23:04] before the first real task what the
[00:23:07] status with the team agent that you
[00:23:09] built cuz this is where a lot of trust
[00:23:12] can be gained or lost. And my role is to
[00:23:16] pick the simplest option that two people
[00:23:18] will actually use this week. And for our
[00:23:21] customer agent, that's probably a
[00:23:23] channel agent or simple like a tool
[00:23:26] agent because four functions needed and
[00:23:28] if I will make it overly complicated and
[00:23:30] people will need to understand how to
[00:23:32] connect to that versus just going into a
[00:23:34] slack or teams channel, it's not going
[00:23:36] to work. So, in in our case, that's
[00:23:37] probably going to be the light solution.
[00:23:39] This decision, I want to move arguably
[00:23:41] to the most important decision and
[00:23:43] that's what it knows. And I think if
[00:23:46] you've built any agent, the recipe will
[00:23:49] sound very familiar. What's different
[00:23:50] for a team is that this is the moment
[00:23:53] the team agrees on the ground truth. How
[00:23:55] the work actually gets done, which
[00:23:57] definitions we use, which versions of
[00:23:58] the pricing policy is the real one. And
[00:24:01] I think that that conversation is worth
[00:24:03] having even if you never ship the agent
[00:24:05] because in most teams, even just
[00:24:07] agreeing on the knowledge is a big deal.
[00:24:10] And it's also where team agents get
[00:24:12] harder because the moment knowledge is
[00:24:14] shared, then you have more contributors
[00:24:16] and more contradictions and more places
[00:24:19] for something important to fall through.
[00:24:21] So, the process around the knowledge
[00:24:22] matters even more than it ever did in
[00:24:24] your private agent. So, you need to pay
[00:24:26] careful attention here. And ideally, you
[00:24:29] should go to these four stages. I want
[00:24:31] you to start by collecting the agent by
[00:24:33] interviewing the people who hold the
[00:24:35] knowledge and harvest what's already
[00:24:37] written in all the channels and all the
[00:24:39] places where information already
[00:24:41] resides. And I want AI do a lot of the
[00:24:44] heavy lifting in terms of aggregating
[00:24:45] and collecting the data. So, for our
[00:24:48] customer agents, for what I would do is
[00:24:50] I'll make sure that sales and solutions
[00:24:52] and success and delivery, they all will
[00:24:54] contribute their own piece. And then I
[00:24:56] want you to refine. I want you to merge
[00:24:58] the information coming from different
[00:25:00] sources, surface the contradictions. I'm
[00:25:02] sure that you will find five versions of
[00:25:04] the truth, and then date everything, and
[00:25:07] keep out what should never be shared. Of
[00:25:10] course, that includes passwords, notes
[00:25:12] about people, one customer's details in
[00:25:14] another customer's space, and so on. And
[00:25:17] then we have to approve it. Each piece
[00:25:18] should be signed off by whoever owns it,
[00:25:21] and the agent's owner puts it all
[00:25:23] together. And lastly, this can go stale
[00:25:26] very quickly, so you have to maintain.
[00:25:28] You need to decide what the agent may
[00:25:30] add to its own memory based on its
[00:25:32] working experience, and what person has
[00:25:35] to review first when it goes into the
[00:25:37] knowledge in the memory. And we want to
[00:25:39] make sure that one person's definition
[00:25:41] of what's last year quietly becomes
[00:25:44] everyone's without any agreement. And of
[00:25:46] course, put the upkeep on a schedule
[00:25:48] because you want the agent to propose
[00:25:51] updates regularly, and a person needs to
[00:25:53] review and approve the updates. And this
[00:25:56] is really the place to be very, very
[00:25:58] diligent and disciplined because it can
[00:26:00] totally make or break your team agent if
[00:26:03] you haven't done a good enough and
[00:26:04] self-sustaining process around acquiring
[00:26:08] and maintaining and verifying the
[00:26:10] knowledge that the agent taps into
[00:26:12] because it no longer serves you where
[00:26:15] you can very quickly fix anything that
[00:26:17] goes wrong. It can create a lot of havoc
[00:26:20] in your company if your team agent is
[00:26:22] not well educated enough on what
[00:26:24] matters. The fourth decision is what it
[00:26:27] can touch, and this is where team agents
[00:26:29] differ from the private ones because
[00:26:31] your own agent acts as you. And a team
[00:26:33] agent acts for many people. So, of
[00:26:36] course, there are many security 101 that
[00:26:39] you need to apply here. Those that apply
[00:26:41] to any agent definitely stick for the
[00:26:44] rules that are specific to like I'm
[00:26:46] going to just stick to the rules that
[00:26:48] they apply to team agents. The first
[00:26:50] thing that you have to decide is whose
[00:26:53] access it uses and you have three
[00:26:55] options. You can use the access or to
[00:26:58] act as whoever is asking. So, it only
[00:27:00] sees what the person that was asking the
[00:27:03] question can see and that's probably the
[00:27:05] safest choice, but sometimes the most
[00:27:07] complicated to execute unless the vendor
[00:27:09] already did it for you and probably the
[00:27:11] right one when people on the team have
[00:27:13] different access levels. The other
[00:27:15] option that you have is to have its own
[00:27:17] account set up with exactly the access
[00:27:20] the job needs and that's right when the
[00:27:22] whole team works on the same shared
[00:27:24] material. And lastly, it can use one
[00:27:26] person's login. Only ever do that for
[00:27:29] read-only and non-sensitive material
[00:27:32] because everyone who talks to the agent
[00:27:34] effectively gets that person's access.
[00:27:36] So, I would not recommend to go down
[00:27:38] that path and what I would probably do
[00:27:41] for our customer agent to is to act as
[00:27:43] the person asking because sales,
[00:27:45] success, and delivery see different
[00:27:47] things in the CRM and in other systems.
[00:27:49] So, I don't want to have the agents
[00:27:51] responding to them with information that
[00:27:53] they shouldn't be able to see. So, that
[00:27:54] was the first rule on what the agent can
[00:27:57] see. The second rule is to decide who
[00:27:59] can ask it. And when the agent has its
[00:28:02] own account, everyone who can talk to it
[00:28:04] can use the account. And if you put an
[00:28:06] agent with access to the pricing sheet
[00:28:08] in a channel of 40 people, a few
[00:28:10] contractors among them, then all of a
[00:28:12] sudden all 40 can now get the pricing by
[00:28:15] asking. The agent knows more than some
[00:28:17] of the people who can reach it. So,
[00:28:19] decide who can talk to it with the same
[00:28:21] care you give to what it can see. Okay?
[00:28:23] So, that's something that happens very
[00:28:26] regularly when people don't pay
[00:28:27] attention. I also want you to decide
[00:28:30] where the answer lands. This one runs
[00:28:32] the other way. The agent uses the
[00:28:34] asker's own access and the asker has
[00:28:37] every right to ask the question. The
[00:28:39] problem is that the answer shows up in a
[00:28:41] shared space in front of people who
[00:28:43] don't. So, this is something that is
[00:28:44] happening right now. If you will look at
[00:28:47] documentation of Claude in Slack, it can
[00:28:49] use the ask own connections inside the
[00:28:51] team channel. And after the person
[00:28:54] approves, and the topic documentation
[00:28:56] currently notes that it doesn't consider
[00:28:59] who else is in the channel. So, if I
[00:29:01] approve to use my connectors and fetch
[00:29:03] all the information that I am permitted
[00:29:05] to see, and now the information is
[00:29:07] stored in the channel where others can
[00:29:09] see that, that's the reality currently
[00:29:11] with the existing Claude implementation.
[00:29:14] So, if it's sensitive, the answer has to
[00:29:16] go to the person who's asking privately
[00:29:18] and not in a shared channel. And lastly,
[00:29:20] keep record of who asked for what. And
[00:29:23] that's an important logging because when
[00:29:25] an agent works under its own account,
[00:29:27] the logs say the agent did it, right?
[00:29:29] And you want to know which person asked
[00:29:31] so you can backtrack and make sure there
[00:29:33] are no unexpected behaviors. And
[00:29:35] everything else, like starting with the
[00:29:37] least access and having a person approve
[00:29:39] anything that can't be undone, is the
[00:29:40] same for any agent. So, I'm not giving
[00:29:43] you security one-on-one. Okay. Lastly,
[00:29:46] last decision and the one that will make
[00:29:48] your team agent live beyond its first
[00:29:50] week or the first month, that's the full
[00:29:52] like operating manual here. Of course,
[00:29:55] the multiplayer sprint has much more
[00:29:57] comprehensive way of thinking about it,
[00:29:59] but these four points are what makes or
[00:30:02] break the agent in practice. So, the
[00:30:04] first thing is one owner. Anyone on the
[00:30:06] team can hand the work, but I want to
[00:30:08] have one person or a very small group of
[00:30:12] of people who owns the priorities,
[00:30:15] maintain the agent, and decide when two
[00:30:17] people ask for opposite things, how to
[00:30:20] evolve the agent knowledge or feature
[00:30:21] set. They also decide on standing
[00:30:24] instructions and so on. So, that's one
[00:30:26] thing. The second thing that I want to
[00:30:28] mention is the clear rules of
[00:30:29] engagement. I want you to tell people
[00:30:31] how to work with it, what it does and
[00:30:33] doesn't do, and what it can see, who can
[00:30:35] see their conversation with it, and
[00:30:37] everything that we discussed so far. We
[00:30:39] also we want to have clear indications
[00:30:42] of how to correct the agent when it's uh
[00:30:44] wrong. And I think that people trust the
[00:30:47] agents that they're using and the team
[00:30:48] agents the more they know they learn
[00:30:51] what it's learning and what's the
[00:30:52] learning process. The next thing I want
[00:30:54] you to do is to put decisions where it
[00:30:55] can see them. So, a team agent only
[00:30:58] knows what's written down in a place
[00:31:00] that it can reach. And if your team
[00:31:02] decides things in private messages and
[00:31:04] hallway conversations, the agent will
[00:31:06] never hear about them and part of
[00:31:08] running it smoothly is still have it be
[00:31:11] able to tap into what's happening in
[00:31:13] real time in in the team and to make
[00:31:15] sure that the team decisions and the
[00:31:16] team ongoing day-to-days are being
[00:31:19] learned by the agent itself. And lastly,
[00:31:21] I want you to keep watching because you
[00:31:23] will probably start with a small
[00:31:25] Ideally, you should start with a small
[00:31:26] pilot group and keep a few test
[00:31:28] questions that you can rerun whenever
[00:31:30] something changes, but I also want you
[00:31:32] to just monitor because we know that
[00:31:35] things change very frequently, so it's
[00:31:36] not just a about having a proper process
[00:31:39] for whenever you want to introduce a new
[00:31:41] model or a new tool or a new knowledge
[00:31:43] or or new changes in instructions, but
[00:31:45] also just to monitor that everything is
[00:31:47] working properly. And of course, in some
[00:31:49] cases we would want to retire the team
[00:31:51] agent if it's not behaving properly as
[00:31:54] we expected. We covered a lot [laughter]
[00:31:56] of ground. And if I need to pull it
[00:31:58] together before we close, first of all,
[00:32:00] I hope that I've convinced you that team
[00:32:02] agents matter for everyone even if
[00:32:04] you're it will take you a while until
[00:32:05] you will actually be building one and
[00:32:08] that building them properly is what
[00:32:10] makes the difference. Of course, not
[00:32:12] every agent should be shared. Private
[00:32:14] agent or shared knowledge and skills
[00:32:16] with private agents or team agents,
[00:32:18] these are all valid options and should
[00:32:19] be used where appropriate. We talked
[00:32:22] about the team agents that are coming in
[00:32:24] four kinds, the experts, the common work
[00:32:26] agent, the bridge agent, the chief of
[00:32:27] staff. And knowing which one your use
[00:32:30] case fit into tells you a lot about how
[00:32:32] to get it right. And we also talked
[00:32:34] about three signs on when to wait,
[00:32:37] whether it's because taste beats the
[00:32:39] standards, whether because nobody can
[00:32:40] owns the knowledge, or when it doesn't
[00:32:43] simplifies the work. And once you're
[00:32:45] building, we went over the five
[00:32:47] decisions in order of what it does,
[00:32:49] where it lives, what it knows, what it
[00:32:51] can touch, and how do you run it. And if
[00:32:54] you take those with you, you have what
[00:32:56] you need in order to get the team agent
[00:32:58] properly. If you want to concretely do
[00:33:01] that, a quick way to do that. So, first
[00:33:03] of all, that we have the multi player AI
[00:33:05] sprint, which is free and will walk you
[00:33:07] through a team activity of in 4 weeks
[00:33:10] configuring everything that we
[00:33:11] discussed, some of them in greater
[00:33:13] detail. If you want to learn how to
[00:33:16] properly build seriously team agents and
[00:33:19] agent rosters and how to do that in the
[00:33:23] best possible way, we have another
[00:33:25] cohort of the executive agent leadership
[00:33:26] that starts on October 5th and we'll be
[00:33:28] happy to see you with all of our
[00:33:30] builders. However, if you feel that you
[00:33:32] need a little bit of a catch-up before
[00:33:33] you go and build agents for teams and
[00:33:37] and rosters of agents and so on, we also
[00:33:38] have the executive catch-up that helps
[00:33:40] you become best-in-class AI user before
[00:33:43] you go and build those agents. And
[00:33:45] lastly, everything is changing. Odds are
[00:33:48] that every week we will get a relevant
[00:33:51] release, and by the time you hear this,
[00:33:53] maybe already something was released.
[00:33:55] But I do think that everything that we
[00:33:56] covered today holds no matter what ships
[00:33:59] next because when an an agent is built
[00:34:01] properly and the decisions are made
[00:34:03] right, it's orthogonal to any specific
[00:34:05] tool or feature. It's the business
[00:34:07] decision and the team standardization
[00:34:10] that matters much more than the tools
[00:34:12] that will help make it better by design
[00:34:15] the more releases we will have. And if I
[00:34:17] need to make some predictions for the
[00:34:19] rest of the year, so I think that we
[00:34:21] will see more and more formalization of
[00:34:23] what we just covered and more tools and
[00:34:25] features that will help us get it even
[00:34:27] better and easier around identity,
[00:34:30] permissions, ownership, and so on. As
[00:34:33] well as uh like we can always trust the
[00:34:35] practitioners to share many of their
[00:34:36] learnings in the public eye, so we can
[00:34:39] learn from many of the [clears throat]
[00:34:40] other AI and like frontier individuals
[00:34:43] and companies and see how it's working
[00:34:45] for them. That's it.
[00:34:47] >> Awesome. Great stuff, Nofar. Um I have a
[00:34:49] few things that I want to lob out there,
[00:34:51] discussion style, just as we close out.
[00:34:53] First of all, I guess the question, you
[00:34:55] know, you gave four archetypes of
[00:34:57] different types of agents that you've
[00:34:58] seen. Do you see Are any of them more
[00:35:02] common starting places than others for
[00:35:04] teams that you've observed?
[00:35:05] >> I think that in theory, your definition
[00:35:08] of an agent that lives between
[00:35:10] individuals or between teams sounds the
[00:35:12] most attractive, but it's the hardest to
[00:35:14] execute. So, I think that's actually the
[00:35:17] ones that will, from what I'm seeing,
[00:35:19] are not the first to go for, and I've
[00:35:21] seen various very successful versions of
[00:35:23] the first one, of the expert agents,
[00:35:25] that help create more redundancy in a
[00:35:28] team, redundancy in the good sense, and
[00:35:30] relieve some of the burden on the those
[00:35:32] bottlenecks within the company. So,
[00:35:34] those I've seen a ton of implementations
[00:35:36] already, and I think the more the tools
[00:35:38] make it more accessible, the easier
[00:35:40] those will be to build. So, those are
[00:35:42] probably the lowest-hanging fruits.
[00:35:44] >> That's funny, cuz that's exactly where
[00:35:46] my head goes. I'm I'm super attracted to
[00:35:48] the ones that I think are are most
[00:35:50] difficult to build. I I've also seen a
[00:35:52] lot of, you know, very simple
[00:35:54] implementation of that expert one,
[00:35:56] which, you know, we've talked about for
[00:35:58] a long time without even identifying it
[00:36:00] as this sort of team agent, is just
[00:36:03] basically the agentified team internal
[00:36:05] knowledge hub, you know, policies around
[00:36:09] whatever, like early dismissal, who
[00:36:11] knows, like what are you know, that just
[00:36:12] the company database of information that
[00:36:14] you can access through the chatbot
[00:36:16] instead. That's been something that
[00:36:17] companies have had a ton of success with
[00:36:20] as just an early, easy, fast use case
[00:36:23] right from the beginning. Another
[00:36:24] question that I have for you is how, you
[00:36:27] know, I'm sure that a lot of folks are
[00:36:29] are sitting there wondering how much
[00:36:31] they should invest in building these
[00:36:35] sorts of things before
[00:36:37] Grok Bot or Microsoft Copilot or one of
[00:36:40] these sort of core tools that they might
[00:36:42] be using OpenAI, Anthropic just drop the
[00:36:45] sort of native version of this. And
[00:36:47] there's clearly some indications that
[00:36:49] they're thinking in this way. I think
[00:36:50] Claude Tag being the best example so
[00:36:51] far, but you know, is this one where the
[00:36:55] value of digging in at this stage is
[00:36:57] going to be so you understand the theory
[00:36:59] and the ways to customize when better
[00:37:01] tools come around in the future or how
[00:37:03] do you think about that trade-off?
[00:37:05] >> I think the heavy lifting is always
[00:37:07] going to be the configuration and the
[00:37:09] knowledge curation. So, I would select
[00:37:12] the one tool that is adjacent the most
[00:37:14] to your existing tool ecosystem and and
[00:37:17] figure out how to implement all the rest
[00:37:19] and and if
[00:37:21] like a new better improved tools come to
[00:37:23] play will be ready because you're
[00:37:24] already already agree on the ground
[00:37:26] truth, on the do's and don'ts of these
[00:37:28] agents, on the use cases. So, even if
[00:37:31] you at first implement them very
[00:37:33] naively, that's going to have you for
[00:37:35] future ready. As for going and building
[00:37:37] these own like a competing product or
[00:37:39] your own like team level harnesses and
[00:37:41] so on,
[00:37:42] if you have the chops and you can do
[00:37:44] that easily and you have the
[00:37:45] justification, you can, but I'm not sure
[00:37:48] that I would have spend my energy now on
[00:37:51] going and building the own like my own
[00:37:53] version of Claude Tag or similar when we
[00:37:55] were I think both of us agreed that all
[00:37:57] of these are coming and will probably be
[00:37:59] made very accessible and very smart and
[00:38:02] your mode [music] is probably in
[00:38:04] everything that these companies cannot
[00:38:05] tap into.
[00:38:06] >> Awesome. Well, thanks as always for
[00:38:08] another great Operators Cut and I'm
[00:38:09] excited to have you back soon.
[00:38:11] >> Thank you. Bye. [music]
[00:38:20] >> [music]
