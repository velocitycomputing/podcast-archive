---
record_id: "podcast:432d1e30-bfb8-4661-895a-b463886b21e0"
episode_id: 432d1e30-bfb8-4661-895a-b463886b21e0
title: Agent Wars!
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/agent-wars/432d1e30-bfb8-4661-895a-b463886b21e0"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/agent-wars/432d1e30-bfb8-4661-895a-b463886b21e0"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-09-22
played_at: "2026-09-22T12:00:00Z"
play_count: 1
duration_seconds: 1800
source: pocketcasts-history-browser
played_label: September 22
history_order: 18
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: a5ffa7ed5bfd2de59be158bd0ae9d853be2e8400802f735e3fa6488f0fccf001
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

The episode's headlines covered three items. SpaceX AI released Grok 4.7, which beats GPT 5.6 Soul on CursorBench 4.0 coding and ranks fourth on Artificial Analysis's coding agent index. Public testing was poor: the 3D render tests were bad, and Theo said real-world costs came out more than 2x Grok 4.6's, above Astra's cost. Treasury Secretary Scott Bessent told CNBC that the Hugging Face incident was OpenAI management's responsibility, not rogue agents. He rejected the labs' reported ask for a liability shield, which drew both support and the objection that catastrophic risks bankrupt any company (the "judgment proof" argument). The Information reported that OpenAI and Anthropic got as far as formal contracting on a deal to safety-test each other's models, then dropped it. The main topic was the "agent wars." Meta's Muse personal agent overtook ChatGPT as the number one free US app, and Bloomberg credited it with lifting AMD and Intel stock. Users reported it buying socks, ordering groceries and canceling about $200 of subscriptions. On Sunday Amazon blocked Muse from shopping on its sites, citing its conditions of use. Commentators read this as Amazon protecting its roughly $76 billion ad business, since agents don't view ads, and as an example of aggregators being aggregated. Amazon also sued Perplexity in November over agent blockers. Shopify partnered with Meta on Monday to support Muse with Shop Pay agentic checkout. Commentators expected a revenue-sharing deal between Meta and Amazon, and some warned that per-agent access fees would favor large companies. Mastercard joined Visa in supporting virtual cards for agents. The host and skeptics such as Ron Johnson, Dave Gerard and Adam Foroughi doubt that agentic shopping will matter much, since many people enjoy browsing and the tasks aren't hard. The host says humility is needed on that question. The transcript cuts off before the rest of his argument.

For you, the practical takeaways are mostly to wait and watch. Don't judge Grok 4.7 yet. The host advises waiting a few days to see how it does in Grokbot. If you were considering it as a cheap workhorse model, test it on your own tasks and measure real token cost, not benchmark claims, because early reports found it slower and costlier than 4.6. If you try Muse or any personal agent, remember that it needs your email, calendar, payment and login access. Start with low-stakes tasks, review what it decided (Bustamante accepted a burger recommendation without scrutiny), and expect it to be blocked on Amazon for now but to work on Shopify stores. If you build or sell online, the episode suggests offering clean APIs or agent-friendly checkout, since smaller players that do will get agent-routed demand. It also suggests watching for paid agent-access deals between platforms. On AI policy, track the liability-versus-regulation debate, because Bessent's stance points toward lab liability and away from a government backstop. A cross-lab safety-testing arrangement is also still being discussed.

## Transcript

