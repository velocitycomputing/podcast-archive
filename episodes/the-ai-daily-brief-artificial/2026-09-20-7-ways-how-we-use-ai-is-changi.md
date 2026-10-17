---
record_id: "podcast:26957f0d-4bf9-47e7-a14e-59bb8a4e3932"
episode_id: 26957f0d-4bf9-47e7-a14e-59bb8a4e3932
title: 7 Ways How We Use AI Is Changing
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/7-ways-how-we-use-ai-is-changing/26957f0d-4bf9-47e7-a14e-59bb8a4e3932"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/7-ways-how-we-use-ai-is-changing/26957f0d-4bf9-47e7-a14e-59bb8a4e3932"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-09-20
played_at: "2026-09-20T12:00:00Z"
play_count: 1
duration_seconds: 1560
source: pocketcasts-history-browser
played_label: September 20
history_order: 59
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 1d18a1a6f36c0446e13a391f9c7dd8e814f171697ae42e9186ecddd8e52d3608
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

Seven shifts in AI interaction are described: product simplification and integration, with Meta’s Muse, Anthropic’s unified Claude Co-work/chat/design experience, Meta Chief AI Officer Alexander Wang, Anthropic Labs lead Mike Kreger, Claude code creator Cat Woo, technologist Tom Goodwin, David Herman, Christian Celig, and Shaunie Matthew arguing that users want fewer choices and one interface; the transcript cites 9,000 sign-ups for a free “claw camp” as evidence that some users still embrace complexity. It also describes “mono threads” enabled by context compaction, citing Codex’s Nick Bowman, developer Anthony Kroger, Cursor, and Claude projects, where one persistent conversation coordinates parallel threads; chatbots become agent fleet managers, with Ethan Malik and Signal arguing that apps may become context databases behind a single agent interface. Voice interaction is framed as table stakes through Grockbot, OpenAI’s Codex/GPT Live ad, Google Gemini Live, and Devon, with Danny Graiosce, Parker Conrad, Garav Bison, and Ali K Miller quoted. The episode also argues users increasingly set goals and design loops rather than prompts, citing /goal, Claude Code, Codex, and OpenClaw creator Peter Steinberger; “multimodelity” or multi-model stacks become a cost/efficiency discipline, especially with Fable 5.1 subagent usage; and shared/multiplayer agents emerge through Claude tag and Mo XYZ’s Mio, which says beta since July saved teams thousands of hours and completed tens of thousands of tasks, and a claim that 2026 is the year agents became real, with Ethan Malik, Arya Bhani, Atlan’s Rishi Batnagar, and Josh Rosen debating memory, context, and org design.

For the user, the actionable move is to audit recurring workflows and convert one or two into persistent, goal-based threads with clear success criteria, letting a coordinator agent delegate subtasks rather than manually restarting chats; test voice input for rapid task entry, but first verify the agent can actually execute actions. Consider a personal multi-model policy: reserve frontier models for planning, synthesis, and high-stakes judgment, route routine subtasks to cheaper models, and monitor usage caps because fleet agents may silently consume expensive capacity. For teams, decide whether shared agents should own channel context, shared memory, or only specific workflows, and ask who is the principal—user, agent, or team—when access, authority, and memory are shared. Research leads include multiplayer AI architecture, shared memory, context ownership, and org adoption; follow-up questions are: Which tasks have measurable success criteria suitable for loops? Which apps can become databases behind a single agent interface? Which workflows are safe for autonomous execution, and what guardrails, review checkpoints, and escalation rules are needed? No direct health implications are indicated in the material.

## Transcript

