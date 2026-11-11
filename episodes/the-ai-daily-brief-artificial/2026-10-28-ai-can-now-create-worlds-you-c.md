---
record_id: "podcast:3d466f77-e93f-4d3f-bdee-f35ede9c7e7e"
episode_id: 3d466f77-e93f-4d3f-bdee-f35ede9c7e7e
title: AI Can Now Create Worlds You Can Change in Real Time
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/ai-can-now-create-worlds-you-can-change-in-real-time/3d466f77-e93f-4d3f-bdee-f35ede9c7e7e"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/ai-can-now-create-worlds-you-can-change-in-real-time/3d466f77-e93f-4d3f-bdee-f35ede9c7e7e"
feed_guid: null
feed_url: "https://anchor.fm/s/f7cac464/podcast/rss"
published_at: null
published_local_date: null
played_date: 2026-10-28
played_at: "2026-10-28T12:00:00Z"
play_count: 1
duration_seconds: 1740
source: pocketcasts-history-browser
played_label: October 28
history_order: 18
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 1360304ee67de4435c054212347f7c84a473f66cef8c5d9ee5d73510f205d311
analysis_mode: health
summary_source: local
model_source: local
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: Qwen3.8-Flash-Next-UD-Q4_K_XL
tagging_model: claude-haiku-4-5
proposed_tags: [research]
proposed_entities: []
status: new
routed_to: null
---

## Summary

Google DeepMind’s Genie 4 world model was the episode’s central technical story: it integrates Google’s broader AI stack—Gemini Omni for realistic video grounding, Gemini 3.8 Flash for reasoning and causality, and Google audio models for sound—to generate interactive, real-time worlds that users can modify with live prompts, add objects or weather to, and navigate with more persistent physics and character behavior than Genie 3, which had been limited to about 60 seconds. Commenters including Ethan Mollick, Justine Moore, and Chris GPT emphasized the leap toward playable generated environments, robotics simulation, and possible spatial reasoning for agents; Google showed a robot playing chess in a simulated world using Gemini 4 Argon, while gaming implications included generative games, AI-assisted porting with Opus 5.5, and projects like a mixed-reality Mario 64. The headlines segment also covered Anthropic’s biotech push: a blog on AI-enhanced drug discovery, partnerships with six organizations, a Bristol Myers Squibb collaboration for early-stage trial planning, and the acquisition of Mythril Medicine, a one-person company whose founder Cody Tranbarger reportedly used Claude to coordinate contracts, logistics, and experiments across 11 external labs, taking a muscular dystrophy treatment from idea to promising mouse results in under 18 months versus a typical 4–7 year preclinical path, with a stated goal of clinical-trial-ready drug work by end of 2028. Skeptics including Scorpion Capital, Peter Yang, and Lenny Rachitsky questioned the “one-person company” framing and founder expertise, while others saw it as Anthropic IPO positioning; market context included Anthropic’s S-1, reported cash above $112 billion as of June, a possible $100 billion IPO, Nasdaq up 2%, the Philadelphia semiconductor index up nearly 6%, and Wall Street’s shift from “P doom” to “P boom.” The episode also covered OpenAI’s scientific breakthroughs and the controversy over verification and access, especially around a math proof, a computer-science result on the exponential time hypothesis, and a physics result said to include an existence proof for Yang-Mills theory; OpenAI’s mathematics advisory group and physicists including Constantine Cogler and Andreas Kark debated whether results should be released openly or vetted privately, while a KPMG/University of Texas at Austin study of more than 500 early-career professionals found top “AI amplifiers” succeeded by guiding, evaluating, and refining AI outputs rather than relying on static knowledge.

For the user, the actionable health lead is to treat Anthropic’s Mythril/Bristol Myers Squibb story as a rare-disease drug-development signal, not a proven medical breakthrough: if muscular dystrophy or related rare-disease research matters to the user, follow up on whether Anthropic/Mythril/BMS programs reach registered clinical trials by 2028, ask whether mouse data has been peer-reviewed, whether regulatory filings exist, and whether independent labs can replicate the results; the practical implication is that AI may shorten early discovery and trial-planning bottlenecks, but clinical benefit still depends on human trials, safety data, and regulatory review. Professionally, the KPMG study suggests the user should build an “AI amplifier” workflow: define the task, require the model to propose steps, evaluate outputs against evidence, iterate, and keep human judgment in the loop rather than assuming similar AI access produces similar results. For research or investing, the episode gives concrete follow-up questions: how reliable are Genie 4’s physics, persistence, and causality outside polished demos; can simulated robot training transfer to real hardware; who owns IP when AI generates games, characters, or ports; how will Anthropic’s IPO, cash position, and capital access affect smaller AI firms; and will OpenAI’s AI-generated scientific results be released openly enough for independent verification. If the user is in gaming, robotics, biotech, or AI strategy, the decisions to consider are whether to prototype with world models, monitor AI-assisted drug pipelines, adopt structured AI evaluation practices, and avoid overvaluing flashy generated media without checking verification, safety, and commercial viability.

## Transcript

