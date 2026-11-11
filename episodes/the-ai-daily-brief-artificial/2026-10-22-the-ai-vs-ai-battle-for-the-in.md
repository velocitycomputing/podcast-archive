---
record_id: "podcast:44fe79f9-97de-4f25-b316-3a63cd300189"
episode_id: 44fe79f9-97de-4f25-b316-3a63cd300189
title: The AI vs AI Battle for the Internet
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/the-ai-vs-ai-battle-for-the-internet/44fe79f9-97de-4f25-b316-3a63cd300189"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/the-ai-vs-ai-battle-for-the-internet/44fe79f9-97de-4f25-b316-3a63cd300189"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-22
played_at: "2026-10-22T12:00:00Z"
play_count: 1
duration_seconds: 1680
source: pocketcasts-history-browser
played_label: October 22
history_order: 38
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 2f00f7b9b3279308a6d04c2f9fe63eaf386822ca568d18423ad0f33445ae15f2
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

Anthropic’s Claude Duet entered the personal-agent market alongside Meta Muse, OpenAI’s dots, and Grokbot/SpaceX bots, emphasizing proactive morning briefs, persistent memory, a virtual machine, connectors, safety classifiers, explicit permission for major actions, and a work/professional focus built on Opus 5.5, with commentators including Dan McCarty, Chubby, and Signal framing the competition as a race to own the user relationship rather than merely the smartest model; Walmart also opened its platform to third-party personal agents with linked accounts, configurable spending limits, default purchase approvals, payment-method restrictions, and returns coverage for compliant agents, while citing its own Sparky agent’s 40% higher order values and Meta’s disclosure that one-quarter of active Muse users shop through the agent with a $200 average purchase value; Meta separately announced a new non-voting stock class to fund AI infrastructure, raising its data-center budget to $135–145 billion, with CFO Susan Li citing AI-driven investment needs and Molus suggesting Meta may need several hundred billion dollars in future capital; the episode also covered a KPMG/University of Texas at Austin study of more than 500 early-career professionals finding that top “AI amplifiers” succeed by guiding, evaluating, and refining AI outputs, and it centered on a major cybersecurity escalation involving Anthropic’s Project Glasswing and Mythos/Fable, the Hugging Face incident, the Open Code attack, a PHP vulnerability called PHP-2-Shell affecting roughly 70% of websites and web apps, discovery by GPT-5.6 Soul at Califf and independently by Wiz, NSA and FBI warnings, Cloudflare CEO Matthew Prince’s report of exploit attempts rising from thousands to millions, and commentary from Volker Dusch, Cameron Wilson, Brecht Units, Mike Shelby, Charles Read, Nick Dobos, Ethan Mollick, Paras Chopra, Peter Levels, Anthony Ronning, Tay Monahan, Christian the Pahl, Frederick Williams, Kenny Lauderdale, The International Cyber Digest, Joshua Achiam, John Ennis, and Box’s Aaron Levie, alongside Railway’s environment-variable/API-key breach and Open Code’s Dax warning that attackers will increasingly use agents against every system surface.

No direct health implications are stated; the actionable consequences are digital-security, AI-adoption, and capital-allocation decisions: if you operate any PHP-based site, web app, server, or legacy web stack, patch immediately, assume possible compromise if unpatched, rotate API keys and environment variables, review logs for unauthorized access, and prepare for repeated emergency patching cycles; if you use personal agents, treat them as privileged accounts by using linked accounts with spending caps, default purchase approvals, restricted payment-method access, connector audits, and clear rules against unintended actions, especially for agentic commerce; organizations should move beyond low-value AI use such as meeting summaries, track where AI creates measurable business value, train employees to guide, evaluate, and refine AI outputs, and budget for agent-driven cybersecurity that scans code, logs, traffic, identities, devices, and infrastructure at scale; research leads include the disclosure strategy around PHP-2-Shell, whether patches should be released before explanations, the long-term viability of personal agents as a product form factor, the legal and commercial template emerging from Walmart’s agent terms, Meta’s non-voting stock and AI-infrastructure funding model, and whether enterprise cybersecurity becomes one of AI’s largest investment and hiring categories; follow-up questions to consider are: Are our systems PHP or dependent on PHP? Have all API keys, secrets, and environment variables been rotated? Do we have agent-use policies, spending limits, and incident-response playbooks? Are employees using AI for high-value work or only summaries? Are we monitoring for AI-agent-driven attacks and defending with AI agents?

## Transcript

