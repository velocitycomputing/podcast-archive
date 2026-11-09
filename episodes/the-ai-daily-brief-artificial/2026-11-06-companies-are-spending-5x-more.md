---
record_id: "podcast:d37dbc56-2eea-4c7e-b773-11373392c0fa"
episode_id: d37dbc56-2eea-4c7e-b773-11373392c0fa
title: Companies Are Spending 5x More on AI Now
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/companies-are-spending-5x-more-on-ai-now/d37dbc56-2eea-4c7e-b773-11373392c0fa"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/companies-are-spending-5x-more-on-ai-now/d37dbc56-2eea-4c7e-b773-11373392c0fa"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-11-06
played_at: "2026-11-06T12:00:00Z"
play_count: 1
duration_seconds: 600
source: pocketcasts-history-browser
played_label: November 6
history_order: 6
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: f9a17eae729a4ba3b30b758141a5ed533e0c02a467b17f566980633b980bb58d
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

Despite headlines about companies such as Apple restricting engineers’ daily AI spend, Menlo’s survey of about 400 U.S. enterprise decision makers responsible for roughly $4B in AI spend, conducted by Morning Consult, estimates enterprise AI spending rose from $1.7B in 2023 to $8.5B in 2024, $33B in 2025, and nearly $177B in 2026; adoption breadth rose only from 55% to 65%, but average spend per adopting enterprise rose 4.7x and companies spent about 2.5x their budgets, with frontier-model share of spend rising from 35% to 63%, Anthropic’s API-spend share reaching 55% (OpenAI 31%, Google 9%), open source taking 4% of spend but 19% of tokens, and lab coding agents Codex/Claude Code revenue jumping from $1B to $24B while other coding platforms grew from $2.6B to $7.8B. Separately, a market drawdown saw the Mag 7 lose about $1T, Nvidia fall 9.3%, Microsoft 3.6%, Micron 17.5%, SanDisk 22.3%, the S&P 500 4.4%, and the Nasdaq 6.4%, with Fundstrat’s Tom Lee and Bloomberg’s Nishant Kumar pointing to hedge-fund deleveraging and forced selling (Walleye, Lone Pine, Millennium) and unrelated names like Walmart and Exxon Mobile also falling; Anthropic IPO uncertainty intensified, with prediction-market odds for a pre-Thanksgiving IPO falling from 85% to 60%, year-end odds from 95% to 66%, secondary valuations near $1.6T versus investor pressure toward $1T, and an $80B October run rate; Meter’s first independent Anthropic safety report found model-improvement pace roughly doubled due to AI-assisted R&D and drew reactions from Sam McCandlish, Ryan Greenblatt, Alex Boras, and Nathan Lambert; and product updates included Claude’s read-only Plaid bank-account personal-finance feature, Meta Muse voice/video animated avatars, and OpenAI Images 2.6 GIF/reference-image generation at 4B images per week.

No direct health implications appear in the material, but the actionable business and research leads are to reframe AI budgets around tokens, agent workloads, and completed outcomes rather than seats, because spend can scale with autonomous work and exceed plans by multiples; create CFO-level controls for variable token costs, separate frontier-model ROI from cheaper/open-source alternatives, and test whether capability differences justify higher prices before moving workloads; monitor concentration and liquidity risk if making vendor, hiring, or investment decisions, given Anthropic/OpenAI dominance and hedge-fund forced selling; treat Anthropic’s IPO valuation, $80B run rate, and possible delay as due-diligence items rather than proof of durable demand; follow Meter’s RSI/acceleration findings, benchmark limitations, and missing cybersecurity/sandboxing details as safety and governance research leads; and consider practical experiments such as read-only financial-data agents for budgeting, voice/video agent prototypes, and fast image/GIF workflows, while asking follow-up questions about task completion rates, cost per outcome, data-access controls, security boundaries, and whether open-source token share translates into real cost savings.

## Transcript

