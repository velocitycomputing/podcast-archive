---
record_id: "podcast:136d7e78-94f9-4a90-8718-15befd0f7321"
episode_id: 136d7e78-94f9-4a90-8718-15befd0f7321
title: How to Navigate the Next Wave of AI Competition
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-to-navigate-the-next-wave-of-ai-competition/136d7e78-94f9-4a90-8718-15befd0f7321"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-to-navigate-the-next-wave-of-ai-competition/136d7e78-94f9-4a90-8718-15befd0f7321"
feed_guid: null
feed_url: "https://anchor.fm/s/f7cac464/podcast/rss"
published_at: null
published_local_date: null
played_date: 2026-08-31
played_at: "2026-08-31T12:00:00Z"
play_count: 1
duration_seconds: 1680
source: pocketcasts-history-browser
played_label: August 31
history_order: 77
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 0a61cb16a5d57b50ccbc8c0862b7f018e291d33ed849af28762a973fc2eba9b4
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

OpenAI said it would cut off access to its models in Cursor by November 12 after SpaceX/Elon Musk’s company acquired Cursor, citing alleged terms-of-service violations tied to XAI/SpaceX; Cursor CEO Michael Troll said OpenAI models serve about 5% of Cursor traffic, while OpenAI product manager Tibo argued those tokens may represent disproportionate value because frontier models can complete tasks with fewer tokens. The episode framed this as part of a broader frontier-lab pattern—Anthropic cut off Windsurf in June 2025, blocked OpenAI’s API in August 2025, blocked xAI in January, and changed subscription terms—while Anthropic’s Tom Brown said Anthropic would continue supporting Cursor, Google’s Logan Kilpatrick hinted OpenAI was making a mistake, and critics including Tim Sweeney and Ysef Altuki called the move harmful. Other headlines covered blue-collar unions organizing for data centers, including Steamfitter UA Local 602 treasurer Sydney Bonia and Electrician Workers Local 26 political coordinator Don Sllayman, with some unions breaking from Democrats and backing a Kansas Republican gubernatorial candidate; investor Gavin Baker and Nvidia’s Jensen Huang praised data centers as reindustrialization. The Trump administration is reportedly drafting Commerce Department rules to block Chinese labs from remote access to NVIDIA chips via Thailand, Malaysia, and Japan, a narrowed version of the AI diffusion rule criticized by Under Secretary Jeffrey Kesler; a federal judge, Rita Lynn, ruled the Pentagon’s supply-chain-risk designation of Anthropic violated the First and Fifth Amendments and ordered it rescinded, though another appeal remains. Apple reported Mac sales up 29%, the fastest product-line growth, with Mac Mini demand tied to agent workloads, enterprise cost-cutting, OpenAI buying tens of thousands of Mac Minis/Mac Studios for reinforcement learning, and Anthropic renting Mac Minis from AWS; OpenAI cut GPT56 Luna API prices 80%, Terra 20%, and Soul 20%, driving OpenRouter usage up 5.6x for Terra and 13.8x for Luna, with about a third staying at full price, illustrating Jevons-paradox-style enterprise adoption. The main strategic claim was that enterprises must move beyond cost-only open-weight model adoption to control over both models and harnesses, citing Microsoft’s “reverse information paradox,” Moody’s David Pan’s “harness engineering,” AT&T and Thomson Reuters using open models, and DeepSeek’s plugin-based DeepSeek Harness.

For enterprise and developer decisions, the concrete takeaway is to treat frontier-model availability as a supply-chain risk, not just a pricing question: if you or your organization depend on Cursor, OpenAI, Anthropic, or another lab, inventory which workflows run through third-party harnesses, set a migration plan before cutoff dates such as November 12, and build direct vendor relationships or contractual protections where possible. Develop an open-weights and routing policy now, identifying tasks that can move to lighter, cheaper, locally controlled models while keeping frontier models for high-value tasks; measure value per task, not just token share, because a small share of tokens can carry outsized revenue or workflow value. Consider owning or controlling the harness—prompts, tools, evals, logs, corrections, orchestration, and data flows—so the organization can switch providers without rebuilding workflows; evaluate open harnesses such as DeepSeek Harness and internal “harness engineering” options, and ask vendors what data, corrections, and proprietary context are learned from usage and how that learning can be kept private or exported. For enterprise buyers, decisions to consider include diversifying model providers, testing open-weight stacks such as Qwen-based architectures, negotiating custom contracts, tracking OpenRouter-style usage and price elasticity, and preparing for Jevons-paradox effects where lower token prices unlock more automation. For policy or investment follow-ups, watch whether Commerce closes the remote-access chip loophole, how the Anthropic Pentagon appeals proceed, whether unions change data-center politics, and whether Apple’s Mac Mini/local-agent trend becomes a durable enterprise cost-control path.

## Transcript

