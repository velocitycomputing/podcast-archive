---
record_id: "podcast:24d15f2c-50bf-4116-9aa5-0b33e0e9f47b"
episode_id: 24d15f2c-50bf-4116-9aa5-0b33e0e9f47b
title: Why a New Class of AI “Judgment Models” Could Have Big Business Implications
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/why-a-new-class-of-ai-judgment-models-could-have-big-business-implications/24d15f2c-50bf-4116-9aa5-0b33e0e9f47b"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/why-a-new-class-of-ai-judgment-models-could-have-big-business-implications/24d15f2c-50bf-4116-9aa5-0b33e0e9f47b"
feed_guid: null
feed_url: "https://anchor.fm/s/f7cac464/podcast/rss"
published_at: null
published_local_date: null
played_date: 2026-09-16
played_at: "2026-09-16T12:00:00Z"
play_count: 1
duration_seconds: 1500
source: pocketcasts-history-browser
played_label: September 16
history_order: 44
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: b63eab5b03ce5805f3766f0dbd1732637ab1db0ed665f113db94bf9db659fbdb
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

Typesafe’s Jev, introduced by Diego Almeida as a new “judgment model” trained with reinforcement learning for calibrated decisions (RLCD), is presented as a non-generative model that returns probabilities, categories, or scores for narrow questions—customer anger, dependency detection, operational changes, lead fit, policy compliance—rather than essays; Almeida claimed it is 20–200x faster, 40–400x cheaper, and output-token-free, while Mike Taylor described it as a smart if-then layer and reported testing 37 documents with 21 questions each, yielding 777 judgments in under 0.7 seconds for about a quarter-cent, and compared it to a linter for knowledge work. Commentary from Michael Lee, Chubby, Nathan Flurry, and Matt Stockton framed Jev as a decision layer between brittle rules and slow LLMs, a possible “LLM proposes, Jev decides, code executes” stack, and a more accessible UX for classic classification/regression problems; the episode also covered AI-safety headlines, including Mark Zuckerberg’s X post that labs should self-pace, Meta’s delayed Muse release, support for independent evaluators, and compute mostly serving people, with reactions from Joseph Carlson, Matthew Bur, Bill Aman, and Kevin Roose; Bernie Sanders and Steve Bannon appeared at the Future of Life Institute’s prohuman assembly, Greg Casar proposed banning systems too powerful to control, and Salesforce’s Dreamforce featured Sam Altman, Jensen Huang, Dario Amodei, and Mark Benioff plus announcements of KOA, a fine-tuned NVIDIA Neotron CRM sales model, and AI Force connectors for third-party agents.

No direct health implications are present; the actionable focus is operational: audit workflows where LLMs are used for classification, routing, scoring, moderation, fraud/risk, support triage, lead qualification, editorial QA, or compliance, and test whether narrow judgment questions plus deterministic code can replace or check them, especially as cheap post-generation validators on every draft or agent action. Research leads include Typesafe’s RLCD architecture, calibration/epistemic honesty, benchmarking the speed/cost claims, integration with LLMs and code, and privacy/security of sending sensitive data to a judgment API; decisions to consider are whether to pilot on low-risk internal workflows, define categories and escalation thresholds, decide when humans must approve consequential actions, and build a model stack where generative models draft while judgment models decide. Follow-up questions should cover false-positive/false-negative costs, model drift, auditability, latency under load, data retention, adversarial or ambiguous inputs, and multiplayer handoffs such as whether a message implies a cross-team commitment, exceeds authority, conflicts with roadmap, or lacks owner approval.

## Transcript