[00:00:00] If you survey just the mainstream media,
[00:00:02] you might have the impression that
[00:00:04] business adoption of AI was in some way
[00:00:07] impaired or slowing down. The stories
[00:00:09] that make the news about enterprise
[00:00:11] adoption of AI seem primarily right now
[00:00:13] to be about companies restricting how
[00:00:15] much their employees can spend on it,
[00:00:17] like Apple, for example, cutting the
[00:00:19] amount that engineers can spend per day,
[00:00:20] which was a story this week. And yet,
[00:00:22] when you take a step back, not only has
[00:00:25] AI adoption in the business sector
[00:00:26] continued unabated, the speed at which
[00:00:28] it is growing is actually increasing,
[00:00:30] defying all logic and expectation as it
[00:00:32] starts from a bigger base. The story of
[00:00:35] enterprise AI adoption this year is very
[00:00:37] clearly the story of agents, and that's
[00:00:39] what we're looking at on today's
[00:00:40] episode.
[00:00:41] The AI Daily Brief is the daily podcast
[00:00:43] and video about the most important news
[00:00:44] and discussions in AI.
[00:00:47] All right, quick announcements before we
[00:00:49] dive in. First of all, thank you to
[00:00:51] today's sponsors, KPMG, CData, Granola,
[00:00:54] and Blitsy. To get an ad-free version of
[00:00:56] the show, go to patreon.com/aidailybrief
[00:00:58] or you can subscribe on Apple Podcasts.
[00:01:00] And if you want to learn more about
[00:01:02] sponsoring the show, send us a note at
[00:01:04] sponsors@aidailybrief.ai.
[00:01:07] One more quick shout out before we dive
[00:01:08] in. Our newest premium AI training
[00:01:10] program is starting soon. It's called
[00:01:12] the AI Champions Boot Camp. It's three
[00:01:15] weeks long, and this one has six live
[00:01:17] sessions led by Nufar Gaspar, frequent
[00:01:19] contributor to the show, and will not
[00:01:21] just help people use agents more
[00:01:22] effectively, but have the skills and
[00:01:24] resources to bring that use to their
[00:01:26] entire teams. You can get all the
[00:01:28] information for that program at
[00:01:29] bsuper.ai, and the boot camp begins on
[00:01:31] November 16th.
[00:01:33] Welcome back to the AI Daily Brief
[00:01:34] Headlines Edition, all the daily AI news
[00:01:36] you need in a round 5 minutes. Well, it
[00:01:39] looks like the markets got a little bit
[00:01:41] annoyed at my overly optimistic analysis
[00:01:44] because yesterday AI stocks plummeted in
[00:01:46] the worst drawdown since 2020.
[00:01:49] Overall, the Mag 7 lost a combined
[00:01:51] trillion dollars in market cap, with
[00:01:53] Nvidia falling 9.3% and Microsoft
[00:01:56] dropping 3.6%. The pain was even greater
[00:01:58] in the supply chain, where Micron lost
[00:02:01] 17.5% and SanDisk plummeted 22.3%.
[00:02:05] The S&P 500 fell by 4.4% and the Nasdaq
[00:02:08] collapsed by 6.4% in the largest
[00:02:10] single-day drop for the major indices
[00:02:12] since March of 2020.
[00:02:14] Fatalistic takes were all over X. Kevin
[00:02:17] Sue from Alpha AI wrote, we're effed,
[00:02:19] absolutely effed. The AI trade is over.
[00:02:21] We all top blasted and holding bags now.
[00:02:23] Tech investor Steven Sinofsky added,
[00:02:25] this is not the AI trade or AI lost the
[00:02:27] election trade as you might read or see,
[00:02:29] but rather the what happens when USAI is
[00:02:32] not going to happen trade.
[00:02:34] In fact, one of the most striking parts
[00:02:35] of the drawdown was how broad-based it
[00:02:37] was. Completely unrelated stocks like
[00:02:39] Walmart and Exxon Mobile took massive
[00:02:41] hits alongside tech.
[00:02:43] Some argued that semiconductors are now
[00:02:45] cheap with Nvidia trading at a 13x
[00:02:47] multiple, making it one of the
[00:02:48] quote-unquote cheapest stocks on the
[00:02:50] market. Then again, investor Jeff Park
[00:02:52] pointed out that boom and bust
[00:02:53] semiconductor stocks always look cheap
[00:02:55] as they head into a bust, commenting,
[00:02:58] nothing outs a newbie faster than
[00:02:59] valuing semis on price to earnings. Now,
[00:03:02] the curious part is that nothing
[00:03:03] substantial changed between Wednesday
[00:03:05] and Thursday that would explain the
[00:03:06] sudden collapse. And whenever that
[00:03:08] happens, when there's no narrative
[00:03:10] explanation, we have to look towards
[00:03:12] market structure and market dynamics as
[00:03:14] the driver. And indeed, Fundstrat's Tom
[00:03:17] Lee told CNBC, I think there are stories
[00:03:20] of some large hedge funds actually being
[00:03:22] liquidated now. And according to
[00:03:23] reports, Walleye has blown up and
[00:03:25] returned their capital. Lone Pine is
[00:03:27] also rumored to have collapsed and
[00:03:28] Millennium is said to have pulled 1.5
[00:03:30] billion in leveraged capital from two
[00:03:32] outside managers. Bloomberg's Nishant
[00:03:34] Kumar wrote, I've covered hedge funds
[00:03:36] for nearly 16 years and I can't remember
[00:03:38] a day like today. Nicholas Mugali from
[00:03:41] TMT Research wrote,
[00:03:42] if you're wondering why this sell-off is
[00:03:44] so aggressive, this is what forced
[00:03:46] selling looks like. It isn't happening
[00:03:48] in one sector. It's literally everywhere
[00:03:50] you look at once, from financials to AI
[00:03:52] infrastructure. And the best businesses
[00:03:54] are falling hardest because they're the
[00:03:55] easiest things to sell when a funds need
[00:03:57] cash. The fundamentals are intact, but
[00:04:00] every chart looks broken right now and
[00:04:01] has been broken for a couple of months.
[00:04:03] In short, rather than investors waking
[00:04:05] up on Thursday and deciding to sell
[00:04:07] everything, it looks like Wednesday's
[00:04:09] drawdown in semiconductors was enough to
[00:04:10] trigger a broad deleveraging across the
[00:04:12] hedge fund industry. That could mark the
[00:04:14] end of the AI bull market, or it could
[00:04:16] be a temporary blip like we saw when
[00:04:18] tariffs were unveiled last year.
[00:04:20] Now with markets in freefall, rumors are
[00:04:22] swirling that the Anthropic IPO might
[00:04:24] get pulled. Previous reports said that
[00:04:26] Anthropic was aiming to get out before
[00:04:27] Thanksgiving, which means their road
[00:04:29] show would need to begin next week.
[00:04:31] Obviously, a Frontier AI lab is going to
[00:04:33] be a harder sell under these market
[00:04:34] conditions, and prediction markets are
[00:04:36] beginning to price in a delay or even a
[00:04:38] cancellation.
[00:04:39] On Thursday, odds of the Anthropic IPO
[00:04:41] before Thanksgiving fell from around 85
[00:04:43] to 60% and the odds they get out by the
[00:04:45] end of the year have fallen from 95% to
[00:04:47] 66% over the past week.
[00:04:50] Thinly traded secondary markets are
[00:04:51] still pricing the company at around 1.6
[00:04:53] trillion, but according to the Wall
[00:04:55] Street Journal, institutional investors
[00:04:57] are increasingly skeptical of the price.
[00:04:59] They wrote that three major investors
[00:05:00] who plan to participate in the IPO say
[00:05:02] the valuation will need to come down,
[00:05:04] with one arguing it needs to be closer
[00:05:05] to 1 trillion. Either that or Anthropic
[00:05:08] might need to trim their reported 100
[00:05:09] billion dollar target for the
[00:05:10] fundraising. This is obviously a big
[00:05:12] shift from where they were in August
[00:05:14] when investors were leaking a 2 trillion
[00:05:16] dollar target in the press. Still, that
[00:05:18] same article in the WSJ reported an 80
[00:05:20] billion dollar run rate for October, up
[00:05:22] from 65 billion reported for the end of
[00:05:24] July. So can Anthropic slough off the
[00:05:26] market turmoil? I think we'll have a
[00:05:28] better sense once the hedge fund blow up
[00:05:29] stops ricocheting around the market, but
[00:05:31] for now, something that was idle chatter
[00:05:33] is getting a lot more attention.
[00:05:35] Now speaking of Anthropic, outside of
[00:05:37] markets, maybe the biggest discussed
[00:05:39] story right now is Meters release of
[00:05:41] their first independent safety report
[00:05:42] for Anthropic, which discloses a major
[00:05:45] acceleration in AI led research. Last
[00:05:47] month, Anthropic announced that they'd
[00:05:49] onboarded Meter as their first
[00:05:50] independent evaluator with employee
[00:05:52] level access. The idea is of course to
[00:05:54] give the public better visibility into
[00:05:55] Anthropic safety practices in the wake
[00:05:57] of so-called rogue agent incidents. The
[00:06:00] key finding of the report was that the
[00:06:01] pace of improvement for Anthropic's
[00:06:03] models has roughly doubled over the past
[00:06:04] year. Meter concluded that the
[00:06:06] acceleration was due to AI being used in
[00:06:08] research efforts. They wrote, we were
[00:06:10] told that R&D is accelerated primarily
[00:06:13] via AI assistance rather than fully
[00:06:15] autonomous contributions, but there are
[00:06:17] some signs that fully autonomous
[00:06:18] contributions will play a larger role
[00:06:20] soon. If AI systems started to
[00:06:22] significantly accelerate further AI
[00:06:24] development, the report stated this
[00:06:25] could lead to a sudden emergence of
[00:06:27] extreme and risky capabilities. Meter
[00:06:29] noted that they were given access to
[00:06:31] internal information that surpassed
[00:06:32] their expectations. This included
[00:06:34] analysis of three unreleased models
[00:06:36] trained since July. The most recent
[00:06:38] model was completed in September or
[00:06:39] October and continued the trend of
[00:06:41] accelerated improvement observed earlier
[00:06:43] in the year.
[00:06:44] Anthropic co-founder and responsible
[00:06:45] scaling officer Sam McCandlish signed up
[00:06:47] for X this week to discuss the report.
[00:06:50] He commented,
[00:06:51] the speed of progress in model
[00:06:52] capabilities is one of the most
[00:06:54] important questions in AI safety, and
[00:06:55] Meter's work here provides the public
[00:06:57] with an independent external view into
[00:06:59] how this is happening inside Anthropic.
[00:07:01] Sam acknowledged criticism that
[00:07:02] Anthropic redacted some of the most
[00:07:04] important evidence that Meter used to
[00:07:05] come to their conclusion, but said that
[00:07:07] Anthropic intends to provide a
[00:07:08] supplemental report on their own
[00:07:09] analysis in the coming weeks.
[00:07:11] Now, in terms of reactions, the AI
[00:07:13] safety folks were rattled by the report,
[00:07:15] claiming it accelerated their timelines.
[00:07:17] Ryan Greenblatt from Meter wrote,
[00:07:19] this report on AI R&D automation is a
[00:07:22] big update towards ASI within one to two
[00:07:24] years. Nathan Calvin, the general
[00:07:26] counsel for Encode AI, called this a
[00:07:27] quote extremely unnerving update.
[00:07:30] New York assemblyman Alex Boras argued
[00:07:31] that there's no time to wait, writing,
[00:07:34] Congress should ban RSI this year if
[00:07:36] possible. But others were a little
[00:07:38] skeptical of the methodology, with open
[00:07:41] model researcher Nathan Lambert noting,
[00:07:42] a lack of good enough benchmarks is a
[00:07:44] bottleneck, at least for the type of RSI
[00:07:46] described as an intelligence explosion.
[00:07:49] Now, some rehashed the criticism that
[00:07:50] Meter is closely affiliated with
[00:07:52] Anthropic, at least in ideology if not
[00:07:54] through actual financial and personnel
[00:07:56] ties. And whatever you think of those
[00:07:58] arguments, the report does highlight the
[00:08:00] issue with presenting Meter as an
[00:08:02] external evaluator. One of the key
[00:08:04] points of appointing Meter was to
[00:08:06] address public concerns about
[00:08:07] cybersecurity breaches from the labs.
[00:08:10] Meter's report, though, only mentioned
[00:08:11] cybersecurity in terms of the models
[00:08:13] getting more advanced, and doesn' touch
[00:08:15] on sandboxing or other safety measures.
[00:08:17] It's essentially non-responsive to
[00:08:18] concerns raised over recent months,
[00:08:20] instead assuming that RSI is the only
[00:08:23] risk that matters. Now, it's perfectly
[00:08:24] reasonable for Meter to decide that that
[00:08:27] is the only concern that they really
[00:08:28] care about, but if that's the case,
[00:08:30] having only Meter here means a very
[00:08:32] incomplete independent auditor suite.
[00:08:34] Now, closing out with some feature and
[00:08:36] product updates, Anthropic has
[00:08:37] relaunched Claude for personal finance
[00:08:39] with the ability to connect to your bank
[00:08:40] account. This is read-only access via
[00:08:43] Plaid, which is common across the
[00:08:44] personal finance industry, so
[00:08:46] theoretically shouldn't be a huge
[00:08:47] concern to the big banks that are
[00:08:48] worried about agents making
[00:08:49] transactions.
[00:08:50] Claude won't even give investment
[00:08:52] advice, instead giving users help with
[00:08:54] budgeting by analyzing their spending
[00:08:55] data, giving a sense of the current
[00:08:57] state of how they talk about AI's
[00:08:58] potential disruption of professional
[00:09:00] services, they wrote.
[00:09:01] Personal finance is a first step. For
[00:09:03] life's bigger money decisions, we think
[00:09:05] people are best served by Claude working
[00:09:07] alongside the licensed professionals and
[00:09:09] regulated firms they trust.
[00:09:11] Over in Metaland, many are rejoicing
[00:09:13] that Muse now has a voice. Meta's
[00:09:15] breakout personal agent now has a
[00:09:16] feature that allows users to communicate
[00:09:18] with it through voice and video chats.
[00:09:20] Now, from the start, Muse has leaned
[00:09:21] into the idea of personalizing your
[00:09:23] agent by giving it a name and an avatar.
[00:09:25] This feature takes that idea to the next
[00:09:26] level, fully animating the avatars for
[00:09:28] voice calls and letting users choose
[00:09:30] from a range of different voice options.
[00:09:32] AI CEO Alexander Wang showed off the new
[00:09:34] feature, demonstrating his agent Euler
[00:09:37] coaching him through problems at work
[00:09:38] related to posting too many memes. The
[00:09:40] feature uses Meta's live voice models,
[00:09:42] which are top-notch, as well as their
[00:09:43] real-time avatar technology. Meta says
[00:09:45] the avatars will use subtle expressions
[00:09:47] and gestures to match the tone of the
[00:09:48] conversation, but they don't actually
[00:09:50] have visual inputs to pick up on
[00:09:52] non-verbal cues. The feature is now live
[00:09:54] for mobile, web, and Mac, and Meta says
[00:09:56] they'll use it to power the forthcoming
[00:09:57] Muse Charm device.
[00:09:59] It also works with the Muse Gadget SDK,
[00:10:01] so you can now talk to your home-brewed
[00:10:03] AI devices as well.
[00:10:05] And lastly, OpenAI has rolled out a new
[00:10:07] version of their image model that now
[00:10:08] supports animated GIFs. Users can now
[00:10:11] prompt a short animation, edit the
[00:10:12] speed, and modify individual frames
[00:10:14] before they share it online.
[00:10:16] OpenAI says that their users are now
[00:10:17] creating four billion images per week,
[00:10:19] up from three billion a couple of months
[00:10:21] ago. Images 2.6, which is the name of
[00:10:23] the new version of the model, is 50%
[00:10:25] faster and able to generate an image in
[00:10:27] as little as six seconds. It can also
[00:10:29] now accept reference images, meaning
[00:10:31] users can upload a rough doodle or
[00:10:33] easily turn it into a high quality
[00:10:34] image. And so if you didn't already have
[00:10:36] plans for the weekend, maybe it's time
[00:10:38] to experiment with making your own
[00:10:40] gifts. For now, that is going to do it
[00:10:41] for the headlines. Next up, the main
[00:10:44] episode.
[00:10:46] Hello everyone. One big change around AI
[00:10:48] is we've shifted our thinking from how
[00:10:50] we rank our pages to how do we become
[00:10:53] the source that AI trusts enough to
[00:10:54] answer with. At KPMG, they're seeing
[00:10:56] this firsthand. AI generated results now
[00:10:59] surface answers directly, often without
[00:11:00] a single click. That's why they are
[00:11:02] increasingly focused on generative
[00:11:03] engine optimization or GEO, structuring
[00:11:06] content so AI systems can retrieve it,
[00:11:08] understand it, and cite it as trusted
[00:11:10] authority. This is not just an SEO
[00:11:12] evolution, but a visibility mandate. And
[00:11:14] indeed, the GEO mandate from KPMG is
[00:11:17] simple. If AI is shaping decisions, your
[00:11:20] expertise needs to show up inside the
[00:11:22] answer. Read all about it at
[00:11:24] kpmg.com/us/geo.
[00:11:27] Again, that is kpmg.com/us/geo.
[00:11:32] This episode is brought to you by C
[00:11:34] Data. Companies rolling out AI keep
[00:11:36] hitting the same wall. Token spend is
[00:11:38] climbing, security is holding agents
[00:11:40] back, and no one knows how AI is truly
[00:11:42] being used. The root cause, AI is cut
[00:11:45] off from the systems and context your
[00:11:47] business runs on. That's why C Data
[00:11:49] built Connect AI Gateway, one control
[00:11:52] point between your AI and your systems.
[00:11:54] Built on the connectivity layer powering
[00:11:56] Palantir, Google, Salesforce, and
[00:11:58] hundreds more, each agent gets exactly
[00:12:00] the data and tools it needs. It governs
[00:12:02] down to the record and lets you finally
[00:12:04] see your org's complete AI usage in one
[00:12:06] place. Accurate answers, a fraction of
[00:12:08] the token cost, and a gateway that
[00:12:10] learns your business with every
[00:12:11] interaction. See how at cdata.ai.
[00:12:16] You're in back-to-back meetings all day.
[00:12:17] You're trying to stay present, but
[00:12:19] you're also worried you'll forget the
[00:12:20] decision, the action item, the important
[00:12:22] next step. is a scenario that we
[00:12:24] absolutely live here at the AI Daily
[00:12:25] Brief, given how fast things move and
[00:12:27] change and how quickly we're evolving
[00:12:28] everything that we do. That's where
[00:12:30] Granola comes in. Granola is an
[00:12:32] AI-powered notepad for meetings. You jot
[00:12:34] down rough notes like you always do, and
[00:12:36] in the background, Granola transcribes
[00:12:38] and turns them into clear, useful notes
[00:12:39] when the meeting ends. No bots joining
[00:12:41] your calls, no distractions, just a
[00:12:43] clean notepad that helps you focus.
[00:12:45] During or after the call, you can chat
[00:12:47] with your notes. Ask Granola to pull out
[00:12:49] action items, help you negotiate, write
[00:12:50] a follow-up email, or even coach you
[00:12:52] using recipes, which are pre-made
[00:12:53] prompts. Once you try it on a first
[00:12:55] meeting, it is very hard to go without.
[00:12:57] Head to granola.ai/aidaily
[00:13:00] and use code aidaily to get 100% off for
[00:13:03] 3 months for new users. That's
[00:13:05] granola.ai/aidaily
[00:13:07] and code aidaily to get 100% off for new
[00:13:10] users for 3 months.
[00:13:12] Blitz's understanding of massive code
[00:13:14] bases unlocks autonomous security fixes,
[00:13:16] modernization, and new features. So what
[00:13:18] happens when there's no legacy code at
[00:13:20] all? Greenfield is supposed to be the
[00:13:22] easy part, clean slate, no technical
[00:13:24] debt. But even Greenfield moves at human
[00:13:26] speed one sprint at a time. Blitz
[00:13:28] changes the unit of work from the
[00:13:29] developer to the project, autonomously
[00:13:31] planning, building, testing, and
[00:13:33] validating entire applications from
[00:13:34] scratch, hundreds of thousands of lines
[00:13:36] of production-ready code. One Blitz
[00:13:38] customer stood up a brand new
[00:13:39] application, 534,000
[00:13:42] lines of code, compressing a 65-week
[00:13:44] roadmap into 2 weeks. Another shipped an
[00:13:46] entire application with no front-end
[00:13:48] engineer. Legacy or Greenfield, the
[00:13:49] answer is the same, software at the
[00:13:51] speed of compute. Build what's next at
[00:13:53] blitz.com. That's blitzy.com.
[00:13:59] Welcome back to the AI Daily Brief.
[00:14:01] Today we are digging into Menlo's latest
[00:14:04] Enterprise AI report. They've been doing
[00:14:06] these State of Enterprise AI reports for
[00:14:08] 3 years now, and they provide a really
[00:14:11] good snapshot into how businesses are
[00:14:13] using AI.
[00:14:14] Now the data for this survey comes from
[00:14:16] a survey of around 400 US enterprise
[00:14:18] decision makers that was conducted by
[00:14:20] Morning Consult in mid-September. So
[00:14:23] this is pretty fresh data. Those
[00:14:25] enterprise decision makers, by the way,
[00:14:26] are responsible for about $4 billion in
[00:14:29] AI spend. So it's a pretty meaningful
[00:14:31] sized group. Now, in terms of caveats,
[00:14:33] of course, Menlo is not some unbiased
[00:14:35] observer. They are heavily invested in
[00:14:37] the AI field, including in Anthropic and
[00:14:39] many other companies. But as we'll see,
[00:14:41] this data all directionally backs up, I
[00:14:43] think, a lot of common sentiment about
[00:14:44] business AI spend right now, even if it
[00:14:46] adds some more color and details as
[00:14:47] well.
[00:14:48] What we're going to do on today's show
[00:14:49] is not go through every single number in
[00:14:51] the deck. Instead, I've pulled out the
[00:14:53] 10 most interesting, each of which I
[00:14:55] think has something else to tell us
[00:14:56] about the AI market.
[00:14:58] The first set of stats are all about how
[00:15:00] much business AI spend has grown. And
[00:15:03] what's interesting about 2026 is that
[00:15:05] not only has spending gone up, the rate
[00:15:07] at which it is growing has also gone up.
[00:15:10] Across the four years, excuse me, I
[00:15:12] think I said three years before, but the
[00:15:13] four years that Menlo has been doing
[00:15:15] this survey, their estimates for
[00:15:16] enterprise AI spending have jumped from
[00:15:18] $1.7 billion annually in 2023 to $8.5
[00:15:21] billion in 2024, to $33 billion last
[00:15:24] year, to almost $177 billion in 2026.
[00:15:28] Now, from a growth rate perspective,
[00:15:29] that means that the growth rate from '23
[00:15:31] to '24 was 5x, but the growth rate from
[00:15:34] '24 to '25 was down to 3.9x. Now, this
[00:15:37] is kind of what you'd expect as a market
[00:15:39] gets more mature, more saturated, and
[00:15:41] the total size of the numbers go up.
[00:15:43] While the sheer amount of spend can
[00:15:44] continue to increase, the multiple of
[00:15:47] the previous year's spend at some point
[00:15:48] has to start coming down. That's sort of
[00:15:50] what it looked like happened between '24
[00:15:52] and '25. Except now in '26, we've had a
[00:15:55] jump not only ahead of the '25 number,
[00:15:58] but a faster growth rate than even the
[00:16:00] '23 to '24 number. And obviously, the
[00:16:03] explanation is agents. This year, the
[00:16:06] big story of 2026 from Opus 45 in
[00:16:08] November of last year on is that AI
[00:16:10] spend stopped being about seats and
[00:16:12] started being about tokens and
[00:16:14] everything that intelligence could do.
[00:16:16] And that has totally transformed our
[00:16:17] expectations of how big the market can
[00:16:19] get.
[00:16:20] This number also shows up in our next
[00:16:21] stat where breadth of AI spend was up
[00:16:23] only incrementally, but depth of AI
[00:16:26] spend was up significantly. So the share
[00:16:28] of enterprises using AI jumped from 55
[00:16:31] to 65% between 25 and 26, which is
[00:16:34] insane that that still means 35% of
[00:16:36] enterprises report not using AI. But
[00:16:38] here we are. If you've ever doubted the
[00:16:40] inertia of the business world, there you
[00:16:41] go. However, the average AI spend per
[00:16:44] enterprise using 2025
[00:16:47] as 1 X is up almost 5 X, 4.7 times more
[00:16:52] per enterprise on average this year.
[00:16:55] Again, the answer is agents, agents that
[00:16:57] can work independently, that can run in
[00:16:59] parallel, that can keep working after
[00:17:01] people step away. Spending then scales
[00:17:03] with work, not with head count.
[00:17:06] Now, one thing that we've been debating
[00:17:08] on this show, and in markets frankly, is
[00:17:10] whether the concentration and top
[00:17:12] heaviness of AI spend is a bearish or
[00:17:15] bullish sign. The bearish sign, at least
[00:17:17] from a market's perspective, is that
[00:17:19] when big chunks of revenue are
[00:17:20] concentrated in a small handful of
[00:17:22] customers, if any one of those customers
[00:17:24] stops spending or changes their spending
[00:17:26] habits significantly, it can have an
[00:17:28] outsized effect on the entire market,
[00:17:30] which could then have knock-on effects
[00:17:31] that drag the whole market down. This is
[00:17:33] why concentration is a risk. The other
[00:17:36] way to look at it, however, is that the
[00:17:37] concentration is not a natural state of
[00:17:40] the market where there are only a
[00:17:42] handful of companies that can use that
[00:17:44] much AI, but instead that those handful
[00:17:46] of companies that are using that much AI
[00:17:48] are leading indicators for where the
[00:17:50] rest of the market will eventually go.
[00:17:52] That is of course the bullish assessment
[00:17:54] that takes what those companies at the
[00:17:55] very top are spending and multiplies
[00:17:57] that across all the other companies that
[00:17:59] could possibly spend that much as well.
[00:18:01] Menlo certainly reads this 5 X growth in
[00:18:04] average spend per enterprise as a sign
[00:18:06] of future demand. They believe that the
[00:18:08] long tail basically is barely getting
[00:18:10] started.
[00:18:11] And one more on growth, and this is
[00:18:12] something that certainly we've been
[00:18:13] seeing companies reconcile with all
[00:18:15] year. Enterprises spent about 2.5 times
[00:18:18] what they had budgeted this year.
[00:18:20] Basically, the average company planned
[00:18:22] to roughly double spend between 25 and
[00:18:24] 26. They had planned to grow spend about
[00:18:26] 1.9 x. So if you spent $10 million in
[00:18:29] 2025, you were anticipating you'd spend
[00:18:32] $19 million in 2026. Those numbers were
[00:18:35] of course calculated by most firms on
[00:18:37] the basis of increased adoption on a per
[00:18:40] seat basis across more parts of their
[00:18:41] companies. In actuality, spend has
[00:18:44] jumped 4.7 x, around 2.5 times more
[00:18:47] growth than they had budgeted for. And
[00:18:49] the challenge of course for CFOs is that
[00:18:51] this isn't necessarily some out of
[00:18:54] control spend. It's people flexing and
[00:18:56] understanding what they can actually do
[00:18:58] with all this raw intelligence power.
[00:19:00] The whip lash that companies have had
[00:19:02] between token maxing on the one hand and
[00:19:04] token restrictions on the other are all
[00:19:06] symptomatic of the fact that we planned
[00:19:08] for one paradigm, a per seat paradigm,
[00:19:10] and instead got a per token paradigm,
[00:19:12] which needs a totally different type of
[00:19:14] strategy. Budgeting for AI is starting
[00:19:16] to look more like budgeting for cloud
[00:19:17] compute, but even that analogy falls
[00:19:19] down as well.
[00:19:20] It really is this new category of thing
[00:19:23] that doesn't cleanly fit in past buckets
[00:19:25] and so needs to be considered on its own
[00:19:26] new terms.
[00:19:28] For our next section, we'll look at what
[00:19:30] Menlo found about the competition and
[00:19:32] where those enterprise dollars were
[00:19:33] going.
[00:19:34] One story that kind of flies in the face
[00:19:37] of some of the conventional wisdom or at
[00:19:38] least some of the narratives for the
[00:19:39] past few months is that overall buyers
[00:19:42] moved to more expensive models. The most
[00:19:45] popular models a year ago were Claude
[00:19:47] Sonnet 4.5, which cost $3 per million
[00:19:49] input tokens and $15 per million output
[00:19:52] tokens, and GPT-5, which was $1.25 and
[00:19:54] $10 respectively. The most popular
[00:19:57] models today are, unsurprisingly, the
[00:19:59] latest generation from each of those
[00:20:00] companies as well, Claude Opus 5.5,
[00:20:02] which is $4 input and $20 output, and
[00:20:05] GPT-6 Astro, which is 10 and 60. The
[00:20:07] frontier model spend of share went from
[00:20:09] 35% to 63%.
[00:20:12] Meanwhile, every other category, mid
[00:20:14] tier, small, and older, went down as a
[00:20:16] percentage of total spend.
[00:20:18] Now part of this is also small model
[00:20:20] price wars. Labs cut small model prices
[00:20:23] by 80% plus, but the story that this
[00:20:26] survey is finding is that buyers still,
[00:20:28] despite all of the narrative about costs
[00:20:30] and cost efficiency, are choosing
[00:20:32] capability over cost. So is the
[00:20:34] narrative that we've had about cost
[00:20:36] wrong or is there room for both of these
[00:20:37] stories simultaneously? I actually think
[00:20:39] that these two things are not mutually
[00:20:41] exclusive. I believe that the continued
[00:20:43] emphasis on frontier models reflects the
[00:20:45] fact that starting with Opus 4.5, we
[00:20:48] really have had a differentiated set of
[00:20:50] capabilities that came online. And since
[00:20:52] the entire year has been businesses
[00:20:53] racing to catch up with those
[00:20:54] capabilities and implement new agent
[00:20:56] decoding, they've sort of been priced
[00:20:58] in, at least initially, to taking
[00:21:00] advantage of the frontier models. Opus
[00:21:02] 5.5 feels like another one of those
[00:21:03] jumps where we're uncovering a bunch of
[00:21:05] use cases that really are significantly
[00:21:07] different with Opus 5.5 and aren't as
[00:21:10] easily translated to other models. I
[00:21:12] don't think that that changes the fact
[00:21:14] that there is still going to be fierce
[00:21:15] and extremely important competition for
[00:21:18] those cheaper and more efficient models.
[00:21:20] I think we're still in an early adoption
[00:21:22] phase where adoption is necessarily
[00:21:23] going to be more heavily concentrated in
[00:21:25] the state of the art. But as that
[00:21:27] adoption matures and the stack matures
[00:21:29] along with it, you will see those
[00:21:31] smaller, more efficient models start to
[00:21:32] come in and form a more complex stack.
[00:21:35] If anything can be said, it's that
[00:21:36] perhaps our narratives and storytelling
[00:21:39] are getting out ahead of where
[00:21:40] businesses actually are. And in that
[00:21:42] way, this is a good reminder that the
[00:21:44] things that we're discussing on the AI
[00:21:46] daily brief and within heavily
[00:21:47] enfranchised AI circles don't
[00:21:49] necessarily reflect the lived reality
[00:21:51] right now of the average business buying
[00:21:54] and using AI.
[00:21:56] Now when it comes to the competition,
[00:21:57] Anthropic has continued its ascendancy.
[00:22:00] Back in 2023, Anthropic had about 12% of
[00:22:03] business API spend. In '24, it jumped to
[00:22:05] 24% and by last year, it was up to 40%.
[00:22:08] Now it has crested over the halfway mark
[00:22:10] at 55%. And if you are once again seeing
[00:22:13] the fingerprints of agents here, you are
[00:22:15] not wrong. The Opus models ever since
[00:22:17] Opus 4.5 have been perhaps the default
[00:22:19] for long horizon agentic encoding tasks
[00:22:22] and that's now showing up in the
[00:22:23] numbers. Now OpenAI has throughout the
[00:22:26] same time in general seen a decline.
[00:22:29] They went from 50% of spend in 23 to 34%
[00:22:31] in 24 to 27 % in 25. Last year, in other
[00:22:35] words, was the first year that Anthropic
[00:22:36] actually flipped OpenAI. This year,
[00:22:38] though, we did see a slight recovery.
[00:22:40] OpenAI is now up to 31% of enterprise
[00:22:43] API spend, and Menlo's read is that this
[00:22:45] represents a strong second half of the
[00:22:47] year recovery. The GPT 5.6 series of
[00:22:50] models, including Soul, Terra, and Luna,
[00:22:51] coming in July, as well as GPT 6 in
[00:22:53] September, and just in general, OpenAI's
[00:22:56] emphasis throughout 2026 on enterprise
[00:22:58] and business use cases is clearly
[00:23:00] bearing fruit. Now, the main company
[00:23:02] that suffered and allowed Anthropic and
[00:23:04] OpenAI to both win more market share is
[00:23:06] Google. Google was down from 21% of
[00:23:09] enterprise spend last year to just 9%
[00:23:11] this year. And again, this is just the
[00:23:13] story of companies flowing to where the
[00:23:15] best model capabilities are. While
[00:23:18] Gemini 3 Pro was at the frontier in
[00:23:20] November before Opus 4 5 came out and
[00:23:22] agentic coding took over everything,
[00:23:24] that was the last time Google could
[00:23:25] reasonably be considered in a three-way
[00:23:27] race for the top of the heap when it
[00:23:28] comes to model capability. Perhaps that
[00:23:30] is changing now with Gemini 4 Carbon.
[00:23:33] Early indications look good, although it
[00:23:35] remains to be seen and needs a little
[00:23:36] bit more battle testing for us to claim
[00:23:38] that. But at the moment, when it comes
[00:23:39] to enterprise AI spend, this is a
[00:23:42] completely two-horse race between
[00:23:44] Anthropic and OpenAI. The near frontier
[00:23:46] models still haven't really broken
[00:23:49] through for as much attention as they
[00:23:50] get. Grok 47, Kimi K3, DeepSeek V4, GLM
[00:23:54] 53 all together still account for under
[00:23:57] 5% of API spend. Although as we'll see
[00:23:59] when we get to open source, when it
[00:24:01] comes to understanding open and cheaper
[00:24:03] models, it's worth looking not only at
[00:24:05] percentage of spend, but percentage of
[00:24:07] tokens.
[00:24:08] Because it turns out that while open
[00:24:10] source only gets 4% of spending, it
[00:24:12] represents about 19% of tokens.
[00:24:14] Interestingly enough, as a percentage of
[00:24:16] spend, open source is actually down. It
[00:24:18] was at 6% in 2025 and is at 4% this
[00:24:21] year. However, as a percentage of
[00:24:23] tokens, it has jumped from 11 to 19 % I
[00:24:26] I argue that in the medium to long-term,
[00:24:29] the token share numbers are more
[00:24:30] significant than the spending numbers.
[00:24:33] Like I argued before, I think right now
[00:24:35] we're still in an early adoption phase
[00:24:37] where companies are concentrating around
[00:24:39] the most expensive models to bring these
[00:24:41] new capabilities online, but the fact
[00:24:43] that you're starting to see open source
[00:24:44] take more share is directionally where
[00:24:46] things will head, and I don't think that
[00:24:48] that's a trend that's reached its peak.
[00:24:50] Now, what this says for the total
[00:24:52] addressable market value of all tokens
[00:24:54] is an interesting debate and one that
[00:24:56] happens on Wall Street all the time.
[00:24:57] There are plenty of smart people who
[00:24:59] think that in the long run, open source
[00:25:01] models represent the vast majority of
[00:25:04] tokens used, but still a relatively
[00:25:06] small percentage of overall spend, which
[00:25:08] is concentrated among the most important
[00:25:10] and elite use cases driven by the
[00:25:11] state-of-the-art closed models. By the
[00:25:13] way, when it comes to open source spend,
[00:25:15] Kimi was the dominant force this year,
[00:25:17] representing 61% of open source
[00:25:19] spending.
[00:25:20] Next up, we move to different categories
[00:25:23] of usage within the enterprise.
[00:25:25] One of the most staggering numbers, not
[00:25:28] unexpected but still staggering in its
[00:25:30] magnitude, was the revenue growth of the
[00:25:33] lab coding agents, Codex and Claude
[00:25:35] Code. That revenue jumped from $1
[00:25:37] billion
[00:25:38] at the end of 2025 to $24 billion at the
[00:25:41] end of 2026. Like I said, not surprising
[00:25:44] given how much Claude Code and Codex
[00:25:46] have just defined the experience of AI
[00:25:49] users throughout the year, but still 24x
[00:25:52] growth in revenue in a single year is
[00:25:53] just astronomical. Now, what's
[00:25:55] interesting is that this didn't
[00:25:56] necessarily come at the cost of other
[00:25:59] coding platforms like Cursor, Cognition,
[00:26:01] Factory, Lovable, etc. Their revenue
[00:26:03] still grew almost 3x this year as well,
[00:26:06] from 2.6 billion last year to 7.8
[00:26:08] billion now. It's just that the lab
[00:26:10] coding apps were by far the more
[00:26:11] significant.
[00:26:13] Now, when you start to go category by
[00:26:14] category, you might expect then that
[00:26:16] coding grew faster than any other
[00:26:19] category when it came to app spending,
[00:26:21] and you'd be almost right. Agentic
[00:26:23] coding apps grew at a 7.7x rate ahead of
[00:26:26] everything except financial services,
[00:26:29] which grew at an 8x rate. Now, the total
[00:26:32] spend on financial services apps was a
[00:26:35] tiny fraction of coding apps.
[00:26:37] Overall, Menlo estimates financial
[00:26:39] services apps saw about $800 million in
[00:26:41] spending compared to the 34 billion for
[00:26:43] coding apps, but still their speed of
[00:26:45] growth is an interesting trend. Some of
[00:26:47] the other notable areas of growth
[00:26:48] include customer success, which grew
[00:26:50] 4.3x, sales apps which grew 3.6x,
[00:26:54] legal which grew 2.8x, and down at the
[00:26:57] bottom, marketing, which grew just 1.8x.
[00:27:00] It's tempting once again, I think, to
[00:27:02] read this chart as at least in part
[00:27:04] emphasizing the fact that applications
[00:27:06] in verifiable domains where the power of
[00:27:08] agentic coding could be brought to bear,
[00:27:10] even if it wasn't for building apps,
[00:27:11] were the ones that benefited the most
[00:27:13] from the developments of 2026.
[00:27:15] Now, when it comes to which companies
[00:27:17] are being chosen to deliver the AI,
[00:27:20] there is a really strong divide between
[00:27:22] AI native companies, by which of course
[00:27:24] I mean companies like Anthropic and
[00:27:26] OpenAI, and the incumbents who are fast
[00:27:28] bringing AI into their services such as
[00:27:30] Service Now.
[00:27:31] When it comes to those coding
[00:27:33] applications, they are dominated by AI
[00:27:35] native companies. AI native companies in
[00:27:37] fact represent 96% of that spend.
[00:27:40] Finance and operations is also up there
[00:27:42] where AI native companies represent 95%
[00:27:44] of spend, and AI natives also rule the
[00:27:46] design field representing 81% of spend.
[00:27:49] Sales is nearly split in the middle with
[00:27:51] 54% of the spend going to AI natives
[00:27:53] versus 46% to incumbents, but then every
[00:27:56] other area, marketing, customer success,
[00:27:58] HR, data science, and IT, all see the
[00:28:01] incumbents getting more than 50% of
[00:28:03] market share. Basically, big chunks of
[00:28:05] enterprise spend has wanted to flow
[00:28:08] towards the solutions they already use
[00:28:10] and already have embedded and already
[00:28:11] have connected to their systems of
[00:28:13] record or which are their systems of
[00:28:14] record rather than ripping that out and
[00:28:16] building something completely new. It
[00:28:18] makes sense then on the other end of the
[00:28:19] spectrum that agentic coding, which is a
[00:28:21] net new capability, doesn't yet have an
[00:28:23] incumbent solution that's plugged into
[00:28:25] all the systems, so it has room for a
[00:28:27] new solution to come in. Compare that to
[00:28:29] IT, for example, where many companies
[00:28:31] have been using the same vendor or
[00:28:33] partner for years, if not decades, and
[00:28:35] it makes sense, perhaps, then that only
[00:28:37] 9% of AI app spend for IT is coming from
[00:28:40] AI native companies compared to 91%
[00:28:43] that's going to incumbents.
[00:28:45] So what does this all mean for software?
[00:28:48] Another question that lurks,
[00:28:48] particularly in the minds of investors
[00:28:50] who are trying to figure out how AI
[00:28:51] plays out, is whether AI just eats SaaS.
[00:28:55] One of the big stories of 2026 was, of
[00:28:57] course, the SaaS pocalypse where for a
[00:28:59] while at the beginning of the year as
[00:29:00] Agentic Coding came online, SaaS stocks
[00:29:03] were just absolutely decimated as people
[00:29:05] operated on the idea that the ability to
[00:29:07] roll your own apps or spin your own apps
[00:29:09] was going to fundamentally undermine the
[00:29:11] use of those SaaS tools.
[00:29:13] That's not exactly the story that Menlo
[00:29:15] found, however. While Menlo did find
[00:29:17] some diminished growth of the SaaS
[00:29:19] application market from 13% growth in
[00:29:21] 2025
[00:29:23] to 11% growth in 2026, they found that
[00:29:26] the majority of new AI spending actually
[00:29:28] came from net new budgets, not existing
[00:29:31] software budgets. Of the AI spending
[00:29:33] that could be accounted for by Menlo,
[00:29:35] 21% came from existing software budgets.
[00:29:38] That compared to 55% which was net new
[00:29:40] budgets.
[00:29:41] Now that's obviously positive news for
[00:29:43] SaaS investors and SaaS companies,
[00:29:45] although I do think that we have barely
[00:29:46] gotten started on the next narrative
[00:29:48] which threatens SaaS, which is the rise
[00:29:49] of agents using software and headless
[00:29:51] software, and all it takes is reading
[00:29:53] some comments from Salesforce to
[00:29:54] understand how significant that
[00:29:55] disruption could be as well.
[00:29:57] For now, however, it looks like a lot of
[00:29:59] AI spend is net new, not just
[00:30:01] cannibalizing spend that already
[00:30:02] existed.
[00:30:03] So that is Menlo's State of Enterprise
[00:30:05] AI. Like I said at the top, I think that
[00:30:07] this broadly reflects a lot of what
[00:30:08] we've been discussing and seeing
[00:30:10] throughout the show. Although it is a
[00:30:11] good reminder that there remains a gap
[00:30:13] between our narratives that we explore
[00:30:15] every day and the trends that we see on
[00:30:17] the horizon and the lived experience
[00:30:19] that companies operate within every day.
[00:30:21] For now, that is going to do it for
[00:30:22] today's AI Daily Brief. Appreciate you
[00:30:24] listening or watching as always, and
[00:30:26] until next time, peace.
