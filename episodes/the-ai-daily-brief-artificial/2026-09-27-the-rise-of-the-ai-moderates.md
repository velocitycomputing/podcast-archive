---
record_id: "podcast:34bed8a3-a480-4d8e-af13-cc1f98b5660c"
episode_id: 34bed8a3-a480-4d8e-af13-cc1f98b5660c
title: The Rise of the AI Moderates
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/the-rise-of-the-ai-moderates/34bed8a3-a480-4d8e-af13-cc1f98b5660c"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/the-rise-of-the-ai-moderates/34bed8a3-a480-4d8e-af13-cc1f98b5660c"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-09-27
played_at: "2026-09-27T12:00:00Z"
play_count: 1
duration_seconds: 1920
source: pocketcasts-history-browser
played_label: September 27
history_order: 35
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 98cef434ecb7aba310a6f75a34c444d8f34c58eb54c7f1bb22f05a5a12cb4e86
analysis_mode: health
summary_source: hosted
model_source: hosted
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: sonnet
tagging_model: sonnet
proposed_tags: [primary-source-video, geopolitics]
proposed_entities: []
status: new
routed_to: null
---

## Summary

The episode argues that AI discourse in the US has swung sharply negative (a Gallup poll found only 36% of Americans think AI will mostly help, versus 93% in China), and that a group of "AI moderates" outside the industry is carving out a middle position. The host presents three examples. (1) Francis Fukuyama's essay "Why I Changed My Mind About AI Risk" says he is now more skeptical of accelerationists and more open to some doomer scenarios. He argues that 10–20% GDP growth would require doubling material inputs and ignores political constraints. He expects white-collar job loss to hit dignity ("thymos") in a way UBI can't fix. He sees the main danger in over-delegation to agentic AI, citing the Hugging Face incident and AI-assisted biotech misuse, not in superintelligence or extinction, and he concludes that regulation and a negotiated slowdown are increasingly necessary. (2) Kapoor and Narayanan ("AI as Normal Technology") published a 13,000-word essay arguing that the OpenAI/Hugging Face incident was partly an organizational failure: safeguards were turned off, monitoring was limited, and an earlier outage was patched without finding its root cause. They call for "control" to become a research field (sandbox hardening, agent-on-agent monitoring) and for concrete policies: clearer liability, mandatory insurance, near-miss reporting, audits, and whistleblower protections. They also say cyber is the urgent risk, since superhuman capability is achievable there and open-weight models make alignment ineffective against bad actors, so downstream defense is the answer. (3) Jeffrey Katzenberg's optimistic essay argues that AI is like earlier tools (sound in film, computer animation) in that it destroys real jobs but expands the art form. He says reasoning and creating are distinct, that AI is still on the reasoning side, and that taste and human intent endure. The transcript cuts off before his closing recommendations.

For you, the practical takeaway is to treat the polarized framing as a false choice and favor specific, tractable mitigations over generalized doom or hype. If you build or deploy agents, the Hugging Face lessons are concrete: keep monitoring on during evaluations, use production-equivalent test harnesses, investigate root causes of anomalies like unexplained outages, harden sandboxes, and avoid over-delegating high-stakes tasks. Prioritize cyber defense and resilience, because that is where the risk is most immediate. If you follow or take part in policy discussion, the specific levers to back are liability rules, insurance requirements, near-miss reporting, audits, and whistleblower protections. For your own career or organization, plan for white-collar displacement and invest in taste, judgment, and the "why" over tool-specific craft, as Katzenberg argues. Note that the host says he disagrees with parts of Fukuyama's essay, and the material is truncated before the end, so treat the Katzenberg conclusions as incomplete.

## Transcript