[00:00:00] It's not every day that we get a new
[00:00:01] model to play around with, and it's
[00:00:03] certainly not every day that we get an
[00:00:04] entirely new approach to model building
[00:00:07] with some fairly different implications
[00:00:09] for how we even use it. Today though, we
[00:00:11] are talking about a new class of models,
[00:00:13] which you might refer to as AI judgment
[00:00:15] models. Rather than producing long
[00:00:17] strings of text, these judgment models,
[00:00:19] like the one we're discussing today, Jev
[00:00:21] from Typesafe, produce probabilities
[00:00:23] around specific questions. Is this
[00:00:25] customer angry? Is there a new
[00:00:27] dependency in this email? Do we need to
[00:00:29] change the operational plan because of
[00:00:31] this? Today, we're exploring the idea
[00:00:32] behind these models, how they're trained
[00:00:34] differently, how they can produce these
[00:00:36] judgments much more quickly and much
[00:00:37] less expensively, and most importantly,
[00:00:40] where they're going to fit in your
[00:00:41] overall model stack. The AI Daily Brief
[00:00:44] is a daily podcast and video about the
[00:00:46] most important news and discussions in
[00:00:48] AI. Welcome back to the AI Daily Brief
[00:00:50] headlines edition. All the daily AI news
[00:00:52] you need in around 5 minutes. The AI
[00:00:55] safety discourse continues to trickle
[00:00:57] out through the tech industry as well as
[00:00:59] mainstream society. But for now, unless
[00:01:01] something absolutely seismic happens,
[00:01:03] we're going to move it into the
[00:01:04] headlines and away from the main
[00:01:05] episode. With that in mind, after
[00:01:07] staying quiet over the weekend, Mark
[00:01:09] Zuckerberg has made his thoughts known
[00:01:10] on this idea of an AI slowdown. On
[00:01:13] Tuesday, Zuckerberg wrote in a post on
[00:01:15] X, "Every lab has the responsibility and
[00:01:18] incentive to move at the pace required
[00:01:20] to train its models safely and the
[00:01:22] ability to take its own actions to
[00:01:23] ensure that happens." Basically, his
[00:01:26] view is that pacing is the
[00:01:27] responsibility of individual labs rather
[00:01:29] than a collective action. And that view
[00:01:31] hinges on two core ideas. First, that
[00:01:34] quote, people don't want to use agents
[00:01:36] that are misaligned with them and that
[00:01:38] don't do what they ask, so labs have a
[00:01:39] strong natural incentive to make their
[00:01:41] models more aligned. and two labs face
[00:01:44] significant liability if their models
[00:01:45] cause harm. So they have a strong
[00:01:46] incentive to prevent this as well.
[00:01:48] Emphasizing the point, Zuckerberg said
[00:01:50] that Meta had delayed the release of
[00:01:51] Muse by several months to work on
[00:01:53] safety. He continued, "We didn't call
[00:01:56] for everyone else to do this before we
[00:01:58] would. We just did it as part of our
[00:01:59] day-to-day work because it was clearly
[00:02:01] the right thing for people and for us."
[00:02:03] Essentially, Zuckerberg is saying that
[00:02:05] the individual incentives and
[00:02:07] consequences that are already in place
[00:02:09] are enough to force AI labs to work on
[00:02:12] alignment and to pace the frontier
[00:02:14] correctly rather than needing some
[00:02:16] exogenous government enforced slowdown.
[00:02:18] Now, Zuckerberg did support the idea of
[00:02:20] independent evaluators and advisers as a
[00:02:22] matter of best practice rather than
[00:02:23] regulation. He claimed that Meta has
[00:02:25] already engaged outside evaluators not
[00:02:27] because it's required of them, but
[00:02:29] because it helps produce better work.
[00:02:30] Finally, he concluded, "Committing the
[00:02:32] significant majority of compute towards
[00:02:34] serving people rather than racing
[00:02:36] towards recursive self-improvement is
[00:02:38] one of the best ways to ensure that we
[00:02:39] develop this technology safely. Meta has
[00:02:42] made this commitment and other labs can
[00:02:43] do this as well." I believe the key to
[00:02:45] building a positive future for everyone
[00:02:46] is maintaining the right balance of
[00:02:48] power. This is within our power to do.
[00:02:51] It's carefully worded, but basically
[00:02:52] this whole thing says, "Come on, guys.
[00:02:54] Let's please stop with the theatrics."
[00:02:57] And a lot of people, frankly, found this
[00:02:58] a breath of fresh air. YouTuber Joseph
[00:03:00] Carlson wrote, "Hold up a minute. You
[00:03:02] are telling me companies can slow down,
[00:03:04] make sure things are safe without
[00:03:05] telling all their competitors to slow
[00:03:07] down." And I would say that broadly
[00:03:08] speaking, reactions fell into one of two
[00:03:10] categories. The first was like that one
[00:03:13] and like this from Matthew Bur. Love
[00:03:15] this model safety and alignment is a
[00:03:17] feature and economically incentivized.
[00:03:19] Or Bill Aman who simply called this the
[00:03:21] proper approach to AI development. But
[00:03:23] then on the other side were those
[00:03:24] arguing effectively that Zuckerberg just
[00:03:26] does not have the trust or standing to
[00:03:28] make this argument regardless of the
[00:03:30] merits of the argument itself.
[00:03:31] Hardfork's Kevin Roose wrote, "Whether
[00:03:33] you're a Democrat or a Republican, an EA
[00:03:36] or an EAC, I think we can all agree that
[00:03:38] the person best suited to protect us
[00:03:40] against the harms of powerful new
[00:03:42] technology is Mark Zuckerberg." Now,
[00:03:44] meanwhile, over in Strange Bedfellows
[00:03:47] Daily, Bernie Sanders and Steve Bannon
[00:03:49] have joined forces to call for human
[00:03:51] ccentric AI regulations in the strangest
[00:03:54] alliance of this political cycle. The
[00:03:56] two highly ideological leaders spoke
[00:03:58] from the same stage on Tuesday at the
[00:03:59] Future of Life Institute's prohuman
[00:04:01] assembly in Washington. Sanders told the
[00:04:03] crowd, "If the lives of every man,
[00:04:05] woman, and child are going to be
[00:04:06] fundamentally changed by this
[00:04:07] technology, then the people of this
[00:04:09] country must make decisions about AI and
[00:04:11] not just a handful of oligarchs." Bannon
[00:04:13] had very similar remarks, stating, "The
[00:04:15] American citizens are not going to be
[00:04:16] supplicants to the oligarchs anymore. We
[00:04:18] can't do it. This is a hinge in history.
[00:04:20] We have to handle this correctly. To
[00:04:22] handle it correctly, number one, we can
[00:04:24] never trust what an oligarch says." Now,
[00:04:26] I will note that while this seems
[00:04:28] strange at first, these two highly
[00:04:31] ideologically opposed people sharing the
[00:04:33] same stage. The broader movements they
[00:04:35] connect to have a fair bit of shared
[00:04:37] context in history. The 2016
[00:04:39] presidential election in which Bernie
[00:04:41] was narrowly beaten by Hillary to miss
[00:04:42] out on becoming the Democrat nominee and
[00:04:44] in which Bannon obviously architected
[00:04:46] the first Trump administration both had
[00:04:47] their roots in populist anger at the
[00:04:50] postGFC financial landscape and the lack
[00:04:52] of accountability for the institutions
[00:04:54] and institutional leaders who were
[00:04:56] involved in creating that particular
[00:04:57] economic crisis. Obviously the left and
[00:04:59] the right's reaction to that particular
[00:05:01] context were different. But it is, I
[00:05:03] would contend, perhaps less surprising
[00:05:05] than you think, that at some point these
[00:05:06] two would find common ground. And to be
[00:05:08] clear, I am not dismissing the common
[00:05:10] ground that they find just on the merits
[00:05:11] of this particular issue itself and the
[00:05:13] power of this particular issue to
[00:05:15] scramble existing political alliances.
[00:05:17] I'm just making the point that their
[00:05:18] stories are actually more intertwined
[00:05:19] than you might think at first glance. In
[00:05:21] any case, the event seemed somewhat less
[00:05:23] about the existential risks of AI that
[00:05:25] have filled the headlines this week and
[00:05:26] more about the class struggle the
[00:05:28] technology has come to represent. TV
[00:05:30] screens played a parody interview from a
[00:05:31] fictional AI CEO described as someone
[00:05:34] who loves people but isn't crazy about
[00:05:36] humans. Throughout the event, it seemed
[00:05:37] that AI itself wasn't the risk that
[00:05:39] needs addressing, but rather the
[00:05:40] unchecked power of oligarchs. Now, you
[00:05:43] might remember that back in August,
[00:05:44] journalist Jasmine Sun towards the
[00:05:46] country speaking to real people who were
[00:05:47] working in opposition to data centers
[00:05:49] and found that the most common complaint
[00:05:51] was not about electricity, water use, or
[00:05:53] noise pollution, but a lack of control
[00:05:55] in the sense that the future was being
[00:05:57] forced upon their communities with
[00:05:58] little input. The same was true about
[00:06:00] this event. Across multiple speakers,
[00:06:02] the risk of AI was not framed around
[00:06:04] cyber security, bioteterrorism, or other
[00:06:06] ex- risks. It was about a lack of agency
[00:06:09] in determining the shape of the future.
[00:06:11] From this followed their main concern,
[00:06:12] which was simply the idea of losing
[00:06:14] control of AI. As Texas Democrat Greg
[00:06:17] Casar, who is sponsoring Bernie Sanders
[00:06:18] super intelligence bill, said, "The
[00:06:20] answer is simple. We ban AI systems that
[00:06:23] are too powerful for humans to control."
[00:06:25] And as strange as it might seem, despite
[00:06:28] all the intensity of this rhetoric
[00:06:29] recently, I still contend that we've
[00:06:31] moved into a new phase that's all about
[00:06:33] negotiating the relationship where
[00:06:35] citizens and governments have a stake in
[00:06:36] this and where given that that is now
[00:06:38] pretty much where everyone is, the next
[00:06:40] phase is likely to include a lot more
[00:06:42] specificity and dare I say nuance. Glenn
[00:06:45] Beck, for example, had a long monologue
[00:06:47] on his show about how he can both have
[00:06:49] signed the prohuman AI declaration
[00:06:51] alongside them, but also disagree with
[00:06:53] them on specifics of data centers. And
[00:06:54] honestly, as crazy as it sounds, I think
[00:06:56] that the more that the political
[00:06:58] discourse kind of frags your brain for
[00:06:59] how confusing and all over the place it
[00:07:01] is, that might just be a sign that we're
[00:07:03] actually making progress. The
[00:07:04] conversation also found its way into
[00:07:06] Salesforce's annual Dreamforce event
[00:07:08] where the company unveiled a new AI
[00:07:11] model, but where a lot of the chatter on
[00:07:12] social media focused on appearances from
[00:07:14] Sam Alman, Jensen Huang, and Dario
[00:07:16] Amade, who each iterated their own
[00:07:18] safety views. Daario argued that he was
[00:07:20] just trying to put forward a set of
[00:07:21] standards that the industry could
[00:07:22] organize around. While Altman said that
[00:07:24] he was very confident in our company's
[00:07:26] ability and our industry's ability to do
[00:07:28] this safely, Jensen Wong, meanwhile,
[00:07:30] reiterated the Zuckerbergian view,
[00:07:32] saying, "Run as fast as you can, but if
[00:07:33] you feel at any given point in time the
[00:07:35] company's out of control or the
[00:07:36] product's not going to be safe, take a
[00:07:38] pause and make sure you get it right."
[00:07:40] And as for Salesforce CEO Mark Beni off,
[00:07:42] he believes that every company has a
[00:07:43] responsibility to uphold ethical
[00:07:45] standards. Still, to give the safety
[00:07:46] debate a bit of a rest, Salesforce also
[00:07:49] had two big practical AI announcements.
[00:07:51] First, they're releasing their first
[00:07:53] in-house model in quite some time called
[00:07:55] KOA. The model is a fine-tune of
[00:07:57] NVIDIA's Neotron and is designed to
[00:07:59] handle sales management within the CRM.
[00:08:01] The announcement reinforces the role
[00:08:02] that opensource has to play in the
[00:08:04] enterprise by enabling this sort of
[00:08:05] narrow vertical model. Secondly,
[00:08:07] Salesforce unveiled a new initiative
[00:08:09] called AI Force. This will be the
[00:08:11] umbrella term for Salesforce's
[00:08:12] connectors that will allow third party
[00:08:13] agents to access Salesforce data. The
[00:08:16] release reinforces Salesforce commitment
[00:08:17] to moving towards headless software in a
[00:08:19] platform agnostic way allowing any agent
[00:08:21] to become the interface. Now obviously
[00:08:23] these are big conversations that are
[00:08:25] important and are going to continue but
[00:08:26] for now that is where we will close the
[00:08:28] headlines. Next up the main episode.
[00:08:31] Welcome back to the AI daily brief. On
[00:08:33] today's main episode we are looking at
[00:08:35] something really different and quite
[00:08:37] rare which is in short a totally
[00:08:40] different approach to AI that is not
[00:08:43] just another LLM. Now, in the nearly
[00:08:46] four years since Chat GBT was released
[00:08:48] and the three and a half that the show
[00:08:49] has been around, the vast majority of
[00:08:50] the things that we and the rest of the
[00:08:52] industry have focused on have been in
[00:08:54] some ways related to large language
[00:08:55] models. And yet, as some have pointed
[00:08:58] out, although often in a way that didn't
[00:09:00] get much traction and was more or less
[00:09:01] screaming into the void, LLMs are not in
[00:09:03] fact the totality of artificial
[00:09:05] intelligence. Yesterday, Diego Almeida
[00:09:08] posted on X, "After co-inventing chatbt,
[00:09:12] I kept asking myself, why have
[00:09:14] superhuman chat models not led to AGI?
[00:09:16] I've spent the last 2 years in stealth
[00:09:18] building a new way to train models,
[00:09:20] RLCD, or reinforcement learning for
[00:09:22] calibrated decisions and a new type of
[00:09:25] frontier AI model that we are releasing
[00:09:27] today, Jev. Jev is 20 to 200 times
[00:09:30] faster, 40 to 400 times cheaper with
[00:09:33] output tokens free. Frontier composable
[00:09:36] intelligence optimized for decisions. As
[00:09:39] far as I can tell, the shortest path to
[00:09:41] AI based economic revolution.
[00:09:44] Now, one could absolutely be forgiven
[00:09:46] for seeing numbers like 20 to 200 times
[00:09:48] faster and 40 to 400 times cheaper and
[00:09:50] being a bit skeptical of the claims to
[00:09:52] say the least. And were this just
[00:09:54] another LLM, that skepticism would be
[00:09:57] entirely warranted. However, with Jev
[00:09:59] and this new strategy, we're dealing
[00:10:01] with something that is quite different.
[00:10:03] The company behind Jev is called
[00:10:04] Typesafe, and in the announcement blog
[00:10:06] post, they talk a little bit more about
[00:10:07] what makes their approach different.
[00:10:09] They write, "We built a new stack
[00:10:11] entirely focused on automation with a
[00:10:13] new model architecture, parallel sampler
[00:10:14] for maximum efficiency, and training
[00:10:16] method we call reinforcement learning
[00:10:18] for calibrated decisions." Whereas
[00:10:20] existing LLMs optimize for human
[00:10:22] preference, i.e. write-ups and chat
[00:10:24] responses that human raiders prefer. The
[00:10:26] new system one models, the first of
[00:10:28] which is Jev, optimized for calibrated
[00:10:30] decisions or answers with epistemically
[00:10:33] honest probabilities. So what does that
[00:10:36] actually mean? Well, let's look at how
[00:10:37] Mike Taylor from Every describes it. He
[00:10:40] writes, "Think of it as a smart if then
[00:10:42] statement that determines what happens
[00:10:44] next when you're automating a workflow.
[00:10:46] Say you're building software that
[00:10:48] prioritizes customer service requests
[00:10:50] and you write code that asks the model,
[00:10:51] "Does this customer sound angry?" Jev
[00:10:54] might answer 0.9, which means there's an
[00:10:57] estimated 90% probability that the
[00:10:59] answer is yes based on what the model
[00:11:00] learned in training. You could also
[00:11:02] provide categories you define like
[00:11:04] annoyed, irritated, offended, furious,
[00:11:06] and enraged, and learn that the customer
[00:11:08] was 60% likely to be classified as
[00:11:10] furious with only a 10% probability of
[00:11:12] being enraged. Going on to explain why
[00:11:15] this matters and how it differs than
[00:11:16] LLMs. Mike continues, "With an answer of
[00:11:19] 0.9, very likely to be angry, the
[00:11:22] software might automatically proceed to
[00:11:24] escalate the customer concern to a
[00:11:26] manager. Or if it answers 0.1, not
[00:11:29] likely to be angry, that request might
[00:11:31] be deprioritized. However, chat bots are
[00:11:34] trained to respond with flowery text
[00:11:36] like, "You're absolutely right. This
[00:11:38] customer does sound very angry. Would
[00:11:40] you like me to compose a draft email
[00:11:41] response in a friendly, supportive tone?
[00:11:43] This text response would cause the
[00:11:45] program you're building to crash because
[00:11:46] it was expecting a number between zero
[00:11:48] and one, not an essay. Teal fellow
[00:11:50] Michael Lee says, "This allows a class
[00:11:52] of decision-making that was neither
[00:11:54] suited to dumb, unintelligent code nor
[00:11:56] to slow, expensive LLMs." As Chubby sums
[00:11:59] up, Jev is an AI model built for
[00:12:01] decisions rather than text generation.
[00:12:04] And it is important to note that the
[00:12:06] trade-off here is that this model does
[00:12:08] not generate text. It is not, in other
[00:12:11] words, a replacement for LLMs in
[00:12:13] general. It's a replacement for a
[00:12:15] certain category of work that LLMs do
[00:12:18] where they've been very square peg
[00:12:20] mashed into a round hole to do it. The
[00:12:22] idea continues, chubby, is to embed
[00:12:24] fast, cheap AI decisions into software.
[00:12:27] So, what is this model actually built
[00:12:29] for? Well, think of how much of office
[00:12:31] work consists of reading something and
[00:12:33] deciding what should happen next. Does
[00:12:35] this message need a response? Which
[00:12:37] department should handle it? Does this
[00:12:38] document answer the question? Is this
[00:12:40] customer describing a bug or asking for
[00:12:42] a feature? Does this draft make a claim
[00:12:44] its source doesn't support? Is the
[00:12:46] situation routine enough to automate or
[00:12:47] should someone review it? These are
[00:12:49] judgments about meaning, and they're
[00:12:51] often difficult to express as fixed
[00:12:52] rules. Jeb then is designed to take the
[00:12:55] relevant information and answer narrowly
[00:12:57] defined questions with probabilities,
[00:12:59] categories, or scores. The surrounding
[00:13:02] software then uses those answers to
[00:13:03] route, rank, flag, or proceed. In the
[00:13:05] type safe documentation, they explicitly
[00:13:08] recommend breaking complex decisions
[00:13:10] into small questions and then combining
[00:13:12] their results in code. So where would
[00:13:14] this show up in normal business? One
[00:13:16] obvious area is customer support where
[00:13:18] the small judgment the model could make
[00:13:20] would be something like is the customer
[00:13:22] frustrated and have previous replies
[00:13:24] failed to address it. With those small
[00:13:26] judgments in hand, the software could
[00:13:28] then next route the ticket, raise its
[00:13:29] priority or request human review. In the
[00:13:32] sales domain, the model could judge, is
[00:13:34] this a buying inquiry? Does the prospect
[00:13:36] fit the product? Are they requesting a
[00:13:38] meeting? The software could then take
[00:13:40] those judgments to sort inbound leads
[00:13:42] and assign follow-up. In marketing and
[00:13:44] editorial, the model might judge whether
[00:13:46] the copy meets specific style rules or
[00:13:48] whether the offer is clear. The software
[00:13:50] that surrounds it could then flag
[00:13:52] passages for revision before
[00:13:53] publication. And importantly, where a
[00:13:56] lot of people went was not just
[00:13:57] understanding where they would use this
[00:13:59] instead of LLMs, but how they might use
[00:14:01] it alongside LLMs. YC founder Nathan
[00:14:04] Flurry wrote, "I'd imagine a lot of
[00:14:06] workflows that look like LLM proposes
[00:14:09] options, Jev decides, code executes." To
[00:14:12] put a clear example on this, imagine
[00:14:13] that a customer writes, "This is the
[00:14:15] third time I've contacted you. We still
[00:14:17] can't export our reports, and our
[00:14:19] renewal is next week." A support
[00:14:21] workflow supported by something like Jev
[00:14:23] could ask several questions together.
[00:14:25] One, is the customer describing a
[00:14:27] product problem? Two, does the message
[00:14:29] indicate repeated unsuccessful support?
[00:14:31] Three, is a commercially significant
[00:14:33] deadline approaching? Four, which team
[00:14:35] is best equipped to help? The software
[00:14:37] that surrounds it could then combine
[00:14:39] those signals with actual account
[00:14:40] information, such as the renewal date,
[00:14:42] and escalate the ticket. From there, you
[00:14:45] would still have a generative model
[00:14:46] draft the reply, but Jev once again
[00:14:48] could check the draft against narrow
[00:14:51] criteria. Does the response acknowledge
[00:14:53] the repeated contacts? Does it address
[00:14:55] the export problem? Does it promise
[00:14:58] something unsupported by the information
[00:14:59] provided? And part of what people are
[00:15:02] excited about opening up with this new
[00:15:03] approach is that cheap judgment makes
[00:15:06] frequent checking more practical. If a
[00:15:09] check adds a noticeable delay or
[00:15:11] expense, a team may run it only on
[00:15:13] selected cases or at the end of a task.
[00:15:15] If it becomes sufficiently fast and
[00:15:17] inexpensive, it could run on every
[00:15:19] incoming request after each draft
[00:15:21] revision across many candidate documents
[00:15:23] before an agent takes a consequential
[00:15:25] step. Back in Mike Taylor's article from
[00:15:27] Every, he gave Jeb the text from all 27
[00:15:29] of his articles alongside 10
[00:15:32] deliberately AI styled counterpoints,
[00:15:34] then asked the same 21 questions
[00:15:36] concurrently across all articles to
[00:15:38] check for AI tells. Basically, the check
[00:15:40] that he was doing with Jev was, does
[00:15:42] this essay do specific things that
[00:15:44] indicate to people that it is AI
[00:15:46] composed? Things like, does the text
[00:15:48] repeat an idea without adding evidence?
[00:15:50] Does it force a symmetrical both sides
[00:15:52] argument? Does it overexlain a
[00:15:53] straightforward point? In less than 0.7
[00:15:56] seconds, Mike said, Jev quote unquote
[00:15:59] read all 37 documents and answered all
[00:16:01] 21 questions for each, returning 777
[00:16:04] judgments for an estimated quarter of a
[00:16:06] cent. As he points out, that's fast and
[00:16:09] cheap enough to AI check everything
[00:16:11] everyone at your company has ever
[00:16:12] written and get the results back in an
[00:16:13] instant. A comparison that Mike makes is
[00:16:16] a code llinter for knowledge work. He
[00:16:18] writes, "In software development, a code
[00:16:20] llinter is a tool that analyzes your
[00:16:22] work and almost instantly flags syntax
[00:16:24] errors, catches bugs, spots bad
[00:16:26] patterns, and enforces stylistic
[00:16:28] consistency. Typesafe's model is so fast
[00:16:30] at turning fuzzy tasks into clear
[00:16:32] structured answers that it could act as
[00:16:34] a kind of code llinter for knowledge
[00:16:36] work. Give Codeex or Claude access to
[00:16:38] Jev and a list of questions, and it can
[00:16:40] quickly check its own work for problems
[00:16:42] you've told it to avoid. Parenrat says
[00:16:45] most software is ultimately a giant tree
[00:16:47] of if this do that. If this route here,
[00:16:49] if this escalate, if this reject, if
[00:16:51] this, ask a human. Jeb is basically
[00:16:53] asking, what if those if statements
[00:16:55] could understand messy human context?
[00:16:57] That's a much more interesting framing
[00:16:59] than another AI model. I can see this
[00:17:01] being very useful for fraud and risk,
[00:17:03] support routing, moderation, PR and QA
[00:17:05] automation, lead scoring, compliance,
[00:17:07] workflow orchestration, and agent
[00:17:08] routing. Early tech obviously he says
[00:17:10] but the category itself makes a lot of
[00:17:12] sense. Now interestingly Matt Stockton
[00:17:15] points out that in some ways companies
[00:17:18] adopting this amounts to a postlm AI
[00:17:21] technology making prelim machine
[00:17:24] learning techniques a little bit more
[00:17:26] accessible. As he writes lots and lots
[00:17:28] of problems in business are
[00:17:30] classification or regression problems.
[00:17:32] Lots and lots of companies don't know
[00:17:33] that the types of problems they have are
[00:17:35] solvable by classic machine learning
[00:17:37] methods. They often solve them with
[00:17:38] people in process instead of technology.
[00:17:40] With the emergence and popularity of
[00:17:42] LLMs, more companies are thinking maybe
[00:17:44] we can use AI for that and are solving
[00:17:46] classification and regression problems
[00:17:47] with LLMs. This is good in some ways
[00:17:50] because companies are potentially
[00:17:51] automating some manual work, but also
[00:17:53] bad in some ways because it's often the
[00:17:54] wrong tool for the job and possibly not
[00:17:56] as good as classic ML methods for what
[00:17:58] they are trying to do. But he points out
[00:18:00] the classical techniques require you to
[00:18:02] label your data, train a model, and host
[00:18:03] that model somewhere. they aren't as
[00:18:05] easy to use compared to calling an LLM
[00:18:07] API. And it requires you in your org to
[00:18:09] be aware of those techniques and capable
[00:18:10] of investing in them. Without going too
[00:18:12] far on the analogy, he basically says
[00:18:14] one way to look at Jev is as a UX for
[00:18:17] using LLM style user interaction
[00:18:19] patterns for classical ML techniques.
[00:18:21] Now, one interesting question that comes
[00:18:23] up is whether this is for individuals or
[00:18:25] teams building systems. And the short
[00:18:27] answer is that while it is absolutely
[00:18:28] both, it also puts a fine point on the
[00:18:31] multiplayer AI themes that we've been
[00:18:32] talking about recently. Certainly,
[00:18:34] individuals could use this sort of
[00:18:35] capability to have personal tools that
[00:18:37] sort an inbox against their own
[00:18:39] priorities, check drafts of their
[00:18:40] writing against an editorial rubric,
[00:18:42] rank saved articles against research
[00:18:44] interests, or flag commitments in
[00:18:46] meeting transcripts, things like that
[00:18:48] that are going to personally help you do
[00:18:49] your work better. But I think that where
[00:18:50] this sort of technique is going to
[00:18:52] really shine is in the domain of
[00:18:54] teamwork that happens through small
[00:18:56] judgments about who needs to know, who
[00:18:58] should act, and whose approval is
[00:19:00] required. When an agent is serving a
[00:19:02] single person, it gets pretty far simply
[00:19:04] by learning that person's preferences.
[00:19:06] An agent operating across a team,
[00:19:08] however, needs to understand the
[00:19:09] relationships between people's work.
[00:19:11] That creates a different set of
[00:19:13] questions. Who owns this? Whose work
[00:19:15] does this affect? Is someone waiting on
[00:19:16] this decision? Does this promise create
[00:19:18] an obligation for another team? Can the
[00:19:20] current owner decide or does this need
[00:19:21] broader agreement? In some ways, the
[00:19:23] interesting unit of work becomes the
[00:19:25] handoff. Consider a salesperson telling
[00:19:27] a customer, "We should be able to
[00:19:28] support that integration before your
[00:19:30] renewal." For the salesperson's personal
[00:19:32] agent, the next steps might be
[00:19:33] straightforward. Update the account
[00:19:35] record, draft a follow-up, and create a
[00:19:37] reminder. But inside the organization,
[00:19:39] that sentence implicates several
[00:19:41] responsibilities. For the sales folks,
[00:19:43] that sentence means for them a potential
[00:19:45] way to secure the renewal, i.e.
[00:19:46] supporting that integration. For
[00:19:48] engineering, that sentence means a
[00:19:50] possible delivery commitment involving
[00:19:51] uncertain work. For product, it means a
[00:19:53] potential change to roadmap priorities.
[00:19:55] And for customer success, it's an
[00:19:57] expectation they may have to manage. A
[00:19:59] multiplayer agent would need to
[00:20:00] recognize the sentence as a possible
[00:20:02] cross team commitment. And a judgment
[00:20:04] model could assess specific questions.
[00:20:06] Does this message imply a delivery
[00:20:08] promise? Does the promise concern work
[00:20:10] outside the speaker's authority? Does it
[00:20:12] conflict with the supplied road map? Is
[00:20:14] there evidence that the responsible team
[00:20:15] agreed? The larger system could then
[00:20:17] create a proposed commitment, identify
[00:20:19] the necessary owners, and request the
[00:20:21] missing decisions. Now again to
[00:20:23] reinforce costs and benefits the big
[00:20:25] cost of Jev and this type of judgment
[00:20:27] model in general to the extent that this
[00:20:29] becomes a category is that it is an
[00:20:31] incomplete category by definition. It
[00:20:33] cannot do all the work that we currently
[00:20:35] have generative AIs do. Judgment models
[00:20:38] are going to have to be part of a more
[00:20:40] complex model architecture. The type of
[00:20:43] model stack that we've been discussing
[00:20:44] for the last several months. The benefit
[00:20:46] of course though is that it can do this
[00:20:48] extraordinarily inexpensively. And
[00:20:51] because this sort of judgment
[00:20:52] intelligence can be applied so cheaply,
[00:20:54] it means that done well, it can be
[00:20:56] integrated incredibly deeply into the
[00:20:59] automated systems we're all building.
[00:21:01] This is obviously just the first day of
[00:21:02] a very new concept and a concept which
[00:21:04] is significant enough that this very
[00:21:06] competent team has spent 2 years working
[00:21:07] on. So obviously we're going to need to
[00:21:09] see how it all plays out in practice.
[00:21:11] But it does have the feel when you dig
[00:21:12] in of something both important and
[00:21:15] obvious. the type of thing that once it
[00:21:17] exists, we will be surprised in the
[00:21:19] future that we didn't have it for so
[00:21:21] long. Certainly, I'm going to be keeping
[00:21:22] an eye on this and I will continue to
[00:21:24] look out for more examples of how people
[00:21:26] are using it as well as where companies
[00:21:28] are running into challenges as they try
[00:21:29] to build these new types of systems. For
[00:21:31] now, though, very cool stuff to go check
[00:21:33] out. And that's going to do it for
[00:21:34] today's AI daily brief. Appreciate you
[00:21:36] listening or watching as always and
[00:21:38] until next time, peace.