[00:00:00] Yesterday, Anthropic announced Claude
[00:00:01] Duet, their answer to Grokbot, and Meta
[00:00:04] Muse, and OpenAI's dots. And yet,
[00:00:06] somehow, Duet is not the focus of our
[00:00:08] main episode. How could that possibly
[00:00:10] be? Well, in short, it's because that
[00:00:12] right now we are living through what may
[00:00:13] ultimately be seen as a key transitional
[00:00:16] moment between two very different eras
[00:00:18] of cybersecurity. One where long-term
[00:00:20] norms held, and even exploits and
[00:00:22] challenges were manageable, and the
[00:00:24] other, newer era, where it's AI versus
[00:00:26] AI, and a battle for who can coordinate
[00:00:28] best.
[00:00:29] The AI Daily Brief is a daily podcast
[00:00:31] and video about the most important news
[00:00:33] and discussions in AI.
[00:00:35] All right, friends. Quick announcements
[00:00:37] before we dive in. First of all, thank
[00:00:39] you to today's sponsors, KPMG, Section,
[00:00:41] C data, and Blitzcy. To get an ad-free
[00:00:44] version of the show, go to
[00:00:44] patreon.com/aidailybrief,
[00:00:46] or you can subscribe on Apple Podcasts.
[00:00:48] And if you want to learn more about
[00:00:49] sponsoring the show, send us a note at
[00:00:51] sponsors@aidailybrief.ai.
[00:00:54] And we kick off today with a story that
[00:00:56] on almost any day on this show would
[00:00:58] absolutely be the main, and in fact,
[00:01:00] would usually be a main-only type
[00:01:02] episode. Anthropic has joined the
[00:01:04] personal agent market with their own
[00:01:06] twist on Muse/dots/grokbot,
[00:01:09] and they're calling it Claude Duet. The
[00:01:11] two reasons that today for us it's just
[00:01:13] a brief headline introduction are that
[00:01:15] one, the massive slate of cyber issues
[00:01:17] going around the internet right now are
[00:01:19] fairly unignorable, both in the
[00:01:21] specifics, but also what they allude to
[00:01:22] for the future. And secondly, I'm
[00:01:24] working on a full-length long read
[00:01:26] Sunday episode, which is going to go
[00:01:27] much deeper into Claude Duet, and
[00:01:29] exactly how I'm using it and its
[00:01:31] competitors, and what I'm finding so
[00:01:33] far. So, come back on Sunday to check
[00:01:35] that out. For now, it appears that
[00:01:37] Anthropic is, perhaps unsurprisingly,
[00:01:40] aiming at the professional and small
[00:01:42] business side of the personal agent
[00:01:43] market, with their main differentiator
[00:01:45] seeming to be a focus on being
[00:01:46] proactive. Describing the core
[00:01:48] functionality, they wrote, "Each
[00:01:50] morning, Duet sends you a short brief on
[00:01:51] the most important items across your
[00:01:53] connected apps. Throughout the day, it
[00:01:54] keeps tabs on those apps, and messages
[00:01:56] you only when something needs your
[00:01:57] attention. You can also hand it tasks of
[00:01:59] all shapes, from simple administrative
[00:02:01] tasks of scheduling meetings to more
[00:02:03] complex ones such as building dashboards
[00:02:05] with dozens of tools, creating financial
[00:02:07] or sales forecasts, prototyping and
[00:02:09] building web apps. Besides the proactive
[00:02:11] approach, Claude Duet has all of the
[00:02:13] features that people have come to expect
[00:02:14] from the current crop of agents. Duet
[00:02:16] has its virtual machine, persistent
[00:02:18] memory, and a full suite of connectors,
[00:02:20] and Anthropic also emphasized the focus
[00:02:21] on safety. Duet will ask for explicit
[00:02:24] permission before taking major actions
[00:02:25] like making a payment or deleting files.
[00:02:28] Anthropic has also created what they
[00:02:29] call a new dedicated classifier and
[00:02:31] safety system prompt that checks each
[00:02:33] message and guards against leaks of
[00:02:34] sensitive information. Right now, Duet
[00:02:36] is being rolled out as a research
[00:02:38] preview, and you can't just decide to
[00:02:39] use it. You have to get on a waitlist.
[00:02:41] Anthropic warned that this is an early
[00:02:43] version, which might have some issues
[00:02:45] like misreading threads or
[00:02:46] miscalibrating what's urgent. And they
[00:02:48] also warned that it won't be as capable
[00:02:49] at personal errands like booking tickets
[00:02:51] as other agents because of the extent to
[00:02:53] which their focus is on work tasks.
[00:02:55] In general, the community treated this
[00:02:56] with excitement, if not surprise. And
[00:02:59] for many, as summed up by Dan McCarty,
[00:03:01] the big and immediate differentiator
[00:03:02] wasn't anything about the proactivity or
[00:03:05] even necessarily its focus on work
[00:03:07] tasks. It was the fact that it was built
[00:03:09] on Opus 5.5. There were a few folks like
[00:03:12] Chubby, who were surprised to see
[00:03:14] Anthropic pursuing a personal agent. He
[00:03:17] basically said that he wasn't sure who
[00:03:18] the target was for this, but I think
[00:03:20] that that might be a category error in
[00:03:22] thinking that personal agents are just
[00:03:24] going to be for personal uses. It seems
[00:03:26] to me that there is a bit of a
[00:03:28] recognition that even though we have
[00:03:29] work and personal lives, the boundaries
[00:03:32] of those things are fairly permeable.
[00:03:33] And when it comes to these so-called
[00:03:35] personal agents, right now it seems like
[00:03:36] the labs are betting that while we might
[00:03:38] gravitate towards one that has our
[00:03:40] particular use cases emphasized, they
[00:03:42] just have to be able to do everything
[00:03:43] that we might want them to do. Signal
[00:03:45] summed it up this way. Pretty much every
[00:03:47] major AI company now has a personal
[00:03:48] agent product except Google. Meta has
[00:03:50] Muse, Anthropic Duet, OpenAI.dot, SpaceX
[00:03:53] bots. Slowly but surely the competition
[00:03:55] is shifting from who has the smartest
[00:03:57] model to who owns the persistent
[00:03:59] relationship with the user. This will be
[00:04:01] even more the case going forward. You're
[00:04:02] seeing this because we likely reached
[00:04:04] peak intelligence required to power most
[00:04:06] of the world's workflows probably
[00:04:07] earlier this year if not late last year.
[00:04:09] Mostly I think the discussion shows just
[00:04:12] how nascent this product category
[00:04:14] remains. There is nothing even
[00:04:16] approaching consensus on whether these
[00:04:18] things are the right form factor or what
[00:04:20] their most important modes of
[00:04:21] interactions are or what even the
[00:04:23] essential features are. People disagree
[00:04:25] around whether we'll have one or many
[00:04:27] and what the most important distinguish
[00:04:28] will be.
[00:04:29] I know that subsequent to my time using
[00:04:31] these personal agents so far, I'm not
[00:04:33] 100% convinced that they're going to
[00:04:35] ultimately be an essential part of the
[00:04:37] portfolio. But like I said, I'm going to
[00:04:38] get a lot deeper into that on Sunday.
[00:04:40] And I guess the last note on Duet for
[00:04:42] those who are keeping track, if I were a
[00:04:44] betting man, I think this is part one of
[00:04:46] a one-two punch heading into the IPO. At
[00:04:48] least from a product perspective for
[00:04:50] Anthropic, release your answer to all
[00:04:51] the personal agents floating around and
[00:04:53] then give it a new model which makes
[00:04:55] everyone feel just so far behind. In
[00:04:57] other words, maybe this is just prelude
[00:04:59] to Fable 55. Next up, staying on the
[00:05:02] theme of agents, contra to some other
[00:05:04] businesses out there, Walmart has
[00:05:05] decided to welcome personal agents onto
[00:05:07] their platform. Recent weeks have seen
[00:05:09] corporate America divided on the risks
[00:05:11] of personal agents interacting with
[00:05:13] services on their owners' behalves.
[00:05:15] Shopify was of course an emphatic yes,
[00:05:17] while Amazon, JP Morgan, and Bank of
[00:05:19] America were a clear no. It should be
[00:05:21] noted that the reason for the no is
[00:05:22] between those companies was a little bit
[00:05:24] different. JP Morgan and Bank of America
[00:05:26] are thinking about risk in terms of
[00:05:28] agents doing something with people's
[00:05:29] money that they shouldn't, while Amazon
[00:05:31] is focused more on competitive risk. In
[00:05:33] that light, Walmart allowing third-party
[00:05:35] agents is kind of a surprising move. The
[00:05:38] retail giant was very early to AI
[00:05:40] adoption and one of the core pillars of
[00:05:42] their strategy was Sparky, their
[00:05:44] proprietary shopping agent. Earlier this
[00:05:46] month, Walmart said customers who used
[00:05:48] Sparky had order values 40% higher than
[00:05:51] non-agentic online shoppers. Still, it
[00:05:53] seems now that Walmart wants to
[00:05:54] encourage agentic commerce, and they
[00:05:56] don't particularly care which agents
[00:05:57] their customers are using. As of next
[00:05:59] month, customers will be able to set up
[00:06:00] a linked account for their personal
[00:06:02] agent with configurable spending limits,
[00:06:04] kind of similar to how a child's account
[00:06:05] might work. Aside from supporting
[00:06:07] third-party agents, Walmart's new policy
[00:06:09] included lengthy terms and conditions
[00:06:11] that could become a template for safer
[00:06:13] agentic shopping. Walmart included rules
[00:06:15] that an agent must not take actions
[00:06:17] beyond what the shopper intended, and
[00:06:18] that agents can't modify a customer's
[00:06:20] payment methods. Walmart will require
[00:06:22] purchases to be approved by default, and
[00:06:24] said they would ban agents that don't
[00:06:26] comply with their guidelines. However,
[00:06:28] for compliant agents, Walmart said
[00:06:30] agentic purchases would have access to
[00:06:31] the returns policy even if an agent
[00:06:33] makes a mistake. Once again, we find
[00:06:35] ourselves in incredibly early days for
[00:06:37] agentic commerce, and I think trying to
[00:06:39] make definitive statements now about how
[00:06:41] this is going to play out is very hard
[00:06:43] if not impossible. Still, early evidence
[00:06:46] suggests that for those who are using
[00:06:47] personal agents, agentic commerce does
[00:06:50] seem to be an early use case that people
[00:06:51] are exploring. During Wednesday night's
[00:06:53] earnings call, Meta said that 1/4 of
[00:06:55] active Muse users are using the agent
[00:06:57] for shopping. The average value of their
[00:06:59] purchases is $200, which surprised even
[00:07:02] the e-commerce veterans who have been
[00:07:04] paying attention to the space. Mark
[00:07:05] Zuckerberg commented, "Plaid told us
[00:07:08] that they hadn't seen activity like
[00:07:09] they're seeing with their connector on
[00:07:10] any other service before." In that
[00:07:12] light, Walmart's strategy begins to look
[00:07:14] a little bit clearer. If the early
[00:07:15] adopters of agentic shopping are very
[00:07:17] valuable customers, Walmart just wants
[00:07:19] to let them shop. Speaking of Meta, the
[00:07:21] company has announced a new class of
[00:07:23] non-voting stock to help fund the next
[00:07:25] leg of their AI buildout. The
[00:07:26] announcement came alongside those same
[00:07:28] third-quarter earnings, which featured a
[00:07:30] very minor upwards revision to their
[00:07:31] data center budget. Meta now expects to
[00:07:33] spend between 135 billion and 145
[00:07:36] billion this year, adjusting the low end
[00:07:38] up from 130 billion. The new stock will
[00:07:41] begin trading in January,
[00:07:42] and allows Meta to raise funds by
[00:07:44] selling equity without diluting Mark
[00:07:46] Zuckerberg's voting control of the
[00:07:47] company.
[00:07:48] CFO Susan Li wrote in the earnings
[00:07:50] report, "The scale of investment
[00:07:51] required to compete, sustain growth,
[00:07:53] expand infrastructure, and pursue new
[00:07:55] strategic initiatives amidst the AI
[00:07:56] transformation taking place in the
[00:07:58] industry is significant." During the
[00:08:00] earnings call, Li added that the new
[00:08:01] class of stock will, quote, "expand our
[00:08:03] funding tools and give us flexibility to
[00:08:05] invest behind the unprecedented momentum
[00:08:07] we're seeing across every part of our
[00:08:08] business driven by AI." There are a few
[00:08:11] reasons why Meta would pivot to funding
[00:08:12] their data center buildout with equity
[00:08:14] rather than debt. Some thought that this
[00:08:16] was a sign that the bond market is
[00:08:17] completely tapped out on AI debt. But,
[00:08:19] of course, it also might be that Meta
[00:08:21] sees that as a possibility moving
[00:08:22] forward rather than a current state
[00:08:24] condition and wants to hedge against it.
[00:08:26] Others noted that Meta has 900 billion
[00:08:28] in liabilities, including 350 billion in
[00:08:31] non-cancelable data center contracts.
[00:08:33] That's a rough gauge of spending over
[00:08:34] the coming decade, but only about 83
[00:08:36] billion of that total is currently on
[00:08:38] issued long-term bonds. Perhaps the
[00:08:40] scale of the buildout suggests they
[00:08:41] won't be able to fund it all with that.
[00:08:43] Now, ultimately, the Occam's razor
[00:08:45] answer, or I guess the generous read
[00:08:47] depending on your position on
[00:08:48] Zuckerberg, is that Meta is tapping all
[00:08:50] available pools of capital and keeping
[00:08:52] their options open. Issuing stock is a
[00:08:54] deep pool of capital as long as Meta
[00:08:57] isn't too concerned about diluting
[00:08:58] existing shareholders. Financial
[00:09:00] planning advice from Molus, which was
[00:09:01] attached to the earnings report, said
[00:09:03] Meta would need to raise several hundred
[00:09:04] billion dollars over the coming years in
[00:09:06] any scenario. They noted that if they
[00:09:07] did issue voting stock, they could still
[00:09:10] raise as much as 700 billion without
[00:09:11] diluting Mark Zuckerberg's vote below
[00:09:13] 50%. Interestingly, Meta stock was up in
[00:09:16] overnight markets, suggesting
[00:09:17] shareholders are willing to deal with
[00:09:18] some dilution for now. What this means
[00:09:20] for the stage of the buildout remains to
[00:09:22] be seen, but it is another important
[00:09:23] signal. The current plan, barring some
[00:09:25] crazy thing happening on Friday, is a
[00:09:27] much deeper dive into what I think are
[00:09:29] the actual most concerning bubble
[00:09:31] signals. So, if you're interested in
[00:09:32] that, come back tomorrow. For now,
[00:09:34] though, that is going to do it for
[00:09:35] today's headlines. Next up, the main
[00:09:37] episode.
[00:09:39] A new study from KPMG in the University
[00:09:41] of Texas at Austin found that when
[00:09:43] people work with AI, similar skills
[00:09:45] don't guarantee similar outcomes.
[00:09:47] Researchers studied more than 500 early
[00:09:49] career professionals and found that the
[00:09:51] best performers consistently amplified
[00:09:53] the value of AI by guiding, evaluating,
[00:09:56] and refining its outputs. These top
[00:09:58] performers, called AI amplifiers,
[00:10:00] weren't defined by what they knew alone,
[00:10:02] but by how they worked with AI. Learn
[00:10:05] more about what separates AI amplifiers
[00:10:07] from everyone else at
[00:10:08] kpmg.com/us/aiamplifiers.
[00:10:14] Here's a harsh truth. Your company is
[00:10:16] probably spending thousands or millions
[00:10:18] of dollars on AI tools that are being
[00:10:19] massively underutilized. Half of
[00:10:22] companies have AI tools, but only 12%
[00:10:24] use them for business value. Most
[00:10:25] employees are still using AI to
[00:10:27] summarize meeting notes. If you're the
[00:10:28] one responsible for AI adoption at your
[00:10:30] company, you need Section.
[00:10:32] Section is a platform that helps you
[00:10:33] manage AI transformation across your
[00:10:35] entire organization. It coaches
[00:10:37] employees on real use cases, tracks
[00:10:39] who's using AI for business impact, and
[00:10:41] shows you exactly where AI is and isn't
[00:10:43] creating value. The result? You go from
[00:10:45] rolling out tools to driving measurable
[00:10:47] AI value. Your employees move from
[00:10:49] meeting summaries to solving actual
[00:10:51] business problems, and you can prove the
[00:10:53] ROI. Stop guessing if your AI investment
[00:10:55] is working. Check out Section at
[00:10:57] sectionai.com.
[00:10:59] That's s e c t i o n a i dot com.
[00:11:03] This episode is brought to you by CData.
[00:11:06] Companies rolling out AI keep hitting
[00:11:07] the same wall. Token spend is climbing,
[00:11:10] security is holding agents back, and no
[00:11:12] one knows how AI is truly being used.
[00:11:15] The root cause? AI is cut off from the
[00:11:17] systems and context your business runs
[00:11:19] on. That's why CData built Connect AI
[00:11:22] Gateway. One control point between your
[00:11:24] AI and your systems. Built on the
[00:11:26] connectivity layer powering Palantir,
[00:11:28] Google, Salesforce, and hundreds more,
[00:11:30] each agent gets exactly the data and
[00:11:32] tools it needs. It governs down to the
[00:11:34] record and lets you finally see your
[00:11:36] org's complete AI usage in one place.
[00:11:38] Accurate answers, a fraction of the
[00:11:40] token cost, and a gateway that learns
[00:11:42] your business with every interaction.
[00:11:44] See how at cdata.ai.
[00:11:47] Blitzy's deep codebase understanding
[00:11:49] unlocks the thing every roadmap owner
[00:11:51] cares about, shipping new features.
[00:11:53] Here's the truth about building inside a
[00:11:54] massive enterprise codebase. Writing
[00:11:56] code was never the bottleneck. Context
[00:11:58] is. Which system does this touch? Which
[00:12:00] contracts can't break? Which standards
[00:12:01] apply? Blitzy already knows because it
[00:12:03] reverse-engineered your entire codebase
[00:12:05] into a dynamic knowledge graph before
[00:12:07] feature work began. With that complete
[00:12:08] picture, Blitzy builds features end to
[00:12:10] end. Architecture, APIs, UI, and tests
[00:12:13] all validated against your existing
[00:12:15] systems. One Blitzy customer built an
[00:12:17] AI-native application from scratch with
[00:12:18] 100% autonomous completion, saving over
[00:12:21] 2,700 engineering hours. Features that
[00:12:23] respect your codebase instead of
[00:12:25] fighting it. Stop letting your backlog
[00:12:26] grow faster than your team. Accelerate
[00:12:28] your roadmap at blitzy.com. That's b l i
[00:12:31] t z y.com.
[00:12:34] Welcome back to the AI Daily Brief. It's
[00:12:36] been clear for some time
[00:12:38] that among all the questions about AI's
[00:12:42] impact on the world, how much it was
[00:12:44] going to change work, whether it was
[00:12:46] going to disrupt jobs, what sort of
[00:12:48] runaway societal risks it might have,
[00:12:51] one of the fairly inarguable conclusions
[00:12:54] has been that it was going to have a
[00:12:55] dramatic impact on cybersecurity and
[00:12:59] cyberinfrastructure.
[00:13:00] One of the seminal moments of 2026 was,
[00:13:03] in fact, when Anthropic announced
[00:13:05] Project Glasswing and their powerful new
[00:13:07] model Mythos, which we would eventually
[00:13:09] get a consumer version of in Fable.
[00:13:11] Glasswing was announced in April, and in
[00:13:13] their announcement post they wrote, "We
[00:13:14] formed Project Glasswing because of
[00:13:16] capabilities we've observed in a new
[00:13:18] frontier model trained by Anthropic that
[00:13:20] we believe could reshape cybersecurity.
[00:13:22] AI models have reached a level of coding
[00:13:24] capability where they can surpass all
[00:13:26] but the most skilled humans at finding
[00:13:28] and exploiting software vulnerabilities.
[00:13:30] As part of the announcement, they noted
[00:13:32] that their preview version of Mythos had
[00:13:33] already found thousands of high-security
[00:13:35] vulnerabilities, including they said
[00:13:37] some in every major operating system and
[00:13:39] web browser. Given the rate of AI
[00:13:41] progress, Anthropic wrote, "it will not
[00:13:43] be long before such capabilities
[00:13:45] proliferate, potentially beyond actors
[00:13:47] who are committed to deploying them
[00:13:48] safely. The fallout for economies,
[00:13:51] public safety, and national security
[00:13:52] could be severe." Now, the way that
[00:13:54] Glasswing worked was that it gave access
[00:13:57] to Mythos to a small handful of
[00:13:59] government and corporate actors in order
[00:14:00] to start using its capabilities
[00:14:02] defensively to try to address possible
[00:14:04] exploits before they could be exploited.
[00:14:06] And yet, as that work has been ongoing,
[00:14:08] there is still been an acceleration in
[00:14:10] the incidents that companies and
[00:14:12] societies at large are starting to have
[00:14:13] to respond to.
[00:14:14] The best known of these, and the one
[00:14:16] that has had the most influence outside
[00:14:17] of the AI and tech space, is of course
[00:14:19] the Hugging Face incident, in which a
[00:14:20] fleet of agents from OpenAI broke
[00:14:22] containment to get access to Hugging
[00:14:24] Face's systems. And then earlier this
[00:14:26] week, the week actually kicked off with
[00:14:28] an attack on Open Code that got into the
[00:14:30] accounts of about running
[00:14:34] up bills on various AI companies' APIs.
[00:14:37] This all now, however, appears to be
[00:14:39] simply prelude. On Wednesday, security
[00:14:41] researchers disclosed a vulnerability in
[00:14:43] PHP that could affect as much as 70% of
[00:14:46] websites and web apps on the internet.
[00:14:48] By way of background for those who
[00:14:49] aren't deep in computer history and
[00:14:51] aren't developers yourselves, PHP is the
[00:14:53] programming language that runs the
[00:14:54] back-end servers that power the
[00:14:55] internet. It's been around since the
[00:14:57] early 1990s, and while some believe it
[00:14:59] is a little archaic, it is still deeply
[00:15:02] enmeshed in this internet that we
[00:15:03] currently use. The vulnerability was
[00:15:05] discovered around 2 months ago using
[00:15:07] GPT-5.6 Soul by a security researcher at
[00:15:10] Califf, and independently by the team at
[00:15:12] Wiz. In the intervening months, OpenAI
[00:15:15] has been coordinating with PHP's
[00:15:16] maintainers, Wiz, Cloudflare, and other
[00:15:19] partners to prepare mitigations and a
[00:15:20] patch ahead of disclosure. The
[00:15:22] vulnerability, dubbed PHP-2-Shell, is
[00:15:25] basically the worst nightmare for cyber
[00:15:27] defenders. It allows a threat actor to
[00:15:29] take control of a back-end server
[00:15:30] without logging in and perform remote
[00:15:32] code execution. Essentially, using this
[00:15:35] vulnerability, a hacker can get access
[00:15:37] to do anything with any server running
[00:15:39] on PHP. Critically, this wasn't a
[00:15:41] vulnerability that only impacted older
[00:15:43] versions of PHP. Even sites running the
[00:15:46] latest versions of server software were
[00:15:48] vulnerable. Volker Dusch, a security
[00:15:50] engineer at the nonprofit that maintains
[00:15:51] PHP, said that this was the most severe
[00:15:54] security issue the programming language
[00:15:55] has faced in over a decade. He compared
[00:15:57] it to Heartbleed, a critical
[00:15:58] vulnerability in the OpenSSL
[00:16:00] cryptographic library that led to a
[00:16:02] global patching effort back in 2014. In
[00:16:05] a blog post discussing the
[00:16:06] vulnerability, OpenAI wrote, "To our
[00:16:08] knowledge, Frontier AI found these
[00:16:10] vulnerabilities before attackers did,
[00:16:12] opening a defender's window for
[00:16:13] maintainers and security providers to
[00:16:15] prepare fixes and protections ahead of
[00:16:17] disclosure." That's technically true,
[00:16:19] and a bug fix was made available
[00:16:21] immediately. However, it seems that
[00:16:23] knowledge of the exploit spread around
[00:16:24] 10 hours ahead of disclosure before
[00:16:27] anyone could update their servers. Many
[00:16:29] government and commercial websites took
[00:16:30] their sites offline as a precaution
[00:16:32] yesterday morning.
[00:16:33] The situation was serious enough that
[00:16:35] the NSA issued a bulletin recommending
[00:16:37] that organizations take their systems
[00:16:38] offline until everything is patched. The
[00:16:41] FBI cyber division joined them asking
[00:16:42] for organizations to report intrusions.
[00:16:45] Now, this is the type of concern that I
[00:16:47] tend to have an almost reflexive
[00:16:49] skepticism towards. As AI reporter
[00:16:51] Cameron Wilson put it, "Real sky is
[00:16:54] falling vibes on the web today." And
[00:16:56] yet, based on the responses of people
[00:16:58] who know a heck of a lot more about this
[00:16:59] than I do, this one kind of seems like
[00:17:01] the real deal.
[00:17:03] Entrepreneur Brecht Units wrote, "Guys,
[00:17:05] this PHP bug is bad, real bad. If you're
[00:17:08] not afraid yet, you should be. I can
[00:17:10] only speak for our startup, but already
[00:17:12] at notebooks.com, we've seen 100% of our
[00:17:14] cookies exposed, entire source code
[00:17:16] stolen, hackers defacing our site on
[00:17:18] their own servers, founders doxed,
[00:17:19] important legal docs leaked. Former
[00:17:21] intelligence officer turned
[00:17:22] cybersecurity entrepreneur Mike Shelby
[00:17:24] wrote,
[00:17:25] "My CTO assures me that our platform has
[00:17:27] no risk from this latest PHP zero-day
[00:17:29] vulnerability thing. However," he adds,
[00:17:31] "we are in the calm before what is
[00:17:32] likely to be the biggest destruction
[00:17:34] event to the internet in 20 years. He's
[00:17:36] an actual hacker, by the way." He
[00:17:38] continues, "Biggest issue I've ever
[00:17:39] seen. Around 70% of websites are
[00:17:41] vulnerable and may have already been
[00:17:43] compromised without anyone knowing it
[00:17:44] yet. So, tomorrow should be fun."
[00:17:47] Investor Charles Read wrote, "I'm pretty
[00:17:49] concerned we're in the early stages of a
[00:17:50] global cybersecurity incident and we
[00:17:52] just don't fully realize the extent of
[00:17:53] it yet." AI engineer Nick Dobos reposted
[00:17:56] that and said,
[00:17:57] "Dozens, if not thousands, of AI agent
[00:17:59] swarms bigger than the hugging face
[00:18:00] incident are hacking about half the
[00:18:01] internet right now."
[00:18:03] He then modified that number to millions
[00:18:05] after seeing a post from Cloudflare CEO
[00:18:07] Matthew Prince, who said, "In the 10
[00:18:09] hours before P2P two shell was
[00:18:10] announced, across the Cloudflare
[00:18:12] network, we saw thousands of attempts to
[00:18:14] exploit it. That jumped to tens of
[00:18:15] thousands in the 45 minutes post
[00:18:16] announcement, hundreds of thousands
[00:18:18] within two hours, and millions now."
[00:18:21] Now, to some, this was inevitable.
[00:18:23] Wharton Professor Ethan Mollick wrote,
[00:18:25] "A visible sign of what AI insiders have
[00:18:26] been warning about since at least the
[00:18:28] mythos release. Acceleration of attack
[00:18:30] and defense at inhuman speeds,
[00:18:32] interacting with the very human systems
[00:18:33] that need to react to them."
[00:18:35] Paras Chopra writes,
[00:18:36] "What's happening with cybersecurity is
[00:18:38] what rationalists freaking out about AI
[00:18:39] capabilities have been predicting for a
[00:18:41] long while. It's the great hackening and
[00:18:43] it's going to get worse. Now, it's a bit
[00:18:45] beyond the scope of the show, but I find
[00:18:46] that particular characterization a
[00:18:48] little disingenuous, given that this
[00:18:50] isn't even close to the main thing or
[00:18:52] main things that that group has been
[00:18:53] warning about, and I think one could
[00:18:54] make a reasonable argument that all of
[00:18:56] the focus on these vague ex-risk
[00:18:58] scenarios for years in advance have, in
[00:19:00] fact, in many cases distracted from much
[00:19:02] more current issues like these
[00:19:03] cybersecurity issues. But, I would also
[00:19:05] say that the best counterpoint to that
[00:19:06] is that being concerned about one thing
[00:19:08] does not mean you don't get to be
[00:19:09] concerned about something else, and so
[00:19:11] we'll return back to our focus on the
[00:19:12] issues that are here right now. Outside
[00:19:14] of our little world, the response is
[00:19:16] more likely to be somewhere between
[00:19:18] uninformed, overwhelmed, or just blasé.
[00:19:21] Solopreneur Peter Levels wrote, "I
[00:19:23] notified a friend working at a big tech
[00:19:24] corporate about the PHP vulnerability as
[00:19:26] their entire infrastructure runs on PHP.
[00:19:29] He answered, 'Thanks. I'll try to patch
[00:19:31] it in a few days as I'm out of office
[00:19:32] right now.' And this is a modern tech
[00:19:34] company." Levels continued, "Imagine the
[00:19:36] traditional companies running PHP."
[00:19:38] Even for those companies not taking a
[00:19:40] blasé attitude, however, this represents
[00:19:41] an incredible challenge. Again, Ethan
[00:19:43] Mollick writes, "Companies I talk to are
[00:19:46] struggling with the rate of patches they
[00:19:47] need to do thanks to AI defenses finding
[00:19:49] issues before the inevitable wave of
[00:19:50] incoming cyber attacks by other AIs.
[00:19:53] Now, consumers are going to have the
[00:19:54] same experience of getting everything
[00:19:55] updated often and fast."
[00:19:58] Now, one question some had was around
[00:20:00] the disclosure method of this particular
[00:20:01] exploit. Maple AI CTO Anthony Ronning
[00:20:04] wrote, "If they've worked on the PHP
[00:20:06] vulnerability for over 2 months, then
[00:20:08] why has there been such a poor
[00:20:09] disclosure and rollout strategy? It's
[00:20:11] basically been a strategy of, quote, 'In
[00:20:13] 24 hours, you're all screwed.'"
[00:20:15] Cybersecurity professional Tay Monahan
[00:20:16] wrote, "This might be a stupid question,
[00:20:18] but given the discovery last week and
[00:20:20] that it started leaking 12 plus hours
[00:20:21] ago, why weren't the PHP patches ready
[00:20:23] to be dropped as soon as the
[00:20:24] vulnerability {slash} POC fully leaked?
[00:20:26] Why is everyone okay arbitrarily waiting
[00:20:28] another 12 hours to patch?" Christian
[00:20:30] the Pahl writes, "I'm no security
[00:20:32] expert, but telling the hacking world
[00:20:34] there's a mega huge apocalyptic exploit
[00:20:36] for PHP and giving them a day to figure
[00:20:37] it out and do as much damage before they
[00:20:39] release the fix seems like a bad idea.
[00:20:41] Couldn't they release the update, then
[00:20:42] after a day explain what it is? Now, my
[00:20:44] understanding from reading accounts from
[00:20:46] people who again know a lot more than I
[00:20:48] do about this is that the patch itself
[00:20:50] makes the exploit obvious. So, the
[00:20:52] concern was that as soon as they
[00:20:53] released the patch, they were also
[00:20:54] essentially making the exploit known in
[00:20:56] the wild. This is why the NSA warned
[00:20:58] everyone to take their sites down ahead
[00:21:00] of the disclosure."
[00:21:01] Frederick Williams wrote, "The real
[00:21:03] hacking world isn't the issue. They
[00:21:04] probably won't target most of us.
[00:21:06] Releasing the exploit/patch unleashes a
[00:21:08] storm of script kiddies that will scan
[00:21:10] and breach everything they find. They
[00:21:12] tried to get everyone ready to update
[00:21:13] the moment it lands.
[00:21:15] Now, before we get into broader
[00:21:16] implications, some are lamenting what
[00:21:18] might be the legacy of this particular
[00:21:20] exploit itself. Kenny Lauderdale writes,
[00:21:23] "This PHP stuff is so depressing because
[00:21:25] there's going to be 15 years worth of
[00:21:26] old sites that are going to become lost
[00:21:27] media now." Cybersecurity news reporting
[00:21:30] account, The International Cyber Digest
[00:21:32] wrote, "4chan has gone read-only and
[00:21:34] Something Awful has shut down its forums
[00:21:35] as American sites brace for the PHP
[00:21:37] patch. Bookmarking service Pinboard,
[00:21:39] game publisher Choice of Games, history
[00:21:40] site Damn Interesting, and the Explain
[00:21:42] xkcd wiki are offline, too." And then to
[00:21:45] add to the idea that these types of
[00:21:47] attacks were not going to be limited in
[00:21:48] their frequency, yesterday also saw
[00:21:50] Railway hit by a major exploit. Railway
[00:21:53] is an AI hosting service similar to
[00:21:54] Vercel. In a disclosure post, Railway
[00:21:57] wrote,
[00:21:57] "Earlier this morning, Railway detected
[00:21:59] anomalous activity involving systems
[00:22:01] that store customer environment
[00:22:02] variables. After further investigation,
[00:22:05] our investigation to date indicates that
[00:22:06] an unauthorized third party may have
[00:22:08] accessed encrypted environment
[00:22:09] variables, and for some of them obtained
[00:22:11] the decrypted contents. Environment
[00:22:12] variables may contain secrets such as
[00:22:14] API keys or database and registry
[00:22:16] credentials. We believe this is part of
[00:22:17] a series of attacks recently targeting
[00:22:19] platform companies with the aim of
[00:22:21] compromising AI inference providers. At
[00:22:23] first glance, this looks very similar to
[00:22:24] the Open Code exploit from last weekend,
[00:22:27] which again saw attackers gain access to
[00:22:28] user API keys, allowing the attackers to
[00:22:30] steal tokens and run up big bills. Like
[00:22:33] the Open Code situation, Railway is
[00:22:34] suggesting all users should rotate API
[00:22:36] keys and roll all environmental
[00:22:37] variables stored on the platform. Leo at
[00:22:40] Synthwave wrote, "Keys actively being
[00:22:42] drained, and they've disabled the
[00:22:43] ability to deploy anything, so can't
[00:22:45] deploy with new variables.
[00:22:46] Nightmare day for cyber, and it's only
[00:22:48] going to get worse from here, I fear."
[00:22:50] Dax from Open Code responded to the
[00:22:51] Railway team and summed up the new
[00:22:53] normal. He wrote, "I'm sure you're all
[00:22:55] better than me at this, but just some of
[00:22:57] what we've seen if it helps. They're not
[00:22:59] going to stop. It's going to get
[00:23:00] increasingly sophisticated, and they're
[00:23:02] going to go after every surface of your
[00:23:03] system and all of your employees. Any
[00:23:05] old projects you've long forgotten about
[00:23:07] will be found and used against you. The
[00:23:08] only reason we're surviving is because
[00:23:10] we have agents going 24/7. We're still
[00:23:12] barely sleeping. Good luck. Sorry you're
[00:23:14] dealing with this, but really it's a
[00:23:16] collective problem we're all facing
[00:23:17] together. Now, if this is the new
[00:23:19] normal, there are very different paths
[00:23:21] that that normal can take. On the one
[00:23:23] end of the spectrum is what was
[00:23:24] suggested by former OpenAI staffer
[00:23:26] Joshua Achiam, who wrote, "Feels like
[00:23:28] March 1st, 2020 for cyber. Not normal,
[00:23:31] something is happening. Internet
[00:23:32] lockdowns in a couple of months?" On the
[00:23:34] flip side, there are those who are
[00:23:35] recognizing that we're probably going to
[00:23:37] have to fight AI with AI. Entrepreneur
[00:23:40] John Ennis wrote, "Well, we just rotated
[00:23:42] every single key across a large number
[00:23:44] of projects very quickly, and I'm struck
[00:23:46] by the fact that this would have been an
[00:23:47] absolute nightmare not too long ago. The
[00:23:49] defensive aspect of AI for cybersecurity
[00:23:51] is really underrated. Where the nuclear
[00:23:53] weapon analogy breaks down with AI is
[00:23:55] that you can't stop a nuclear weapon
[00:23:56] with another nuclear weapon, but you can
[00:23:58] stop an AI attack with an AI." Box's
[00:24:01] Aaron Levie built on those themes,
[00:24:02] writing, "Cyber is going to be one of
[00:24:04] the most profound aspects of AI. We now
[00:24:06] have a tireless workforce that can hunt
[00:24:08] down, discover, patch, or attack any
[00:24:10] system and software ever created. We
[00:24:12] will use agents to identify the
[00:24:13] long-standing risks in existing systems
[00:24:15] and infrastructure. Attackers will use
[00:24:17] agents to accelerate the discovery of
[00:24:18] gaps in environments. We will equally
[00:24:20] use agents to defend attacks and
[00:24:22] discover anomalous patterns to better
[00:24:23] protect our data and much more. We're
[00:24:25] entering a new cyber regime, and we'll
[00:24:27] probably use 100x more tokens on this
[00:24:29] loop than we're imagining right now,
[00:24:30] because we can scan every log, look at
[00:24:32] every line of code, look through
[00:24:33] traffic, and process data at a scale
[00:24:35] that wasn't comprehensible before. More
[00:24:37] than ever, enterprises are going to care
[00:24:39] deeply about how they manage their
[00:24:40] networks, systems, software, data,
[00:24:42] identity, devices, and more. Agents will
[00:24:44] largely become the solution to these
[00:24:46] challenges, but they will keep everyone
[00:24:48] up in the process." In another post,
[00:24:50] Aaron wrote, "If you want to know all
[00:24:51] the jobs that AI will produce, look no
[00:24:53] further than cybersecurity. This is
[00:24:55] going to become one of the biggest
[00:24:56] investment areas for enterprises going
[00:24:57] forward, and even as that work becomes
[00:24:59] more agentic and autonomous, you will
[00:25:01] need more talent to point the agents at
[00:25:03] the most critical work, review findings,
[00:25:04] patch systems, respond to incidents, and
[00:25:06] more. Lots of opportunity right now for
[00:25:08] the systems that protect data in
[00:25:09] enterprises, as well as the
[00:25:10] professionals that are deploying them
[00:25:12] and protecting organizations. It's only
[00:25:14] going to get more wild out there.
[00:25:16] Embroidering co-founder Zach Korman
[00:25:18] argues in more colorful language that
[00:25:19] the only way out is through. He posted,
[00:25:22] "There is only one answer to
[00:25:23] cybersecurity threats, fix your
[00:25:26] Scared of threat actors using AI?
[00:25:27] Worried about rogue agents? Think
[00:25:29] obliterated models are spooky? Fix your
[00:25:31] The ban AI models and regulate GPU
[00:25:34] access crowd should instead fix their
[00:25:36] shit."
[00:25:36] And yet going back to the talent gap
[00:25:38] that Aaron Levie was just talking about,
[00:25:40] others think that that sort of fixing is
[00:25:41] not going to come easy and it's not
[00:25:43] going to be available for everyone. Will
[00:25:44] Manidis writes, "If today is any
[00:25:47] indication of the pace, markets are not
[00:25:49] nearly pricing in the rate at which
[00:25:50] banks/healthcare, et cetera, are going
[00:25:52] to have to merge to acquire enough scale
[00:25:54] to defend against AI-driven security
[00:25:56] vulnerabilities."
[00:25:57] Summing it up, Enclave's Tal Hoffman
[00:25:59] writes, "What a day. The future of
[00:26:01] cybersecurity is swarms. Swarms of
[00:26:04] agents attacking and swarms of agents
[00:26:05] defending, or rather, fleets versus
[00:26:07] swarms. Governed agents on defense
[00:26:10] versus cheap and relentless agents on
[00:26:11] offense. Whoever coordinates faster
[00:26:14] wins."
[00:26:15] In a post called Towards Securing the
[00:26:16] Internet, OpenAI president Greg Brockman
[00:26:19] wrote about how, in his word, "New
[00:26:20] approaches will be needed." He said, "We
[00:26:23] are actively thinking about those and
[00:26:24] looking for feedback from the community
[00:26:26] to help us collectively rise to the
[00:26:27] challenge of improving the security of
[00:26:28] the internet as models improve. As
[00:26:30] vulnerability discovery ramps, we will
[00:26:32] need new defensive solutions,
[00:26:33] potentially including authorized
[00:26:35] defenders such as government scanning
[00:26:37] the internet for vulnerable hosts, and
[00:26:38] either notifying or, in extreme cases,
[00:26:40] patching those systems remotely." After
[00:26:42] discussing some more of OpenAI's
[00:26:43] commitments, he concludes, "I believe
[00:26:45] we're entering a new phase of
[00:26:46] cybersecurity, where the models are able
[00:26:48] to find vulnerabilities with
[00:26:49] internet-scale impact. We believe that
[00:26:51] defenders everywhere have a part to play
[00:26:53] applying models to their own defenses,
[00:26:55] finding and fixing issues in shared
[00:26:56] infrastructure, and sharing best
[00:26:58] practices that can ultimately make the
[00:26:59] internet more secure. And the most
[00:27:01] optimistic take is that ultimately
[00:27:03] software will be more secure. A16Z's
[00:27:05] Martin Casado wrote, "In the long run,
[00:27:08] AI is going to make software so much
[00:27:10] more capable and so much more secure and
[00:27:12] reliable. But before that, things are
[00:27:14] going to get much, much worse." Longtime
[00:27:17] listeners will have heard me say before
[00:27:19] that across so many aspects of AI, I am
[00:27:22] an incredible long-term optimist. And
[00:27:24] yet long-term optimism does not deny the
[00:27:27] potential chaos, pain, and agony of
[00:27:29] short or even medium-term transitions. I
[00:27:32] believe that's the case for jobs, and it
[00:27:33] is certainly the case for cybersecurity.
[00:27:35] And boy, are we in it now. I will of
[00:27:37] course keep you informed as things
[00:27:39] evolve. For now, however, that is going
[00:27:40] to do it for today's AI daily brief.
[00:27:42] Thanks as always for listening or
[00:27:43] watching, and until next time, peace.