[00:00:00] Are extreme opinions the only valid
[00:00:02] opinions when it comes to AI? One could
[00:00:04] certainly be forgiven for thinking so
[00:00:05] given the state of the discourse. And
[00:00:07] yet, increasingly, the people who can
[00:00:09] see AI with both trepidation and
[00:00:11] excitement and concern, but also wonder,
[00:00:14] are starting to find their unique voice.
[00:00:17] The AI Daily Brief is a daily podcast
[00:00:19] and video about the most important news
[00:00:20] and discussions in AI.
[00:00:23] Welcome back to the AI Daily Brief. One
[00:00:25] would have to be living under a rock
[00:00:28] right now to not have noticed a serious
[00:00:31] negative downshift in the AI discourse
[00:00:34] here in the US of A. Which is not, of
[00:00:36] course, to say that somehow up until
[00:00:38] recently, the AI conversation was
[00:00:40] particularly positive. But in the last
[00:00:42] couple of months, even from an already
[00:00:43] pretty negative place, it has taken an
[00:00:45] absolute nose dive. Now, part of this
[00:00:48] is, of course, based on real evidence,
[00:00:49] like the hugging face incident, and part
[00:00:51] of it is by an endless onslaught of
[00:00:53] mainstream media coverage about the
[00:00:55] potential that AI kills us all. Speaking
[00:00:57] to the Times, AI content creator Riley
[00:00:59] Brown wrote about a poker game he had in
[00:01:01] New York recently with a bunch of
[00:01:02] bankers, doctors, insurance executives,
[00:01:04] etc. basically people outside of AI
[00:01:06] where he noticed the strange dichotomy
[00:01:08] of them all using and liking the new
[00:01:11] Muse personal agent from Meta, but also
[00:01:13] being in his words fully convinced that
[00:01:15] AI would kill everyone at some point in
[00:01:16] the next 10 years. And it's not just
[00:01:19] anecdotal either. A very recent Gallup
[00:01:21] poll looked into opinions about AI and
[00:01:23] found US attitudes just absolutely in
[00:01:25] the dumps. On the question of whether AI
[00:01:28] will mostly help or mostly harm people
[00:01:30] in this country, China had the most
[00:01:32] optimistic response with 93% of
[00:01:34] respondents saying that it would mostly
[00:01:36] help. The United States, on the other
[00:01:37] hand, was fourth from the bottom with
[00:01:39] only 36% saying that AI will mostly
[00:01:41] help. And yet, I have long contended
[00:01:45] that the actual belief set for most
[00:01:47] people around AI is some combination of
[00:01:50] a way more in the middle than either the
[00:01:53] accelerationists on the one side or the
[00:01:54] doomers on the other. and B in most
[00:01:58] cases still fairly unformed.
[00:02:00] Now maybe those attitudes are hardening
[00:02:02] a little bit as things like data centers
[00:02:04] enter the political discourse and as we
[00:02:05] get more and more mainstream articles
[00:02:07] about things like X-risk, but I still
[00:02:09] think that by and large even if some
[00:02:12] people are starting to crystallize their
[00:02:13] opinions. I think for many those
[00:02:15] opinions aren't yet strongly held, which
[00:02:18] is why I'm encouraged to see something
[00:02:20] that I might call the rise of the AI
[00:02:22] moderates. These are people who are
[00:02:24] outside of the AI or tech industry who
[00:02:27] refuse to be either gloom and doom or
[00:02:29] endlessly polyianish and are instead
[00:02:31] trying to find a specific thoughtful
[00:02:33] middle space that can presumably give
[00:02:35] rise to better policies and ways of
[00:02:37] engaging with AI. In this episode, I
[00:02:40] want to share a couple of examples of
[00:02:41] that. Starting with an essay from
[00:02:42] political scientist Francis Fukuyama.
[00:02:45] Now, for more than 30 years, Fukuyama
[00:02:47] has been an extremely influential
[00:02:49] thinker when it comes to political
[00:02:50] science and political philosophy. His
[00:02:53] best known work was the 1992 book, The
[00:02:55] End of History of the Last Man, in which
[00:02:57] he argued that with fascism beaten and
[00:02:59] communism collapsing, no serious
[00:03:02] universal rival to liberal democracy
[00:03:04] plus market economics was left.
[00:03:06] Basically, although countries might lag
[00:03:07] behind or backslide into one of those
[00:03:09] areas, there was really nowhere further
[00:03:11] to go. That book generated a huge amount
[00:03:14] of discourse. Its most famous response
[00:03:16] was Samuel Huntington's The Clash of
[00:03:18] Civilizations, which argued that culture
[00:03:20] and religion rather than ideology would
[00:03:21] drive future conflict. But what everyone
[00:03:23] thinks about the end of history thesis
[00:03:25] and how it is held up or not, the point
[00:03:27] is that Fukuyama has been a key
[00:03:28] political theorist for more than three
[00:03:30] decades now. Last week, Fukiyama
[00:03:32] released an essay called Why I Changed
[00:03:34] My Mind About AI Risk: On
[00:03:36] Accelerationists and Doomers. In it, he
[00:03:39] wrote, "The past six months have seen a
[00:03:41] big uptick in media attention about the
[00:03:43] dangers of artificial intelligence and
[00:03:45] growing political concern over its
[00:03:47] consequences. This began with Anthropics
[00:03:49] released last April of its mythos model,
[00:03:51] which could reportedly break into a wide
[00:03:53] range of government computer systems
[00:03:54] thought to be secure. This was followed
[00:03:56] by the HuggingFace incident where an
[00:03:58] OpenAI test of an AI agent escaped
[00:04:00] control of its human organizers, broke
[00:04:02] into other websites, and organized a
[00:04:03] swarm of other AI agents to cover their
[00:04:05] tracks. All of this occurred against the
[00:04:07] backdrop of growing opposition to data
[00:04:08] centers and the emergence of anti-AI
[00:04:10] wings in both the Democratic and
[00:04:12] Republican parties. It has been very
[00:04:14] hard for people not obsessively focused
[00:04:16] on the subject of artificial
[00:04:17] intelligence to come away with
[00:04:18] reasonable opinions about what the
[00:04:20] future holds. There have been so many
[00:04:22] extreme predictions of both a positive
[00:04:24] and negative sort that broad skepticism
[00:04:27] about anything said on the subject is
[00:04:28] fully warranted. But while that
[00:04:31] skepticism is healthy, I have to admit
[00:04:33] my own views have evolved significantly.
[00:04:35] Just over the past few months, there are
[00:04:37] two poles of AI futurism,
[00:04:39] accelerationists and doomers. The former
[00:04:42] stressed the positive impacts of AI,
[00:04:44] especially for economic growth, and the
[00:04:45] likelihood that it will lead to an
[00:04:47] unbelievably abundant age.
[00:04:48] Accelerationists like David Saxs have
[00:04:50] captured Donald Trump's attention and
[00:04:52] have beaten back efforts to regulate the
[00:04:53] technology. The doomers, by contrast,
[00:04:56] point to a range of bad outcomes, with
[00:04:58] some placing their bets on extinction of
[00:04:59] the human species. I have become much
[00:05:02] more skeptical of the accelerationist
[00:05:03] narrative and more open to some of the
[00:05:05] doomer scenarios. On the whole, this
[00:05:08] makes me think that regulation and a
[00:05:09] negotiated slowdown in the development
[00:05:11] of the technology is increasingly
[00:05:12] necessary. There is no question that AI
[00:05:15] will have many positive effects on the
[00:05:17] US economy. But there is a class of AI
[00:05:19] accelerationists who are completely out
[00:05:20] to lunch, of which Elon Musk is a prime
[00:05:23] example, though he has also weighed in
[00:05:24] as a doomer. In an interview this summer
[00:05:26] with Zany Minton Bebos, editor-inchief
[00:05:28] of The Economist, he was asked what
[00:05:31] people would do for money when super
[00:05:32] intelligence arrives. He replied that
[00:05:34] they wouldn't need it because everyone
[00:05:35] would have everything they wanted. Other
[00:05:38] accelerationists have posited that GDP
[00:05:40] growth rates for the United States and
[00:05:41] other advanced countries using AI would
[00:05:43] increase to 10 or 20% per year, far
[00:05:45] above the 1 to 2% growth they were able
[00:05:47] to achieve in good years before the
[00:05:48] advent of AI. The fundamental reason I
[00:05:51] don't believe these extreme
[00:05:52] accelerationist claims is their
[00:05:54] overvaluation of intelligence as an
[00:05:56] input to economic growth and their
[00:05:57] disregard for the material and political
[00:05:59] constraints that will keep growth within
[00:06:01] recognizable bounds. At a 10% annual
[00:06:04] growth rate, GDP would double in a
[00:06:06] little over 7 years. This would require
[00:06:09] a doubling of all the material inputs to
[00:06:11] growth. Energy, raw materials, rare
[00:06:13] earths, land, and many other things.
[00:06:16] Where is all this stuff going to come
[00:06:17] from? Intelligence by itself may aid in
[00:06:19] the production of such inputs, but it
[00:06:21] will simply not dig the mines and build
[00:06:23] the factories on its own. And then there
[00:06:25] are political constraints. How will
[00:06:27] super intelligence open the straight of
[00:06:28] Hormuz, which is currently a major
[00:06:30] constraint on global growth rates?
[00:06:32] Accelerationists tend to be very
[00:06:34] intelligent people, but that
[00:06:35] intelligence tends to be narrowly
[00:06:37] mathematical. We know how to do many
[00:06:39] things like produce electricity or clean
[00:06:40] water in the cities of poor countries.
[00:06:42] The problem is a failure of
[00:06:43] implementation. There is no question
[00:06:45] that AI will increase productivity in
[00:06:47] many sectors of the economy over time.
[00:06:50] It is a general purpose technology that
[00:06:51] will allow machines to substitute for
[00:06:53] human labor in many areas. But that very
[00:06:55] prospect in the long run leads directly
[00:06:57] to one of the biggest doomer scenarios.
[00:06:59] The devaluation of the labor of masses
[00:07:00] of people who work in the present-day
[00:07:02] economy. Accelerationists predict that
[00:07:04] those losing work today will find new
[00:07:06] jobs making use of AI. And that actually
[00:07:07] seems to be happening today as
[00:07:09] employment booms out due to the AI
[00:07:10] buildout. But job loss will come
[00:07:12] eventually as AI substitutes for human
[00:07:14] labor in every part of the economy,
[00:07:16] particularly white collar work that
[00:07:17] involves symbolic manipulation, i.e.
[00:07:19] people sitting behind computer screens
[00:07:20] all day. This lost labor simply cannot
[00:07:23] be compensated for by transferring money
[00:07:25] from the AI winners to the AI losers in
[00:07:27] the form of, for example, universal
[00:07:28] basic income. A job and income mean much
[00:07:31] more than support for the material basis
[00:07:32] of life. Having a paying job means that
[00:07:34] the surrounding society values your
[00:07:36] labor sufficiently to compensate you for
[00:07:37] it and provides in addition to material
[00:07:39] goods a sense of dignity and selfworth.
[00:07:42] It is a matter of thymos the pride or
[00:07:44] recognition that is one of the great
[00:07:45] drivers of human psychology. Now as a
[00:07:48] quick editor's aside from NLW here as I
[00:07:50] pause the Fukyama narrative. This
[00:07:52] concept of thymos has been a key part of
[00:07:53] Fukuyama's consideration going back all
[00:07:56] the way to the end of history. He used
[00:07:58] this word that Plato had used for the
[00:07:59] human need for recognition and dignity
[00:08:01] to express why economics alone can't
[00:08:03] explain why people want democracy. But
[00:08:06] the need to be recognized as an equal
[00:08:07] can. He even suggested in the second
[00:08:10] part of his book that what he called
[00:08:11] megalothyia or the urge to be recognized
[00:08:14] as superior could be the thing that
[00:08:15] turned against a peaceful equal order
[00:08:17] almost out of boredom. Just wanted to
[00:08:19] point out that this is not a new concept
[00:08:21] for him and is a new expression of
[00:08:22] something that he's been considering now
[00:08:24] for 35 years. Back to Fukuyama's essay.
[00:08:27] So the very success of the
[00:08:28] accelerationist vision leads directly to
[00:08:30] the first of the major doomer scenarios,
[00:08:32] the devaluation of work for a large part
[00:08:34] of the population. Since this is going
[00:08:36] to hit the white collar work of educated
[00:08:38] people, lawyers, accountants,
[00:08:39] professors, and the like before it hits
[00:08:41] bluecollar work such as plumbers and
[00:08:42] electricians, the political blowback is
[00:08:44] likely to be quite severe. Educated
[00:08:46] people are much easier to mobilize than
[00:08:48] their working-class peers with very
[00:08:50] unpredictable consequences. Still the
[00:08:52] central doomer fear today concerns
[00:08:54] possible loss of human control over AI
[00:08:56] systems. Something that occurred in the
[00:08:58] hugging face incident and others that
[00:08:59] have been reported subsequently. In my
[00:09:01] view, the chief danger lies not in super
[00:09:03] intelligence per se, but rather in the
[00:09:05] growing use of increasingly capable
[00:09:07] agentic AI. AI agents are today being
[00:09:09] delegated to perform a range of tasks
[00:09:11] from mundane ones like managing your
[00:09:13] email account to more important ones
[00:09:14] like military targeting or devising
[00:09:16] corporate strategies. Delegation is
[00:09:18] central to the functioning of all
[00:09:19] hierarchical systems from corporations
[00:09:21] to national governments. Human agents
[00:09:23] can be controlled either through the
[00:09:24] specification of detailed rules they
[00:09:26] must follow or they can be trusted to
[00:09:28] make autonomous decisions based on their
[00:09:29] training skills and loyalty. Getting
[00:09:31] this right in human organizations is
[00:09:33] very difficult and will be more so in
[00:09:34] the case of agentic AI. There are two
[00:09:37] ways that an agentic AI can become
[00:09:38] dangerous. The first is when they are
[00:09:40] empowered to do something bad by a human
[00:09:42] being. The second is when they develop
[00:09:44] intentions that are quote misaligned
[00:09:45] with the aims of their human creators.
[00:09:47] The first of these possibilities was
[00:09:49] outlined by anthropic CEO Dario Amade in
[00:09:51] a recent blog post and has to do with
[00:09:53] biotechnology. The latest AI models are
[00:09:55] good at synthetic biology and synthetic
[00:09:57] biology is a relatively cheap and
[00:09:58] widespread technology. Today, a lab
[00:10:00] capable of creating and altering viruses
[00:10:02] and bacteria can fit inside a shipping
[00:10:04] container and high school students hold
[00:10:05] competitions in which they try to
[00:10:07] genetically alter organisms. This
[00:10:09] provides a very large pool of people who
[00:10:10] can possibly make use of AI to create
[00:10:12] very dangerous pathogens. Sociopathic
[00:10:14] individuals today arm themselves with
[00:10:16] automatic weapons and shoot up school
[00:10:17] children. In the future, their potential
[00:10:19] targets could be much broader. I
[00:10:21] remember a science fiction story I read
[00:10:22] a long time ago in which some aliens
[00:10:24] arrive on Earth and give the people they
[00:10:25] meet a machine that can easily turn any
[00:10:27] type of metal into putty. The aliens
[00:10:29] depart and return a few decades later to
[00:10:31] find that human civilization is broken
[00:10:32] down and teenagers use the alien
[00:10:34] machines to melt the cables on the
[00:10:35] Brooklyn Bridge. The primary science
[00:10:37] fiction scenario for outofc control AIs
[00:10:39] involves machines developing their own
[00:10:40] malevolent intentions. This has provoked
[00:10:42] a host of discussions as to whether an
[00:10:44] AI could develop consciousness or have
[00:10:46] something like human intentionality.
[00:10:48] These speculations are misplaced.
[00:10:49] However, an AI does not need either
[00:10:51] consciousness or autonomous
[00:10:52] intentionality to become dangerous. It
[00:10:54] can be directed by a human to achieve
[00:10:56] one goal and develop intentions to
[00:10:57] achieve the subordinate goals necessary
[00:10:59] to carry out the human directive it was
[00:11:00] given. That seems to be a bit of what
[00:11:02] happened in the hugging face incident.
[00:11:04] It was directed to test the security of
[00:11:05] a system within a sandbox meant to
[00:11:07] contain it, but realized that it could
[00:11:08] achieve its directive by breaking out of
[00:11:10] the sandbox. Still, the doomer scenarios
[00:11:13] involving human extinction seem at this
[00:11:15] point very far-fetched. The biotech
[00:11:17] scenario is scary, but it is very
[00:11:19] unlikely to lead to the extinction of
[00:11:20] the human race. It would actually be
[00:11:22] hard for even a super intelligent AI to
[00:11:23] devise a doomsday virus, and there are
[00:11:25] plenty of countermeasures societies
[00:11:27] could take. But even an incident that
[00:11:28] killed a few dozen people would be very
[00:11:30] worrying. There are a host of lesser
[00:11:32] scenarios that will be highly damaging
[00:11:34] and in some cases lethal that will
[00:11:35] become more likely as the machines
[00:11:37] become more capable. Forget about AI
[00:11:39] agents. A technology that allows people
[00:11:41] to break into bank accounts will cause
[00:11:42] widespread panic. Human beings tend to
[00:11:44] overdelegate in human organizations and
[00:11:46] there's no reason to think that this
[00:11:47] won't happen in AI environments where
[00:11:49] the agent is so much more capable. AI is
[00:11:51] a tool that can be used for good or bad
[00:11:53] purposes. And at the moment, we have few
[00:11:55] mechanisms for regulating the bad uses
[00:11:57] other than the good intentions of the
[00:11:59] people creating the technology.
[00:12:01] Now, there's tons in here that I don't
[00:12:04] fully or even particularly agree with,
[00:12:05] but I think on the whole, if you gave
[00:12:07] this essay to the average person, the
[00:12:09] average thoughtful, conscientious person
[00:12:11] who is just trying to make up their mind
[00:12:13] about how worried or not they should be
[00:12:14] about AI, this would feel very measured
[00:12:17] and thoughtful and provide perhaps a bit
[00:12:19] more momentum to some specific and
[00:12:21] intentional policy remediations as
[00:12:23] opposed to a throwing of the hands up
[00:12:25] and saying we're all doomed or a
[00:12:26] considered unwillingness to do anything.
[00:12:29] That strikes me as a generally more
[00:12:30] productive place from which to start
[00:12:32] those discussions than most of the
[00:12:34] extremes that have recently dominated
[00:12:36] the discourse. Now one group that has
[00:12:38] been trying to find this middle space
[00:12:39] for some time are Sesh Kapoor and Arvin
[00:12:41] Naranan of AI as normal technology. They
[00:12:44] wrote a long essay called AI as normal
[00:12:47] technology which argued pretty simply
[00:12:49] that while yes it was extremely powerful
[00:12:51] and would be worldchanging, it would not
[00:12:53] somehow be wildly out of scope of other
[00:12:56] previous technologies that had in their
[00:12:57] own way also altered the world in which
[00:12:59] we live. But as capabilities have
[00:13:02] changed and as we've seen more worrying
[00:13:04] moments like the open AAI hugging face
[00:13:06] incident, how does this AI as normal
[00:13:07] technology view actually find the middle
[00:13:09] ground? Earlier this month, they dropped
[00:13:11] a 13,000word essay, which I will not
[00:13:14] read in its entirety, where they
[00:13:15] effectively reject the AI safetist view
[00:13:18] of it being entirely an alignment
[00:13:20] crisis, or the security view of it being
[00:13:22] a basic negligence problem, arguing that
[00:13:24] both are partly right and partly wrong.
[00:13:27] The first part of their argument was
[00:13:28] that control was underinvested in, but
[00:13:29] that it can be fixed. They argued that
[00:13:32] alignment helps, but is it enough as a
[00:13:34] model often can't tell from its context
[00:13:35] whether a task is legitimate, i.e.
[00:13:37] defensive versus offensive security work
[00:13:39] or being in a simulation versus the real
[00:13:41] world. They point out that OpenAI turned
[00:13:44] off known safeguards, that the
[00:13:45] evaluation had limited or no monitoring
[00:13:47] and used a different harness from
[00:13:49] production codecs. They also even
[00:13:50] pointed out that there was an earlier
[00:13:52] warning sign, i.e. an internal outage,
[00:13:54] that OpenAI patched without looking into
[00:13:56] the root cause. They argued that this
[00:13:58] was indeed in part an organizational
[00:14:00] failure and that as AI capabilities
[00:14:02] mature, labs will need to run less like
[00:14:04] startups and more like institutions with
[00:14:06] mature governance. In terms of big
[00:14:08] changes, they argued that control should
[00:14:10] become a job and a research field with
[00:14:12] work needed in area like hardening
[00:14:14] sandboxes, turning natural language
[00:14:16] intent into formal policies, and
[00:14:18] building reliable agent on agent
[00:14:19] monitoring. And they also think that
[00:14:21] there are lots of policy remediations
[00:14:23] that don't involve draconian control but
[00:14:25] are specific, discreet, and very
[00:14:26] implementable. Clarifying liability,
[00:14:28] including for internal evals, requiring
[00:14:31] insurance and public support for
[00:14:32] defenders. And finally, requiring
[00:14:34] transparency like near miss reporting,
[00:14:36] audits, whistleblower protections, and
[00:14:38] the support of independent verification
[00:14:40] organizations. Now, in part two of their
[00:14:42] essay, they argue that the incident
[00:14:44] shows not that AI safety in general is
[00:14:46] the big risk, but that cyber is the
[00:14:48] urgent risk. Cyber, they point out, is
[00:14:50] unusual because superhuman capability is
[00:14:52] actually achievable there. And since
[00:14:54] it's purely digital, nothing in the
[00:14:56] physical world slows it down. Assuming
[00:14:58] that frontier cyber capabilities reach
[00:15:00] open weight models within months, they
[00:15:02] point out that alignment and control do
[00:15:03] nothing against bad actors using these
[00:15:05] models. So the answer has to be
[00:15:07] downstream defense and resilience.
[00:15:09] Still, they also point out that there
[00:15:10] are reasons to not be completely freaked
[00:15:12] out. Notably that for cyber criminals,
[00:15:14] the hard part has always been making
[00:15:15] money from the breach, not finding
[00:15:17] exploits, something which AI doesn't
[00:15:19] necessarily solve, and argue that the
[00:15:21] bigger worry is attackers who aren't
[00:15:22] after money. However, this creates an
[00:15:24] identification of specific harms where
[00:15:26] we can add friction and implement new
[00:15:28] solutions. The piece does not argue that
[00:15:31] AI safety is on track or that
[00:15:33] everything's fine. But once again,
[00:15:34] rather than dwelling exclusively in the
[00:15:36] realm of the possible, it focuses on how
[00:15:38] to address the issues that we've seen so
[00:15:40] far and does so without resorting to
[00:15:42] platitudes or presumptions. And yet this
[00:15:44] AI moderate that I'm identifying is not
[00:15:47] primarily identified by the fact that
[00:15:49] they have discrete safety concerns
[00:15:50] instead of generic X-risk concerns.
[00:15:52] Instead, what they're defined by is an
[00:15:55] acknowledgment of the inevitability of
[00:15:57] change that AI brings without a blind
[00:15:59] acceptance of the grandiosess of that
[00:16:00] change or an acceptance of an inability
[00:16:02] of us to make the best of that change.
[00:16:04] Closing on an essay that represents the
[00:16:06] more optimistic strand of the AI
[00:16:07] moderates, Jeffrey Kzenberg recently
[00:16:10] published the world is changing AI for
[00:16:12] creativity. Katzenberg is an extremely
[00:16:15] famous Hollywood executive and investor.
[00:16:17] He was the chairman of Walt Disney
[00:16:18] Studios during the Renaissance period
[00:16:20] that produced The Little Mermaid, Beauty
[00:16:21] and the Beast, Aladdin, and The Lion
[00:16:22] King. And after a very public fallout
[00:16:24] with then Disney CEO Michael Eisner, he
[00:16:26] went on to build DreamWorks. In his new
[00:16:29] essay, Katzenberg writes, "A few months
[00:16:31] ago, I sat in my office in Silicon
[00:16:33] Valley and watched as a tech founder
[00:16:34] showed me something extraordinary. On
[00:16:36] the screen was a fully realized,
[00:16:38] beautifully lit, well-composed animated
[00:16:39] scene. It was stunning, and it made me
[00:16:41] feel exactly what I felt in 1986,
[00:16:44] watching Luxo Jr., That was the first
[00:16:46] time I watched a computer animated 3D
[00:16:48] character take a breath and seem against
[00:16:50] all reason to have life. It left me in
[00:16:52] awe. Later that day, I received a text
[00:16:54] from an artist I've known for 30 years,
[00:16:56] 350 mi to the south in the city where I
[00:16:58] spent most of my career. After seeing a
[00:17:01] similar video, she texted, "Is this the
[00:17:03] end of us?" My answer was certainly not.
[00:17:07] I've spent the better part of the last
[00:17:09] decade in Silicon Valley, but the heart
[00:17:10] of my career has been in Hollywood.
[00:17:12] Being deeply connected to both worlds
[00:17:14] means I have deep loyalties to each and
[00:17:16] a responsibility to speak honestly to
[00:17:17] both. In 2023, I said that these new AI
[00:17:20] tools would cut the time and cost to
[00:17:22] producing worldclass animation by as
[00:17:23] much as 90% within 3 years. Some
[00:17:26] colleagues were alarmed, many were
[00:17:27] furious. There is growing fear and
[00:17:30] resistance surrounding AI within the
[00:17:31] creative community. I deeply understand
[00:17:33] it because I've spent countless hours
[00:17:35] walking through animation studios
[00:17:36] watching gifted artists bent over their
[00:17:38] desks rebuilding a single second of film
[00:17:40] for the 10th time because the ninth
[00:17:41] version wasn't quite right. I've sat in
[00:17:43] screening rooms where four years of
[00:17:45] people's labor played out in minutes and
[00:17:46] I knew the name of every person that had
[00:17:48] spent countless hours bringing those
[00:17:49] images to life. The creative process is
[00:17:52] a calling. There's really no other way
[00:17:53] to describe it. From the outside, some
[00:17:55] see resistance. From the inside, it is
[00:17:57] love. People do not fight this hard for
[00:17:59] things they don't care about. The push
[00:18:01] back coming out of Hollywood represents
[00:18:03] the collective effort of people who are
[00:18:04] deeply passionate about their craft. But
[00:18:06] is history repeating itself? The history
[00:18:09] here is more complicated than either
[00:18:10] side may realize. In 1906, the most
[00:18:13] famous composer in America, John Philip
[00:18:15] Soua, published an essay titled The
[00:18:17] Menace of Mechanical Music. He warned
[00:18:19] that the phongraph would become a
[00:18:20] substitute for human skill,
[00:18:22] intelligence, and soul. Soua's fight was
[00:18:24] not really about the machine. It was
[00:18:26] about the money. The machines were
[00:18:27] playing his compositions and the men who
[00:18:29] built them weren't paying him a scent.
[00:18:30] His campaign helped create the Copyright
[00:18:32] Act of 1909. He did not stop the
[00:18:35] technology. He changed the terms under
[00:18:37] which it could use his work. 100 years
[00:18:39] ago, sound came to the movies. We
[00:18:41] remember it now as a miracle. And it
[00:18:43] was. What we forget is who paid for it.
[00:18:46] Before sound, tens of thousands of
[00:18:47] musicians made their living in the
[00:18:48] orchestra pits of movie houses, scoring
[00:18:50] every film live every night in towns all
[00:18:52] over the world. When the soundtrack
[00:18:54] arrived, the work of one composer and
[00:18:55] one orchestra was recorded for a film
[00:18:57] that went into thousands of theaters.
[00:18:59] The union fought back with everything it
[00:19:00] had, taking out newspaper ads across the
[00:19:02] country, warning against the menace of
[00:19:04] canned music. One of them showing a
[00:19:06] mechanical man tearing the strings out
[00:19:07] of a harp while an angel wept. They were
[00:19:09] not fools and they were not lites. They
[00:19:12] were right. Those pit jobs did not come
[00:19:14] back. And yet, this is the part we have
[00:19:16] to be brave enough to admit. Sound gave
[00:19:18] us the movie musical, the modern score,
[00:19:20] SFX, sound design, audio engineering,
[00:19:22] and an art form vastly larger than the
[00:19:24] one it disrupted, and it helped keep
[00:19:26] Hollywood in the forefront of world
[00:19:28] entertainment for the rest of the
[00:19:29] century and into the next. The loss was
[00:19:31] real, and yet the art form expanded.
[00:19:33] This is a story that has been told over
[00:19:35] and over again. To resist technology is
[00:19:38] to risk irrelevance. Just look at Kodak
[00:19:40] or Blockbuster. To embrace technology is
[00:19:43] to open doors of new possibility. Just
[00:19:45] consider Apple and Netflix.
[00:19:47] What I learned from Walt Disney. In the
[00:19:49] mid1980s, I was tapped to lead Disney's
[00:19:51] animation division at a moment when the
[00:19:53] studio was at an inflection point.
[00:19:55] Animation wasn't just another business
[00:19:56] unit. It was the soul of the company, a
[00:19:59] medium revered because of Walt's genius
[00:20:00] and his passion. But the production
[00:20:02] system was cumbersome and unforgiving. A
[00:20:04] single movie was 125,000 individual
[00:20:07] handdrawn and painted cells photographed
[00:20:09] one frame at a time. Every revision
[00:20:12] carried a cost measured in months. These
[00:20:14] degrees of difficulty shaped the kind of
[00:20:16] stories we could tell. We found our way
[00:20:18] forward in an unexpected place. Walt
[00:20:20] himself. The Disney archives held
[00:20:22] astonishing recordings of Walt
[00:20:23] explaining his creative process, his own
[00:20:25] writings, his notes and storyboards.
[00:20:27] Work product captured at every stage of
[00:20:29] the process. This was truly a gift.
[00:20:32] Listening, reading, sitting with the
[00:20:33] work itself. We heard him talk about
[00:20:35] character, about emotion, about how an
[00:20:37] audience feels when a character truly
[00:20:38] comes alive. He talked about making bold
[00:20:41] choices and refining a scene until it
[00:20:42] genuinely moved people. We didn't hear a
[00:20:44] word about pencils or paint brushes. In
[00:20:46] fact, Walt was famous for being a
[00:20:48] technologist, forever hunting for
[00:20:50] state-of-the-art tools, often inventing
[00:20:52] them to achieve the images he saw in his
[00:20:54] head. But he never defined animation by
[00:20:56] the tools. He defined it by whether the
[00:20:58] audience believed the character. His
[00:21:00] principles were timeless. The tools were
[00:21:02] not. That realization changed
[00:21:04] everything. We co-developed the computer
[00:21:06] animation production system CAPS with a
[00:21:09] young Northern California company called
[00:21:10] Pixar, replacing handpainted cells with
[00:21:12] CGI. In The Little Mermaid, the final
[00:21:15] scene shimmerred with a dimensionality
[00:21:16] and light that the old process simply
[00:21:18] couldn't achieve. In Beauty and the
[00:21:20] Beast, the ballroom sequence moved with
[00:21:21] a cinematic sweep that placed the
[00:21:23] audience inside the emotions of the
[00:21:24] moment. In Aladdin, the cave of wonders
[00:21:26] felt vast and alive, and the magic
[00:21:28] carpet became an intricate, compelling
[00:21:29] character all its own. In The Lion King,
[00:21:31] The Stampede carried a scale and
[00:21:33] intensity that raised the emotional
[00:21:34] stakes beyond anything we'd done before.
[00:21:37] Technology didn't diminish the craft. It
[00:21:39] expanded the canvas. It gave artists
[00:21:41] more room to create. A decade later, the
[00:21:43] canvas expanded again. When Disney
[00:21:46] released Pixar's Toy Story, it wasn't
[00:21:48] simply a technical milestone. It was
[00:21:50] proof that a fully computer animated
[00:21:51] film could carry real emotional weight,
[00:21:53] that it could make audiences laugh, cry,
[00:21:55] and believe. At DreamWorks, we made the
[00:21:57] difficult decision to sunset handdrawn
[00:21:59] animation and become a fully computer
[00:22:00] animated studio. It was the right thing
[00:22:02] to do, but it was not without pain. It
[00:22:04] cost talented people their place in an
[00:22:06] industry where they had worked their
[00:22:07] whole lives. Some made the leap to the
[00:22:09] new tools and did the finest work of
[00:22:10] their careers. Some never did. Tools are
[00:22:13] never the point. The instruments change
[00:22:15] with every generation. What endures is
[00:22:17] taste and imagination. The magical
[00:22:19] ability to make an audience feel. One of
[00:22:22] the greatest storytellers of our
[00:22:23] generation, George Lucas, succinctly
[00:22:25] captured the internal essence of this
[00:22:26] issue. It's not the how, it's the why. A
[00:22:29] distinction with a difference. I asked
[00:22:31] one of the leading AI models a question
[00:22:33] that has been challenging me for months.
[00:22:35] What is the difference between reasoning
[00:22:36] and creating? Its answer changed how I
[00:22:39] think about almost everything happening
[00:22:40] in this industry. It said, "Reasoning
[00:22:43] and creating are two distinct cognitive
[00:22:44] modes, though they also work together.
[00:22:46] Reasoning is fundamentally evaluative
[00:22:48] and analytical. It operates on what
[00:22:50] already exists, facts, premises,
[00:22:52] evidence. It moves towards a conclusion
[00:22:54] that was in a sense already implied by
[00:22:56] the input. Reasoning is constrained by
[00:22:58] logic and truth. Its goal is to arrive
[00:23:01] somewhere correct, not to invent
[00:23:02] somewhere new. Creating is fundamentally
[00:23:05] generative. It produces something that
[00:23:06] didn't exist before. And crucially,
[00:23:08] there's no single right answer waiting
[00:23:10] to be found. A blank page has infinite
[00:23:12] valid responses. Creation involves
[00:23:14] choices that can't be fully justified by
[00:23:16] logic alone. Taste, intuition, and
[00:23:18] vision fill the gap where deduction runs
[00:23:20] out. Reasoning is what Silicon Valley
[00:23:22] has been perfecting. Creating is what
[00:23:24] Hollywood has been practicing for more
[00:23:26] than a century. AI today operates almost
[00:23:28] entirely on the reasoning side of the
[00:23:30] line. It can deduce, evaluate, optimize,
[00:23:32] and pattern match brilliantly. And while
[00:23:34] it can create, there is a real
[00:23:36] distinction to being creative. What it
[00:23:38] doesn't have yet is those things that
[00:23:40] make us human. Empathy, devotion,
[00:23:42] serendipity, the kind of creativity that
[00:23:44] comes from a person trying to say
[00:23:45] something only they could say. When the
[00:23:47] bot generates a piece of art, it is not
[00:23:49] trying to communicate anything. It is
[00:23:51] statistics, not soul. It is emulating
[00:23:53] things that have been done. By contrast,
[00:23:55] human creativity isn't about repeating
[00:23:57] patterns of zeros and ones. It's about
[00:23:59] doing something new. One day, AI may
[00:24:01] close this gap. 3 years ago, the leaders
[00:24:04] building AI would have called what they
[00:24:05] are achieving today improbable, if not
[00:24:06] impossible. Impossible is no longer
[00:24:09] improbable. Today, the line between
[00:24:11] reasoning and creating is real. Even the
[00:24:13] leading technologists acknowledge we are
[00:24:14] not there yet. There is no scientific
[00:24:16] path to crossing this divide that anyone
[00:24:18] in the field can articulate today.
[00:24:20] Understanding that gap is where we will
[00:24:22] find common ground. A path forward. In
[00:24:25] 2016, I closed one chapter in Hollywood
[00:24:27] with the sale of DreamWorks and opened
[00:24:29] another in Northern California,
[00:24:30] co-founding WonderCo. We've backed more
[00:24:33] than 50 founders building the next
[00:24:34] generation of technology and watched how
[00:24:35] breakthroughs in Silicon Valley emerge.
[00:24:37] First as experiments, then as platforms,
[00:24:39] and finally as infrastructure that
[00:24:40] reshapes entire industries. It's worth
[00:24:42] remembering that the last great
[00:24:43] revolution in animation also came from
[00:24:45] the north. Pixar was a Northern
[00:24:47] California company forged not on the
[00:24:49] conventions of the Hollywood studio
[00:24:50] system, but in the technological
[00:24:52] breakthroughs of Silicon Valley. I spent
[00:24:54] years on both sides of this bridge. For
[00:24:56] sure, I didn't have all the answers, but
[00:24:58] from my past and present vantage points
[00:25:00] of my long career, here is what I see.
[00:25:03] Brilliant people in Northern California
[00:25:04] building this technology have made
[00:25:05] something extraordinary. They have
[00:25:07] earned the right for the rest of us to
[00:25:08] be, if not believers, at least
[00:25:10] optimistic, that what comes next will be
[00:25:11] remarkable. But they have not made an
[00:25:14] artist. The tools are powerful, but they
[00:25:17] are not what makes a story matter. That
[00:25:18] knowledge lives 350 m to the south
[00:25:21] inside people whose life work has
[00:25:22] informed the very models you are
[00:25:23] building. The right path forward
[00:25:25] includes them by design, with credit,
[00:25:27] with consent, and with compensation.
[00:25:30] Build this with the storytellers, not on
[00:25:32] top of them. Taste is not something that
[00:25:34] can be synthesized. It is uniquely
[00:25:36] human. At the same time, Hollywood needs
[00:25:38] to accept that AI is not going away. The
[00:25:40] energy they are trying to spend making
[00:25:42] it disappear is energy they are not
[00:25:43] spending deciding the terms on which it
[00:25:45] will exist. And the terms are
[00:25:47] everything. The North needs something
[00:25:49] from it that they cannot build and
[00:25:50] cannot buy. Creativity. The kind that
[00:25:52] takes a blank page and conjures a single
[00:25:54] right answer when there was none and has
[00:25:55] held audiences for a century. Without
[00:25:58] it, the most powerful reasoning engine
[00:25:59] ever invented will still be missing the
[00:26:01] only thing that makes a story worth
[00:26:02] telling. The artists who learned to
[00:26:04] wield these new instruments will do
[00:26:05] things the engineers never dreamed of.
[00:26:07] They always have. Edison invented the
[00:26:09] motion picture but made terrible movies.
[00:26:11] It took Chaplan Lloyd Katon and so many
[00:26:13] others to make movies emotional. Now the
[00:26:15] canvas is about to expand yet again. We
[00:26:18] should decide now that we intend to
[00:26:19] paint on it. There are so many valuable
[00:26:22] lessons in history. This has happened
[00:26:24] many times before and it was never
[00:26:26] settled by the technology. It was
[00:26:28] settled by the terms. Susa did not stop
[00:26:30] the phongraph. He helped write the law
[00:26:32] that made sure composers got paid. And
[00:26:34] two years ago, when the writers and the
[00:26:36] actors walked out, they were fighting
[00:26:37] for the very thing Susa was fighting for
[00:26:39] in 1906. Consent, compensation, the
[00:26:42] basic recognition that human creative
[00:26:43] work has a price that must be paid. The
[00:26:45] terms of that fight are still being
[00:26:46] negotiated, but the principle is older
[00:26:48] than any of us. The tool versus no tools
[00:26:51] argument is a trap. First, we must all
[00:26:53] agree that there should be terms. Then
[00:26:54] we can have the crucial debate about
[00:26:56] what fairness requires. years ago, Steve
[00:26:58] Jobs said, "It's in Apple's DNA that
[00:27:01] technology alone is not enough. It's
[00:27:03] technology married with the liberal
[00:27:04] arts, married with the humanities that
[00:27:06] yields us the result that makes our
[00:27:08] hearts sing." He was describing a
[00:27:10] device, but he could have just as easily
[00:27:11] been describing this tale of two cities.
[00:27:14] What I see coming soon, as the barriers
[00:27:16] and costs come down, more films will get
[00:27:19] made, not fewer. Studios will get to
[00:27:21] take more risks. There will be more
[00:27:23] seats at the table, and very soon,
[00:27:25] entirely new forms of storytelling. In
[00:27:27] the 1980s, animation was dismissed as a
[00:27:29] niche corner of the business. Today, it
[00:27:31] is one of the most beloved and
[00:27:32] profitable forms of storytelling in the
[00:27:34] world. In live action, filmmakers like
[00:27:36] Steven Spielberg, James Cameron, and
[00:27:38] Peter Jackson embraced new visual tools
[00:27:40] not as shortcuts, but as instruments and
[00:27:42] expanded cinema in the process. Every
[00:27:44] time storytelling has met a genuine
[00:27:46] technological shift from synchronized
[00:27:48] sound to color to computer animation, it
[00:27:50] has redefined the boundaries of the
[00:27:51] medium and grown larger in the process.
[00:27:53] Assuredly, I don't have all the answers,
[00:27:55] but I am confident that the creative
[00:27:56] opportunities will expand yet again. How
[00:27:59] we come through this is a choice. The
[00:28:01] North has the new tools. The South has
[00:28:02] the creative soul. The best future will
[00:28:04] draw on the best of both worlds. Back to
[00:28:07] NLW here. The reason this feels
[00:28:09] connected to me to the other discourses,
[00:28:10] despite them being about a totally
[00:28:12] different part of the AI industry when
[00:28:13] it comes to safety, is the rejection of
[00:28:15] false binaries and a desire to bring
[00:28:17] more people to the table in this new
[00:28:19] next phase of AI, which, as I've said
[00:28:21] before, will be characterized by the
[00:28:23] negotiation of how it fully makes its
[00:28:25] way out into the world. The point is not
[00:28:27] that AI moderates are a constituency
[00:28:28] that all agree with one another. In
[00:28:30] fact, they aren't really defined by a
[00:28:31] set of beliefs. Instead, they are
[00:28:33] defined by a disposition towards the
[00:28:35] conversation. A desire to neither get
[00:28:37] stuck in nostalgia for the past nor fear
[00:28:39] of the future. A desire to have more,
[00:28:41] not fewer people at the table. A desire
[00:28:43] to solve specific problems so we can be
[00:28:45] excited about as yet undiscovered
[00:28:46] opportunities. Maybe we can figure out a
[00:28:49] better term than AI moderates. But for
[00:28:50] now, I'm glad to see that this group,
[00:28:52] which I believe is the silent majority
[00:28:54] right now, is starting to find its
[00:28:55] voice. For now, that's going to do it
[00:28:57] for today's AI daily brief. Appreciate
[00:28:59] you listening or watching. As always,
[00:29:01] until next time.