[00:00:00] Late last week, OpenAI announced that
[00:00:01] they would be cutting off access to
[00:00:03] their models in Cursor. Now, for many
[00:00:05] Cursor users, this is a huge blow. They
[00:00:07] invested in that harness ecosystem and
[00:00:09] view OpenAI's move as some version of
[00:00:11] competitive pettiness. Other observers
[00:00:13] think that this was always inevitable as
[00:00:15] soon as SpaceX AAI decided to buy
[00:00:17] Cursor. They point to other examples
[00:00:18] like anthropic cutting off Windfur in
[00:00:20] mid 2025 to say that this is just the
[00:00:22] way that Frontier Lab competition is
[00:00:24] going to work from here on out. And
[00:00:25] while this all might seem like just
[00:00:26] psycho drama competition between the
[00:00:28] labs, for enterprise AI users, it has
[00:00:30] very significant implications. Already
[00:00:33] there was a push in enterprises to
[00:00:35] understand and to better be able to take
[00:00:36] advantage of open weights models to
[00:00:38] build the capability to have more
[00:00:40] complex model architectures that allow
[00:00:42] their users to better match the task
[00:00:43] with the capability level in a way that
[00:00:45] is more cost-effective. What these moves
[00:00:47] make clear is that this is not just a
[00:00:48] costefficiency conversation, but is more
[00:00:50] broadly about control and resilience.
[00:00:52] And what these latest moves make clear
[00:00:54] is that enterprises have to think not
[00:00:55] only about these questions in terms of
[00:00:57] models, but in terms of harnesses as
[00:00:59] well. The AI Daily Brief is a daily
[00:01:01] podcast and video about the most
[00:01:02] important news and discussions in AI.
[00:01:05] Welcome back to the AI Daily Brief
[00:01:07] headlines edition. All the daily AI news
[00:01:09] you need in around 5 minutes. Today we
[00:01:12] begin with a follow-up in the ongoing
[00:01:13] saga of the data center debate where
[00:01:15] bluecollar labor unions are organizing
[00:01:18] to support data center construction. As
[00:01:20] data centers become a pivotal political
[00:01:22] issue for the midterms, labor unions are
[00:01:24] becoming the backlash to the backlash
[00:01:26] and are threatening to withhold support
[00:01:27] from candidates who oppose data centers.
[00:01:30] The Wall Street Journal viewed a memo
[00:01:31] from Steamfitter UA Local 602, whose
[00:01:34] members install industrial piping across
[00:01:36] Virginia and Maryland covering the
[00:01:37] region known as data center alley. The
[00:01:40] union said that they were drawing a
[00:01:41] quote clear line and won't back any
[00:01:43] politicians running on an anti-data
[00:01:45] center platform. They added, "This is an
[00:01:48] existential moment for local 602. In
[00:01:51] some cases, unions are breaking their
[00:01:52] long-standing alliance with local
[00:01:54] Democrats over the issue. The Kansas
[00:01:56] HVAC and Railroad workers union have
[00:01:58] supported the Republican gubernatorial
[00:02:00] candidate for the first time in decades
[00:02:01] over the issue. Sydney Bonia, the
[00:02:04] treasurer for Steamfitters Local 602,
[00:02:05] emphasized that union support isn't just
[00:02:07] about votes. He said his union also
[00:02:09] participates in doornocking and
[00:02:11] fundraising to support local campaigns.
[00:02:13] Bonia expects unions across the country
[00:02:15] to follow suit in rejecting anti-data
[00:02:17] center candidates, commenting, "We are
[00:02:19] dependent on these jobs." Other union
[00:02:21] leaders are asking politicians which
[00:02:23] side they are on. Don Sllayman, the
[00:02:25] political coordinator for Electrician
[00:02:26] Workers Local 26 in Virginia and
[00:02:28] Maryland said, "You're not a friend if
[00:02:30] you're taking away great career
[00:02:31] opportunities. This is a once in a
[00:02:33] generation opportunity to really get in
[00:02:34] the upper middle class." Now, if you
[00:02:36] have been paying attention to my
[00:02:38] coverage of this issue for the last
[00:02:39] several months, you will have seen this
[00:02:41] start to bubble and emerge. In fact, in
[00:02:43] my last episode that was a primer all
[00:02:45] about this issue, one of my arguments
[00:02:46] was that these labor unions were most
[00:02:48] uniquely suited to intercede in the
[00:02:50] middle between these communities and the
[00:02:52] tech companies that are building the
[00:02:53] data centers. Given that the unions are
[00:02:55] both deeply rooted in those communities,
[00:02:56] but also stand to benefit economically
[00:02:58] from the transformation that they bring.
[00:03:00] Overall, I think it's an extremely
[00:03:02] positive development that could bring a
[00:03:03] lot of common rationality to the
[00:03:05] discussion that has been lacking thus
[00:03:07] far. For some, this is a moment to turn
[00:03:09] the tide. Investor Gavin Baker wrote,
[00:03:12] "There were reasonable concerns about
[00:03:13] data centers 18-ish months ago. Water,
[00:03:15] taxes, jobs, electricity prices, the
[00:03:17] environment, and what they would do to
[00:03:19] small towns. Well ststructured data
[00:03:21] center projects have largely addressed
[00:03:22] these concerns today, and we should be
[00:03:24] celebrating this. On balance, data
[00:03:26] centers are awesome for America in every
[00:03:28] way. No less than Nvidia's Jensen Huang
[00:03:31] reposted Gavin and said, "Spoton, AI is
[00:03:33] bringing manufacturing back to America
[00:03:35] and re-industrializing the nation after
[00:03:37] decades of offshoring. We have the
[00:03:39] opportunity to create lasting benefits
[00:03:40] for communities across America and help
[00:03:42] America lead the next industrial
[00:03:43] revolution."
[00:03:45] Next up, another frequent topic in the
[00:03:47] headlines. The Trump administration is
[00:03:49] developing rules to prevent Chinese labs
[00:03:51] from getting remote access to AI chips.
[00:03:53] Now, earlier this month, CNBC reported
[00:03:56] that multiple Chinese firms had access
[00:03:57] to cuttingedge NVIDIA chips through data
[00:03:59] center hubs in Thailand, Malaysia, and
[00:04:01] Japan. Alongside renting compute from
[00:04:03] third party operations, the reporting
[00:04:05] claimed that some of the data centers
[00:04:06] were owned by Alibaba and Bite Dance.
[00:04:08] Importantly, none of this was illegal as
[00:04:10] the export controls only govern physical
[00:04:12] exports into China. But of course, if
[00:04:14] the administration's goal was to block
[00:04:16] access to cuttingedge chips, then this
[00:04:18] sort of arrangement undermines the
[00:04:19] entire policy. The information reports
[00:04:21] that the Commerce Department is
[00:04:22] currently working on a new rule aimed at
[00:04:24] closing the loophole. Sources described
[00:04:26] it as a slim down version of the AI
[00:04:28] diffusion rule, which was introduced in
[00:04:29] the final week of the Biden
[00:04:31] administration and immediately scrapped
[00:04:32] once Trump took office. The rule was
[00:04:34] heavily criticized for having a huge
[00:04:36] enforcement and administrative burden,
[00:04:37] but it would have made it difficult to
[00:04:39] establish third-country data center hubs
[00:04:40] for the Chinese labs. Among other
[00:04:42] things, the diffusion rule capped AI
[00:04:44] chip imports at a very low level for
[00:04:46] unaligned nations. Those caps could be
[00:04:48] raised if national governments worked
[00:04:49] with the US to ensure their data centers
[00:04:51] wouldn't service Chinese companies. Now,
[00:04:53] it's unclear from the reporting exactly
[00:04:55] how far the new rule would go and
[00:04:57] whether it even has support within the
[00:04:58] administration. Critics of the diffusion
[00:05:01] rule argued that it would weaken
[00:05:02] America's dominance in the chip
[00:05:03] industry, pushing most of the world to
[00:05:04] adopt Chinese technology. Senior
[00:05:06] officials at the Commerce Department
[00:05:08] have been vocally critical of the
[00:05:09] diffusion rule with Under Secretary
[00:05:11] Jeffrey Kesler telling Congress in July,
[00:05:13] "I don't want to replace the diffusion
[00:05:14] rule because I don't think the rule is
[00:05:15] worth replacing. It's a bad rule and
[00:05:17] we're glad that it's not being
[00:05:18] enforced." But if you have watched
[00:05:20] anything when it comes to AI policy out
[00:05:22] of this particular White House, you know
[00:05:23] that among three people, there's going
[00:05:25] to be four opinions. So, we'll just have
[00:05:26] to wait and see where it lands.
[00:05:29] Speaking of this administration,
[00:05:30] Anthropic has won their lawsuit against
[00:05:32] the Pentagon with a federal judge ruling
[00:05:34] that the government had no basis for
[00:05:36] declaring them a supply chain risk. In
[00:05:38] her order, US District Judge Rita Lynn
[00:05:40] found the government hadn't provided
[00:05:42] evidence that anthropic represented a
[00:05:43] genuine threat to national security.
[00:05:45] Instead, Judge Lynn wrote, "Defendants
[00:05:47] contemporaneous words and deeds
[00:05:48] confirmed that the challenged actions
[00:05:50] were based on a desire to make a public
[00:05:52] example out of anthropic for its quote
[00:05:54] unquote arrogance in criticizing the
[00:05:55] government. The empty invocation of
[00:05:57] national security is not a blank check
[00:05:59] to punish and retaliate against
[00:06:00] government critics. In particular, Judge
[00:06:03] Lynn noted that the government's
[00:06:04] continued use of anthropics models
[00:06:06] undermine the Pentagon's claims. The
[00:06:07] order found that the government had
[00:06:08] violated the First and Fifth Amendments
[00:06:10] in making the designation. Judge Lynn
[00:06:12] wrote, "Though the Department of War is
[00:06:14] undisputedly free to select the AI
[00:06:15] vendor of its choice, the evidence
[00:06:17] demonstrates that the broad measures
[00:06:18] imposed on anthropic were illegal and
[00:06:21] baseless. The order directed the
[00:06:23] government to rescend all guidance and
[00:06:24] directives that blacklisted Anthropic as
[00:06:25] a supply chain risk. Consequently, the
[00:06:27] order directed the government to rescend
[00:06:29] all guidance and directives that
[00:06:30] blacklisted Anthropic as a supply chain
[00:06:32] risk. Now, while this is a big win for
[00:06:34] Anthropic, they are certainly not out of
[00:06:36] the woods just yet. A second lawsuit in
[00:06:38] the DC appeals court is still waiting a
[00:06:39] ruling, and the judge in that case has
[00:06:41] been so far a bit more receptive to the
[00:06:43] Pentagon's arguments. One funny little
[00:06:45] story, in a follow-up to the Mac Mini
[00:06:47] craze of earlier this year. In their
[00:06:49] most recent earnings report, Apple said
[00:06:50] that Mac sales were up 29% over the past
[00:06:53] year, which was the fastest growth of
[00:06:54] any product line at the company. And of
[00:06:56] course, for those in the no, the
[00:06:57] openclaw boom was a big part of that,
[00:06:59] leading to an estimated $und00 million
[00:07:01] plus of Mac Mini sales. Now, most
[00:07:03] assumed this was just a consumer trend
[00:07:05] with hobbyists and early adopters
[00:07:07] snatching up Mac Minis to run their new
[00:07:09] suite of agents. when the new Mac Mini
[00:07:10] line was unveiled last week. Although
[00:07:12] the specs were up, the price was up
[00:07:14] meaningfully as well, making it
[00:07:15] potentially a little bit more out of
[00:07:16] reach for that generalist sort of
[00:07:18] audience. Over the weekend, however, the
[00:07:20] information published a deep dive on
[00:07:21] how, in fact, a big part of the Mac Mini
[00:07:23] explosion has been enterprise demand. In
[00:07:26] June, Apple held an enterprise focused
[00:07:28] hardware sales event with significant
[00:07:30] emphasis on the Mac Mini, which was
[00:07:31] pitched as a cost cutting measure,
[00:07:33] allowing simple agents and AI models to
[00:07:35] be run locally instead of contributing
[00:07:36] to rising cloud bills. Former Apple
[00:07:39] enterprise marketing manager Todd Daly
[00:07:41] remarked on how out of character this
[00:07:43] was for Apple. Apple doesn't have a
[00:07:45] dedicated engineering team for business
[00:07:46] customers or even a developer relations
[00:07:48] team. Daly commented, "The idea that any
[00:07:50] team at Apple has an actual plan for
[00:07:52] embracing enterprise AI is a joke.
[00:07:54] Still, enterprise demand seems to be
[00:07:56] very real in some pockets." Sources told
[00:07:58] the information that OpenAI has
[00:08:00] purchased tens of thousands of Mac minis
[00:08:02] and Mac Studios for reinforcement
[00:08:04] learning. The machines are used to train
[00:08:06] computer use agents and sources said
[00:08:07] OpenAI is desperate to buy more.
[00:08:09] Anthropic is apparently also renting Mac
[00:08:11] minis from AWS according to people
[00:08:13] familiar with the operations. In other
[00:08:15] words, even with the price increases, it
[00:08:17] seems that the humble Mac Mini will
[00:08:18] continue to play a significant role in
[00:08:20] the next wave of AI.
[00:08:22] Now, speaking of OpenAI, the subject of
[00:08:25] today's main episode is about a big
[00:08:27] decision that OpenAI made at the end of
[00:08:29] last week and what it means for
[00:08:30] enterprises and companies who have to
[00:08:32] position themselves for a new
[00:08:33] competitive reality. Well, speaking of
[00:08:36] competitive realities, OpenAI recently
[00:08:38] introduced some significant price cuts.
[00:08:40] They cut prices on GPT56 Luna by 80% and
[00:08:43] the larger Terra version by 20% through
[00:08:45] the API. They later announced a 20%
[00:08:48] price reduction on Soul, although that
[00:08:49] pricing has only been in effect for a
[00:08:51] couple of weeks now. The assumed goal of
[00:08:53] all of this is to drive up usage on
[00:08:54] third party platforms like open router.
[00:08:57] This could be part and parcel of a
[00:08:58] recognition that the Frontier Labs now
[00:09:00] have to compete not just on the frontier
[00:09:01] when it comes to raw capability, but
[00:09:03] also when it comes to the frontier of
[00:09:05] efficiency. However, some also
[00:09:07] speculated that because media uses
[00:09:08] thirdparty platform usage like Open
[00:09:10] Router as a proxy for overall token
[00:09:12] consumption, even though that's a pretty
[00:09:14] massive misread of the data, that
[00:09:16] perhaps OpenAI's goal was to get an
[00:09:18] outsized PR effect from a relatively
[00:09:20] minor move. With the battle heating up
[00:09:22] ahead of Anthropic's IPO in the coming
[00:09:24] months, this could be a way for OpenAI
[00:09:26] to generate some concerning headlines.
[00:09:28] Whatever the motivation and the ultimate
[00:09:30] goal, Open Router is reporting a massive
[00:09:32] boost in usage for OpenAI's models. They
[00:09:34] report that daily usage of Terra is up
[00:09:36] 5.6x after the discount and Luna rose a
[00:09:39] massive 13.8x. Soul was not yet
[00:09:42] discounted during the window they looked
[00:09:43] at and its usage was relatively flat
[00:09:45] with just a 10% gain. What's more, while
[00:09:48] the discounts on Terra and Luna expired
[00:09:50] on August 14th, Open Router reports that
[00:09:52] users stuck around with nearly a third
[00:09:54] of them continuing with OpenAI's models
[00:09:55] at full price. Boxes Aaron Levy reposted
[00:09:58] the chart and said, "Sometimes people
[00:10:00] don't have an intuitive sense of what
[00:10:01] Javvon's paradox looks like for token
[00:10:03] consumption. Those of us working with
[00:10:04] enterprises get to see this firsthand
[00:10:06] every day. Basically, enterprises have
[00:10:09] an unending stream of tasks that they'd
[00:10:10] love to be able to bring automation to,
[00:10:12] but for each individual task, it's
[00:10:14] either ROI positive or not based on the
[00:10:16] cost of bringing automation to it. As
[00:10:18] tokens get cheaper at a certain
[00:10:19] capability threshold, enterprises can
[00:10:21] afford bringing more of them to the work
[00:10:23] that they do. This could be processing
[00:10:24] every contract, reading every log,
[00:10:26] watching new streams of data for
[00:10:28] insights, having background agents
[00:10:29] execute workflows, and so on. Anytime we
[00:10:32] can lower the cost of tokens, we will
[00:10:34] see a disproportionate increase in
[00:10:35] consumption. Even a 50% drop in token
[00:10:38] prices could result in a 5x increase in
[00:10:40] tokens for these kinds of workloads.
[00:10:42] That's why it's critical to keep
[00:10:43] bringing down the cost of AI and why
[00:10:45] that's good for all market participants.
[00:10:47] For cells, Brandon Gailing added,
[00:10:49] "Beyond just Javvon's paradox, cheaper
[00:10:51] tokens means entire use cases go from 0
[00:10:53] to one in viability given an
[00:10:54] organization's willingness to spend and
[00:10:56] their risk tolerance for experiments.
[00:10:58] Many tasks require some minimum quantity
[00:11:00] of tokens to actually do the job. If the
[00:11:02] pricing doesn't allow you to hit that
[00:11:03] minimum feasibility, it won't be done.
[00:11:05] When the pricing drops, enterprises are
[00:11:07] able to get to the point of value and
[00:11:08] greenlight use cases that were
[00:11:09] previously not viable before. Their
[00:11:11] total token spend increases, but so does
[00:11:13] the value and ROI they get from it. Now,
[00:11:16] like I said, today's main episode is all
[00:11:18] about some new competitive moves. And
[00:11:19] the reason I wanted to end on this story
[00:11:21] about the impact of OpenAI's competitive
[00:11:23] pricing experiments is that it's
[00:11:24] exemplary of the experimental moment
[00:11:26] that I think we're heading into. But
[00:11:28] with that, let's close the headlines and
[00:11:30] move on over into that main episode.
[00:11:33] Welcome back to the AI daily brief. On
[00:11:35] Friday night, OpenAI announced that they
[00:11:37] would be ending their relationship with
[00:11:38] Cursor. This is a highly consequential,
[00:11:41] if not necessarily particularly
[00:11:42] surprising, decision. And on the one
[00:11:44] hand today we are going to discuss what
[00:11:46] this means for the state of AI
[00:11:48] competition among the frontier labs. But
[00:11:50] we will also get into what is I think
[00:11:52] the more important discussion at least
[00:11:53] for all of us in an applied sort of way
[00:11:55] which is how to position ourselves and
[00:11:57] our companies for the inevitabilities
[00:11:59] that that next phase of competition
[00:12:01] bring. While we can't read the future I
[00:12:03] think that there are some pretty clear
[00:12:04] patterns that have some fairly
[00:12:06] significant implications for how we
[00:12:07] think about enterprise AI strategy. But
[00:12:10] first, let's talk about the move that
[00:12:11] OpenAI made. In a late Friday
[00:12:13] announcement, OpenAI basically said, "We
[00:12:15] love Curser, but we hate Elon, so sorry
[00:12:17] Cursor users. You don't get to use
[00:12:19] OpenAI models anymore." Now, they tried
[00:12:21] to frame it a little bit nicer in the
[00:12:22] press release. They wrote, "To work with
[00:12:24] a large partner like SpaceX, we
[00:12:26] typically rely on custom contracts to
[00:12:27] ensure compliance with our terms of
[00:12:29] service, and the integration provides
[00:12:30] for safety at scale." After Musk
[00:12:32] acquired Twitter, now part of SpaceX,
[00:12:34] the company broke the terms of our
[00:12:35] contract alongside many others. Under
[00:12:37] oath earlier this year, Musk admitted
[00:12:39] that XAI, now also part of SpaceX, had
[00:12:41] violated OpenAI's terms of service. On
[00:12:44] the flip side, when it comes to Curser,
[00:12:45] they said, "We've worked with Curser for
[00:12:46] nearly four years and have enormous
[00:12:48] respect for their team, their product,
[00:12:49] and what they've built for the developer
[00:12:51] community. We know that the people most
[00:12:53] affected by this decision are the
[00:12:54] developers who rely on OpenAI models in
[00:12:57] Cursor. We care about their experience
[00:12:59] in this transition, and we're ready to
[00:13:00] go above and beyond to support them."
[00:13:02] Now the cutoff will not actually come
[00:13:04] until November 12th and that long
[00:13:06] deadline seems to be intentional with
[00:13:07] OpenAI saying that they are giving the
[00:13:09] maximum notice provided by their
[00:13:11] contract. Now Elon's response will
[00:13:13] likely come as no surprise. He responded
[00:13:15] to a post on X saying I couldn't care
[00:13:17] less and using his favorite moniker of
[00:13:19] calling Sam Alman scam Altman. Cursor
[00:13:22] CEO Michael Troll said that they were
[00:13:23] sorry to see the note and were seeing if
[00:13:25] they couldn't come to some different
[00:13:26] agreement. Now, he also included a note
[00:13:28] that OpenAI models serve about 5% of
[00:13:30] cursor user traffic. Clearly with the
[00:13:32] implication that even if they weren't
[00:13:34] able to come to some agreement that this
[00:13:35] wouldn't be all that bad. OpenAI product
[00:13:38] manager Tibo for some reason felt the
[00:13:39] need to clarify on that 5% reposting
[00:13:42] Michael Troll and arguing tokens are not
[00:13:44] a proxy for revenue nor value created
[00:13:46] and the OpenAI models are on the very
[00:13:47] frontier of token efficiency. Smaller or
[00:13:50] less strong models require many more
[00:13:51] tokens to achieve a task and therefore
[00:13:53] will inflate traffic share
[00:13:54] significantly. His point in other words
[00:13:56] is that even if that 5% of token traffic
[00:13:58] is factually accurate, it might
[00:14:00] represent more like 10 or 15 or 20 or
[00:14:02] even more percentage of the actual value
[00:14:04] created because of what particular tasks
[00:14:06] people are using OpenAI models for and
[00:14:08] how much more efficiently they do them.
[00:14:10] Now, why he decided that he had to
[00:14:12] increase everyone's awareness of the
[00:14:13] pain that they were causing for cursor
[00:14:15] users isn't exactly clear, but Epic
[00:14:17] founder Tim Sweeney was happy to jump in
[00:14:19] and say, "Maybe don't screw over chatbt
[00:14:21] customers who use cursor then. No
[00:14:23] developers on Earth want you guys waging
[00:14:25] corporate warfare inside our computers.
[00:14:27] Now, a natural question might be, is
[00:14:29] Anthropic going to follow suit? However,
[00:14:31] co-founder and chief comput officer Tom
[00:14:33] Brown said absolutely not. He posted on
[00:14:35] X, Cursor has been a trusted partner of
[00:14:37] Anthropic since Sonnet 3.5. We'll
[00:14:40] continue to increase compute to support
[00:14:41] cloud models in Cursor and are excited
[00:14:43] for what comes next with them at SpaceX.
[00:14:45] Google's Logan Kilpatrick, vague, but
[00:14:46] not that vague, tweeted, "If your
[00:14:48] opponent is busy making a mistake, don't
[00:14:50] interrupt them." And certainly for many
[00:14:52] in the community, it is OpenAI who's
[00:14:54] making a mistake here. Daim ManX writes,
[00:14:57] "Biggest loser here is OpenAI. Cursor
[00:14:59] already has Gro 4.7 on the way, Composer
[00:15:01] 3, and a bunch of open models. What Open
[00:15:03] AAI just did is going to make every
[00:15:04] partner start thinking about plan B."
[00:15:07] Ysef Altuki writes, "This behavior is
[00:15:09] genuinely so poor. Most of my usage of
[00:15:11] OpenAI models was on Cursor. Cursor,
[00:15:14] unlike Codeex, has a fast mode toggle
[00:15:16] for the models that actually works and
[00:15:17] causes a 2x speed increase. Cursor IDE
[00:15:19] has the most gorgeous UX. Open AAI is
[00:15:22] stripping this away from paying users
[00:15:23] due to nothing but pettiness. There is
[00:15:25] no valid reason to stop paying users
[00:15:26] from using the model of their choice and
[00:15:28] the harness of their choice. Then to add
[00:15:30] insult to injury, they replied to
[00:15:31] Curser, actually when you look at our
[00:15:33] efficiency, we contributed more than 5%.
[00:15:35] No point other than rubbing salt in the
[00:15:37] wound of customers. And yet for others,
[00:15:39] there are pretty clearly some reasons
[00:15:41] other than pettiness for OpenAI to make
[00:15:43] this move. Benjamin Decracker writes,
[00:15:45] "The entire reason SpaceXI bought Cursor
[00:15:48] is to harvest training data from people
[00:15:49] using it for coding. This is very
[00:15:51] obvious and this advantage was openly
[00:15:53] touted as a huge win for XAI when the
[00:15:55] acquisition was announced. Isn't it
[00:15:57] somewhat reasonable for OpenAI to opt
[00:15:59] out their advanced models being included
[00:16:01] in that training data harvester?"
[00:16:03] Pragmatic Engineering's Gugglia Rose
[00:16:04] writes, "Frontier model companies don't
[00:16:06] offer direct integration of their models
[00:16:08] for tools built by other Frontier model
[00:16:10] companies. Eg. You can't use GPT56 from
[00:16:12] claw code or opus 5 from codec out of
[00:16:14] the box. Cursor is now SpaceX, so OpenAI
[00:16:17] pulling GPT. Not all that surprising.
[00:16:20] Gail Weiner writes, "What was OpenAI
[00:16:22] supposed to do? This isn't just a
[00:16:23] competitor bought Cursor, but it's a
[00:16:24] competitor who took them to court to try
[00:16:26] to destroy them. And much more
[00:16:28] significantly of all, many pointed out
[00:16:29] that this is not some isolated incident,
[00:16:32] but this is just the norm now of how
[00:16:33] Frontier Labs behave. An early example
[00:16:36] of this came back in June of 2025. After
[00:16:38] Bloomberg reported that OpenAI was close
[00:16:40] to nearing a deal to acquire Windinsurf,
[00:16:43] Anthropic cut off Windsurf's access to
[00:16:45] their models. On June 3rd, 2025,
[00:16:48] Windsurf's Von Moan wrote, "With less
[00:16:50] than 5 days of notice, Anthropic decided
[00:16:51] to cut off nearly all of our first party
[00:16:53] capacity to claude 3.x models." This was
[00:16:56] a point that many brought up with Tom
[00:16:57] Brown in the comments when he posted
[00:16:59] about Cursor being a trusted partner of
[00:17:01] Anthropics in Sonnet 3.5. Replet CEO
[00:17:04] Amjad Msad wrote, "Maybe you've changed
[00:17:06] your ways, but we all remember what you
[00:17:07] did to Windsurf, which was infinitely
[00:17:09] nastier." Amjad continued pointing out
[00:17:11] that it is likely that part of
[00:17:12] Anthropic's difference of approach here
[00:17:14] has to do with the fact that they now
[00:17:15] have a compute relationship with SpaceX
[00:17:17] AI that is integral to the training of
[00:17:19] their future models. AI researcher Meu
[00:17:21] Mohan writes, "I don't get the hate
[00:17:23] OpenAI is getting for banning Cursor and
[00:17:25] how Anthropic is somehow trying to be
[00:17:26] the good guy here. Anthropic literally
[00:17:28] did the same thing with Windsurf one
[00:17:29] year ago and would 100% have done the
[00:17:31] same with SpaceXI if Anthropic was not
[00:17:32] paying a billion dollars per month for
[00:17:34] compute to them. Why is this
[00:17:35] controversial? And the Windsurf thing
[00:17:38] wasn't an isolated incident. In August
[00:17:39] of 2025, Anthropic blocked OpenAI's
[00:17:42] access to the API. They claimed a
[00:17:44] violation of terms of service, which
[00:17:45] most believed was about using
[00:17:46] Anthropic's models to build a competing
[00:17:48] AI model. OpenAI's story was that they
[00:17:50] were just benchmarking the models, but
[00:17:52] clearly in retrospect, the whole move
[00:17:53] was about concerns about distillation.
[00:17:56] Then in January of this year, Enthropic
[00:17:58] also blocked XAI. In a Slack message in
[00:18:01] January, XAI co-founder Tony Wu said,
[00:18:03] "Hi team, I believe many of you have
[00:18:05] already discovered that Enthropic models
[00:18:06] are not responding on Cursor. According
[00:18:08] to Cursor, this is a new policy
[00:18:09] anthropic is enforcing for all its major
[00:18:11] competitors. This is both bad and good
[00:18:14] news. We will get a hit on productivity,
[00:18:15] but it really pushes us to develop our
[00:18:17] own coding models and products. We're at
[00:18:19] a time in which AI is now a critical
[00:18:21] technology for our own productivity. The
[00:18:23] team is rapidly developing our own
[00:18:24] models and product. We will have
[00:18:26] something to share with everyone soon.
[00:18:27] In the meantime, you may still try
[00:18:28] different kinds of models in Grock
[00:18:30] Build. Then, of course, over the next
[00:18:31] couple of months, Enthropic changed the
[00:18:33] way their subscriptions work to not
[00:18:35] cover third party tools, specifically
[00:18:37] things like OpenClaw and Hermes. Hermes
[00:18:39] co-founder Technium was happy to point
[00:18:41] this one out to Tom Brown as well. A
[00:18:43] couple months later, Anthropic partnered
[00:18:44] with Figma publicly and then poached an
[00:18:46] executive and launched Claw Design to
[00:18:48] compete directly, which led to a July
[00:18:50] story in the Wall Street Journal about a
[00:18:52] concern that Anthropic was going to use
[00:18:54] proprietary information that they got
[00:18:55] from people using their models to build
[00:18:57] competing services to their customers.
[00:18:59] And while these examples have all been
[00:19:01] anthropic, many have been beating the
[00:19:02] drum that this is just the way that it's
[00:19:04] going to work in the next phase of
[00:19:05] competition. Palanteers Alex Karp has
[00:19:07] been screeching about this to anyone and
[00:19:09] any news outlet that will listen. And
[00:19:11] the presumption that there is a
[00:19:12] fundamental misalignment between the
[00:19:14] Frontier Labs and their customers now
[00:19:17] seems to be core to no less than
[00:19:18] Microsoft strategy. A couple of months
[00:19:21] ago, Microsoft CEO Sacha Nadella
[00:19:23] released a blog post called the reverse
[00:19:24] information paradox. In it, he wrote,
[00:19:27] you essentially pay for intelligence
[00:19:28] twice. Once with money and again with
[00:19:30] something even more valuable. The
[00:19:32] proprietary knowledge you must reveal to
[00:19:34] make that intelligence useful. The
[00:19:36] better you want the model to perform,
[00:19:37] the more of that knowledge you have to
[00:19:38] feed it. Over time, the information
[00:19:40] asymmetry becomes increasingly skewed.
[00:19:42] The seller learns more and more about
[00:19:44] you as you use what you purchased, while
[00:19:45] you learn very little about what the
[00:19:47] seller is learning in return. That is
[00:19:49] what I think of as the reverse
[00:19:50] information paradox. This requires more
[00:19:52] than data protection. Models learn from
[00:19:55] exhaust, the prompts people write, the
[00:19:56] tools agents use, and especially the
[00:19:58] corrections people make when the model
[00:19:59] is wrong. Every correction is distilled
[00:20:02] into institutional knowhow. It's the
[00:20:03] kind of knowledge a competitor could
[00:20:05] never buy and the kind that leaks almost
[00:20:06] imperceptibly trace by trace, correction
[00:20:08] by correction, eval by eval. It's
[00:20:11] imperative that we distribute the
[00:20:12] learning infrastructure to every firm so
[00:20:14] that they can control their own learning
[00:20:16] loop. Now, if you've been paying
[00:20:18] attention, this has set the tone for
[00:20:19] every move that Microsoft has made
[00:20:20] subsequently. Their new models that they
[00:20:22] recently released are very much designed
[00:20:24] to be the base for customizations and
[00:20:27] post- training, which while they are
[00:20:28] certainly not open weights, are designed
[00:20:30] to be more customizable and more owned
[00:20:32] by the customer as opposed to just
[00:20:33] sending off information into a black box
[00:20:35] that only the Frontier Lab can access.
[00:20:37] And as much as OpenAI tries to say that
[00:20:40] this is a move that is not general, but
[00:20:41] is specific to issues with Elon based on
[00:20:43] a demonstrated pattern, the implication
[00:20:45] for many is clear. As you jin put it,
[00:20:48] when Elon acquires cursor, OpenAI cuts
[00:20:50] off cursor. When OpenAI tried to acquire
[00:20:52] Windsurf, Anthropic cuts off Windsurf.
[00:20:55] Not your weights, not your product. Now,
[00:20:58] functionally for enterprises, it doesn't
[00:21:00] matter if there is substantive
[00:21:01] difference in these two things. The
[00:21:03] response that they're going to have to
[00:21:04] have is very similar. As AI content
[00:21:07] creator Theo put it, if you want to
[00:21:08] avoid getting hurt by companies beefing
[00:21:10] with each other, make sure you own your
[00:21:12] tools and your relations with the
[00:21:13] products you rely on are direct and not
[00:21:15] routed through other layers like this. I
[00:21:17] have a feeling this is not a one-off
[00:21:19] thing. If anything, it's the start of
[00:21:21] the end. We're probably going to see
[00:21:22] more and more moves like this from
[00:21:24] Anthropic and OpenAI and probably even
[00:21:26] companies like Google and SpaceX. And of
[00:21:28] course, already even before this, we had
[00:21:31] seen companies starting to get more
[00:21:32] acquainted with openweight models.
[00:21:34] Earlier in August, the Wall Street
[00:21:35] Journal profiled how AT&T had started
[00:21:38] working with open models and Business
[00:21:39] Insider also talked about how Thompson
[00:21:41] Reuters had done something similar,
[00:21:42] building off of a base of Alibaba's
[00:21:44] Quen. Now, these stories mostly posited
[00:21:46] this as a cost control measure.
[00:21:48] Obviously, a big part of the narrative
[00:21:49] for the last several months has been how
[00:21:51] companies build more complex model
[00:21:52] architectures that allow them to match
[00:21:54] task difficulty with model capability in
[00:21:57] a way that is more cost-effective.
[00:21:59] However, there is clearly now a
[00:22:00] sovereignty and control aspect of those
[00:22:02] moves. And what this shows is that those
[00:22:04] questions are moving from strictly the
[00:22:06] model layer to also the harness layer as
[00:22:08] well. Again, in the Wall Street
[00:22:10] Journal's CIO journal, a recent post
[00:22:12] introduced the idea of an AI model
[00:22:14] harness to a wider audience. In
[00:22:16] explaining why businesses need a model
[00:22:18] harness, Moody's David Pan called it a
[00:22:20] way for companies to take back control
[00:22:22] of their AI. The journal writes,
[00:22:24] "Developing their own software around AI
[00:22:26] models, a practice PAN calls harness
[00:22:28] engineering, gives businesses a way to
[00:22:30] decouple their workflows from the models
[00:22:32] themselves, and that helps them become
[00:22:34] less reliant on a single AI provider,"
[00:22:36] said Pan. "If you bring that harness
[00:22:38] inhouse and control it, you're baking in
[00:22:40] a lot more business resilience." And
[00:22:42] given that this article came out a week
[00:22:43] ago, Pan's advice that companies build
[00:22:45] their own harnesses rather than rely on
[00:22:47] those offered by labs like OpenAI and
[00:22:49] Anthropic seems particularly precient.
[00:22:52] So, if you are an enterprise AI buyer,
[00:22:54] what is the move here? First of all,
[00:22:56] this is another reminder that if you
[00:22:58] don't have a policy around open weights
[00:23:00] models yet, you need to go figure it
[00:23:02] out. Now, to be clear, what I do not see
[00:23:04] is companies abandoning frontier closed
[00:23:06] models entirely. Frankly, even among
[00:23:08] sophisticated users, it's not like some
[00:23:10] big majority of use cases have even
[00:23:12] moved over to those new models yet. But
[00:23:14] what the sophisticated enterprise AI
[00:23:15] users understand is that being able to
[00:23:18] integrate and route certain types of
[00:23:20] tasks to lighter, cheaper, more
[00:23:23] controllable open weights type models is
[00:23:25] going to be a key capability that they
[00:23:26] need to have and that like any
[00:23:28] capability, it's going to take time and
[00:23:29] they need to start now. What I think
[00:23:31] that this cursor move puts a point on is
[00:23:33] that this is not just a model
[00:23:34] conversation but also a harness
[00:23:36] conversation as well. My very strong
[00:23:39] prediction is that you're going to see a
[00:23:40] lot more discourse around not just open
[00:23:42] models, but open harnesses. An early
[00:23:44] example of this is that once again
[00:23:45] earlier this month, Deepseek released
[00:23:47] Deepseek Harness. In their announcement
[00:23:49] post, they wrote, "Deepse harness is an
[00:23:51] agent harness built around one core
[00:23:53] idea. Everything is a plug-in. Models,
[00:23:56] tools, skills, sessions, sandboxes, file
[00:23:58] systems, loops, orchestration, and UI
[00:24:00] are all implemented as plugins and can
[00:24:02] be mixed, matched, replaced, and
[00:24:03] extended. And first impressions of DeepC
[00:24:05] Carnis are pretty good. But I think that
[00:24:07] the deep sea harness itself matters less
[00:24:09] than the fact that open harnesses are
[00:24:11] now a tool that enterprises are going to
[00:24:12] have access to as well. Ultimately, I
[00:24:15] don't think anything about the cursor
[00:24:16] move is particularly surprising, which
[00:24:18] certainly doesn't mean that cursor users
[00:24:19] shouldn't yell and scream at OpenAI and
[00:24:21] see if they can't change their position.
[00:24:23] I think a highly bulcanized world of
[00:24:24] models and harnesses is inherently worse
[00:24:26] for everyone than the one we seem to be
[00:24:27] going into. So, I am fully in support of
[00:24:29] people using market pressure to try to
[00:24:30] change the policy. But for enterprises,
[00:24:32] the lesson is clear. If you want to not
[00:24:35] be subject to the whims of the companies
[00:24:37] that control your models and control
[00:24:39] your harnesses, you basically can't be
[00:24:41] relying on any one company to control
[00:24:43] your models or to control your
[00:24:44] harnesses. So, you know, for
[00:24:46] enterprises, just a whole additional set
[00:24:47] of things that you have to get good at
[00:24:48] to make AI work for you. Anyways,
[00:24:51] interesting times. This is a trend that
[00:24:52] we will watch closely. For now, though,
[00:24:53] that is going to do it for today's AI
[00:24:55] daily brief. I appreciate you listening
[00:24:56] or watching as always and until next
[00:24:58] time, peace.