[00:00:00] And just like that, the AI agent wars
[00:00:02] have begun.
[00:00:03] Meta's new personal agent has been a
[00:00:05] breakout consumer success. This week the
[00:00:08] app surged over ChatGPT to be the number
[00:00:10] one free app in the US, and there are
[00:00:12] reports from satisfied users all over
[00:00:14] social media. But with that sort of
[00:00:16] success brings competition. And this
[00:00:18] weekend Amazon decided to cut off Muse's
[00:00:20] ability to shop on Amazon sites. Will
[00:00:23] that impact Muse's momentum? Does
[00:00:25] agentic shopping even matter? As
[00:00:27] personal agents become a thing, we have
[00:00:29] a whole new set of questions to explore.
[00:00:32] The AI Daily Brief is a daily podcast
[00:00:34] and video about the most important news
[00:00:35] and discussions in AI.
[00:00:38] Welcome back to the AI Daily Brief
[00:00:39] Headlines edition. All the daily AI news
[00:00:41] you need in around 5 minutes. SpaceX AI
[00:00:44] has kicked off what could be a big week
[00:00:46] for model releases with the launch of
[00:00:48] Grok 4.7. They call the model a notable
[00:00:51] improvement over Grok 4.6 at the same
[00:00:53] price and speed. Now, Grok models in
[00:00:56] general are competing in the
[00:00:57] increasingly difficult middle ground
[00:00:59] between ultra cheap and cutting-edge
[00:01:01] frontier. Grok 4.6 lagged behind GPT 5.6
[00:01:04] Soul and Fable 5.1 on performance and
[00:01:07] was outcompeted on cost by Muse 1.2.
[00:01:09] Still, the model had its fans and was
[00:01:11] clearly capable of driving the success
[00:01:13] of Grokbot. And what's more, for many
[00:01:15] people, showed that SpaceX AI was very
[00:01:17] much not out of the model race. This
[00:01:20] release sees some significant
[00:01:21] improvements at least on the benchmarks.
[00:01:23] For coding, Grok 4.7 picked up six
[00:01:26] points on CursorBench 4.0 to overtake
[00:01:28] GPT 5.6 Soul, but is still five points
[00:01:31] short of Fable 5.1 score. On Deep Suite,
[00:01:33] the model improved by six points to
[00:01:35] overtake Fable 5.1, coming in just short
[00:01:37] of GPT 5.6 Soul. Purely on the
[00:01:40] benchmarks then, Grok 4.7 looks like it
[00:01:42] should be a competitive coding model at
[00:01:44] a discount price. SpaceX highlighted
[00:01:46] significant improvements on long-horizon
[00:01:48] agentic work. For Double A Briefcase,
[00:01:50] which measures multi-hour white-collar
[00:01:51] work, the model scored 1,657 Elo points,
[00:01:55] putting it ahead of GPT 5.6 Soul and
[00:01:57] very close behind Fable 5.1. Benchmark
[00:01:59] scores for legal, electrical
[00:02:00] engineering, and healthcare were
[00:02:02] similarly impressive. In a practical
[00:02:04] demonstration of the upgrade, SpaceX AI
[00:02:06] showed off a head-to-head comparison of
[00:02:07] an open game world. Grok 4.6's version
[00:02:10] was pretty low quality and unimpressive,
[00:02:12] while Grok 4.7 did a noticeably better
[00:02:14] job on both graphics and physics.
[00:02:17] Artificial Analysis gave the model a
[00:02:18] fairly favorable review, ranking it
[00:02:21] seventh on their intelligence index
[00:02:22] behind Astra, two iterations of Fable,
[00:02:25] Opus, MuSpark 1.3, and GPT5.6 Soul. And
[00:02:28] on the coding agent index, it was ranked
[00:02:30] fourth, inching ahead of GPT5.6 Soul,
[00:02:33] but falling short of Opus, Astra, and
[00:02:34] Fable 5.1. Elon Musk celebrated the
[00:02:37] result, declaring that SpaceX AI is now
[00:02:39] the third-place lab for agent decoding
[00:02:41] behind OpenAI and Anthropic. He wrote,
[00:02:44] "When factoring in that Grok is
[00:02:45] significantly faster and lower cost,
[00:02:48] it's a great choice for your everyday
[00:02:49] workhorse."
[00:02:51] Yet, as is sometimes the case,
[00:02:53] benchmarks appear not to tell the full
[00:02:55] story, and the model's initial
[00:02:56] impressions didn't survive contact with
[00:02:58] public testing. Bobby showed his results
[00:03:01] in an AI rendering test against Kimmi
[00:03:03] K3, with both models tasked with
[00:03:05] animating a rocket takeoff. Grok's
[00:03:07] animation was fairly bizarre, with the
[00:03:09] screen wobbling all over, leading Bobby
[00:03:11] to ask, "What's wrong with Grok?" Scott
[00:03:14] animated a star-shaped Jell-O mold, and
[00:03:16] while he gave the render a passing
[00:03:17] grade, he noted it took 40 minutes,
[00:03:20] while Astra's version of the test took
[00:03:21] just 5 minutes. And Theo declared that
[00:03:23] Grok's version of his fish game was the
[00:03:25] quote I've seen this year.
[00:03:27] A few people did have slightly more
[00:03:29] positive rendering results. Open Claw
[00:03:31] maintainer Tac showed off a pretty slick
[00:03:32] animation made in Blender, although his
[00:03:34] prompt was just to make something cool
[00:03:36] that can be accomplished in 10 minutes.
[00:03:38] But, of course, if you're sitting here
[00:03:39] thinking to yourself, are we really
[00:03:41] going to judge a new model based on 3D
[00:03:42] renders that are completely outside the
[00:03:44] use cases of most people? I think that's
[00:03:46] a fairly decent thing to ask. AI
[00:03:48] developer Kun Chen came to the defense
[00:03:50] of Grok, commenting, "Ignore the reports
[00:03:53] that say it's terrible and the only
[00:03:54] thing they reference is a public
[00:03:55] benchmark. The same benchmarks told us
[00:03:57] Opus 5 was better than Fable. They are
[00:03:59] useless. Also, ignore the reports that
[00:04:01] compare models with 3D games. That's not
[00:04:03] real work. It's made for attention on
[00:04:05] social media. I used Grok 4.7 for a
[00:04:07] whole day as my first mate and it has
[00:04:09] been a really solid model with visible
[00:04:11] improvements over 4.5." Cut noted, "I'm
[00:04:13] ignoring 4.6 because 4.5 has been
[00:04:16] working better in my experience.
[00:04:18] Still, overall, the first impression
[00:04:20] verdict on Twitter is not good. V
[00:04:23] posted, "So, let me get this straight.
[00:04:25] After releasing Grok 4.6 a month
[00:04:27] earlier, Elon spent 10 days teasing an
[00:04:29] imminent Grok 4.7 release only to
[00:04:31] postpone it and then shift the narrative
[00:04:33] from pacing AI to vague claims about how
[00:04:35] 4.7 and 4.8 would be Fable killers. Now,
[00:04:37] Grok 4.7 is finally out and it's giving
[00:04:40] Temu Sonic 5 vibes. Believing benchmarks
[00:04:42] in September should be a crime."
[00:04:44] In some ways, I think the trajectory of
[00:04:46] the latest Grok models shows how
[00:04:48] difficult this middle space between
[00:04:50] state-of-the-art and really, really
[00:04:51] cheap actually is. AI entrepreneur and
[00:04:54] content creator Theo wrote, "Grok 4.5
[00:04:56] was an incredible model for the price.
[00:04:58] Fast, pleasant to use, reliable, solid
[00:05:00] default model. Grok 4.6 was a forgivable
[00:05:04] step in the wrong direction in my
[00:05:05] opinion. Slower and more expensive,
[00:05:07] using way more tokens per task for a
[00:05:08] slight edge in intelligence. I get it
[00:05:10] though, they have to climb benchmarks.
[00:05:12] Grok 4.7 is much harder to forgive. They
[00:05:15] claimed it would be more token efficient
[00:05:16] and it's less by 30 to 80%. It scores
[00:05:19] worse than Grok 4.6 in various
[00:05:21] benchmarks. It's slower, it's less
[00:05:22] pleasant to use, and real-world costs
[00:05:24] come out to more than 2x above Grok 4.6,
[00:05:27] putting it over Astra's cost in
[00:05:29] real-world use. This was a very
[00:05:31] disappointing release. I hope that the
[00:05:32] SpaceX AI team can acknowledge that and
[00:05:34] impress us with the next one."
[00:05:36] Now, I will certainly say before you
[00:05:37] jump to judgment, I would wait a couple
[00:05:39] days to see how it performs,
[00:05:40] particularly in its native environment
[00:05:42] of Grokbot, but as of right now, just
[00:05:44] about a day in, that's where the
[00:05:46] conversation stands.
[00:05:48] Next up, Treasury Secretary Scott
[00:05:49] Bessent seems to be trying to shift the
[00:05:51] narrative on safety, rejecting the idea
[00:05:53] of rogue agents, and insisting that AI
[00:05:56] companies need to bear responsibility.
[00:05:58] In an interview with CNBC, Bessent said,
[00:06:01] "The Hugging Face incident, that is the
[00:06:02] responsibility of the OpenAI management,
[00:06:04] not a bunch of agents. It is humans who
[00:06:06] are responsible, not the AI." Now, these
[00:06:09] comments are fairly consequential. As
[00:06:11] Bessent has found himself as more or
[00:06:13] less leading the administration's AI
[00:06:15] policy. He was also extremely credulous
[00:06:17] about AI risk during the release of
[00:06:18] Mythos, so was the most likely to
[00:06:20] support the current regulatory
[00:06:21] proposals, but it seems he just isn't
[00:06:24] buying it. He said,
[00:06:26] "A sitting employee came out, said
[00:06:27] there's a 10% chance of an
[00:06:28] extinction-level event. But then the
[00:06:30] labs also said, 'Take the liability off
[00:06:32] of our hands, and we will not do that.'
[00:06:34] What the president was saying is that we
[00:06:35] cannot say we absolve you of
[00:06:36] responsibility, and the government is
[00:06:38] going to take responsibility. These labs
[00:06:40] need to take responsibility for
[00:06:41] themselves. They can slow down anytime
[00:06:43] they want to."
[00:06:44] Now, presumably there are a lot of
[00:06:46] discussions going on behind closed doors
[00:06:47] right now. It's entirely unclear whether
[00:06:49] Bessent is speaking to a proposal put
[00:06:51] forward by the labs, or if discussions
[00:06:53] with advisers have led him to believe
[00:06:55] the labs are looking for liability
[00:06:56] protection. Still, the Treasury
[00:06:58] Secretary could not have been clearer
[00:06:59] about the administration's position. He
[00:07:01] continued, "What did they try to do last
[00:07:03] week? It was, 'Well, there's a 10%
[00:07:05] chance we destroy the world, but we want
[00:07:07] the government to give us a liability
[00:07:08] shield.' That's good business for them,
[00:07:10] bad business for the American people."
[00:07:12] For some, the response to this was a
[00:07:13] solemn head nod, and a sturdy good.
[00:07:16] Investor Bill Gurley wrote,
[00:07:17] "Consequences will both harden the
[00:07:19] product and reduce the press releases
[00:07:20] where companies brag about their product
[00:07:22] flaws." Lex on X wrote, "Lol, watch the
[00:07:25] fear marketing vanish entirely once
[00:07:27] senior management becomes legally liable
[00:07:29] for all the tall tales they've been
[00:07:30] telling." Texas Congressman Chip Roy
[00:07:32] wrote, "100% agree that AI companies
[00:07:34] must take on all liability. Competition
[00:07:36] and full ownership of liability, and tax
[00:07:38] cost, energy demands, etc., is the path
[00:07:41] here. That addresses many of the
[00:07:42] questions and concerns.
[00:07:44] Of course, not everyone agrees. Armand
[00:07:46] Domalewski writes,
[00:07:48] "Imagine if we said we don't need a TSA
[00:07:49] or FAA to prevent terrorism because
[00:07:51] holding airlines liable for 9/11 would
[00:07:53] have been sufficient to prevent it. When
[00:07:55] potential catastrophes are so big that
[00:07:56] they would render a company bankrupt,
[00:07:58] the company becomes essentially judgment
[00:08:00] proof." In Code AI General Counsel
[00:08:02] Nathan Calvin wrote, "We're in a strange
[00:08:04] situation where the frontier AI
[00:08:06] companies, Congress, and the White House
[00:08:08] all do not really want dealing with
[00:08:09] these impending risk from AI to be
[00:08:11] thought of as their problem to solve. I
[00:08:13] agree it would be good for the companies
[00:08:15] to take more responsibility here than
[00:08:16] they have, but catastrophic AI risks
[00:08:18] seem like the archetypal sort of public
[00:08:20] policy issue where government
[00:08:21] intervention is needed to address market
[00:08:23] failures and collective action problems
[00:08:25] and protect the public."
[00:08:27] Still speaking of the companies getting
[00:08:28] a little bit more responsible, although
[00:08:30] the current discussion around AI safety
[00:08:32] is focused on government intervention,
[00:08:34] the frontier labs reportedly came close
[00:08:35] to agreeing to their own arrangement
[00:08:37] earlier in the year. The information
[00:08:39] reports that OpenAI and Anthropic have
[00:08:40] been negotiating deal to perform safety
[00:08:42] tests on each other's models. Sources
[00:08:44] said the arrangement reached the stage
[00:08:45] of formal contracting with lawyers
[00:08:47] hashing out the bilateral arrangement,
[00:08:49] but at some point the deal was abandoned
[00:08:50] for unknown reasons.
[00:08:52] Still the idea lingers with Elon Musk
[00:08:54] proposing a similar arrangement last
[00:08:55] week at the All-In Summit. He claimed
[00:08:57] that distillation wouldn't be a concern
[00:08:59] because it would be evident in the
[00:09:00] testing logs and that labs couldn't risk
[00:09:02] releasing an unsafe model after a rival
[00:09:04] raised the red flag because, quote, "The
[00:09:05] liability in that case would be
[00:09:07] enormous." Microsoft's Suleyman wrote,
[00:09:10] "OpenAI and Anthropic stress testing
[00:09:12] each others models is the smartest
[00:09:13] safety idea in months. No more grading
[00:09:16] your own homework. Now make it mandatory
[00:09:18] and add XAI and Google to the deal."
[00:09:21] Like I said, friends, we are in the
[00:09:22] negotiation phase of this next era, and
[00:09:25] all the proposals should be on the
[00:09:26] table. For now, however, that is going
[00:09:28] to do it for today's headlines. Next up,
[00:09:30] the main episode.
[00:09:32] Welcome back to the AI Daily Brief. Last
[00:09:34] week we talked about how, through a
[00:09:36] combination of GrokBot as a personal
[00:09:40] agent interface optimized for work and
[00:09:43] Muse, a personal agent focused on the
[00:09:45] consumer or personal experience, people
[00:09:47] were revisiting their priors when it
[00:09:49] came to personal agents and wondering if
[00:09:51] this was now going to be an increasingly
[00:09:53] important part of the AI landscape. And
[00:09:55] over the weekend as Amazon blocked
[00:09:57] Meta's Muse, it became pretty clear that
[00:10:00] the agent wars are on. Now, at this
[00:10:02] point, the driving force of this new
[00:10:04] phase is Meta's Muse. I think one could
[00:10:07] argue now that it has solidified its
[00:10:09] early success to become the first
[00:10:11] personal agent to reach, if not
[00:10:13] mainstream success, then certainly this
[00:10:15] level of mainstream curiosity. We have
[00:10:17] seen many agents catch fire throughout
[00:10:20] the course of 2026 and even a little bit
[00:10:22] into 2025. Manas had some early
[00:10:25] interest. Open Claw obviously set up a
[00:10:27] lot of the landscape that we've been
[00:10:28] living in ever since. Hermes in many
[00:10:30] ways took the baton from Open Claw. And
[00:10:32] then more recently we've had more
[00:10:33] consumer-focused offerings like Town and
[00:10:35] Instinct. And yet still, in general,
[00:10:38] these have either been crawl through
[00:10:40] glass to make them work work tools or
[00:10:43] tech toys for early adopters who are
[00:10:45] willing to push through some rough
[00:10:46] edges. Muse is the first agent that's
[00:10:48] appearing to see steady and growing
[00:10:50] consumer adoption outside of tech
[00:10:52] circles with the clearest sign of
[00:10:54] success being how the app is performing
[00:10:56] on the App Store charts. During launch
[00:10:58] week it reached the number two spot on
[00:10:59] Apple's free app charts, but momentum
[00:11:02] continued to grow and it even managed to
[00:11:04] overtake ChatGPT to snatch the number
[00:11:06] one spot. In the four years since
[00:11:09] ChatGPT was released, you might be
[00:11:11] shocked how little time it has spent not
[00:11:13] at number one. And indeed for many, the
[00:11:16] success of Muse is a bit of a surprise.
[00:11:19] On release, the tech press was very
[00:11:21] skeptical that people would willingly
[00:11:23] connect their email, calendar, and other
[00:11:25] personal information to a Meta product.
[00:11:28] And yet, those who don't pay as much
[00:11:30] attention to consumer tech are learning
[00:11:32] one of consumer tech's few enduring
[00:11:34] lessons. Citrini Research commented, "In
[00:11:37] June 2024, I was on Odd Lots talking
[00:11:40] about consumer agents and Apple's
[00:11:41] potential leg up due to trust. Joe
[00:11:44] Weisenthal said flatly that nobody cares
[00:11:46] about privacy. After watching everyone
[00:11:48] give their email, messages, credit
[00:11:50] cards, location, screen access, and
[00:11:52] logins to both Instinct and Muse, I got
[00:11:55] to say, good call, Joe." Now, at this
[00:11:58] stage, Muse has fully broken out and is
[00:12:01] even getting credit for a broader stock
[00:12:03] market rally. Bloomberg is attributing a
[00:12:05] rise in AMD and Intel stock to the
[00:12:08] success of Meta's agent. And while Meta
[00:12:11] does use some AMD and Intel chips, the
[00:12:13] reporting is mostly focused on the
[00:12:15] narrative. As Bloomberg put it,
[00:12:17] "Semiconductor stocks soared Monday as
[00:12:19] early signs of success for Meta's new
[00:12:21] artificial intelligence agents sparked a
[00:12:23] wave of enthusiasm around demand for the
[00:12:25] chips needed to power such agents." At
[00:12:27] least when it comes to market observers,
[00:12:29] personal agents have arrived in the
[00:12:30] mainstream, and everyone is now sitting
[00:12:32] up and paying attention. Microsoft's
[00:12:34] Nicholas Bustamante wrote,
[00:12:36] "It's funny. Meta went from having my
[00:12:38] Instagram and WhatsApp data to now
[00:12:40] having access to my email, calendar,
[00:12:42] DoorDash, Amazon, and pretty much
[00:12:43] everything. In the last 24 hours, it
[00:12:45] bought me socks, ordered my Whole Foods
[00:12:46] groceries, booked a cleaning service,
[00:12:48] and got me a burger for dinner. Meta's
[00:12:50] last disclosed North American Facebook
[00:12:52] ARPU was around $227 per year, largely
[00:12:55] from ads. I suspect it can push that
[00:12:57] number significantly higher now that it
[00:12:59] understands not only what I look at, but
[00:13:02] what I need, what I buy, and what I'm
[00:13:04] planning to do. Also, the much bigger
[00:13:06] opportunity might be becoming the
[00:13:07] aggregation layer between me and the
[00:13:09] entire internet. If Meta can take even a
[00:13:11] tiny percentage of the commerce it
[00:13:13] facilitates, or of the money it saves
[00:13:15] me, this could become enormous. It
[00:13:17] already saved me $200 by canceling
[00:13:19] subscriptions and services I no longer
[00:13:21] needed. This feels much bigger than
[00:13:22] better ad targeting. Ads are useful, but
[00:13:24] giving me money back is better in my
[00:13:26] opinion. One additional thought, the
[00:13:29] agent is increasingly making the
[00:13:30] decisions for me. I knew nothing about
[00:13:32] that burger place. The agent researched
[00:13:34] it, told me which burger I should order,
[00:13:35] and I just said okay without giving it
[00:13:37] much more thought. Agents are becoming
[00:13:38] the decision makers in both B2C and B2B.
[00:13:41] Increasingly, every business will be
[00:13:43] selling not just to humans but to their
[00:13:44] agents. Everything becomes B2A.
[00:13:48] Box's Aaron Levie reposted that and
[00:13:50] added, "The monetization potential of
[00:13:52] personal agents that are transacting on
[00:13:53] your behalf is quite significant. You'll
[00:13:55] start by slinging your daily simple and
[00:13:57] annoying tasks at the agent, then as
[00:13:59] people get used to it, they'll start to
[00:14:00] throw more complex tasks, ultimately
[00:14:02] leading to even more spend through these
[00:14:03] systems than what they were doing
[00:14:04] before."
[00:14:05] And yet, if this feels like a whole new
[00:14:08] commercial dimension of the AI race
[00:14:10] opening up, you had to imagine some
[00:14:12] friction between the platforms. And
[00:14:14] indeed, on Sunday, Amazon altered a
[00:14:16] policy that could have some big
[00:14:17] implications for Muses' momentum.
[00:14:20] Effective immediately, Muse agents won't
[00:14:21] be able to shop for Amazon products on
[00:14:23] behalf of their users. A pop-up on the
[00:14:25] site read, "Continued access by an
[00:14:28] unauthorized AI agent violates Amazon's
[00:14:30] conditions of use to which our customers
[00:14:32] have agreed."
[00:14:33] Now, for many, the decision was kind of
[00:14:35] baffling. Entrepreneur Jesse Frizelle
[00:14:37] wrote,
[00:14:38] "It's weird to me Amazon would do this
[00:14:40] when a purchase is a purchase. They're
[00:14:41] making money either way. Kind of
[00:14:43] stupid." Now, officially, Amazon has
[00:14:45] said, "We think it's fairly
[00:14:47] straightforward that third-party
[00:14:48] applications that offer to make
[00:14:49] purchases on behalf of customers from
[00:14:51] other businesses should operate openly
[00:14:53] and respect service provider decisions
[00:14:55] about whether or not to participate."
[00:14:56] And yet, this is actually a fairly out
[00:14:59] of consensus decision. In general, all
[00:15:02] indications have suggested that the
[00:15:03] business environment is getting geared
[00:15:05] up for agents to make more purchasing
[00:15:07] decisions, not less. Last week, for
[00:15:09] example, Mastercard joined Visa in
[00:15:11] officially supporting virtual credit
[00:15:12] cards for agents. Jorn Lambert,
[00:15:14] Mastercard's chief product officer,
[00:15:16] acknowledged that the personal agents
[00:15:18] era has clearly arrived, commenting, "We
[00:15:20] believe it's not about if, it's about
[00:15:22] when, and how quickly. At the same time,
[00:15:24] a Amazon has been fairly aggressive on
[00:15:26] agentic shopping for a while now. They
[00:15:28] have their own shopping agent that's
[00:15:30] tied to their site, and they've been
[00:15:31] very willing to defend that turf over
[00:15:33] the past year. In November, they went so
[00:15:35] far as to sue Perplexity for
[00:15:36] circumventing their agent blockers. The
[00:15:39] argument wasn't just that Perplexity was
[00:15:40] violating the terms of service, but that
[00:15:42] they were imposing dramatic costs on
[00:15:44] Amazon. I.e., serving web traffic costs
[00:15:47] money, and agents can ping the website
[00:15:48] significantly more frequently than
[00:15:50] humans.
[00:15:51] Still, YouTuber Joseph Carlson believes
[00:15:53] there's another story going on beyond
[00:15:54] the competition for agentic shopping. He
[00:15:56] commented, "Amazon blocks Muse. Sure,
[00:15:59] they will blame it on security, but
[00:16:01] Amazon made 76 billion in the last 12
[00:16:03] months on advertising. Agents don't look
[00:16:05] at ads. A new age of agentic battle has
[00:16:08] begun." In other words, as exciting as
[00:16:10] the new opportunities of agentic
[00:16:12] shopping might be, and all sorts of new
[00:16:14] financial opportunities it could
[00:16:16] theoretically open up, in economics,
[00:16:18] there's no such thing as a free lunch.
[00:16:20] And when humans hand over the
[00:16:21] decision-making, one of the first things
[00:16:22] that might become less valuable is
[00:16:23] digital advertising.
[00:16:25] By far the most common response to this
[00:16:28] was some version of strap in. Bucco
[00:16:30] Capital posted, "Amazon cuts off Muse.
[00:16:33] While I am bullish meta and Muse, I
[00:16:35] think many people are overlooking the
[00:16:36] digital knife fight that's about to
[00:16:38] occur. Nobody wants to get commoditized
[00:16:40] or layered here. Let the games begin."
[00:16:42] MTS's Theo Jaffy sees Balkanization on
[00:16:45] the horizon. He said, "This is an early
[00:16:47] sign of agent wars. There are going to
[00:16:49] be some different agent providers, and
[00:16:51] some of them will be allowed on some
[00:16:52] sites, and some of them will be banned
[00:16:53] on some sites." Palo Alto Networks'
[00:16:56] Nikesh Arora writes,
[00:16:57] "This will be a bigger battle than
[00:16:59] anyone anticipates. It's only a matter
[00:17:01] of time before there is an Apple and
[00:17:02] Google version of Muse, and possibly
[00:17:04] TikTok, in addition to the Frontier LLM
[00:17:06] agents. Maybe a commerce agent from
[00:17:08] Amazon. Every app that is a services,
[00:17:10] marketplace, or commerce app will need
[00:17:12] to essentially decide to open APIs for
[00:17:14] consumer agents to interact. Smaller
[00:17:16] players have no choice. Add revenues are
[00:17:18] more than transaction fees. Either the
[00:17:20] consumer benefits or distribution
[00:17:22] aggregators will demand a higher
[00:17:23] transaction fair. I don't know I want an
[00:17:25] agent for each app. I would like my
[00:17:27] agent to be able to do tasks I require.
[00:17:30] We can already see consumers getting
[00:17:31] trained on that behavior by the frontier
[00:17:32] labs. Those with network motes,
[00:17:35] restaurants, groceries, drivers, might
[00:17:37] be able to withstand for a while, but
[00:17:39] over time convenience and end user
[00:17:40] experience will win and they will have
[00:17:42] to align. Content motes protected by
[00:17:44] copyright could decide to allow agents
[00:17:46] or choose to hold on to the consumer
[00:17:47] interaction. I suspect other than a
[00:17:49] feeling of a lack of control it won't
[00:17:50] change their economics. Commoditized
[00:17:52] backends will need to worry. Insurance,
[00:17:54] tickets, hotels, services, if they don't
[00:17:56] adapt, new players will. Nicholas
[00:17:59] Bustamante again chimed in. The most
[00:18:01] insightful thing I read about technology
[00:18:02] 11 years ago was Ben Thompson's
[00:18:04] aggregation theory. Amazon blocking news
[00:18:06] is another perfect example. Customers
[00:18:08] want one agent that knows them and can
[00:18:10] get things done. The platforms being
[00:18:12] aggregated want the opposite. They want
[00:18:14] to own the customer relationship, not
[00:18:16] become interchangeable suppliers behind
[00:18:17] someone else's interface. And they want
[00:18:20] to protect their ad business. Imagine
[00:18:21] groceries. Your agent can compare
[00:18:23] Amazon, Instacart, DoorDash, and Uber
[00:18:25] Eats, then route every order to the best
[00:18:27] option. Amazon can block that access
[00:18:29] because it is a gigantic company, but
[00:18:32] smaller players have every incentive to
[00:18:33] offer agents a clean API and a seamless
[00:18:35] experience. If Instacart embraces agents
[00:18:38] while Amazon blocks them, the agent will
[00:18:39] increasingly route demand to Instacart.
[00:18:41] Customers will be happy and Amazon will
[00:18:43] eventually face the dilemma. Keep
[00:18:44] protecting the relationship or match the
[00:18:46] better value proposition. This will be
[00:18:48] the defining tension of the agent
[00:18:50] economy. Aggregators realize they are
[00:18:52] now being aggregated. Amazon will push
[00:18:55] its own assistant, of course, but a
[00:18:57] vertical Amazon agent will struggle
[00:18:58] against a horizontal agent that already
[00:19:00] knows my email, calendar, preferences,
[00:19:02] memories, and entire life context. Many
[00:19:04] companies will want to become the
[00:19:06] aggregation layer. Very few actually
[00:19:08] can.
[00:19:09] Many also pointed out that for Amazon,
[00:19:11] there's basically no choice here. Tom
[00:19:13] Goodwin wrote, "A lot of people don't
[00:19:15] get that Amazon's customer isn't the
[00:19:17] consumer. They sell to suppliers and
[00:19:19] vendors to charge them listing fees and
[00:19:20] advertising. It's often closer to a
[00:19:22] shakedown than customer marketing.
[00:19:24] Retail margins could be 0 to 3%. Ad
[00:19:26] margins are 70%. The idea they want
[00:19:29] agents is laughable. The reason the site
[00:19:31] always looks awful is that they don't
[00:19:32] care about you buying things easier or
[00:19:33] faster or being more happy. They want to
[00:19:36] monetize your confusion."
[00:19:37] Shail Mohanot agrees, writing,
[00:19:39] "I hate it as a consumer, but it's the
[00:19:41] right move for Amazon. Agents want to
[00:19:43] replace the storefront and level the
[00:19:44] playing field, but Amazon is big enough
[00:19:46] to say no. Owning the customer
[00:19:47] relationship matters even more than
[00:19:49] logistics in my opinion. Will be
[00:19:50] interesting to see it play out. What
[00:19:52] people are definitely understanding is
[00:19:54] that this is an opening salvo. A16z's
[00:19:57] Angela Strange writes, 'This is just the
[00:19:59] beginning of the agent and data wars.
[00:20:01] Amazon cuts off Muse. Every platform who
[00:20:04] has done the hard work of aggregating
[00:20:05] users is trying to figure out how not to
[00:20:07] become dumb pipes. Do they one, try to
[00:20:10] block the agents, but risk pissing off
[00:20:11] their customers in favor of only their
[00:20:13] own agentic experience? Two, strike
[00:20:15] business development deals to at least
[00:20:17] extract dollars from the new
[00:20:18] multi-agentic interaction that accesses
[00:20:20] their data and platforms? Three,
[00:20:22] something else, question mark?'
[00:20:24] Signal thinks the answer is number two,
[00:20:26] some form of BD deal. They write,
[00:20:28] "The likely resolution to the Meta and
[00:20:30] Amazon fight is some kind of revenue
[00:20:32] sharing agreement where Meta pays Amazon
[00:20:33] for agent access through Muse. There is
[00:20:35] no doubt the BD teams are cooking here
[00:20:37] on an agreement. Facebook likely is fine
[00:20:40] eating the short-term cost to make Muse
[00:20:41] relevant initially. That may become the
[00:20:43] first real business model for agents
[00:20:45] interacting with large platforms where
[00:20:46] they pay for access to the service,
[00:20:48] potentially share data, and maybe pay a
[00:20:50] per user or per agent fee. But if every
[00:20:53] major platform starts charging agents
[00:20:54] for access, only companies with enormous
[00:20:56] scale can afford to build truly general
[00:20:58] agents, which would create some big
[00:21:00] moats for already large companies."
[00:21:03] And Joseph Carlson points out that this
[00:21:04] isn't something that Amazon can just
[00:21:05] kick the can down the road on. He adds,
[00:21:08] "Amazon is going to have to deal with
[00:21:09] Muse. There's no way around it. Agents
[00:21:11] are not going away. Amazon can't close
[00:21:13] their eyes and pretend they don't exist.
[00:21:15] Today, it's Muse, next it's ChatGPT's
[00:21:17] agent, then Anthropic's. Users will
[00:21:19] adopt these in huge numbers. Amazon will
[00:21:21] be forced to develop a verified and
[00:21:23] approved process for allowing agents to
[00:21:24] shop for customers." And yet, Pagio
[00:21:26] Labs' Matt Slotnick says, "I wouldn't
[00:21:28] overly read into Amazon's posture
[00:21:30] regarding Muse right now. Shopify
[00:21:32] obviously will play nice with Meta and
[00:21:33] be a first mover. Amazon has more at
[00:21:35] stake and will be more demanding about
[00:21:37] the relationship because they have
[00:21:38] leverage. Amazon is not anti-agent, nor
[00:21:40] are they dead because they blocked Muse
[00:21:41] in the first week of availability.
[00:21:43] They're not dumb and they have weight to
[00:21:44] throw around." And indeed, almost
[00:21:46] prophetically,
[00:21:47] Shopify did jump in to be the
[00:21:50] anti-Amazon here. On Monday, the company
[00:21:52] announced a partnership with Meta to
[00:21:54] officially support Muse. Similar to
[00:21:56] their partnership with OpenAI, Shopify
[00:21:58] will allow Muse to access their back end
[00:22:00] directly, giving much better search
[00:22:02] performance while optimizing traffic.
[00:22:04] Muse will also see official support in
[00:22:05] Shopify's agentic checkout, Shop Pay,
[00:22:07] across all Shopify stores.
[00:22:10] The announcements are very clearly meant
[00:22:12] to be a poke in the eye for Amazon.
[00:22:14] Meta's chief AI officer, Alexander Wang,
[00:22:15] wrote,
[00:22:16] "We are excited for Muse to be
[00:22:17] partnering deeply with Shopify to enable
[00:22:19] agentic checkout with Shop Pay on all
[00:22:21] Shopify stores. We want to give our
[00:22:23] Musers access to a wide range of stores
[00:22:25] to find the absolute perfect products."
[00:22:27] Mark Zuckerberg even weighed in on X,
[00:22:29] writing,
[00:22:30] "Teaming up with Shopify to make
[00:22:31] shopping and checkout easier in Muse.
[00:22:33] Shopify's find more, shop sell more.
[00:22:36] More partnerships like this coming
[00:22:37] soon."
[00:22:38] Now, I think it would be easy to be a
[00:22:39] bit dismissive of this, believing that
[00:22:41] while yeah, there's a cool opportunity
[00:22:43] for Shopify to get out ahead on agentic
[00:22:45] shopping, this is not going to somehow
[00:22:47] allow them to overtake Amazon, which is
[00:22:49] one of the largest retailers in the
[00:22:50] world. And yet, I continue to think that
[00:22:52] the significance of Shopify is wildly
[00:22:54] underestimated on just about every
[00:22:56] dimension. I know for myself and for
[00:22:58] many others, for basically anything
[00:23:00] that's not on Amazon, if there's not a
[00:23:03] Shop Pay link, which can pull up all my
[00:23:05] information automatically without
[00:23:07] another login, I'm probably just not
[00:23:09] buying for that outlet. In fact, one of
[00:23:11] my more out-there predictions for 2026
[00:23:13] was Shopify being one of the most
[00:23:15] important platforms when it comes to
[00:23:16] general AI adoption, with my logic being
[00:23:19] that so many small business
[00:23:20] entrepreneurs now use Shopify that it
[00:23:23] was a place where a lot of people who
[00:23:24] might otherwise be inclined to go along
[00:23:26] with the tide of disliking AI would find
[00:23:28] out how valuable the tools were when it
[00:23:30] came to everything surrounding their own
[00:23:31] small businesses.
[00:23:33] Still, underlying all of this is a
[00:23:34] question about how much agentic shopping
[00:23:36] is actually going to matter. I've always
[00:23:39] been fairly skeptical that the sort of
[00:23:41] food ordering and airplane ticket buying
[00:23:42] use cases that people have pitched for
[00:23:45] years as their demonstrated use cases
[00:23:47] for personal AI were actually going to
[00:23:49] move the needle when it came to getting
[00:23:51] people to adopt new tools. In addition
[00:23:53] to those things just not being all that
[00:23:54] difficult, or at least when it comes to
[00:23:56] something like flights, it being at
[00:23:58] least as difficult to explain all of the
[00:24:00] nuanced conditions that you have to an
[00:24:02] agent as it is to just look on the
[00:24:03] flight website itself, there's also the
[00:24:05] fact that for many people, the browsing
[00:24:07] and discovery is part of the value of a
[00:24:09] shopping experience. Now, of course, we
[00:24:11] don't have to view shopping as a
[00:24:13] monolith. And if someone argued to me
[00:24:14] that even for the most excited shoppers,
[00:24:16] there are going to be types of shopping
[00:24:18] experiences that they don't care at all
[00:24:19] about and are basically time wasting for
[00:24:21] them, I would probably agree. But I'm
[00:24:23] certainly not the only one to have some
[00:24:25] amount of skepticism around agentic
[00:24:26] shopping. Ron Johnson, Apple's retail
[00:24:29] guru, recently commented in an
[00:24:30] interview, "AI is a new technology that
[00:24:32] will improve the online shopping
[00:24:34] experience, but I don't know that it's
[00:24:35] going to change which way we shop."
[00:24:38] Upstart founder Dave Gerard wrote, "I'm
[00:24:40] skeptical Muse and the like will go
[00:24:41] mainstream with consumers. 99% of what I
[00:24:44] buy online is via Amazon, Shopify,
[00:24:46] Instacart, and DoorDash. I'm not sure an
[00:24:48] agent will make those purchases any
[00:24:49] simpler, more pleasing, more automated,
[00:24:51] or meaningfully less expensive. Same
[00:24:53] with restaurants and travel. My view is
[00:24:55] that the winners in consumer agents will
[00:24:56] be those tied to the dominant devices,
[00:24:58] i.e. Apple and Google, who can make
[00:25:00] hundreds of small moments in your day
[00:25:01] easier.
[00:25:02] AppLovin CEO Adam Foroughi says,
[00:25:05] "The reality is part of the world will
[00:25:07] start using things like agents to
[00:25:08] optimize certain shopper behavior. For
[00:25:10] instance, I might put my supplement
[00:25:11] subscription into an agent and have it
[00:25:13] optimized every single month and
[00:25:14] delivered on time. But these discovery
[00:25:16] platforms aren't that, and the typical
[00:25:18] shopper is not the person who's deep
[00:25:19] into agents and sitting on Twitter and
[00:25:20] adopting the latest technology. There's
[00:25:22] still a ton of people using Yahoo
[00:25:23] properties every single day. The typical
[00:25:25] shopper wants to find a product and
[00:25:27] wants to actually go through that
[00:25:28] shopper behavior. They want to window
[00:25:29] shop. They want to go through the
[00:25:30] transaction experience. They want to
[00:25:32] track it. And if you told them after the
[00:25:33] fact, 'Hey, an agent could have done
[00:25:35] this for you and saved you 20%.' I don't
[00:25:37] think that matters on a $50 transaction,
[00:25:39] because the dopamine hit from going
[00:25:40] through it is what they enjoy."
[00:25:42] Still, like so much of AI, this is
[00:25:45] another area where I think epistemic
[00:25:47] humility is greatly required. Although I
[00:25:49] have some amount of skepticism around
[00:25:51] the power of agentic shopping as a
[00:25:53] conversion experience for users to adopt
[00:25:55] AI agents, my confidence in that
[00:25:57] assessment is not high. And push comes
[00:25:59] to shove, whatever combination of
[00:26:01] dealing with your email or unsubscribing
[00:26:03] or buying things, the personal agent
[00:26:05] experience is being driven by, the
[00:26:07] success of Muse is going to be fairly
[00:26:09] unignorable for the other AI labs.
[00:26:11] Indeed, the information reports that
[00:26:12] OpenAI is working on a personal agent to
[00:26:14] compete with Grokbot and have discussed
[00:26:16] a Muse competitor as well.
[00:26:18] AI leaker Tibor Blaho suggested we could
[00:26:20] be getting OpenAI's agent pretty soon,
[00:26:22] leaking some platform code associated
[00:26:24] with an agent called AON.
[00:26:26] AI news aggregator Andrew Curren
[00:26:27] believes AON could be launched this
[00:26:28] Thursday as one of the big releases for
[00:26:30] OpenAI's Dev Day.
[00:26:32] Now, one of the interesting dimensions
[00:26:33] of OpenAI launching a dedicated personal
[00:26:35] agent is that Codex already could do
[00:26:37] everything a user would want. It can
[00:26:39] triage emails, handle a calendar, or
[00:26:41] even shop for you. But as the
[00:26:43] information puts it, many OpenAI users
[00:26:45] aren't necessarily aware of these
[00:26:46] features. And it's safe to say SpaceX
[00:26:49] and Meta have stolen some thunder with
[00:26:50] their respective agent products in
[00:26:51] recent weeks. In other words, there are
[00:26:54] certain use cases for AI where being at
[00:26:56] the absolute state of the art is all
[00:26:57] that matters. But when it comes to agent
[00:26:59] management, you got to have a user
[00:27:01] experience that people understand and
[00:27:03] that leaves them with something more
[00:27:04] than a blank page. I think it is likely
[00:27:07] that we get a lot more on this topic
[00:27:08] very soon. For now though, that is the
[00:27:10] story. Agent wars have begun and that's
[00:27:12] going to do it for today's AI daily
[00:27:14] brief. Appreciate you listening or
[00:27:15] watching as always and until next time,
[00:27:18] peace.