[00:00:00] Just how close are we to AI being able
[00:00:02] to invent worlds on the fly? And as it
[00:00:04] gets closer, what are the implications
[00:00:06] for games and video and all sorts of
[00:00:08] different types of experiences that we
[00:00:10] have today? Those questions are back at
[00:00:12] the top of the discourse today as Google
[00:00:14] releases Genie 4, its latest world model
[00:00:16] and one that shows that where we are
[00:00:17] headed might be very different indeed
[00:00:19] than where we are right now.
[00:00:21] The AI Daily Brief is a daily podcast
[00:00:23] and video about the most important news
[00:00:25] and discussions in AI.
[00:00:27] All right, friends. Quick announcements
[00:00:29] before we dive in. First of all, thank
[00:00:31] you to today's sponsors KPMG, C data,
[00:00:34] Granola, and Blitsy. To get an ad-free
[00:00:36] version of the show, go to
[00:00:37] patreon.com/aidailybrief,
[00:00:39] or you can subscribe in Apple Podcasts.
[00:00:41] To learn more about sponsoring the show,
[00:00:42] send us a note at
[00:00:43] sponsors@aidailybrief.ai.
[00:00:45] Lastly today, if you haven't yet, please
[00:00:47] go check out How We Got Here. It is a
[00:00:49] new weekly video podcast that I am doing
[00:00:52] that is all about the history behind
[00:00:54] today's biggest phenomenon, trends,
[00:00:56] anything that's happening in our world
[00:00:57] that we assume is inevitable, but which
[00:00:59] actually came to be through a set of
[00:01:00] very decisions. For those of you who
[00:01:02] like the more ponderous exploratory
[00:01:04] episodes of AIDB, that is a place to get
[00:01:06] even more of that. You can find a link
[00:01:07] in the show notes or go to how we got
[00:01:09] here.com. With that out of the way
[00:01:11] though, let's talk about AI creating
[00:01:13] worlds.
[00:01:15] Welcome back to the AI Daily Brief
[00:01:16] Headlines Edition, all the daily AI news
[00:01:18] you need in around 5 minutes. Anthropic
[00:01:22] is doubling down on biotech with a big
[00:01:24] acquisition of a very small company. On
[00:01:27] Tuesday, Anthropic published a blog post
[00:01:29] talking through their approach to
[00:01:31] AI-enhanced drug discovery. They wrote,
[00:01:34] "Developing a drug involves many varied
[00:01:35] tasks, doing early research to identify
[00:01:38] a target for a drug and the right type
[00:01:39] of drug to engage it, designing a
[00:01:41] molecule with the right properties,
[00:01:42] optimizing it to be manufactured
[00:01:44] reliably at scale, drafting the
[00:01:45] regulatory filings needed to run
[00:01:47] clinical trials, designing and
[00:01:49] administering those trials, and much
[00:01:50] more. Our strategy to realize AI's
[00:01:52] medical benefits is based on having AI
[00:01:54] increasingly involved in all of these
[00:01:57] tasks. There is no single problem to
[00:01:59] solve. The bottlenecks are distributed
[00:02:01] all throughout the drug development
[00:02:02] process. The best way to identify and
[00:02:04] work through these bottlenecks is to get
[00:02:06] deeply involved in real drug programs
[00:02:08] across many different disease areas and
[00:02:10] stages of development. To that end,
[00:02:12] Anthropic said that they've been
[00:02:13] partnering with six organizations as
[00:02:15] well as launching drug discovery efforts
[00:02:16] of their own. They included several case
[00:02:18] studies showing how Claude had
[00:02:19] accelerated both the scientific and
[00:02:21] operational work required to develop
[00:02:23] promising drug candidates.
[00:02:25] In addition, they announced a new
[00:02:26] partnership with Bristol Myers Squibb to
[00:02:28] use AI to address bottlenecks and
[00:02:30] enhance planning in early-stage clinical
[00:02:31] trials. But the news that caught
[00:02:33] everyone's attention was another biotech
[00:02:35] acquisition. They wrote, "We've acquired
[00:02:38] Mythril Medicine, a one-person company
[00:02:40] that has been developing treatments for
[00:02:41] two rare forms of muscular dystrophy.
[00:02:43] Its founder, Cody Tranbarger, used
[00:02:45] Claude to organize contracts, logistics,
[00:02:47] and experiments with 11 external labs,
[00:02:49] and delegate many other aspects of
[00:02:51] Mythril's operations to Claude. As a
[00:02:53] result, Mythril took a possible
[00:02:55] treatment for one form of muscular
[00:02:56] dystrophy from an idea to promising
[00:02:58] results in mice in less than 18 months.
[00:03:01] Anthropic hopes to have a drug ready for
[00:03:02] clinical trials by the end of 2028, and
[00:03:05] this would be a significant acceleration
[00:03:06] of the typical 4-7 year timeframe for
[00:03:08] preparing a new drug for human testing,
[00:03:10] largely due to a big reduction in the
[00:03:12] drug discovery phase."
[00:03:14] The thing that stood out most to many
[00:03:15] folks was the feasibility of a
[00:03:17] single-person biotech startup. News
[00:03:19] aggregator Andrew Curran commented, "Sam
[00:03:21] Altman's one-person company prediction
[00:03:23] is coming true. Anthropic just bought
[00:03:25] one. The founder of Mythril Medicine
[00:03:26] used Claude to take a muscular dystrophy
[00:03:28] antibody treatment from concept to proof
[00:03:30] of principle in mice in 18 months with
[00:03:32] just himself, Claude, and part-time
[00:03:34] consultants."
[00:03:35] Yuchen Jin wrote, "The real one-person
[00:03:37] billion-dollar company. A solo smart
[00:03:40] high-agency CEO and AI can have an
[00:03:42] outsized impact on the world."
[00:03:44] Then again, not everyone is bought in
[00:03:45] yet. Activist short-seller Scorpion
[00:03:47] Capital wrote, "Founder of Mythril
[00:03:49] Medicine one-person drug company
[00:03:50] acquired by Anthropic is not a scientist
[00:03:52] or academic as we assumed, but a Harvard
[00:03:54] MBA, ex-Goldman Sachs banking analyst,
[00:03:56] and ex-hedge fund guy.
[00:03:58] Now, some did note that the founder has
[00:04:00] a master's in biotech, meaning they are
[00:04:02] not completely foreign to the science,
[00:04:04] but mostly this is a Rorschach test for
[00:04:06] whether you see the death of expertise
[00:04:07] or a demonstration of democratization
[00:04:09] that could lead to more innovation.
[00:04:12] Others questioned the entire premise of
[00:04:13] the one-person AI company. Peter Yang
[00:04:15] commented, "Some of these one-person
[00:04:18] companies look highly suspicious to me,
[00:04:19] to be honest." Lenny Rachitsky from
[00:04:21] Lenny's Podcast agreed, adding, "I'm
[00:04:24] very skeptical of a one-person company
[00:04:25] reaching massive scale. Just the support
[00:04:27] time alone makes it impossible to
[00:04:29] handle, unless you don't count
[00:04:30] contractors helping you with support.
[00:04:32] Don't think AI will ever solve this for
[00:04:34] a one-person company."
[00:04:36] Elsewhere on X, people viewed this as a
[00:04:37] very shrewd marketing move from Entropic
[00:04:39] ahead of their IPO. Fundamentally, this
[00:04:42] was a restatement of their thesis that
[00:04:43] AI can massively accelerate drug
[00:04:45] discovery and make research into
[00:04:46] low-frequency diseases more financially
[00:04:48] viable. Still, Entropic hammered home
[00:04:50] that AI use in biotech isn't about full
[00:04:53] automation, it's about reducing friction
[00:04:55] and bottlenecks throughout the process.
[00:04:57] Commenting on the meta strategy of
[00:04:58] promoting the IPO, Chubby on X wrote,
[00:05:00] "Drug discovery will be one of the most
[00:05:02] significant revenue streams in the
[00:05:03] future. The goal here is to set the
[00:05:05] right course early on. Most diseases
[00:05:07] will become treatable, a market
[00:05:09] encompassing 7 billion people. The
[00:05:10] timing is clearly intentional, announced
[00:05:12] just before the IPO to signal to
[00:05:14] investors that the business will
[00:05:15] continue to thrive in the future. This
[00:05:17] will likely make it clear even to those
[00:05:18] outside the tech nerd sphere why AI is
[00:05:20] so important. It goes beyond just
[00:05:22] writing code. It solves problems for
[00:05:24] humanity."
[00:05:25] And picking up a theme that we've
[00:05:26] explored a bit in the past few weeks,
[00:05:28] for some, this is yet another example of
[00:05:30] an AI company diversifying their revenue
[00:05:32] streams outside of just selling tokens.
[00:05:35] Martin Varsavsky writes, "The tens of
[00:05:37] millions from the better molecule go to
[00:05:39] whoever owns the molecule. If AI labs
[00:05:41] want to be paid for value, they will
[00:05:42] have to own the outcome. Discover the
[00:05:44] drug, run the trial, hold the patent.
[00:05:46] That is why Isomorphic Labs, the drug
[00:05:48] discovery company Alphabet spun out of
[00:05:49] DeepMind, matters more than any pricing
[00:05:52] page. Selling intelligence is becoming a
[00:05:54] commodity business. Owning what
[00:05:56] intelligence discovers is not.
[00:05:58] But, you can count on that to continue
[00:06:00] to be a debate and one that gets nothing
[00:06:01] but more fierce when Anthropic IPOs.
[00:06:04] Speaking of which, the assessment that
[00:06:06] the market was generally positive on the
[00:06:07] Anthropic S-1 seems to have been
[00:06:09] validated. The public reveal of
[00:06:11] Anthropic's IPO filing came after a
[00:06:13] 3-week drawdown for tech stocks and a
[00:06:15] 4-month bear market in semiconductors.
[00:06:17] So far this week, however, the AI trade
[00:06:19] has been nothing but green. The Nasdaq
[00:06:21] index is up 2% since trading opened on
[00:06:23] Monday, and the Philadelphia
[00:06:24] semiconductor index has rebounded by
[00:06:26] almost 6%. Certainly, the market is not
[00:06:28] assessed that Anthropic has no
[00:06:29] weaknesses in the business, but for
[00:06:31] investors who were expecting the filing
[00:06:33] would confirm no path to realizing a
[00:06:34] return on AI CapEx, the picture of a
[00:06:36] booming business with a realistic path
[00:06:38] forward was enough to get many of those
[00:06:40] investors back on sides. Heavy Chan from
[00:06:42] Vantage Global Prime said, "Anthropic's
[00:06:44] landmark IPO filing alongside Meta's
[00:06:46] aggressive CapEx push has reignited
[00:06:48] broader risk appetite, pulling capital
[00:06:50] out of its defensive crouch and firmly
[00:06:52] restoring chip stocks back to the
[00:06:54] driver's seat." James Wee, the chief
[00:06:56] market strategist at Tiger Brokers, said
[00:06:58] it was all about Anthropic's cash pile,
[00:06:59] commenting, "With more than 112 billion
[00:07:02] in cash and cash equivalents as of June,
[00:07:04] even before any potential IPO proceeds,
[00:07:06] Anthropic appears to have considerable
[00:07:08] financial capacity to support its
[00:07:09] expansion."
[00:07:11] Meanwhile, the Wall Street Journal is
[00:07:12] reinforcing the point that I raised on
[00:07:14] Monday's show that it's really in
[00:07:16] everyone in the AI industry's best
[00:07:17] interest for this IPO to go well. I
[00:07:19] argued that that could be a very good
[00:07:21] reason for OpenAI to just sit back,
[00:07:23] mothball their next model release, and
[00:07:25] let Anthropic have the limelight for
[00:07:26] just a couple of weeks with Fable 5.5.
[00:07:29] The Journal took it a step further,
[00:07:30] pointing out that the IPO will say a lot
[00:07:32] about access to capital for the entire
[00:07:34] industry. If Anthropic can raise $100
[00:07:36] billion with room to spare, which would
[00:07:38] be the largest IPO in history, then it
[00:07:40] bodes well for smaller companies with
[00:07:41] more pressing fundraising needs. In a
[00:07:44] separate article, the journal grappled
[00:07:45] with how Wall Street will price
[00:07:46] existential risk. The logic is simple,
[00:07:49] writes the journal, if there's a 10%
[00:07:50] chance that artificial intelligence
[00:07:52] could kill all humans in the next
[00:07:53] decade, as an anthropic researcher said
[00:07:55] last month, there's a 90% chance it's
[00:07:57] really, really good, but designers
[00:07:59] managed to rein in its genocidal
[00:08:00] instincts. An AI smart enough to kill us
[00:08:02] all, but which prefers to help us is
[00:08:04] supremely useful and should generate
[00:08:06] healthy gains for its inventors. Now, I
[00:08:08] don't know exactly how firmly author
[00:08:10] James Macintosh's tongue is in his
[00:08:12] cheek, but it does appear that this week
[00:08:13] at least, it looks like Wall Street has
[00:08:15] stopped focusing on P doom and is
[00:08:17] starting to price in P boom.
[00:08:19] Lastly, in a brief follow-up to
[00:08:20] yesterday's story about new scientific
[00:08:22] breakthroughs from OpenAI, a group of
[00:08:24] scientists are still unhappy with how
[00:08:26] OpenAI went about their disclosure.
[00:08:28] During the giant dump of novel math
[00:08:30] proofs earlier this month, the criticism
[00:08:32] was that OpenAI didn't do enough to
[00:08:34] verify results. This time around, OpenAI
[00:08:36] tried to address this criticism by
[00:08:38] appointing groups of scientific experts
[00:08:40] to shepherd the breakthrough results.
[00:08:42] These experts recommended a different
[00:08:43] approach for each result. The math proof
[00:08:46] was just released publicly as an
[00:08:47] academic paper. The computer science
[00:08:49] result disproving the exponential time
[00:08:50] hypothesis had proofs and AI sessions
[00:08:52] released alongside with a team of
[00:08:54] scientists appointed to do further work
[00:08:56] explaining the result and exploring its
[00:08:57] implications. However, the physics
[00:08:59] result, which was said to include an
[00:09:00] existence proof for Yang-Mills theory,
[00:09:02] was kept private while a group of
[00:09:04] physicists worked on verifying and
[00:09:05] formalizing the result.
[00:09:07] Following OpenAI's announcement, their
[00:09:09] own advisory group on mathematics and
[00:09:11] artificial intelligence publicly
[00:09:12] disagreed with this approach. In a
[00:09:14] public recommendation, the mathematics
[00:09:15] advisory group said they had great
[00:09:17] respect for the physicists appointed to
[00:09:18] shepherd the results, but that, quote,
[00:09:20] "Understanding should develop in the
[00:09:22] open with everyone given the same
[00:09:23] access."
[00:09:25] Later on Tuesday, the group of
[00:09:26] physicists in question released a
[00:09:28] response, commenting, "The length and
[00:09:30] complexity of the OpenAI manuscripts are
[00:09:32] formidable, and some time will be needed
[00:09:33] to digest its methodology and meaning in
[00:09:35] both physics and mathematics. Before we
[00:09:37] release it, we would like to be
[00:09:38] convinced that it is correct. This is an
[00:09:40] experiment in how the academic community
[00:09:42] can deal with the rapid development of
[00:09:44] new knowledge by AI. We intend to
[00:09:46] proceed very carefully.
[00:09:48] Still, the frustration with the delayed
[00:09:49] publication seems to be playing out in
[00:09:51] faculty lounges across the country. The
[00:09:53] Verge spoke with several physics
[00:09:54] professors, with many of them calling
[00:09:56] for an immediate release. Constantine
[00:09:58] Cogler from the Institute for Advanced
[00:09:59] Study said, "I'm fine with them
[00:10:01] releasing the problems as they did
[00:10:02] today." Referring to releasing a smaller
[00:10:04] batch of three extremely important
[00:10:05] results. However, Cogler added, "It
[00:10:08] doesn't make any sense that only a few
[00:10:09] distinguished scientists can look at
[00:10:10] them." Andreas Kark from the University
[00:10:12] of Texas Austin said, "The fact that
[00:10:14] they handpicked a group is a disaster.
[00:10:16] The large labs have enough power as it
[00:10:18] is. They should not be picking winners
[00:10:20] and losers." Kark initially suggested a
[00:10:22] merit-based selection criteria, although
[00:10:24] he acknowledged that this would likely
[00:10:25] produce the same group that included
[00:10:27] Nobel laureates. Instead, he simply
[00:10:29] called on OpenAI to release the proof
[00:10:30] saying, "This would democratize access
[00:10:32] while still showing that they care about
[00:10:34] making results meaningful and
[00:10:35] understandable."
[00:10:37] I don't know, man. I think on this one,
[00:10:38] OpenAI simply can't win. If they release
[00:10:40] everything they have as soon as
[00:10:41] possible, they're criticized for
[00:10:43] creating a gigantic verification problem
[00:10:44] for academics to deal with. If they
[00:10:46] arrange their own verification working
[00:10:48] groups and hold back important results
[00:10:49] until they're fine, they're criticized
[00:10:50] for gatekeeping science.
[00:10:52] The thing that's totally understandable
[00:10:54] is that people are uncomfortable with
[00:10:55] how much power these labs have. And that
[00:10:57] is not solely based on specific
[00:10:59] decisions that the labs make. It is
[00:11:01] based on the intractable reality of
[00:11:03] where they sit vis-a-vis this new
[00:11:04] intelligence. But when it comes to this
[00:11:06] sort of specific, they're pretty much
[00:11:08] damned if they do and damned if they
[00:11:09] don't. Stanford mathematician Jared
[00:11:11] Duker Lichtman commented, "My sense is
[00:11:13] that for any approach, there is going to
[00:11:15] be someone who is upset. So, it's just a
[00:11:17] question of finding the least offensive
[00:11:19] option.
[00:11:20] I am glad that is not my job. And for
[00:11:22] now, that's going to do it for the
[00:11:23] headlines. Next up, the main episode.
[00:11:27] A new study from KPMG and the University
[00:11:29] of Texas at Austin found that when
[00:11:31] people work with AI, similar skills
[00:11:33] don't guarantee similar outcomes.
[00:11:35] Researchers studied more than 500 early
[00:11:37] career professionals and found that the
[00:11:39] best performers consistently amplify the
[00:11:41] value of AI by guiding, evaluating, and
[00:11:44] refining its outputs. These top
[00:11:46] performers, called AI amplifiers,
[00:11:48] weren't defined by what they knew alone,
[00:11:50] but by how they worked with AI. Learn
[00:11:53] more about what separates AI amplifiers
[00:11:55] from everyone else at
[00:11:56] kpmg.com/us/aiamplifiers.
[00:12:02] This episode is brought to you by C
[00:12:04] data. Companies rolling out AI keep
[00:12:06] hitting the same wall. Token spend is
[00:12:08] climbing, security is holding agents
[00:12:10] back, and no one knows how AI is truly
[00:12:12] being used. The root cause? AI is cut
[00:12:15] off from the systems and context your
[00:12:17] business runs on. That's why C data
[00:12:19] built connect AI gateway. One control
[00:12:22] point between your AI and your systems.
[00:12:24] Built on the connectivity layer powering
[00:12:26] Palantir, Google, Salesforce, and
[00:12:28] hundreds more,
[00:12:29] each agent gets exactly the data and
[00:12:31] tools it needs. It governs down to the
[00:12:33] record and lets you finally see your
[00:12:34] org's complete AI usage in one place.
[00:12:37] Accurate answers, a fraction of the
[00:12:39] token cost, and a gateway that learns
[00:12:40] your business with every interaction.
[00:12:42] See how at cdata.ai.
[00:12:46] You're in back-to-back meetings all day.
[00:12:48] You're trying to stay present, but
[00:12:49] you're also worried you'll forget the
[00:12:50] decision, the action item, the important
[00:12:52] next step. This is a scenario that we
[00:12:54] absolutely live here at the AI Daily
[00:12:56] Brief. Given how fast things move and
[00:12:57] change and how quickly we're evolving
[00:12:58] everything that we do. That's where
[00:13:00] Granola comes in. Granola is an
[00:13:02] AI-powered notepad for meetings. You jot
[00:13:04] down rough notes like you always do, and
[00:13:06] in the background, Granola transcribes
[00:13:08] and turns them into clear, useful notes
[00:13:09] when the meeting ends. No bots joining
[00:13:11] your calls, no distractions, just a
[00:13:13] clean notepad that helps you focus.
[00:13:15] During or after the call, you can chat
[00:13:17] with your notes. Ask Granola to pull out
[00:13:19] action items, help you negotiate, write
[00:13:21] a follow-up email, or even coach you
[00:13:22] using recipes, which are pre-made
[00:13:24] prompts. Once you try it on a first
[00:13:26] meeting, it is very hard to go without.
[00:13:28] Head to granola.ai/aidaily
[00:13:30] and use code AI daily to get 100% off
[00:13:33] for 3 months for new users. That's
[00:13:35] granola.ai/aidaily
[00:13:37] and code AI daily to get 100% off for
[00:13:40] new users for 3 months.
[00:13:42] Here's why most legacy modernization
[00:13:44] projects fail. The AI doing the work
[00:13:46] can't understand code bases at scale. It
[00:13:49] sees a small slice of context, examines
[00:13:50] syntax, and misses years of decisions
[00:13:53] distributed across the global
[00:13:54] application ecosystem. Blitsy solves
[00:13:56] this the way it solves everything.
[00:13:57] Grounded in your code before any
[00:13:59] migration begins, Blitsy's agents
[00:14:00] reverse engineer the entire legacy
[00:14:02] system into a persistent knowledge
[00:14:04] graph. Every dependency, every
[00:14:05] constraint, every piece of tribal
[00:14:06] knowledge that used to live in one
[00:14:08] engineer's head. From that
[00:14:09] understanding, Blitsy autonomously
[00:14:11] executes language migrations, framework
[00:14:12] upgrades, and monolith to microservices
[00:14:14] transformations, all validated
[00:14:16] end-to-end. One Blitsy customer
[00:14:18] modernized a $10 million monolithic
[00:14:19] insurance stack in 16 weeks against a
[00:14:22] 137-week baseline with coding agents.
[00:14:24] That's 9x compression. Retire technical
[00:14:27] debt while accelerating your road map.
[00:14:29] See how at blitsy.com. That's b l i t z
[00:14:32] y.com.
[00:14:34] Welcome back to the AI Daily Brief.
[00:14:36] Quick note before we dive into today's
[00:14:37] episode. There is going to be a lot of
[00:14:40] visual content. As always, I will do my
[00:14:42] best to make it relevant even if you are
[00:14:44] just listening, not watching, but this
[00:14:45] might be a good one to go check out
[00:14:46] either on Spotify with video or on
[00:14:48] YouTube. Apple continues to roll out
[00:14:50] video podcasting, but has not yet made
[00:14:52] it available for my particular host.
[00:14:54] Hopefully, that will come soon. Today,
[00:14:56] we are talking about Genie 4. It's the
[00:14:58] latest iteration of Google's world
[00:15:00] model, and it could have some big
[00:15:02] implications for robotics, gaming, and
[00:15:04] more.
[00:15:05] On the AI Daily Brief, we've been
[00:15:07] tracking the development of world models
[00:15:09] since they first began showing up in
[00:15:10] 2024. One of the reasons for that was
[00:15:13] because AI luminaries like Yann LeCun
[00:15:15] and Fei-Fei Li believed that world
[00:15:18] models were a more viable path to AGI
[00:15:20] than large language models. The argument
[00:15:22] was basically that you had to have a
[00:15:23] different physical understanding of the
[00:15:25] world around to achieve AGI, not just be
[00:15:27] able to read a bunch of stuff.
[00:15:29] Obviously, I'm being wildly over
[00:15:30] reductive, but you get the idea.
[00:15:32] The early experiments in world models
[00:15:34] were breathtaking tech demos. They
[00:15:36] showed us something completely different
[00:15:38] to anything we'd seen AI do before. At
[00:15:40] the time, generative video was still in
[00:15:42] its infancy. So, the ability to create
[00:15:44] fully 3D worlds at all was a massive
[00:15:46] breakthrough. And yet, even then it was
[00:15:48] clear that these demos really weren't
[00:15:50] about what was available now, to come.
[00:15:52] Over the next year or so, Google made
[00:15:54] rapid progress with their Genie models.
[00:15:56] Genie 2, which was first revealed in
[00:15:58] December 2024, was very impressive. But,
[00:16:01] when Genie 3 was previewed in January
[00:16:02] 2025, it was clear that Google had made
[00:16:05] a huge leap. The model was eventually
[00:16:07] served to the public in August of 2025
[00:16:09] and allowed users to prompt worlds into
[00:16:11] existence and then navigate those worlds
[00:16:13] with a keyboard and a mouse for the
[00:16:14] first time. One of the most impressive
[00:16:16] technical breakthroughs was a level of
[00:16:18] persistence that we hadn't seen before.
[00:16:20] Users could change something about the
[00:16:22] world, like paint a symbol on a wall,
[00:16:24] look away, and then look back, and the
[00:16:26] symbol would be the same. At the time,
[00:16:28] generative video models were struggling
[00:16:30] mightily to achieve that level of
[00:16:31] consistency.
[00:16:32] Google said that this was an emergent
[00:16:34] property of how the models worked,
[00:16:35] rather than a feature they added. Genie
[00:16:37] 3 generated each frame of video auto
[00:16:39] regressively based on what had come
[00:16:41] before. So, the model kept a record of
[00:16:43] the world as it was being generated. And
[00:16:45] yet, still we were very clearly in the
[00:16:47] tech demo stage of world models.
[00:16:50] Incredibly cool tech demos, but far, far
[00:16:52] too limited for practical use.
[00:16:54] Technologists suggested world models
[00:16:56] could help train robots or generate
[00:16:57] fully playable games in real time. But,
[00:16:59] Genie 3 was limited to 60 seconds of
[00:17:01] generation because of the high compute
[00:17:02] requirements. Now, alongside all of
[00:17:05] this, Google has of course, in the eyes
[00:17:06] of many, been languishing without a
[00:17:08] state-of-the-art language model to
[00:17:09] compete in the main areas of AI
[00:17:11] competition right now, like agenda
[00:17:12] coding. And yet, for most people who are
[00:17:14] paying close attention, there was never
[00:17:16] any question of Google's proficiency in
[00:17:18] advanced multimodal AI. Now Google has
[00:17:21] revealed Genie 4 and with it a pathway
[00:17:23] to making world models far more
[00:17:25] practical and useful. With this
[00:17:27] iteration, DeepMind has made a huge
[00:17:29] change to the model's architecture.
[00:17:31] Rather than being a standalone model,
[00:17:33] Genie 4 integrates other Google models
[00:17:35] to provide things that Genie can't do by
[00:17:37] itself. Gemini Omni, Google's video
[00:17:39] model, quote anchors the simulations in
[00:17:42] real-world appearance and behavior.
[00:17:43] Presumably that means something like
[00:17:45] Omni creates a video clip for reference,
[00:17:47] which Genie then expands out into a
[00:17:48] fully playable world. In addition,
[00:17:50] Gemini 38 Flash provides a reasoning
[00:17:52] engine for physical interactions, giving
[00:17:54] the model reliable causality. On top of
[00:17:56] that, some unspecified combination of
[00:17:58] Google's audio models bring sound to
[00:18:00] generated worlds for the first time. The
[00:18:02] result is Google's entire AI ecosystem
[00:18:04] being leveraged towards creating the
[00:18:06] most realistic world simulations we've
[00:18:07] seen to date.
[00:18:09] In their announcement post, Google
[00:18:10] highlighted four key features that they
[00:18:12] viewed as the big advances for Genie 4.
[00:18:14] First, users can now deliver prompts to
[00:18:16] guide the simulation in real time.
[00:18:18] Previous iterations of Genie only
[00:18:19] allowed users to create the world with a
[00:18:21] prompt up front, then navigate whatever
[00:18:23] was generated as a stable world. Now,
[00:18:26] users can give live prompts to guide the
[00:18:27] camera or to modify the environment by
[00:18:29] changing the weather or introducing a
[00:18:31] new object or character.
[00:18:33] Second, Google highlighted the huge jump
[00:18:35] in realism since Genie 3. They wrote,
[00:18:37] "Built on an advanced physical
[00:18:39] understanding of the world, Genie 4
[00:18:40] simulates real-world physics scenarios
[00:18:42] such as aerodynamics, collisions, and
[00:18:44] more." The most dramatic leap is how
[00:18:46] Genie 4 simulates people, creating
[00:18:47] characters that move naturally, respond
[00:18:49] organically to their environments, and
[00:18:51] can be interactively steered in real
[00:18:52] time. The third highlight was generative
[00:18:55] audio, which as I mentioned we haven't
[00:18:56] seen in world models before. Now,
[00:18:58] Google's Omni video model featured
[00:19:00] impressive sound, as did their Lyra
[00:19:02] music model, so it's not all that
[00:19:04] surprising to find amazing audio in the
[00:19:05] new version of Genie, but the fact that
[00:19:07] the worlds can not only include music or
[00:19:09] human speech, but but sound effects,
[00:19:11] gives creators a whole different level
[00:19:12] of tooling than was available before.
[00:19:14] Check out, for example, the otherworldly
[00:19:16] sounds to match an abstract landscape,
[00:19:18] such as those that go alongside the
[00:19:19] stained glass wilderness scene that they
[00:19:20] used as an example.
[00:19:29] Now, the speech does feel a little
[00:19:31] behind the state of the art, still
[00:19:32] featuring that hollow and echoey style
[00:19:34] that was the hallmark of dialogue in
[00:19:35] generative video until about 3 months
[00:19:37] ago, such as this example of a couple
[00:19:38] talking while riding on a motorcycle.
[00:19:41] >> Do you really think we're going to make
[00:19:42] it?
[00:19:43] >> Finally, Google highlighted what adding
[00:19:45] a reasoning model in the background
[00:19:47] brings to the table. Genie can now
[00:19:48] simulate complex multi-step actions with
[00:19:51] a much higher level of realism than
[00:19:52] we've seen before.
[00:19:54] Explaining how this works, Google wrote,
[00:19:56] "To achieve this in real time, Gemini 3
[00:19:58] 8 flash serves as a guiding agent in the
[00:20:00] loop. As Genie 4 generates a world in
[00:20:02] real time, Gemini continuously observes
[00:20:04] the scene, breaks down goals into a
[00:20:05] sequence of steps, and reviews incoming
[00:20:08] frames to track the progress and verify
[00:20:09] that each step succeeded. As the world
[00:20:11] shifts or the user intervenes, Gemini
[00:20:13] adapts its plan in the moment, unlocking
[00:20:15] worlds with reliable causality,
[00:20:17] procedural behaviors, and multi-step
[00:20:18] reasoning." The result is undeniably a
[00:20:21] huge step up in world models. We now
[00:20:24] have the realism of modern video models
[00:20:26] combined with the reasoning capabilities
[00:20:27] of modern LLMs baked into a fully
[00:20:29] playable world simulator.
[00:20:31] One immediate implication is a new
[00:20:33] paradigm in robotics. Google has been
[00:20:35] experimenting with using Gemini 4 Argon
[00:20:37] rather than Gemini 3 8 flash as the
[00:20:39] back-end reasoning model for
[00:20:40] cutting-edge research. Showing a
[00:20:42] demonstration of a robot playing chess
[00:20:44] inside a Genie simulation, they wrote,
[00:20:46] "Argon breaks down a user-instructed
[00:20:48] task into steps for Genie to render.
[00:20:50] These steps are interleaved as text
[00:20:51] captions to Genie 4 as the simulation is
[00:20:53] rendering. Because Genie 4 can be
[00:20:55] steered in real time with text captions
[00:20:57] using Gemini, this now unlocks the path
[00:20:59] of adapting the simulation as it
[00:21:00] progresses towards the completion of
[00:21:01] that task. This capability becomes a
[00:21:03] path for simulating a breadth of
[00:21:04] scenarios in imagined worlds using
[00:21:06] Gemini 4 Argon and Genie 4. Put a little
[00:21:09] less densely, Google can now create
[00:21:11] entirely simulated training environments
[00:21:12] for robots, unlocking training at
[00:21:14] software speed completely untethered
[00:21:16] from real-world limitations.
[00:21:18] The general response from the community
[00:21:20] was jaws hitting floors, and I think
[00:21:22] it's worth noting since I've critiqued
[00:21:24] before the fact that everyone has an
[00:21:26] incentive to focus on 3D renderings and
[00:21:28] things like that because they're popular
[00:21:29] social media shares when a model first
[00:21:31] gets released. That's a little bit
[00:21:32] different in this case because that is
[00:21:34] the entirety of what this model does. In
[00:21:36] other words, it's not a model that
[00:21:37] you're going to use for agenda coding or
[00:21:39] writing essays that people are judging
[00:21:40] on the basis of its ability to make 3D
[00:21:42] renders. The visual and interactive
[00:21:43] worlds that you're creating and sharing
[00:21:45] are the purpose of the model at core.
[00:21:47] Professor Ethan Mollick wrote, "Genie 4
[00:21:49] is quite an insane experience,
[00:21:51] generating game-like environments as you
[00:21:53] go. It isn't flawless, but I can type
[00:21:55] neo-Gothic brutalist city inhabited by
[00:21:57] robots and horses, and it creates one in
[00:22:00] a minute. Then I asked it to add
[00:22:01] dragons, then a friendly otter NPC, all
[00:22:04] in real time." Ethan also created a
[00:22:06] scene of a Victorian high tea where the
[00:22:08] main character was a mouse in
[00:22:09] appropriate garb, and then in real time
[00:22:12] added a porcupine walking by, the mouse
[00:22:13] growing wings, the mouse flying to the
[00:22:15] teacup. He says, "It's glitchy, but also
[00:22:18] impossibly advanced compared to a couple
[00:22:20] of years ago."
[00:22:21] If you had to sum up people's reactions
[00:22:22] with a single emoji, it would certainly
[00:22:24] be the mind-blown emoji as shared by
[00:22:26] Justine Moore from a16z. Sharing a clip
[00:22:28] of a Lovecraftian style game, she
[00:22:30] writes,
[00:22:31] "This is a fully generated interactive
[00:22:33] world from a single starting prompt. You
[00:22:35] can now prompt to change the world and
[00:22:36] interact with it with native audio." She
[00:22:38] also created a new version of Grand
[00:22:39] Theft Auto and said,
[00:22:41] "We got GTA Waymo before GTA 6."
[00:22:44] Chris GPT tried to explain why this
[00:22:46] matters for the larger advancement of AI
[00:22:48] as well. He writes, "A lot of people may
[00:22:50] not understand the purpose of world
[00:22:51] models, but I think Genie 4 gives us a
[00:22:53] clearer glimpse of how they could help
[00:22:55] us get closer to AGI. Google is already
[00:22:57] combining Genie with Gemini.
[00:22:59] Unfortunately, 3.8 flash in the live
[00:23:01] loop. Gemini can watch the simulation,
[00:23:03] break goals down into simpler steps, and
[00:23:05] adjust its plan as the world changes.
[00:23:07] Eventually, pairing an LLM's reasoning
[00:23:09] with a world model's learned physical
[00:23:10] dynamics could give agents a way to test
[00:23:12] actions and improve their
[00:23:13] spatio-temporal reasoning. Similar to
[00:23:15] how humans can imagine a real-world
[00:23:17] scenario and think through what might
[00:23:18] happen before doing something. This
[00:23:20] gives agents a place to compare actions
[00:23:22] and learn from simulated outcomes before
[00:23:23] trying them in the real world, assuming
[00:23:25] these simulations are accurate enough. I
[00:23:27] think this could help with some of the
[00:23:28] spatial and physical reasoning problems
[00:23:30] models still struggle with. Humans can
[00:23:32] mentally rehearse what they're about to
[00:23:33] do, but LLMs are only able to do
[00:23:35] text-based reasoning and can describe
[00:23:37] physics and math possibilities in text,
[00:23:39] but an interactive world model gives AI
[00:23:41] a way to play them out. The physics and
[00:23:42] long-term consistency still need work,
[00:23:44] obviously, but this is a great step
[00:23:46] towards giving AI richer environments to
[00:23:47] interact with and learn from.
[00:23:50] Now, as you might imagine, one place
[00:23:51] that people are seeing very clear
[00:23:52] implications is for the world of gaming.
[00:23:54] In fact, since the earliest days of
[00:23:56] world models, most have assumed that
[00:23:58] that was where this technology would
[00:23:59] have its first big impacts. The idea is
[00:24:01] that one day, perhaps one day soon,
[00:24:03] gamers will be able to prompt their own
[00:24:05] personalized game using a world model
[00:24:07] and create a fully tailored generative
[00:24:08] gaming experience. In fact, the release
[00:24:11] of Genie 3 sent gaming stocks
[00:24:12] plummeting, although this Genie 4
[00:24:14] release was less damaging to the sector.
[00:24:16] It seems investors have gotten a little
[00:24:17] bit more sophisticated in their
[00:24:18] understanding that the technology is
[00:24:20] still a little way off for being able to
[00:24:21] disrupt the gaming industry. Still,
[00:24:23] there's already a huge AI transition
[00:24:25] underway in that industry, driven by
[00:24:27] Opus 5 5's ability to decompile and
[00:24:29] repackage games. The first few weeks of
[00:24:31] that saw weird mashups like dropping
[00:24:33] Mario into Dark Souls. Then there was
[00:24:35] the wave of ports with people realizing
[00:24:37] Opus could make basically any game
[00:24:39] compatible with pretty much any
[00:24:40] hardware. After a tech reporter ported
[00:24:42] Tim Sweeney's first game from PC to the
[00:24:44] NES, the Epic Games CEO commented, "This
[00:24:47] is amazing and shows what would have
[00:24:48] taken a vast manual effort in the past
[00:24:50] can be done as a hobby project very
[00:24:52] efficiently. Truly a new age of gaming
[00:24:54] and software ahead."
[00:24:56] Now people are bringing some truly zany
[00:24:57] ideas to life. Lucas Ratinhas managed to
[00:25:00] turn Mario 64 into a mixed reality game.
[00:25:02] The gameplay is presented on a virtual
[00:25:04] screen inside of VR glasses and the
[00:25:06] player can reach in and interact with
[00:25:07] Mario as he's running around. For
[00:25:09] example, using their hand as an
[00:25:10] additional platform. The player can also
[00:25:12] grab Mario, pull him out of the game and
[00:25:14] place him on their kitchen table,
[00:25:15] turning their real world space into
[00:25:17] another world for Mario to run around
[00:25:18] in.
[00:25:19] In short, while the tech might not be
[00:25:21] ready for fully generative games, AI
[00:25:23] users are figuring out how to do some
[00:25:24] strange and incredible things with the
[00:25:25] technology we have which will inevitably
[00:25:28] shape what comes next. As with Genie 3,
[00:25:31] Google is making Genie 4 fully available
[00:25:32] for Gemini Ultra subscribers to try out.
[00:25:35] It's still only capable of 2-minute
[00:25:36] simulations, which is double the limits
[00:25:38] of Genie 3, but still short of a fully
[00:25:40] generative gaming experience. So for
[00:25:42] now, this is still a bit of a tech toy,
[00:25:44] although one that's starting to show
[00:25:45] glimmers of a very useful technology.
[00:25:48] There is one more aspect of the Genie 4
[00:25:49] announcement, however, that's worth
[00:25:51] digging into a little bit. In short,
[00:25:53] it's the interpretation by some that
[00:25:55] Genie 4 is a sign that DeepMind still
[00:25:56] has another act. The past 6 months have
[00:25:58] been, putting it fairly mildly,
[00:26:00] disappointing for Google on the LLM
[00:26:02] front. Google for Argon, their most
[00:26:04] recent model, got a passing grade but
[00:26:06] certainly didn't put Google back in the
[00:26:07] AI race. Still, in Anthropic's S1
[00:26:10] paperwork, they named Google as one of
[00:26:12] only two other major competitors
[00:26:13] alongside OpenAI. If the AI frontier is
[00:26:16] jagged, DeepMind's output is perhaps the
[00:26:18] most jagged of all. They haven't been
[00:26:20] able to fully catch up on LLMs, but
[00:26:22] their progress on multimodal is still
[00:26:24] unrivaled. With Genie 4, Google is
[00:26:26] demonstrating that combining a series of
[00:26:27] disparate model architectures can
[00:26:29] produce entirely novel AI systems with
[00:26:31] huge amounts of potential.
[00:26:33] What's more, as an AI business, Google
[00:26:35] also continues to have some diverging
[00:26:36] bets that are paying off. When Google
[00:26:38] started ramping up TPU production last
[00:26:40] year and leaked discussions about
[00:26:42] selling the chips externally, many
[00:26:43] semiconductor analysts scoffed at the
[00:26:45] idea. Nvidia had a stranglehold on AI
[00:26:47] chips and Google was starting from zero
[00:26:49] on sales and business development.
[00:26:51] Still, TPU sales have grown to become a
[00:26:53] significant line item in the revenue
[00:26:54] statement, albeit almost entirely
[00:26:56] through sales to Anthropic. This week,
[00:26:58] however, the information reports that
[00:26:59] Google has won two new customers in
[00:27:01] OpenAI and Oracle. Terms weren't
[00:27:03] disclosed for the OpenAI deal, so it's
[00:27:05] difficult to know how many TPUs will be
[00:27:07] purchased and how they will be deployed,
[00:27:08] but Oracle is set to become the first
[00:27:10] large cloud provider aside from Google
[00:27:12] to rent GPUs to outside customers.
[00:27:14] And in addition to their hardware sales,
[00:27:16] the other big thing to watch for Google
[00:27:18] in the coming months will be whether
[00:27:19] they can rapidly iterate on their LLMs.
[00:27:22] Even before Gemini 4 Argon was released,
[00:27:25] Google already had their follow-up model
[00:27:26] ready for internal testing. The model is
[00:27:28] known by the code name Gemini 4 Carbon,
[00:27:30] and it seems like it's getting positive
[00:27:32] reviews from the Googlers who tried it.
[00:27:34] Critically, Gemini 4 Argon isn't just a
[00:27:36] new commercial model. It's also a new
[00:27:39] ultra-large base model that Google can
[00:27:40] train on top of. They don't need to
[00:27:42] complete another long pre-training run.
[00:27:44] They can apply relatively fast
[00:27:46] post-training on top of Argon. We've
[00:27:48] seen what that meant for Meta with the
[00:27:49] release of Muse Spark. The first version
[00:27:51] was pretty dismal, but they released
[00:27:52] three additional versions in 5 months,
[00:27:54] and bootstrapped their way to a
[00:27:55] competitive mid-sized model.
[00:27:57] Reinforcement learning runs on an
[00:27:58] ultra-large model won't be quite as
[00:28:00] fast, but it still gives Google a clear
[00:28:02] pathway to rapid model improvement.
[00:28:04] There's also the fact that the creators
[00:28:06] and listeners of this podcast may be a
[00:28:08] little too deep in AI to understand how
[00:28:10] much existing distribution matters over
[00:28:12] even model capabilities. A week ago,
[00:28:14] Google's Logan Kilpatrick posted, "In
[00:28:16] just the first 72 hours since Gemini 4
[00:28:18] Argon launched, we processed around 25
[00:28:20] trillion tokens. The demand for
[00:28:22] intelligence is incredible and still
[00:28:24] underappreciated."
[00:28:26] At the end of the day, Genie 4 is still
[00:28:28] not out of the tech demo stage when it
[00:28:30] comes to world models, but you can feel
[00:28:32] it's getting tantalizingly close to that
[00:28:34] inflection, where tech demo becomes
[00:28:35] real-world application. And in the case
[00:28:37] of world models and Genie specifically,
[00:28:39] that could be a big change indeed.
[00:28:42] For now, that's going to do it for
[00:28:43] today's AI daily brief. Appreciate you
[00:28:45] listening or watching as always, and
[00:28:46] until next time, peace.
