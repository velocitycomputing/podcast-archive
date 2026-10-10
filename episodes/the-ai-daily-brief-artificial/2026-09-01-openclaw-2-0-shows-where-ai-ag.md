---
record_id: "podcast:58c44575-6781-44d8-9612-491707f77b25"
episode_id: 58c44575-6781-44d8-9612-491707f77b25
title: OpenClaw 2.0 Shows Where AI Agents Are Going Next
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/openclaw-20-shows-where-ai-agents-are-going-next/58c44575-6781-44d8-9612-491707f77b25"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/openclaw-20-shows-where-ai-agents-are-going-next/58c44575-6781-44d8-9612-491707f77b25"
feed_guid: null
feed_url: "https://anchor.fm/s/f7cac464/podcast/rss"
published_at: null
published_local_date: null
played_date: 2026-09-01
played_at: "2026-09-01T12:00:00Z"
play_count: 1
duration_seconds: 1560
source: pocketcasts-history-browser
played_label: September 1
history_order: 74
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: b843f152e98218c4b02198baeeea40074ffe1375aab21678692563e7d1a3de28
analysis_mode: health
summary_source: local
model_source: local
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: Qwen3.8-Flash-Next-UD-Q4_K_XL
tagging_model: claude-haiku-4-5
proposed_tags: [geopolitics, primary-source-video]
proposed_entities: []
status: new
routed_to: null
---

## Summary

OpenClaw 2.0 is presented as a ground-up rework of the open-source agent harness, with 933 contributors across 16,000 pull requests, simplified installation, faster first conversations, easier inbox-monitoring workflows, and a major shift toward “multiplayer” shared agents; Peter Steinberger and maintainer Colin describe team.openclaw.ai as a shared workspace where developers can open the same agent session, add context, steer work, and hand off tasks without transcript dumps, while Alex Finn reports update breakage and compatibility problems, and News Research’s Hermes “Pantheon” release 0.21.0 adds bot mode, Hermes peer bot-to-bot DMs, and new model support. The episode also covers AI security and policy: Hugging Face reportedly used open Chinese models during an OpenAI-related attack because closed-model guardrails blocked defensive actions; Obliteration.AI released “Obliterated Model Large V2,” based on GLM 5.3, with guardrails removed at the weights level, a 1 million context window, zero input/output retention, claimed 2x cyber exploitation versus 5.2, and a #3 Terminal Bench 4.0 ranking behind Opus 5 and Fable, drawing reactions from Ethan Mollick, Chubby, Clement Dumas, Lucas Pombo, and others about uncensored frontier cyber capability. Anthropic’s “Improving Our Alignment and Security Efforts” update disclosed agentic-testing incidents, motivated reasoning, willingness to take harmful actions, sandbox redesigns, real-time escape-detection classifiers, a two-week RL pause, and a finding that 10% of testing environments were prone to reward hacking; Chinese state media tied to CCTV attacked Anthropic ahead of AI talks, framing Mythos as a potential cyber weapon and accusing the U.S. of double standards. OpenAI’s advertising business reached a $1 billion revenue run rate in 200 days across 40 countries, below its $2.4 billion projection and still small versus its roughly $40 billion total run rate, while President Trump’s pro-data-center Truth Social post drew responses from Senator John Fetterman, AOC, Justin Amash, Vice President J.D. Vance, and pollster Mark Michelle, with polling suggesting data centers remain unpopular.

Actionable takeaways are mainly operational, security, and strategic: if the user works with AI agents, test multiplayer workflows carefully by piloting shared sessions, defining ownership and access rules, preserving audit trails, and treating handoffs as shared work artifacts rather than private chat logs; do not assume OpenClaw 2.0 is stable or secure merely because the team says it is, and use version pinning, backups, and rollback plans because update breakage is reported. For security or research work, treat Obliteration.AI’s uncensored cyber model as a high-risk research lead: authorized red-team testing, isolated sandboxes, air-gapped environments, real-time monitoring, and clear legal boundaries are essential, and follow-up questions should include how guardrails can move into harnesses or legal controls when open weights can be uncensored, how to evaluate cyber capability without enabling misuse, and whether defensive teams should rely on open models when closed-model guardrails block legitimate defense. For business or product decisions, watch whether shared agent workspaces become the default for team-level knowledge work, whether OpenAI’s ad platform scales toward its $100 billion ambition, and whether Anthropic’s alignment fixes reduce reward hacking and harmful agentic behavior; no direct health implications are stated, but if agents are applied to health-related tasks, require human clinical review, treat model outputs as unverified, and ask follow-up questions about privacy, liability, hallucination risk, and regulatory compliance before deployment.

## Transcript