[00:00:00] The way we use AI is changing. First, we
[00:00:03] were prompt engineers, then context
[00:00:05] engineers, then harness engineers, then
[00:00:07] loop engineers. And while it's tempting
[00:00:09] to view all of these things as just one
[00:00:11] silly buzzword giving way to the next,
[00:00:13] the reality is that we are all together
[00:00:14] on this journey figuring out just the
[00:00:16] best way to use a completely new
[00:00:18] technology that is changing both how we
[00:00:20] do our current work and opening up new
[00:00:22] possibilities of what work we can even
[00:00:23] do. Today, we're talking about seven
[00:00:25] ways that how we use AI is changing. The
[00:00:28] AI Daily Brief is a daily podcast and
[00:00:30] video about the most important news and
[00:00:32] discussions in AI.
[00:00:34] Welcome back to the AI Daily Brief.
[00:00:36] Today's episode is about a bunch of
[00:00:38] patterns that are shifts, I think, in
[00:00:40] how on average we interact with AI on a
[00:00:44] daily basis. One thing that's been true
[00:00:46] since the very beginning of Chat GBT is
[00:00:48] that our patterns of interaction with AI
[00:00:50] have never been static for long. At the
[00:00:52] beginning, it was people discovering new
[00:00:54] ways to prompt the AI that had better or
[00:00:56] worse results, which was then
[00:00:57] communicated through hundreds of
[00:00:58] articles, posts, YouTube videos,
[00:01:00] podcasts, and courses. But over time,
[00:01:02] the interaction pattern shifts have
[00:01:04] gotten more significant and more
[00:01:05] substantive. Over the last week or so, I
[00:01:08] saw a number of announcements that
[00:01:09] really reinforce some fairly big shifts
[00:01:12] in these interaction patterns. And while
[00:01:14] I don't think that how we use AI will
[00:01:16] ever be truly static, I do think that
[00:01:18] some of these shifts, which I'm going to
[00:01:20] cover in this show, are fairly
[00:01:21] fundamental and likely to stick. And
[00:01:23] thus, of course, if one is trying to be
[00:01:24] efficient with their time, maybe more
[00:01:26] worthy of attention. So, first up is an
[00:01:29] interaction pattern that is not so much
[00:01:31] us changing how we interact with AI, but
[00:01:34] product design decisions that are
[00:01:36] shifting the options that we have to
[00:01:37] interact with AI. Very clearly there is
[00:01:40] a push towards simplification and
[00:01:41] integration and user experiences that
[00:01:44] have less rather than more cognitive
[00:01:46] decision-making for the end user. One
[00:01:48] thing that's been interesting for me
[00:01:49] sitting in this seat that I have is the
[00:01:51] extent to which early AI has tended to
[00:01:54] defy traditional Silicon Valley logic
[00:01:56] that users won't show up unless you give
[00:01:58] them an incredibly simple and clear
[00:02:00] experience. In fact, quite to the
[00:02:02] contrary of that, a lot of the early
[00:02:03] adopters, not just from tech circles,
[00:02:05] but from broader knowledge work circles,
[00:02:07] have, rather than resisting complexity,
[00:02:09] thrown themselves in head first. A great
[00:02:12] example of this for me was when 9,000
[00:02:14] people, most of whom weren't even close
[00:02:16] to engineers or really technical in any
[00:02:17] way, signed up for the free claw camp
[00:02:19] program I put out earlier this year,
[00:02:21] which basically had them crawling
[00:02:22] through glass to figure out how to build
[00:02:24] their own agents. And yet it appears
[00:02:26] that perhaps even if the portion of
[00:02:28] people who were willing to do that sort
[00:02:29] of hard work has been higher in AI than
[00:02:32] in other past tech sectors, there are
[00:02:34] still a lot of folks who want that
[00:02:35] simplicity. Certainly simplicity is one
[00:02:37] of the watchwords for the new MetaMuse
[00:02:39] product and something that even the
[00:02:41] power users who fully have the
[00:02:43] capability of dealing with complexity
[00:02:45] are lauding in the product. how II's
[00:02:48] Claire Vo has discussed in numerous
[00:02:50] places how well thought out she thinks
[00:02:52] the Muse design is specifically around
[00:02:54] what it does and doesn't obiscate from
[00:02:56] the user nojs creator Ryan Dah who again
[00:03:00] certainly has no shortage of complexity
[00:03:02] capability also shouted out Muse for
[00:03:04] having nailed the simplicity wrote
[00:03:06] technologist Tom Goodwin the beauty of
[00:03:08] Muse is that they've managed to
[00:03:09] introduce it in a very accessible way
[00:03:11] don't tell me how you work just show me
[00:03:13] how to do things David Herman wrote I
[00:03:15] think Muse is going to win in the casual
[00:03:17] AI race. I showed my dad who was nearly
[00:03:19] 70 and it clicked. He was amazed that I
[00:03:21] could have it create an entire contract
[00:03:23] for me, update things on it, then email
[00:03:25] and send it to a customer all through
[00:03:26] texts. Claude, OpenAI are great, but so
[00:03:29] far I'd say less than 1% of the
[00:03:31] population gets what these models are.
[00:03:33] Meta just made it all super easy. And
[00:03:35] it's clear that this was intentional.
[00:03:37] Meta Chief AI officer Alexander Wang
[00:03:39] wrote, "A big part of the team's focus
[00:03:41] when building Muse was to make something
[00:03:43] that just worked. So much work went into
[00:03:45] all the little details to make the
[00:03:46] product simple and easy to use. And of
[00:03:48] course, the thing that makes this a
[00:03:50] trend, not just a design decision from
[00:03:51] the meta team, is that this sort of
[00:03:53] simplification is showing up everywhere.
[00:03:55] One of the biggest product updates that
[00:03:57] we got this week came when Anthropic
[00:03:58] announced that Claude Co-work and chat
[00:04:00] are no longer separate things. Claude is
[00:04:03] careening towards an experience where
[00:04:04] instead of it being fragmented and full
[00:04:06] of decisions for the user before they
[00:04:07] even get started, instead a single
[00:04:09] unified experience. And again, the watch
[00:04:12] word was simplicity. simplification. And
[00:04:15] by the way, as pointed out by Claude
[00:04:16] code creator Cat Woo, this simplicity
[00:04:18] extends not only to eliminating the
[00:04:20] difference between co-work and chat, but
[00:04:22] also to integrating Claude design so
[00:04:24] that your standard core Claude also has
[00:04:27] all of the capabilities to do things
[00:04:29] like make slides, designs, docs without
[00:04:31] having to switch into some specialized
[00:04:33] experience. And again, the team at
[00:04:35] Anthropic reports that this was based on
[00:04:37] direct user feedback. Enthropic Labs
[00:04:39] lead and former Instagram co-founder
[00:04:41] Mike Kreger wrote, "The most common
[00:04:42] thing we hear, people aren't sure which
[00:04:44] product to start with. That friction
[00:04:46] gets in the way of getting the best from
[00:04:47] what these models can do." Now, as I
[00:04:49] mentioned in an earlier episode this
[00:04:50] week, I'm not totally sold on this on a
[00:04:52] personal level because I feel like I
[00:04:54] like having more specific control, but
[00:04:55] boy, do I seem out of sync with the
[00:04:57] average here. Christian Celig reposted
[00:04:59] the announcement and said, "Can we do
[00:05:01] this with Codeex 2, please? The two
[00:05:03] modes are like having two parents
[00:05:04] fighting." Shaunie Matthew summed up
[00:05:07] people don't want to interact with two
[00:05:08] to three text agents, two to three
[00:05:10] chatbot agents, two to three terminals
[00:05:11] on desktop. You want a simple unified
[00:05:14] interface, and want the agents to
[00:05:15] coordinate how it gets done. You simply
[00:05:17] want to ask and receive. The platform
[00:05:20] should coordinate and delegate agents,
[00:05:21] route models for tasks, handle whether
[00:05:23] it's local cloud or VM, be proactive and
[00:05:25] reactive about tasks. Instinct, Muse,
[00:05:28] and Grockbot really hit a nerve, and
[00:05:29] it's increasingly clear we're in another
[00:05:31] paradigm shift moment in my opinion. Now
[00:05:34] if the first change is about the
[00:05:35] simplicity of the interfaces through
[00:05:36] which we use AI, the second change is
[00:05:38] itself also a version of simplicity that
[00:05:41] has to do with how we control AI. And
[00:05:43] this is the trend towards mono threads.
[00:05:46] The idea of a mono thread is that
[00:05:48] instead of having to switch context
[00:05:50] windows and explain new needs and new
[00:05:52] prompts separate from the previous
[00:05:54] things that you've done, instead you use
[00:05:56] a single long continuously running
[00:05:58] thread that inherits the context from
[00:06:00] past conversations as a way to manage
[00:06:02] the entire experience. Now, previously
[00:06:04] this was limited by the context window.
[00:06:07] At some point, the AI would get tired,
[00:06:09] i.e. its context window would get filled
[00:06:11] and it would start doing weird things,
[00:06:12] making errors, losing instructions, etc.
[00:06:15] Many of the earlier courses and lessons
[00:06:16] that I did from late last year and early
[00:06:18] this year were all about how to build
[00:06:20] good handoff documents to move context
[00:06:22] between different threads. That started
[00:06:24] to shift this year though, especially as
[00:06:26] the team at Codeex really focused on
[00:06:28] compaction to change the way that people
[00:06:30] could interact specifically with codecs
[00:06:32] through a single unified thread. Codex's
[00:06:35] Nick Bowman wrote back in April, "So
[00:06:37] much coding agent design is built on the
[00:06:39] assumption that breaching context
[00:06:41] windows and compacting context yields
[00:06:43] progressively worse results. When you
[00:06:45] drop this assumption, the product
[00:06:47] direction it opens up is very exciting."
[00:06:49] He was responding to developer Anthony
[00:06:51] Kroger who had written, "I literally
[00:06:53] never worry about context windows using
[00:06:55] codecs. It can compact like three times
[00:06:57] and the model still remembers the
[00:06:58] details somehow." In a post about a week
[00:07:00] later, Nick from the Codex team expanded
[00:07:02] on his thoughts in a PC called my codeex
[00:07:04] threads are alive. In it, he wrote, "The
[00:07:07] most useful codeex thread I have right
[00:07:09] now is the one I've been using for the
[00:07:10] last 3 weeks. Every hour, it checks my
[00:07:12] Slack, Gmails, and PRs I wrote or I'm
[00:07:14] watching. Every hour, it turns the noise
[00:07:16] into clear signal I can act on. My
[00:07:19] codeex usage has shifted from starting
[00:07:20] lots of short-lived chats to keeping a
[00:07:22] smaller number of threads alive around
[00:07:24] recurring work streams. I still start
[00:07:26] fresh threads constantly, but some work
[00:07:28] should not reset every time I ask a
[00:07:30] question. In some, he writes, I have
[00:07:32] become mono thread pilled. Nick
[00:07:34] continues, I recently said that the
[00:07:36] compaction improvements made by the
[00:07:37] codeex team are opening up new product
[00:07:39] directions for coding agents. A lot of
[00:07:41] agent product design assumes long
[00:07:43] threads eventually degrade. If that is
[00:07:45] true, the product should push users
[00:07:46] towards creating new threads and writing
[00:07:48] context summaries. The codeex team has
[00:07:50] been doing a lot of work on compaction,
[00:07:51] and that work weakens the assumption.
[00:07:53] When a thread can stay useful across
[00:07:55] many turns, I want the same thread to
[00:07:57] keep working on the recurring task. Put
[00:07:59] simply, with good context compaction, a
[00:08:02] thread's value increases over time. Now,
[00:08:04] Nick wrote about that back in April, and
[00:08:06] I have very much found myself throughout
[00:08:07] the year seeing more and more of my
[00:08:09] behavior shift to that pattern.
[00:08:11] Everything that I do on the AI Daily
[00:08:13] Brief website, for example, is managed
[00:08:15] at the moment from a single clawed code
[00:08:17] thread. When I pop in to make a change
[00:08:19] or an update, I'm not starting that
[00:08:21] thread all over. I'm just jumping into
[00:08:22] where we left off. The social pipeline
[00:08:24] through which I use Claude to generate
[00:08:26] video clips from the show is another
[00:08:27] thread. And I've even found this
[00:08:29] behavior start to influence how I
[00:08:30] interact in other parts of Claude
[00:08:32] outside of just Claude code. Over the
[00:08:33] past couple of months, for example,
[00:08:35] inside projects, I find that when it's
[00:08:37] things that I do frequently, such as
[00:08:39] updating or writing new ad copy, instead
[00:08:41] of starting a fresh thread or
[00:08:42] conversation every time I need to do
[00:08:43] that task, I just jump in at the end of
[00:08:46] the last time I did a similar task.
[00:08:48] Well, it turns out I haven't been the
[00:08:50] only one who has started to shift their
[00:08:51] behavior in this way. In fact, this is
[00:08:54] now, as of this week, officially how
[00:08:56] Claude projects work. On Thursday, the
[00:08:58] Claude account posted, "Projects now run
[00:09:00] from one conversation starting in Claude
[00:09:02] Code. You describe what needs doing, and
[00:09:04] Claude directs parallel threads that
[00:09:06] keep working after you close your
[00:09:07] laptop." In other words, it's not that
[00:09:09] there aren't multiple threads, it's that
[00:09:11] those multiple threads are managed by
[00:09:13] Claude and what you do is interface with
[00:09:15] Claude through a single thread. This is
[00:09:17] very similar to the pattern that I had
[00:09:19] just described. And by the way, a week
[00:09:20] before this came to Claude, it had also
[00:09:22] come to cursor. In fact, when cursor
[00:09:24] introduced their version of projects, it
[00:09:26] had this logic built in. In their
[00:09:28] announcement, they write, "Rather than
[00:09:30] creating a chat for every task, you work
[00:09:32] with a coordinator agent in a single
[00:09:34] persistent thread." And the impacts of
[00:09:36] this shift are pretty big. Cloud code
[00:09:39] creator Boris Churnney wrote, "Projects
[00:09:41] have changed not only how I interact
[00:09:42] with Claude, but how I code. I stopped
[00:09:44] managing sessions. I just send thoughts
[00:09:46] as they come. Claude splits them into
[00:09:48] threads and the project remembers how I
[00:09:50] work. And this I think gets to a very
[00:09:52] related shift in how we work with AI,
[00:09:54] which is that chat bots are increasingly
[00:09:57] agent fleet managers. If you look at all
[00:09:59] of those examples that I just gave, what
[00:10:01] was changing was the place that we
[00:10:03] interact with a coordinator AI, but that
[00:10:05] coordinator AI was still spinning up
[00:10:07] lots of different sub aents to do
[00:10:09] different parts of the work. What's
[00:10:10] interesting about this to me is that I
[00:10:12] think for a while many of us would have
[00:10:14] assumed that the chatbot interface
[00:10:15] itself was perhaps an intermediate
[00:10:18] interface, something that was convenient
[00:10:20] and familiar for the time, but might
[00:10:21] give way to something else. What's
[00:10:23] interesting is that when you take the
[00:10:24] combination of mono threads and chat
[00:10:26] bots as agent fleet managers, what has
[00:10:28] happened is that instead of shifting
[00:10:29] away from chat bots, the model and
[00:10:31] harness companies have quietly shifted
[00:10:33] what chatbots actually are, but without
[00:10:35] pulling the interface rug out from under
[00:10:37] our feet. We still get that same
[00:10:39] comfortable experience of interacting
[00:10:40] with a chatbot. In fact, one that's even
[00:10:42] more simplified because we can do it
[00:10:44] from a single thread, but what that
[00:10:46] chatbot is doing is very, very different
[00:10:48] than what it was doing a year ago. Ethan
[00:10:50] Malik wrote, "What makes Claude project
[00:10:52] so interesting is that it handles teams
[00:10:54] of agents really well. You talk to a
[00:10:56] main orchestrator agent and it spins up
[00:10:58] specialists. Basically, it creates an
[00:11:00] organization to solve your issues,
[00:11:01] mixing expensive and cheap agents
[00:11:03] depending on your preferences. This
[00:11:04] also, by the way, has implications for
[00:11:06] the rest of our software services, which
[00:11:08] might increasingly start to look like
[00:11:10] context databases for our main
[00:11:12] coordinator agents. Signal wrote, "All
[00:11:14] of my iMes now run through a single
[00:11:16] agent interface. I still text, but I
[00:11:19] delete every email client from my phone
[00:11:20] and canceled every email subscription or
[00:11:22] app I had. Gmail is basically just a
[00:11:24] database to me now. Increasingly, so are
[00:11:26] the rest of Google services. I.e., I
[00:11:28] never want to manually write an email,
[00:11:30] create a doc, build slides, organize a
[00:11:31] calendar, or manage files again. I just
[00:11:33] want to express intent and have the
[00:11:35] underlying systems of record updated
[00:11:37] correctly. I think now you'll see apps
[00:11:39] disappear quickly. Many will become
[00:11:40] databases at best or entirely obsolete
[00:11:42] at worst. The agent will be the default
[00:11:44] interface to your personal and
[00:11:46] professional life. And even if that
[00:11:48] doesn't fully happen or if it takes a
[00:11:50] lot longer than someone as forward
[00:11:51] thinking as signal might think, it is
[00:11:52] certainly the case that the chatbots
[00:11:54] that you interact with are doing
[00:11:55] something different than they used to.
[00:11:57] And by the way, one simple but profound
[00:11:59] change which we've talked about a lot on
[00:12:00] this show is that the way that you're
[00:12:02] interacting with that chatbot is
[00:12:03] increasingly going to be through your
[00:12:04] voice. Every free learning program I've
[00:12:07] released this year starts by imploring
[00:12:09] people to either use native chat GPT
[00:12:11] voice control or to get something like
[00:12:12] whisper flow set up for the sheer
[00:12:14] efficiency and expanded context that
[00:12:16] voice is going to enable. And
[00:12:17] increasingly this is just table stakes
[00:12:19] for agent products as well. This week
[00:12:21] Grockbot joined the party with its own
[00:12:23] native voice integration. SpaceX AAI's
[00:12:25] Danny Graiosce wrote, "Using voice mode
[00:12:27] to rapidfire tasks to your chief of
[00:12:29] staff while it orchestrates your bot
[00:12:30] team feels like magic." Parker Conrad
[00:12:33] from that same team wrote, "Grockbot
[00:12:34] already took such a leap towards a more
[00:12:36] seamless interaction model. I'm bullish
[00:12:37] on voice taking that even further."
[00:12:39] Garav Bison pointed out that it's not
[00:12:42] just voice alone, but the fact that
[00:12:43] voice is now meeting expanded underlying
[00:12:45] capabilities. He wrote, "Tried voice on
[00:12:48] a bunch of agent products this year, and
[00:12:49] it always felt like a gimmick until the
[00:12:51] agent could actually go do things. Voice
[00:12:53] plus real work is the combo. And even
[00:12:56] the companies and projects that were
[00:12:57] already voice are getting even more so.
[00:12:59] OpenAI just released a new codeex ad
[00:13:01] with two of their team's developers
[00:13:03] talking to the voice agent in codecs
[00:13:04] powered by their new GPT live 1 model
[00:13:06] while they're working out. Google is
[00:13:09] also on the same tip, releasing Gemini
[00:13:11] 38 Live and 38 Live extended thinking
[00:13:13] this week, writing that major upgrades
[00:13:15] in intelligence and parallel reasoning
[00:13:17] make it more intuitive to collaborate
[00:13:18] and execute complex tasks using your
[00:13:20] voice. Last week, similar to the thing
[00:13:22] that Codex was advertising in that
[00:13:23] workout ad, we got Devon voice which
[00:13:25] allowed developers using Devon to also
[00:13:27] tap into the new GPT live model to code
[00:13:29] by talking. And Ali K Miller summed it
[00:13:31] up when she said, "Whenever I see a new
[00:13:33] voice first interface, a tiny voice
[00:13:35] inside of me screams with joy. Voice is
[00:13:37] the interface of the present and
[00:13:39] future." Now, alongside mono threads and
[00:13:42] more capable agent coordinators that
[00:13:43] manage their own fleets and voice-based
[00:13:46] instructions, the nature of the
[00:13:47] instructions that we give to our AI has
[00:13:49] also changed this year. Summarizing the
[00:13:52] big shift, instead of prompting our AIS,
[00:13:55] we increasingly set goals for them.
[00:13:57] Inherently, this creates more latitude
[00:13:59] and agency on the part of the AIS for
[00:14:01] figuring out how that work should get
[00:14:03] done and for working in recurring loops
[00:14:05] until that work gets done. This started
[00:14:08] with the introduction of primitives like
[00:14:09] /goal and claude code and codecs. It was
[00:14:12] a formalization of this interaction
[00:14:13] pattern that allowed people to specify
[00:14:16] goals instead of just dropping a prompt.
[00:14:18] This would later expand to the whole
[00:14:20] idea of loop engineering, which is
[00:14:21] something we've talked about throughout
[00:14:22] the summer and even did a webinar on
[00:14:23] about a month ago. The idea of loops
[00:14:25] really got a big lift when open clock
[00:14:27] creator Peter Steinberger wrote, "You
[00:14:29] shouldn't be prompting coding agents
[00:14:31] anymore. You should be designing loops
[00:14:32] that prompt your agents." This idea of a
[00:14:34] loop is simply that in addition to
[00:14:36] defining the goal, you define success
[00:14:38] criteria for the goal that the agent can
[00:14:40] measure itself against so that it can
[00:14:42] run in a continuous loop until it
[00:14:44] achieves said goal based on the
[00:14:45] quantifiable criteria given. And the
[00:14:48] thing is, and the reason that it's worth
[00:14:49] mentioning in this show is that although
[00:14:51] loops and loop engineering has all of
[00:14:53] the hallmarks of the type of buzzy terms
[00:14:54] that we love over in our early adopter
[00:14:56] circles, but which reasonably elicit eye
[00:14:58] rolls among the rest, this is actually a
[00:15:01] fairly critical mindset shift when it
[00:15:03] comes to thinking about how to get the
[00:15:05] most out of our interactions with AI,
[00:15:07] which is why we spend so much time on it
[00:15:08] here. The sixth change in how we
[00:15:10] interact with AI is, I guess you might
[00:15:13] call multimodelity,
[00:15:15] i.e. the using of multiple different
[00:15:17] models in a personal stack, not just on
[00:15:19] an organizational level, but even within
[00:15:21] the domain of an individual user's work.
[00:15:23] I have not yet settled on the exact
[00:15:25] right language to describe this
[00:15:26] multimodality, as a number of my
[00:15:28] patreons love to point out. But while on
[00:15:30] the one hand, many advanced AI users
[00:15:32] have always viewed model selection as a
[00:15:34] way to get benefits. In other words, not
[00:15:36] just being constrained to a single model
[00:15:38] because that's the one you pay for a
[00:15:39] subscription for, but finding the model
[00:15:41] that does the best with your particular
[00:15:42] task. The difference now is that the
[00:15:44] complexity, difficulty, depth, and
[00:15:46] duration of the work combined with the
[00:15:48] cost of the most advanced models and
[00:15:50] shifts in the subsidy of those models in
[00:15:51] the standard plans means that this is
[00:15:53] not just an early adopter alpha thing
[00:15:55] anymore, but basically a cost and
[00:15:56] efficiency requirement. Now, it's also
[00:15:59] enabled by the fact that the more time
[00:16:01] that goes on, the more that cheaper
[00:16:02] models that are just outside the
[00:16:04] state-of-the-art can do things that
[00:16:05] would have been state-of-the-art just a
[00:16:07] couple of months ago. You saw this a lot
[00:16:09] when Fable 5.1 dropped. You had people
[00:16:11] all over X and the other AI communities
[00:16:13] sharing their hacks on how to get the
[00:16:14] most out of the model without breaking
[00:16:16] the bank. And increasingly, you can see
[00:16:17] this moving from expost hacks to actual
[00:16:20] usage systems discipline. And this
[00:16:22] interaction pattern shift dubtales very
[00:16:24] closely with the idea of chatbots as
[00:16:26] agent fleet managers. One of the things
[00:16:28] that a lot of folks have noticed is that
[00:16:30] at least at current, the default for a
[00:16:32] model like Fable 5.1 is to not just use
[00:16:35] the most advanced model as the
[00:16:37] coordinator, but also to use it for all
[00:16:38] the sub aents. Many of us have had the
[00:16:41] experience where we give Fable what we
[00:16:42] think is a fairly standard task only to
[00:16:45] come back and see a major percentage of
[00:16:46] our current usage cap tapped because it
[00:16:48] turns out that the five or 10 sub aents
[00:16:50] that had spun up to go do some sort of
[00:16:51] research were all using the most
[00:16:53] advanced Fable model as well even though
[00:16:54] that was completely not required for the
[00:16:56] task at hand. TLDDR understanding where
[00:16:59] different types of models and model
[00:17:00] capabilities are needed and how to
[00:17:02] normalize that in your management of
[00:17:03] your AI is going to increasingly be an
[00:17:06] important discipline. And by the way,
[00:17:08] this is one trend that if not careful
[00:17:10] could kind of run at odds with that
[00:17:12] trend towards simplicity. As all of the
[00:17:14] model and harness labs try to make the
[00:17:16] average experience more simple. In many
[00:17:19] cases that will mean obscuring or even
[00:17:20] doing away with the more fine grain
[00:17:22] controls for determining things like
[00:17:24] which tasks get which model. Now
[00:17:26] theoretically the labs and model
[00:17:28] companies will try to build automated
[00:17:29] systems underneath that can figure out
[00:17:31] those specifics for you. I.e. to realize
[00:17:33] that the sub aents needed for a research
[00:17:35] task are not state-of-the-art, but I'm
[00:17:37] not sure that they're always going to
[00:17:38] get it right. And so, I think that this
[00:17:40] will still be something that people need
[00:17:41] personal agency around. The last
[00:17:43] interaction pattern shift is one that
[00:17:45] I've talked about a lot recently, so I
[00:17:46] won't go too deep on, but is the idea of
[00:17:48] shared agents. 2026 will be looked back
[00:17:51] at as the year that agents became real
[00:17:53] after years and years of excitement. But
[00:17:55] for the first twothirds of the year,
[00:17:57] almost all of that agent behavior was
[00:17:58] siloed to individuals. It was each of us
[00:18:01] individually building our open claw
[00:18:03] teams, changing how we do work, but not
[00:18:05] necessarily changing how our teams do
[00:18:07] work overall. You're starting to see
[00:18:09] that shift. An example of that came this
[00:18:11] summer when Claude introduced Claude
[00:18:12] tag, which replaced the old system of
[00:18:14] Claude and Slack, where each individual
[00:18:16] could call upon their own Claude
[00:18:18] instance with a new team-based system
[00:18:20] where each channel had its own Slack
[00:18:22] that could work across the context of
[00:18:24] that channel, not tied to any one
[00:18:26] individual. Now, the idea here is pretty
[00:18:28] clear. Some amount of our work gets
[00:18:30] done, yes, as individuals, but a lot of
[00:18:32] it gets done in teams. And we're
[00:18:33] probably going to need agents that live
[00:18:35] at the intersection of our teams, not
[00:18:36] just agents that live in our own little
[00:18:38] individual worlds. And you're now
[00:18:40] starting to see tons of efforts towards
[00:18:42] these ends. Mo XYZ launched this week as
[00:18:45] the quote, "First AI employee your whole
[00:18:47] team shares." In their announcement
[00:18:49] post, they wrote, "In beta since July,
[00:18:51] Mio saved teams thousands of hours and
[00:18:53] completed tens of thousands of tasks.
[00:18:55] You don't need another agent. You need a
[00:18:57] shared one with your team. On any given
[00:18:59] day, I feel like I see a half dozen or
[00:19:01] more examples of this same impulse.
[00:19:02] Although exactly what multiplayer AI
[00:19:05] means, is still very much in
[00:19:07] development. Earlier this month, Ethan
[00:19:09] Malik wrote, "Multiplayer AI, where many
[00:19:11] people in an organization can use AI
[00:19:13] together to accomplish goals, remains
[00:19:14] one of the biggest non-technical
[00:19:16] problems in using AI right now.
[00:19:18] Approaches tend to be pretty primitive
[00:19:19] and based around AI as a person in your
[00:19:21] group chat. That is limiting." Arya
[00:19:24] Bhani writes, "We still don't have a
[00:19:26] consistent mental model for who the
[00:19:27] principle is in a multiplayer agentic
[00:19:29] system. Is it you, the user? Agent is
[00:19:32] your proxy inheriting your context,
[00:19:34] access, and authority. Is it the agent
[00:19:36] itself? Agent has its own identity,
[00:19:38] relationships, memory, and access?" It's
[00:19:40] the difference, Arya continues, between
[00:19:42] agent civilizations versus human
[00:19:43] civilizations at agent speed.
[00:19:45] Realistically, the answer is both, but
[00:19:47] for different systems and use cases.
[00:19:50] Atlan's Rishiar of Batnagar writes,
[00:19:51] "Multiplayer AI will be one of the
[00:19:53] biggest design problems of 2027. The
[00:19:56] phrase alone means something different
[00:19:57] to every person I talk to. Is it shared
[00:19:59] memory, context, org design, or
[00:20:01] something else entirely?" And what's
[00:20:03] interesting is that Rishi then goes on
[00:20:04] to show why each of these sounds
[00:20:06] compelling when you look at it in
[00:20:07] isolation. The memory lens, he writes,
[00:20:10] five agents on one project, five
[00:20:12] different versions of what happened,
[00:20:13] none of them talking to each other. It's
[00:20:14] a mess. Fixing it, one shared memory
[00:20:16] instead of five private copies is the
[00:20:18] whole game. But then there's the context
[00:20:20] lens. Rishi continues, "Nearly everyone
[00:20:22] I talk to has built their own little
[00:20:24] context layer for their own agents. It
[00:20:26] works for them. Stretch it across the
[00:20:28] whole team and it falls apart. Personal
[00:20:30] context feels solved or wide is wide
[00:20:32] open." And then of course there's the
[00:20:33] organizational change dimension. Rishi
[00:20:36] concludes the hardest part of
[00:20:37] multiplayer AI might not be technical at
[00:20:39] all. Getting a whole team to adopt one
[00:20:41] shared way of working is more org than
[00:20:43] engineering. Nobody wants that to be
[00:20:45] true. What's clear is that there is
[00:20:48] going to be a ton of work done in this
[00:20:49] area. Josh Rosen writes, "We've decided
[00:20:52] AI is going multiplayer before we've
[00:20:54] agreed on the architectural patterns for
[00:20:55] multiplayer AI, but then of course
[00:20:57] proceeds by trying to explain all of
[00:20:59] that and get us to a slightly more
[00:21:01] coherent answer. Now, if this is
[00:21:03] something that you are interested in, I
[00:21:04] will show for a moment the latest free
[00:21:06] self-directed training program that
[00:21:07] we've dropped here, which is the
[00:21:09] multiplayer AI sprint for teams. This
[00:21:11] does not assume that multiplayer AI is
[00:21:13] figured out or frankly almost any of the
[00:21:15] answers to those important questions.
[00:21:18] What the sprint does is it gets people
[00:21:20] to start to build the foundations to how
[00:21:23] multiplayer AI, which is really just
[00:21:25] another way in our case of saying shared
[00:21:26] agents can function inside your team.
[00:21:29] Over the course of the four sprints,
[00:21:31] which we've divided into weeks, but
[00:21:32] don't have to be split up that way,
[00:21:34] you're going to inventory first what
[00:21:35] your team is actually running right now
[00:21:37] for AI and or to the extent that you are
[00:21:39] even more new. Perhaps bring in some
[00:21:41] champion or export from your
[00:21:42] organization who is a little bit farther
[00:21:43] in their stack to help you understand
[00:21:45] best practices in your specific
[00:21:46] organizational context. And once you
[00:21:48] have that sort of inventory, you move
[00:21:50] then into sprint two, which is all about
[00:21:52] context, writing down what your AI knows
[00:21:54] about you and what it should know about
[00:21:55] you. Sprint 3 is looking at the overlap
[00:21:58] in work streams and in context, which is
[00:22:00] going to give you your possible places
[00:22:01] to build shared agents. And sprint four
[00:22:04] is going to be where you actually do
[00:22:05] that building. And of course, you can
[00:22:06] then repeat sprint 3 and sprint 4
[00:22:08] multiple times to experiment with
[00:22:09] multiple agents as much as it helps.
[00:22:11] There are going to be tons and tons of
[00:22:13] product experiences and great product
[00:22:15] thinking coming to the multiplayer AI or
[00:22:17] shared agent space in very short order.
[00:22:19] And so to the extent you want to kick
[00:22:21] that can down the road just a little bit
[00:22:22] and let the industry and norm settle a
[00:22:24] bit more, I totally understand.
[00:22:26] That said, I do think for teams who want
[00:22:27] to dive in, there is certainly some
[00:22:29] alpha to be had by getting out ahead of
[00:22:31] that. And hopefully that's what the
[00:22:32] multiplayer AI sprint, which is of
[00:22:33] course linked in the show notes, can
[00:22:35] maybe help you do. So that is the seven
[00:22:38] ways that how we use AI is changing.
[00:22:40] Hopefully this gives you some
[00:22:41] interesting new directions to explore
[00:22:43] and some new ways to think about your
[00:22:45] relationship with AI. For now, that's
[00:22:47] going to do it for today's AI daily
[00:22:48] brief. I appreciate you listening or
[00:22:50] watching as always and until next time,
[00:22:52] peace.