[00:00:00] When OpenClaw came out, it was an
[00:00:02] absolute sensation. And it wasn't
[00:00:03] because it was easy or user-friendly,
[00:00:05] it's because it showed the potential of
[00:00:08] what agents could do for us in a real
[00:00:09] way for the first time. Now, after the
[00:00:12] initial craze, a lot of that energy
[00:00:13] dissipated into other areas. And in many
[00:00:16] ways, the biggest impact of OpenClaw was
[00:00:18] how it influenced the next wave of
[00:00:19] agentic products that would come to
[00:00:21] market. Well, now OpenClaw is back with
[00:00:23] OpenClaw 2.0. And once again, I believe
[00:00:25] that they are embracing an interaction
[00:00:27] pattern which is not the norm right now,
[00:00:28] but will be normalized very soon. That
[00:00:30] pattern is about shared agents and
[00:00:32] multiplayer AI.
[00:00:34] The AI Daily Brief is a daily podcast
[00:00:36] and video about the most important news
[00:00:37] and discussions in AI.
[00:00:39] All right, friends. Quick announcements
[00:00:41] before we dive in. Our next agent
[00:00:42] training for executives program, which
[00:00:44] is coming up just after Labor Day,
[00:00:46] registration for that is open now.
[00:00:48] One of the interesting sub-stories of
[00:00:50] the OpenAI
[00:00:51] hack was that Hugging Face had to turn
[00:00:53] to open models from China to defend
[00:00:56] against the attack because the
[00:00:57] guardrails on the closed models wouldn't
[00:01:00] allow them to do what they needed. Now,
[00:01:02] this of course points out an inherent
[00:01:03] challenge in these really powerful
[00:01:05] models, which is of course that the
[00:01:06] guardrails that are used to block
[00:01:08] malicious actors can also prevent
[00:01:09] legitimate actors from using those
[00:01:11] models to defend against malicious
[00:01:12] actors. Well, now one company called
[00:01:15] Obliteration.AI has come along and said,
[00:01:17] "Don't worry, we got you." They write,
[00:01:20] "Today, we're releasing Obliterated
[00:01:21] Model Large V2 based on GLM 5.3, which
[00:01:25] is number three on Terminal Bench 4.0
[00:01:26] behind only Opus 5 and Fable with two
[00:01:29] times the cyber exploitation of 5.2. We
[00:01:32] obliterated and hosted it so it does the
[00:01:34] offensive cyber red teaming and agent
[00:01:36] testing work other models refuse to do.
[00:01:38] US hosted, 1 million context window,
[00:01:40] zero input output prompt retention, live
[00:01:42] now.
[00:01:44] The cyber jump, they write, is why 5.3
[00:01:45] exists. Obliteration, they say, finds
[00:01:48] the directions in the model's
[00:01:49] activations that produce refusals and
[00:01:51] removes them from the weights. The
[00:01:52] coding, cyber, and agentic ability stay.
[00:01:54] The The stops refusing the rest of the
[00:01:56] chain. For offensive cybersecurity, AI
[00:01:58] red teaming, agent testing, and trust
[00:02:00] and safety, the model will follow
[00:02:02] through instead of shutting down.
[00:02:04] If your current model still stops
[00:02:05] halfway through an authorized exploit
[00:02:07] chain, a red team eval, or a TNS
[00:02:09] adversarial prompt reply with the task
[00:02:10] it refuses, we'll tell you a few two
[00:02:12] handles it. So, obviously this is being
[00:02:15] presented as a tool for cyber defenders.
[00:02:18] Mostly what people are picking up on
[00:02:20] though is that this is a powerful cyber
[00:02:22] focused model with the guardrails
[00:02:24] removed at a weights level.
[00:02:26] Professor Ethan Mollick says, "That
[00:02:27] didn't take long." Hero with a thousand
[00:02:29] faces sums up the feelings of many when
[00:02:31] they write,
[00:02:32] "Why would you do this? Why on earth
[00:02:34] would you do this? I don't mean to be a
[00:02:35] doomer, but why?" 0.005 seconds writes,
[00:02:38] "Homeboy released the crime LLM."
[00:02:41] Clement Dumas sums up, "Remove
[00:02:43] guardrails of a frontier model with high
[00:02:44] cyber capabilities, no system card, eval
[00:02:47] on exploit gym, the one that made OpenAI
[00:02:49] agents crazy. Can't wait for the next
[00:02:51] version, takeover large V3."
[00:02:53] Lucas Pombo writes, "Get ready to test
[00:02:56] your predictions, everyone. Point,
[00:02:57] counterpoint, this model will
[00:02:58] destabilize the entire internet and set
[00:03:00] off a global shockwave of cybercrime
[00:03:02] versus no, it won't."
[00:03:04] Now, holding aside whatever
[00:03:05] Obliteration's intents are, Chubby
[00:03:07] points out the question that this brings
[00:03:08] up about all the guardrails.
[00:03:10] They write, "They took the safety layer
[00:03:12] out of GLM 5.3 and turned it into an
[00:03:14] admin panel. It's questionable what all
[00:03:16] the guardrails at Anthropic and OpenAI
[00:03:18] actually achieve given that open weights
[00:03:21] models, which are virtually state of the
[00:03:22] art, can be deployed completely
[00:03:23] uncensored shortly thereafter." And
[00:03:26] indeed, when you dig into the
[00:03:26] discussion, it's a lot of people talking
[00:03:28] about in what ways can guardrails moving
[00:03:30] to other parts of the stack like the
[00:03:32] harness help, or whether it's inevitably
[00:03:33] going to come down to legal protections.
[00:03:36] Now, along the same topic, Anthropic
[00:03:37] released an update this week called
[00:03:39] Improving Our Alignment and Security
[00:03:40] Efforts. And while the Hugging Face
[00:03:42] attack may have grabbed all the
[00:03:43] headlines, Anthropic disclosed similar
[00:03:45] events stemming from agentic testing
[00:03:47] earlier this year. The report states,
[00:03:49] "We believe the incidents reflect a
[00:03:50] failure of operational security, as well
[00:03:52] as two alignment issues: motivated
[00:03:54] reasoning and willingness to take
[00:03:56] harmful actions in pursuit of a narrow
[00:03:57] task. Regarding their updates to
[00:03:59] security, Anthropic's changes largely
[00:04:01] come down to monitoring and better
[00:04:02] practices around sandboxes. Anthropic
[00:04:05] has redesigned their sandboxes to ensure
[00:04:06] they're properly air-gapped from the
[00:04:08] internet, but they've also begun using a
[00:04:10] real-time classifier to detect when a
[00:04:11] model is attempting to escape a testing
[00:04:13] environment. Anthropic disclosed that
[00:04:15] they paused reinforcement learning
[00:04:16] efforts for 2 weeks while hardening
[00:04:18] systems and auditing reinforcement
[00:04:19] learning environments, but have now
[00:04:21] resumed the majority of their training
[00:04:22] efforts. Discussing the recent open
[00:04:24] letter that called for pacing the
[00:04:25] frontier, Anthropic noted that efforts
[00:04:27] within an individual company are
[00:04:28] different to an industry-wide approach
[00:04:30] that likely requires government
[00:04:32] coordination. Still, they say they would
[00:04:33] support such an effort, writing, "We
[00:04:35] believe the world would benefit if the
[00:04:36] industry adopted a lawful, verifiable,
[00:04:39] effective mechanism for coordinated
[00:04:40] pacing as soon as possible." Alignment
[00:04:42] efforts are still ongoing, but Anthropic
[00:04:44] is now digging in on why the models were
[00:04:45] willing to take harmful actions once
[00:04:47] they gained access to the internet. The
[00:04:49] hypothesis at this stage is that the
[00:04:50] models couldn't easily distinguish
[00:04:52] between a simulated test environment and
[00:04:53] the live internet. Anthropic is also
[00:04:55] taking this opportunity to further
[00:04:57] explore the issue of reward hacking,
[00:04:59] where a model takes an unintended path
[00:05:00] to successfully complete an eval. Reward
[00:05:02] hacking has been a persistent problem
[00:05:04] for Anthropic, and their audit found
[00:05:05] that 10% of testing environments were
[00:05:07] prone to reward hacking or broken tasks.
[00:05:09] After testing different RL setups, their
[00:05:11] conclusion was that the presence of
[00:05:13] reward hacking in the training process
[00:05:14] contributed to that behavior during
[00:05:15] testing.
[00:05:16] Obviously, these topics are going to do
[00:05:18] nothing but grow in importance, but they
[00:05:20] are not the only place that Anthropic is
[00:05:21] in the news.
[00:05:22] Chinese state media has lashed out at
[00:05:24] Anthropic in a precursor to AI talks
[00:05:26] later this month. In a social media
[00:05:28] post, an account tied to state
[00:05:29] broadcaster CCTV argued that the US must
[00:05:32] prove their AI companies are subject to
[00:05:33] the same safety, disclosure, and audit
[00:05:35] rules as Chinese labs before substantive
[00:05:37] discussions can take place. In a post
[00:05:39] titled "Anthropic Has Contracted the
[00:05:41] American Disease," the account wrote, "A
[00:05:43] clear distinction must be drawn between
[00:05:45] genuine security threats and more
[00:05:46] technological competition. This line
[00:05:48] must be drawn jointly by all
[00:05:49] participating parties. Bloomberg
[00:05:51] suggested that this account is often
[00:05:53] used to signal official government
[00:05:54] positions. Taking aim at Anthropic, the
[00:05:56] post continued, "The problem is that
[00:05:58] America's own frontier models have
[00:06:00] already developed in a distorted
[00:06:01] direction. This means the negotiation is
[00:06:03] not simply a technical dialogue from the
[00:06:05] start, but a continuation of the earlier
[00:06:07] problems. The US is trying to turn these
[00:06:09] safety boundaries it has drawn into the
[00:06:10] default rules for the entire world."
[00:06:12] Sources familiar with the thinking of
[00:06:14] Chinese officials said that they view
[00:06:15] Mythos as the larger problem. They
[00:06:17] reportedly see the potential for Mythos
[00:06:18] to be used as a cyber weapon against
[00:06:20] China, and essentially the post argued
[00:06:22] that the US government is insisting on a
[00:06:23] double standard where US labs are free
[00:06:25] to distribute cyber weapons, while the
[00:06:26] Chinese labs are threatened for matching
[00:06:28] the technology. The post said, "The
[00:06:30] {quote} control proposed by the US is in
[00:06:32] essence an attempt to make China accept
[00:06:35] an order partly defined by American
[00:06:36] companies." Now, with President Xi
[00:06:38] visiting the US at the end of this
[00:06:39] month, expect to see a lot more
[00:06:41] jockeying and positioning in narrative
[00:06:42] claiming, particularly around hot-button
[00:06:44] issues like AI.
[00:06:45] Moving from Anthropic over to OpenAI,
[00:06:48] that company is celebrating a major
[00:06:49] milestone after their advertising
[00:06:50] business hit a billion dollars in
[00:06:52] revenue run rate. OpenAI began testing
[00:06:54] ads on free ChatGPT accounts in
[00:06:56] February, and after a rocky start, the
[00:06:58] business seems to be scaling up. Ads are
[00:07:00] now being shown across more than 40
[00:07:01] countries, and the revenue milestone was
[00:07:03] reached in just 200 days. For
[00:07:05] advertisers, OpenAI has progressively
[00:07:07] added more features to track conversion
[00:07:08] metrics and optimize campaigns. And
[00:07:10] after starting with a manual ad buying
[00:07:12] process, OpenAI is rolling out their
[00:07:13] self-service platform to markets across
[00:07:15] India, Europe, the Middle East, and
[00:07:16] North Africa this week. You might not
[00:07:18] remember just how controversial ChatGPT
[00:07:20] ads were at the beginning. Anthropic
[00:07:22] even chose to focus on them for their
[00:07:24] Super Bowl ad campaign, which I thought
[00:07:26] was just absolutely insane back then.
[00:07:28] And the total lack of enduring concern
[00:07:30] around ads kind of validates my points.
[00:07:33] It's not that all of a sudden people are
[00:07:34] excited about ads or anything like that.
[00:07:36] There's just a natural acceptance that
[00:07:37] this is the business model of the
[00:07:39] internet, and you're not going to have
[00:07:40] free AI without it.
[00:07:42] Now, in terms of the company's own
[00:07:43] expectations, while a billion dollar run
[00:07:45] rate is a meaningful first step, it does
[00:07:47] actually fall short of OpenAI's
[00:07:48] ambitions. OpenAI had projected 2.4
[00:07:51] billion in advertising revenue this
[00:07:53] year, growing to more than 100 billion
[00:07:55] to become their largest revenue stream
[00:07:56] by the end of the decade. For now,
[00:07:58] advertising remains a small fraction of
[00:07:59] their roughly 40 billion in revenue run
[00:08:01] rate, although that is likely to change
[00:08:03] over time.
[00:08:04] Lastly today, President Trump has
[00:08:06] weighed in on the data center debate
[00:08:08] with some characteristically coarse
[00:08:09] framing. On Truth Social on Monday, he
[00:08:11] posted, "The only reason that
[00:08:13] communities throughout the USA should
[00:08:15] not want data centers is if they want to
[00:08:17] end up being backwards and poor. If they
[00:08:19] want to be successful and rich with far
[00:08:20] lower taxes and jobs all over the place,
[00:08:22] let data rain."
[00:08:24] "The good news is that there are plenty
[00:08:25] of other places that want them. If we
[00:08:27] kill the golden goose, you will only
[00:08:29] have yourselves to blame. China could
[00:08:30] not be happier with this anti-data
[00:08:32] center movement. Actually, they can't
[00:08:34] believe it's happening." And with that,
[00:08:36] the tinderbox ignited. Senator John
[00:08:38] Fetterman gave his full support,
[00:08:39] although he's just about the only one.
[00:08:41] The Pennsylvania Democrat posted,
[00:08:43] "Agreed. We must win the war for AI
[00:08:45] supremacy over China. They foment the
[00:08:47] anti-argument through misinformation.
[00:08:49] There's nothing more damaging to a
[00:08:50] Democrat than agreeing with Trump and
[00:08:52] data centers, but what's right is
[00:08:53] right." Other Democrats seized on the
[00:08:55] opportunity to push their own sound
[00:08:56] bites. AOC told a reporter, "How about
[00:08:59] we put one in Mar-a-Lago? I love that.
[00:09:01] Let's put a data center up in Mar-a-Lago
[00:09:02] and we'll see how backwards and poor he
[00:09:03] is in response to that." Former
[00:09:05] Republican Congressman Justin Amash
[00:09:07] posted, "Communities have many
[00:09:09] legitimate concerns about data centers.
[00:09:10] To dismiss millions of Americans as
[00:09:12] people who just want to be backwards and
[00:09:13] poor shows how out of touch Trump has
[00:09:15] become."
[00:09:16] Now, people jumped in to point out that
[00:09:17] that's sort of a misrepresentation of
[00:09:19] the words, but good luck getting that
[00:09:20] nuance through when it comes to
[00:09:21] politics.
[00:09:23] And even with Trump's main base, the
[00:09:24] message didn't necessarily hit. Trump's
[00:09:27] post on Truth Social had dozens of
[00:09:28] negative responses with one Florida
[00:09:30] resident commenting,
[00:09:32] "The statement is insane. I'm already on
[00:09:34] a water restriction."
[00:09:35] Now, later in the day, Vice President
[00:09:37] J.D. Vance massaged the message into
[00:09:39] something a little bit more palatable.
[00:09:40] He told reporters, "What the president
[00:09:42] said about data centers is that they're
[00:09:44] an important part of the AI economy, but
[00:09:45] when people build them, they have to
[00:09:46] build the power plants along with the
[00:09:48] data centers. I think probably 99% of
[00:09:50] the backlash has come in areas where
[00:09:52] building a data center means higher
[00:09:53] utility and higher electricity for
[00:09:54] people on the ground. I think what these
[00:09:56] companies have to do is take advantage
[00:09:58] of some of the deregulatory efforts
[00:09:59] we've undertaken. If you build a data
[00:10:01] center, you should be putting power back
[00:10:02] into the grid, not taking it out. If
[00:10:04] that is happening, I don't think the
[00:10:05] data centers are that controversial."
[00:10:07] Pollster Mark Michelle writes, "Love
[00:10:09] them or hate them, the polling says data
[00:10:11] centers are very unpopular. You can
[00:10:12] blame China or whoever, but that doesn't
[00:10:14] make them popular. Today, Trump just dug
[00:10:16] in on a very unpopular thing two months
[00:10:18] before the midterms."
[00:10:20] There is a lot that could be said about
[00:10:21] this, but pretty much all of it is
[00:10:23] beyond the scope of this show. So, for
[00:10:24] now, that's going to do it for the
[00:10:25] headlines. Next up, the main episode.
[00:10:28] Welcome back to the AI Daily Brief.
[00:10:30] Today, we are talking about the latest
[00:10:32] release from Open Claw, Open Claw 2.0.
[00:10:35] And believe it or not, even if you were
[00:10:37] one of the folks that tried Open Claw
[00:10:39] for a little while and then went away,
[00:10:41] or just watched the wave pass, I believe
[00:10:43] that they are once again early to a
[00:10:44] pattern of AI usage that will shape
[00:10:46] where we go next, even if it's not with
[00:10:49] Open Claw.
[00:10:50] The initial launch of Open Claw was one
[00:10:52] of the most important moments in AI this
[00:10:53] year. In November and December, we had
[00:10:55] gotten a significant capabilities leap.
[00:10:57] Opus 4.5, GPT 5.2 were significant
[00:11:00] upgrades that would take folks until the
[00:11:02] holiday break to really understand how
[00:11:04] powerful they were. Now, of course, the
[00:11:07] upgrade wasn't just in the models, it
[00:11:08] was also in the harnesses through which
[00:11:10] those models were being used. Both of
[00:11:12] those Frontier Labs were placing
[00:11:13] significant and increasing emphasis on
[00:11:16] their Claude code and Codex harnesses,
[00:11:18] and by the beginning of 2026, awareness
[00:11:20] and usage of those harnesses had
[00:11:22] started, perhaps very nascently, but
[00:11:24] started to move outside of strictly
[00:11:26] software developers into other knowledge
[00:11:28] workers of all different stripes. Then,
[00:11:29] towards the end of January, Open Claw
[00:11:31] happened. Originally named ClaudeBot, c
[00:11:34] l a w, and then very briefly MoldBot,
[00:11:38] before landing in its final form of
[00:11:40] OpenClaw, it was effectively an
[00:11:42] open-source harness that helped people
[00:11:44] actually make the potential of AI agents
[00:11:47] real. It was technically complex, but if
[00:11:50] you waited through and used AI as an
[00:11:52] assistant to help you figure it out, you
[00:11:54] could build individual agents or teams
[00:11:55] of agents that felt to many like they
[00:11:57] unlocked the agentic capabilities that
[00:11:59] we had been promised for so long for the
[00:12:01] very first time. And of course, for a
[00:12:03] moment there, OpenClaw was a bonafide
[00:12:05] craze. And not just in the US. Chinese
[00:12:08] citizens went nuts for the technology,
[00:12:10] leading to articles like this one from
[00:12:11] CNBC in March, "How China is getting
[00:12:13] everyone on OpenClaw from gear heads to
[00:12:15] grandmas." Now, since that initial
[00:12:17] moment of experimentation, that agentic
[00:12:19] big bang, if you will, the energy that
[00:12:21] was initially captured by OpenClaw has
[00:12:24] found its way into a lot of different
[00:12:25] places. After its founder, Peter
[00:12:27] Steinberger, was absorbed into OpenAI,
[00:12:29] some folks turned their attention to
[00:12:31] competing open harnesses like Hermes
[00:12:33] from News Research. And of course, as
[00:12:35] we've seen lately with things like
[00:12:36] GrokBot, a lot of these features have
[00:12:38] also slowly made their way into tools
[00:12:40] that don't have as much technical
[00:12:41] complexity as the original OpenClaw did.
[00:12:43] OpenClaw itself was converted into a
[00:12:45] non-profit foundation, and for a while
[00:12:47] saw a blistering pace of development,
[00:12:49] pushing updates every few days. For the
[00:12:51] last 7 weeks, however, the OpenClaw team
[00:12:53] has been quiet. And what was going on
[00:12:55] was nothing less than a complete rework
[00:12:58] of OpenClaw from the ground up.
[00:13:00] The new OpenClaw 2.0 featured 933
[00:13:03] contributors across 16,000 pull
[00:13:05] requests, and it really is meant to be a
[00:13:07] complete rework of how the system works,
[00:13:09] from installation to messaging to memory
[00:13:12] to skills, to automations to browsers,
[00:13:15] to plugins to security, along with a
[00:13:17] very long tail of other fixes. A lot of
[00:13:19] the emphasis was on simplifying and
[00:13:21] making it easier for new people to
[00:13:22] engage. For example, they have tried to
[00:13:25] massively simplify the first time
[00:13:26] install process, latching onto existing
[00:13:29] subscriptions or API keys, and reducing
[00:13:31] a bunch of the initial configuration,
[00:13:33] helping people get to conversations with
[00:13:34] their Grok bots faster, and allowing
[00:13:36] them to do other necessary
[00:13:37] configurations later through the chat
[00:13:39] interface with their Grok bots. They
[00:13:41] reduce the amount of initial
[00:13:42] configurations, making people's time to
[00:13:44] first conversations with their claws
[00:13:46] much faster. People can then finish
[00:13:47] setting up or customizing their claw
[00:13:49] later via direct conversation with it.
[00:13:51] There's also a renewed focus on making
[00:13:53] simple tasks easy to set ensuring they
[00:13:56] work well. An example they give is inbox
[00:13:58] monitoring where they write, "A simple
[00:14:00] workflow might have it watch your inbox
[00:14:01] for your kids school emails and send you
[00:14:03] a Telegram message whenever something
[00:14:04] important comes through, like homework
[00:14:06] due or an upcoming activity you need to
[00:14:08] prepare for." Their vision is basically
[00:14:10] to have people start simply and then
[00:14:11] expand from there.
[00:14:13] Now, on the face of it, all of these
[00:14:14] feel like great upgrades and certainly
[00:14:15] address the types of things that have
[00:14:17] been barriers to entry for people in the
[00:14:18] past. And you can tell from the response
[00:14:20] that concern around complexity remains
[00:14:22] fairly high among the AI community. On
[00:14:25] the announcement tweet, a user named
[00:14:26] Mela responded, "Do I still need a PhD
[00:14:28] in computer science to install?"
[00:14:30] Aurelius asks, "Um, is it secure now?"
[00:14:33] To which Open Claw responded, "Yes."
[00:14:35] Another responder on that initial thread
[00:14:37] was AI creator Alex Finn, who gained
[00:14:39] prominence around the first Open Claw
[00:14:41] move based on his experiments to see
[00:14:43] just how far he could push his claws.
[00:14:45] Alex did not have such a great
[00:14:46] experience with this update. He wrote,
[00:14:49] "I updated and it immediately broke Open
[00:14:51] Claw. Legit 70% plus of the time I
[00:14:54] update Open Claw, it breaks it. Do you
[00:14:56] guys test before releasing this? I've
[00:14:57] never used any other AI tool where this
[00:14:59] so consistently happens. Luckily, I have
[00:15:01] a lot of patience, but I can't imagine
[00:15:02] most normies do."
[00:15:04] It seemed like the issue was
[00:15:05] compatibility between older versions of
[00:15:07] Open Claw and this newer version, and
[00:15:09] the inability to simply ask Open Claw to
[00:15:11] update itself.
[00:15:12] In a separate review video, he called
[00:15:14] Open Claw the most frustrating,
[00:15:15] disappointing release of the year.
[00:15:17] Now, inevitably, a lot of the
[00:15:18] conversation came back to the comparison
[00:15:20] between Open Claw and Hermes. Responding
[00:15:23] to one post making that comparison, Hans
[00:15:25] Rudolph, who does community and dev
[00:15:26] relations at OpenClaw, said, "We're not
[00:15:28] selling anything here or asking people
[00:15:30] to trust one company, one model, or one
[00:15:32] AI provider, because OpenClaw is open
[00:15:34] source and belongs to the people who use
[00:15:35] it and help build it. The us versus them
[00:15:37] is a crap take on things. If you like
[00:15:39] Hermes, use it. If you like OpenClaw,
[00:15:41] use it." Now, speaking of Hermes, as
[00:15:43] they seem to always do whenever anyone
[00:15:45] announces anything else, they also had a
[00:15:47] release today, this one actually being
[00:15:49] an aggregation of a bunch of smaller
[00:15:50] releases that they had over the past
[00:15:52] several weeks. News Research called it
[00:15:54] the Pantheon release, technically
[00:15:56] version 0.21.0,
[00:15:58] and it formalizes things like bot mode,
[00:16:00] which was a Grokbot-style interface, as
[00:16:02] well as a bunch of other new features,
[00:16:03] like Hermes peer, which is bot-to-bot
[00:16:05] DMs, and support for a set of new
[00:16:07] models.
[00:16:08] Now, for some, all of this is just hypie
[00:16:10] early adopters being excited about toys
[00:16:12] that'll never make their way to normal
[00:16:13] businesses or consumers.
[00:16:15] Arnav Gupta posts,
[00:16:16] "How does the entire timeline get a
[00:16:18] whole new round of psychosis from
[00:16:19] basically the same thing every time?
[00:16:21] OpenClaw, Manas, Hermes, Instinct. It's
[00:16:24] the same thing over and over again. If
[00:16:26] it works, how come you're hopping from
[00:16:27] one to another and not happy with the
[00:16:29] existing one?"
[00:16:30] Harshal Madhav responded, "Because none
[00:16:32] of these are end-state products. Only
[00:16:33] techies could use OpenClaw, but it broke
[00:16:35] a lot. Hermes broke less. Instinct is
[00:16:37] less technical and usable by a much
[00:16:39] larger population than Hermes and
[00:16:40] OpenClaw. Yes, there are hype maxers,
[00:16:42] but this is also a sign of how early
[00:16:44] things are. We're nowhere near an
[00:16:46] end-state where any of these work for
[00:16:47] everyone yet. With every iteration, a
[00:16:49] newer population discovers this and gets
[00:16:51] excited, sometimes overexcited, about
[00:16:53] where it is headed."
[00:16:54] I think that's true, but I'd go even
[00:16:55] farther. I think that these products,
[00:16:58] and the early adopters who use them, are
[00:16:59] the incubatory cauldron where people are
[00:17:01] figuring out what sort of interaction
[00:17:04] patterns are actually going to be useful
[00:17:06] when it comes to interfacing with
[00:17:07] agents. Pretty much all knowledge
[00:17:09] workers are somewhere along the journey
[00:17:11] of figuring out which parts of their job
[00:17:12] they're going to continue to actually do
[00:17:14] versus which parts they're going to
[00:17:15] outsource to agents, which is a step
[00:17:17] change that's significantly bigger than
[00:17:19] just adopting a new tool. It's a whole
[00:17:21] new way of thinking about and completing
[00:17:22] one's job. We need folks who are willing
[00:17:24] to hack through even inefficiently, to
[00:17:27] experiment in these open sandboxes, to
[00:17:29] better understand which of the patterns
[00:17:30] that they reveal need to come to a
[00:17:32] broader audience. In other words,
[00:17:34] something like Grok Bot, which has the
[00:17:36] potential to be used by a wider audience
[00:17:38] than something like Open Claw, needs to
[00:17:40] be able to observe what Open Claw and
[00:17:42] Hermes users do in order to design the
[00:17:44] right experiences for that broader
[00:17:46] audience.
[00:17:47] And so, if we take that idea, that a big
[00:17:49] part of the importance of things like
[00:17:51] Open Claw and Hermes is to understand
[00:17:53] where we are all headed, I think that
[00:17:55] the most significant update around Open
[00:17:57] Claw is its move to multiplayer. Open
[00:18:00] Claw creator Peter Steinberger posted,
[00:18:02] "Two months ago, we started the mission
[00:18:04] to build Open Claw with Open Claw, and
[00:18:06] bit by bit, we moved everyone from using
[00:18:08] their local coding harness to using
[00:18:10] team.openclaw.ai,
[00:18:13] our shared agent that knows what
[00:18:14] everyone's working on and orchestrates
[00:18:16] it all. Multiplayer coding and infinite
[00:18:18] compute with nodes and cloud sessions
[00:18:20] has been a game changer for how we
[00:18:21] build. Local harnesses feel like relics
[00:18:24] of the past now." Open Claw maintainer
[00:18:26] Colin wrote more extensively about this.
[00:18:28] In a post called from Discord bots to a
[00:18:30] multiplayer agent workspace, Colin
[00:18:32] wrote,
[00:18:33] "We already had agents. We had different
[00:18:35] agents set up in Discord, and they
[00:18:36] worked. We could give them tasks, run
[00:18:38] commands, and interact with our
[00:18:39] development environment from a messaging
[00:18:41] platform we already used every day. But,
[00:18:43] it still felt like messaging a bot. What
[00:18:45] we wanted was a way for both developers
[00:18:47] to see the work itself. If an agent
[00:18:49] paused because it needed clarification,
[00:18:51] either of us should be able to jump in.
[00:18:53] If something needed a second set of
[00:18:55] eyes, we should be able to open the same
[00:18:56] session and look at the same context. No
[00:18:58] screenshots, no copied transcripts, no
[00:19:01] here's what the agent has done so far
[00:19:02] data dump. Just open the work and
[00:19:04] continue. Open Claw's new multiplayer
[00:19:06] web UI is the first time that workflow
[00:19:08] has really clicked for us.
[00:19:10] Now, their first attempt at multiplayer
[00:19:11] was to manage all their agents in a
[00:19:13] shared Discord, but that still lost a
[00:19:15] lot of the features they needed. While
[00:19:16] the coordination happening in the shared
[00:19:18] space was an upgrade, they still
[00:19:19] couldn't really interact with other
[00:19:21] people's agents, like adding context to
[00:19:23] an existing thread or taking over when
[00:19:24] an agent was waiting for input. Indeed,
[00:19:26] Colin said that the moment that
[00:19:27] multiplayer felt real was when they were
[00:19:29] able to share a session while work was
[00:19:31] happening. He writes, "When something
[00:19:33] needed another opinion, we could both
[00:19:35] open the same thread. When the agent
[00:19:37] needed information one of us had, that
[00:19:39] person could add it directly. There was
[00:19:40] no need to copy the conversation into
[00:19:42] Discord, explain what happened, and then
[00:19:43] carry the answer back. We were working
[00:19:45] inside the same context. That sounds
[00:19:48] like a small interface improvement, but
[00:19:49] it changes the way you collaborate with
[00:19:51] an agent. The session stops being a
[00:19:53] private conversation between one
[00:19:54] developer and a model. It becomes a
[00:19:56] shared piece of work that another
[00:19:57] trusted developer can inspect, steer, or
[00:19:59] take over." To get a sense of how big
[00:20:01] the difference is in practice, Colin
[00:20:03] shared how he had been working to set up
[00:20:05] a fresh development server, but needed
[00:20:06] to hand that project over to someone
[00:20:08] else. "Normally," he writes, "that kind
[00:20:10] of handoff requires assembling
[00:20:11] everything I know into a document or a
[00:20:13] long message. Why certain decisions were
[00:20:15] made, which approaches had already
[00:20:16] failed, which state the project was in,
[00:20:18] which details existed only in my head,
[00:20:20] what the agent had already learned.
[00:20:22] Instead," he writes, "the other
[00:20:23] developer started a thread with our
[00:20:24] shared agent. I opened that same thread
[00:20:27] and added the missing context directly.
[00:20:29] The agent, the other developer, and I
[00:20:30] were all working from one continuous
[00:20:32] record. Then they were off and running.
[00:20:34] There was no copy and paste handoff, and
[00:20:36] no attempt to reconstruct a private
[00:20:37] agent conversation. The session itself
[00:20:40] became the handoff document." Now,
[00:20:43] obviously this new multiplayer style
[00:20:44] environment brings up a lot of
[00:20:45] challenges. There are questions of
[00:20:47] ownership and authority and access. And
[00:20:50] as Colin puts it, "This is still early,
[00:20:51] and we're treating it that way." Still,
[00:20:53] he writes, "the direction is exciting."
[00:20:55] Quote, "Most developer agent workflows
[00:20:57] still assume one developer, one
[00:20:59] terminal, and one private conversation.
[00:21:01] The final code may eventually be shared,
[00:21:03] but the process of getting there remains
[00:21:04] hidden inside individual sessions. A
[00:21:06] multiplayer agent workspace makes that
[00:21:08] process collaborative. Another developer
[00:21:11] can see the work, understand the
[00:21:12] context, add what they know, and
[00:21:13] continue from exactly where it stopped.
[00:21:15] No transcript dump, no broken handoff,
[00:21:18] no rebuilding the context from scratch.
[00:21:20] Just one shared place where the
[00:21:21] developers and the agent can keep the
[00:21:23] work moving.
[00:21:24] Now, what's so interesting about this to
[00:21:26] me is that I think it is once again an
[00:21:28] example of Open Claw getting to the
[00:21:30] place that we're going to head next
[00:21:32] before the rest of us. Even as I record
[00:21:34] this, in the background, my coding
[00:21:36] agents are working on the next free AIDB
[00:21:38] learning experience. And that one is not
[00:21:40] just about new individual skills, but a
[00:21:43] new way of building agents that operate
[00:21:45] at the team level. If you take all the
[00:21:47] work you do inside your company, it's
[00:21:48] going to come in two forms. Work you do
[00:21:51] alone, and work you do with others. So
[00:21:53] far, agents have only really been
[00:21:55] designed and enabled for work you do
[00:21:57] alone. And yet, a huge portion of our
[00:21:59] work is work we do together. I think
[00:22:01] that's about to change. I think that's
[00:22:03] the next big development for agents. And
[00:22:05] I think once again, even if you are not
[00:22:06] planning on being an Open Claw user long
[00:22:08] term, checking out the way that they're
[00:22:10] thinking about multiplayer might unlock
[00:22:12] some new ideas.
[00:22:14] More on that project soon, but for now,
[00:22:15] that is going to do it for today's AI
[00:22:17] Daily Brief. Appreciate you listening or
[00:22:19] watching, as always, and until next
[00:22:20] time, peace.
