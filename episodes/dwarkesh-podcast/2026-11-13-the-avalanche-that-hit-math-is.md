---
record_id: "podcast:c5d4e3ff-20d1-4e3e-9752-6887ccf8a52e"
episode_id: c5d4e3ff-20d1-4e3e-9752-6887ccf8a52e
title: The avalanche that hit math is coming for AI development
podcast_title: Dwarkesh Podcast
url: "https://pocketcasts.com/podcast/dwarkesh-podcast/6d554750-84ac-0138-ee2b-0acc26574db2/the-avalanche-that-hit-math-is-coming-for-ai-development/c5d4e3ff-20d1-4e3e-9752-6887ccf8a52e"
audio_url: "https://pocketcasts.com/podcast/dwarkesh-podcast/6d554750-84ac-0138-ee2b-0acc26574db2/the-avalanche-that-hit-math-is-coming-for-ai-development/c5d4e3ff-20d1-4e3e-9752-6887ccf8a52e"
feed_guid: null
feed_url: "https://apple.dwarkesh-podcast.workers.dev/feed.rss"
published_at: null
published_local_date: null
played_date: 2026-11-13
played_at: "2026-11-13T12:00:00Z"
play_count: 1
duration_seconds: 1620
source: pocketcasts-history-browser
played_label: Yesterday
history_order: 2
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: rss-podcast-transcript
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: fcc234409dfdcf8dab30d48278e9c420e872ce1bc0292337ee829a7bf7cead79
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

The speaker argues that AI progress is accelerating enough that AI systems may match the best human AI researchers in a couple of years or months, compressing progress so that by 2030, and possibly next year, AIs could match top human experts across fields. He cites Meter’s three-month embedded evaluation of Anthropic, which concluded Anthropic’s rate of AI progress on well-scoped tasks is 2x a year ago and that a majority of acceleration is likely attributable to Anthropic’s extensive AI use; OpenAI’s September post about internal coding-agent use by its heaviest 10% of researchers; and Anthropic’s September report that Claude leads 26% of its AI R&D work, up from under 1% in February. He uses mathematics as the central analogy, naming Dario, Toby Ort, Sholto Douglas, Chris Olah, Ajay Khotra, and Zuckerberg, and cites milestones: 2023 four-digit addition failures, 2024 weak high-school competition performance, 2025 International Math Olympiad gold, niche open problems earlier this year, and an OpenAI Millennium Prize problem solved in 88 hours. He also discusses the transformer as a recombination of known ideas, the formalization of Fermat’s Last Theorem by many agents, and estimates a median 2028 for automated AI researchers, with at least a 25% chance of after 2032 and a possible 2027 date, while weighing a “software-only singularity” against a “spark” scenario, with labs currently quadrupling R&D compute and doubling workforce yearly just to maintain progress.

For the user, the actionable takeaway is to treat the claimed 2x acceleration and 26% Claude-led R&D share as leading indicators to monitor rather than settled facts: track independent evals, lab publications, compute constraints, and whether model-generated research produces verified improvements in training efficiency, data filtering, RL environments, attention kernels, or benchmark performance. Research leads include the Meter Anthropic report, OpenAI and Anthropic September posts, Toby Ort’s essay on AI’s limits in asking powerful mathematical questions, Sholto Douglas’s transformer essay, Ajay Khotra’s takeoff modeling, and automated theorem proving/parallel agent workflows. Decisions to consider: if working in AI or adjacent technical fields, prioritize verifiable experiment design, evaluation, data pipelines, compute-efficient methods, and cross-domain synthesis; if investing or policy-planning, watch talent concentration, compute supply, safety governance, and the risk that a “spark” compresses years of capability gains into one year. Health-wise, the compressed timeline can create anxiety and information overload, so set bounded news checks, separate evidence from speculation, and maintain sleep, exercise, and offline routines while following rapid developments. Follow-up questions should ask how much of AI research is actually verifiable, whether 26% Claude-led work translates into causal progress, what compute bottlenecks remain, and what independent metrics would distinguish a software-only singularity from a spark.

## Transcript

WEBVTT
1
00:00:00.251 --> 00:00:00.672
<v SPEAKER_00> Thank you.
2
00:00:00.690 --> 00:00:04.250
<v SPEAKER_00>If you had asked me earlier this year how far away we are from superintelligence,
3
00:00:04.250 --> 00:00:06.629
<v SPEAKER_00>I'd probably have said at least a better part of a decade.
4
00:00:06.629 --> 00:00:09.378
<v SPEAKER_00>But over the last three months, I've updated my views a ton.
5
00:00:09.378 --> 00:00:13.872
<v SPEAKER_00>I've been debating people both on and off the podcast about this question.
6
00:00:13.872 --> 00:00:18.738
<v SPEAKER_00>And of course, I'm watching the progress of AI on verifiable domains and thinking
7
00:00:18.738 --> 00:00:21.269
<v SPEAKER_00>about what that implies for AI research itself.
8
00:00:21.269 --> 00:00:24.243
<v SPEAKER_00>And I've come to the view that we're only a couple years away,
9
00:00:24.293 --> 00:00:26.426
<v SPEAKER_00>and possibly only a couple months away,
10
00:00:26.476 --> 00:00:30.462
<v SPEAKER_00>from AIs that are as good as the best humans at AI research.
11
00:00:30.963 --> 00:00:34.558
<v SPEAKER_00>And I've also come to believe that automating AI research will compress
12
00:00:34.608 --> 00:00:40.810
<v SPEAKER_00>so much progress into a single year that soon thereafter, by 2030 and plausibly as
13
00:00:43.014 --> 00:00:47.063
<v SPEAKER_00>early as next year, we'll have AIs that are at least as good
14
00:00:47.063 --> 00:00:49.962
<v SPEAKER_00>as the best human experts in every field.
15
00:00:49.962 --> 00:00:54.561
<v SPEAKER_00>I know this is a wild claim and it's one that I myself didn't believe even
16
00:00:54.561 --> 00:00:58.610
<v SPEAKER_00>a couple months ago. Let me walk you through how my thinking has changed.
17
00:00:58.610 --> 00:01:01.014
<v SPEAKER_00>Before we get into the more speculative arguments about what will happen
18
00:01:01.034 --> 00:01:02.923
<v SPEAKER_00>in the future, I want to point out
19
00:01:03.097 --> 00:01:07.541
<v SPEAKER_00>that AI is already dramatically speeding up further AI progress at the frontier.
20
00:01:07.683 --> 00:01:11.461
<v SPEAKER_00>For example, Meter, which is an independent evaluation organization,
21
00:01:11.569 --> 00:01:14.010
<v SPEAKER_00>spent three months embedded of Anthropic,
22
00:01:14.270 --> 00:01:17.750
<v SPEAKER_00>and afterwards concluded that Anthropics' rate of AI progress
23
00:01:17.750 --> 00:01:22.170
<v SPEAKER_00>on well -scoped tasks is 2x what it was a year ago.
24
00:01:22.390 --> 00:01:27.350
<v SPEAKER_00>And that a quote majority of this acceleration today is likely attributable
25
00:01:27.350 --> 00:01:34.022
<v SPEAKER_00>to Anthropic's extensive use OpenAI published a blog post about this in September,
26
00:01:34.242 --> 00:01:36.986
<v SPEAKER_00>where they showed that the heaviest 10%
27
00:01:37.066 --> 00:01:42.034
<v SPEAKER_00>of AI users amongst OpenAI's researchers went from using about $1,000 a day
28
00:01:42.214 --> 00:01:43.992
<v SPEAKER_00>of internal coding agents at the
29
00:01:45.979 --> 00:01:52.967
<v SPEAKER_00>And also in September, Anthropic put out a similar post on its own AI uplift.
30
00:01:53.447 --> 00:01:58.573
<v SPEAKER_00>They reported that Claude now leads 26% of Anthropic's AI R&D work,
31
00:01:58.993 --> 00:02:02.157
<v SPEAKER_00>up from under 1% as recently as February.
32
00:02:05.776 --> 00:02:09.588
<v SPEAKER_00>In thinking about how big a deal it would be for AIs to automate AI research
33
00:02:09.638 --> 00:02:12.138
<v SPEAKER_00>and how much that would speed up AI progress,
34
00:02:12.279 --> 00:02:16.331
<v SPEAKER_00>a really important update for me has just been seeing how fast the capabilities
35
00:02:16.381 --> 00:02:18.902
<v SPEAKER_00>of AI models in mathematics have exploded.
36
00:02:19.522 --> 00:02:24.514
<v SPEAKER_00>Current AIs are slicing through well-scoped problems in maths like a hot knife through butter.
37
00:02:24.564 --> 00:02:28.690
<v SPEAKER_00>It was only two years ago that I asked Dario why LLMs aren't able
38
00:02:28.730 --> 00:02:32.736
<v SPEAKER_00>to use their vast knowledge across so many different fields in order
39
00:02:32.756 --> 00:02:36.145
<v SPEAKER_00>to connect together different ideas and make new discoveries.
40
00:02:36.542 --> 00:02:42.731
<v SPEAKER_00>And lo and behold, here we are in a wholly very Ais are doing the search
41
00:02:42.771 --> 00:02:47.157
<v SPEAKER_00>and match discovery to such a great extent that hundreds of important results,
42
00:02:47.318 --> 00:02:49.981
<v SPEAKER_00>which the top mathematicians and computer scientists
43
00:02:50.001 --> 00:02:54.448
<v SPEAKER_00>in the world had spent decades trying to resolve, are being churned out.
44
00:02:56.129 --> 00:02:59.712
<v SPEAKER_00>It's crazy how fast this progress has happened.
45
00:03:00.152 --> 00:03:04.319
<v SPEAKER_00>As recently as 2023, these models couldn't reliably add four-digit numbers.
46
00:03:04.536 --> 00:03:08.980
<v SPEAKER_00>In 2024, they could barely solve any problems in a high school math competition.
47
00:03:09.199 --> 00:03:13.199
<v SPEAKER_00>In 2025, they could win a gold medal in the International Math Olympiad.
48
00:03:13.482 --> 00:03:17.656
<v SPEAKER_00>To earlier this year, where they finally started to solve some niche open problems.
49
00:03:17.706 --> 00:03:23.210
<v SPEAKER_00>To a month ago, where OpenAI solved a Millennium Price problem in 88 hours.
50
00:03:24.031 --> 00:03:26.905
<v SPEAKER_00> I'm reminded of a line from the novel East of Eden.
51
00:03:26.955 --> 00:03:30.460
<v SPEAKER_00>Quote, And there is one sure thing about the fall of gods.
52
00:03:31.061 --> 00:03:32.473
<v SPEAKER_00>They do not fall a little.
53
00:03:32.523 --> 00:03:34.706
<v SPEAKER_00>They crash and shatter. End quote.
54
00:03:35.207 --> 00:03:38.485
<v SPEAKER_00>Now, it's true that progress has screwed disproportionately
55
00:03:39.029 --> 00:03:41.646
<v SPEAKER_00>Towards the verification -laden parts of mathematics,
56
00:03:41.646 --> 00:03:45.341
<v SPEAKER_00>like finding counterexamples rather than say coming up with new theory.
57
00:03:45.341 --> 00:03:48.117
<v SPEAKER_00>Toby Ort recently wrote a great essay about this he writes quote
58
00:03:48.117 --> 00:03:50.415
<v SPEAKER_00>while current AI systems are starting
59
00:03:50.415 --> 00:03:54.327
<v SPEAKER_00>to automate mathematical proof there is currently very little evidence
60
00:03:54.327 --> 00:03:58.781
<v SPEAKER_00>that they can ask powerful questions or find profound new fields
61
00:03:58.781 --> 00:04:00.588
<v SPEAKER_00>of mathematical inquiry, end quote.
62
00:04:00.588 --> 00:04:03.729
<v SPEAKER_00>But another way to say that same exact sentence would be this.
63
00:04:03.729 --> 00:04:09.387
<v SPEAKER_00>Current AI systems have solved a millennium -priced problem all without the ability
64
00:04:09.387 --> 00:04:14.055
<v SPEAKER_00>to ask powerful questions or found profound new field of mathematical enquiry
65
00:04:14.055 --> 00:04:18.061
<v SPEAKER_00>And this ability to solve well-scoped problems is going to be an even bigger deal
66
00:04:18.101 --> 00:04:22.601
<v SPEAKER_00>for machine learning research than it has been for mathematics broadly construed.
67
00:04:22.728 --> 00:04:26.143
<v SPEAKER_00>That's because the goal of mathematics research is not just to prove
68
00:04:26.193 --> 00:04:29.318
<v SPEAKER_00>or disprove long lists of conjectures, Rather,
69
00:04:29.598 --> 00:04:32.876
<v SPEAKER_00>to extend the human understanding of mathematical concepts.
70
00:04:33.464 --> 00:04:38.832
<v SPEAKER_00>Coming up with the idea of topology, or group theory, or going back even further,
71
00:04:38.852 --> 00:04:43.919
<v SPEAKER_00>the Cartesian grid, matters far more than knowing exactly how many
72
00:04:47.264 --> 00:04:51.370
<v SPEAKER_00>We mainly care about such abstruse questions insofar
73
00:04:51.530 --> 00:04:53.944
<v SPEAKER_00>as they might elicit new mathematical theory.
74
00:04:53.994 --> 00:04:57.579
<v SPEAKER_00>But in AI research, the priorities are exactly reversed.
75
00:05:01.420 --> 00:05:06.500
<v SPEAKER_00>Recipe empirically makes training more efficient or elicit smarter models.
76
00:05:06.640 --> 00:05:08.950
<v SPEAKER_00>They don't care about theory for its own sake,
77
00:05:09.000 --> 00:05:12.300
<v SPEAKER_00>and all the progress that we've made in deep learning over the last decade
78
00:05:12.300 --> 00:05:15.240
<v SPEAKER_00>and a half has not required much new theory anyways.
79
00:05:15.480 --> 00:05:17.540
<v SPEAKER_00>The equivalent of just grinding
80
00:05:17.540 --> 00:05:22.380
<v SPEAKER_00>through random conjectures would be enormously valuable in machine learning in a way
81
00:05:22.380 --> 00:05:23.880
<v SPEAKER_00>that it just isn't for mathematics.
82
00:05:23.880 --> 00:05:28.821
<v SPEAKER_00>AI research is actually surprisingly similar to The kind of mathematical progress
83
00:05:28.841 --> 00:05:31.515
<v SPEAKER_00>which current AIs are disproportionately good at,
84
00:05:31.565 --> 00:05:35.971
<v SPEAKER_00>which is unlocking a ton of low-hanging fruit by applying a combination
85
00:05:36.012 --> 00:05:40.899
<v SPEAKER_00>of incredible persistence and a superhuman capacity to connect ideas from lots
86
00:05:40.939 --> 00:05:44.531
<v SPEAKER_00>of adjacent domains. For example, let's talk about the transformer architecture.
87
00:05:44.581 --> 00:05:47.581
<v SPEAKER_00>This is the big breakthrough that enabled modern LLMs.
88
00:05:48.003 --> 00:05:51.175
<v SPEAKER_00>My friend Sholto Douglas, who is an AI researcher himself,
89
00:05:51.225 --> 00:05:53.726
<v SPEAKER_00>has this perennially half-finished blog post
90
00:05:53.766 --> 00:05:58.388
<v SPEAKER_00>where he explains how you could have invented the transformer two years earlier
91
00:05:58.448 --> 00:05:59.837
<v SPEAKER_00>than people actually did.
92
00:05:59.969 --> 00:06:03.925
<v SPEAKER_00>And maybe this video will finally get him to quit stalling and complete his essay.
93
00:06:03.975 --> 00:06:07.270
<v SPEAKER_00>But in the meantime, I'll summarize a bit of the discussion I had with him
94
00:06:07.320 --> 00:06:09.098
<v SPEAKER_00>about the contents of his essay.
95
00:06:09.283 --> 00:06:12.116
<v SPEAKER_00>Before the Transformer paper was published in 2017,
96
00:06:12.247 --> 00:06:15.311
<v SPEAKER_00>many researchers had already identified attention As a way
97
00:06:15.331 --> 00:06:19.844
<v SPEAKER_00>to better parallelize training and communicate information across longer sequences.
98
00:06:19.894 --> 00:06:25.237
<v SPEAKER_00>Chris Ola, who was an active researcher at the time, has said, quote, At that time,
99
00:06:25.597 --> 00:06:29.249
<v SPEAKER_00>my sense is that the transformer architecture was a natural combination
100
00:06:29.299 --> 00:06:32.141
<v SPEAKER_00>of many ideas like attention and residual networks,
101
00:06:32.521 --> 00:06:36.632
<v SPEAKER_00>which had independently been effective, taken to quite aggressive lengths,
102
00:06:36.743 --> 00:06:37.353
<v SPEAKER_00>end quote.
103
00:06:37.403 --> 00:06:41.596
<v SPEAKER_00>In other words, none of the core pieces were a surprise to researchers active in the field.
104
00:06:41.646 --> 00:06:44.257
<v SPEAKER_00>So then why didn't people invent the transformer sooner?
105
00:06:44.307 --> 00:06:48.029
<v SPEAKER_00>One reason was that this new architecture was only obviously better
106
00:06:48.111 --> 00:06:51.454
<v SPEAKER_00>than the state-of-the-art at the time once you connected together half
107
00:06:51.494 --> 00:06:53.406
<v SPEAKER_00>a dozen additional tweaks and innovations.
108
00:06:53.456 --> 00:06:56.990
<v SPEAKER_00>And though almost all of them had been known in the literature for years,
109
00:06:57.040 --> 00:07:01.014
<v SPEAKER_00>no one knew how to combine these puzzle pieces together in just the right way.
110
00:07:01.064 --> 00:07:03.842
<v SPEAKER_00>Doing so required great research taste, of course,
111
00:07:03.906 --> 00:07:07.017
<v SPEAKER_00>but it also required tons and tons of small experiments.
112
00:07:07.690 --> 00:07:09.321
<v SPEAKER_00>But what I've just described above,
113
00:07:09.371 --> 00:07:13.273
<v SPEAKER_00>which is persistently and intelligently matching dozens of different combinations
114
00:07:13.314 --> 00:07:16.215
<v SPEAKER_00>of ideas, is exactly the kind of capability
115
00:07:16.576 --> 00:07:20.648
<v SPEAKER_00>that AIs have shown themselves disproportionately skilled at in their contributions
116
00:07:20.698 --> 00:07:21.698
<v SPEAKER_00>in mathematics.
117
00:07:21.839 --> 00:07:24.290
<v SPEAKER_00>This is all to say that even the Transformer,
118
00:07:24.340 --> 00:07:27.802
<v SPEAKER_00>which is arguably the biggest breakthrough in ML since AlexNet kicked off
119
00:07:27.822 --> 00:07:29.878
<v SPEAKER_00>the deep learning revolution in 2012,
120
00:07:29.944 --> 00:07:33.756
<v SPEAKER_00>is the kind of thing that Cloud7 could have invented if Chris Ola asked
121
00:07:33.806 --> 00:07:37.250
<v SPEAKER_00>to try really hard to get this attention thing to work better.
122
00:07:37.407 --> 00:07:42.463
<v SPEAKER_00> Now, I wanna clarify that some parts of AI research are in fact less verifiable than math.
123
00:07:42.795 --> 00:07:45.795
<v SPEAKER_00>That's why OpenAI hasn't fired all of its researchers,
124
00:07:45.959 --> 00:07:46.981
<v SPEAKER_00>despite having a model
125
00:07:47.021 --> 00:07:50.576
<v SPEAKER_00>that can apparently autonomously solve Millennium Prize problems.
126
00:07:50.626 --> 00:07:55.953
<v SPEAKER_00>But I think that AI research is verifiable Now,
127
00:07:56.154 --> 00:08:00.500
<v SPEAKER_00>explaining why requires getting into the nitty-gritty
128
00:08:00.740 --> 00:08:02.703
<v SPEAKER_00>of how AI research actually works.
129
00:08:03.324 --> 00:08:06.435
<v SPEAKER_00>And because those details are interesting but technical,
130
00:08:06.769 --> 00:08:10.314
<v SPEAKER_00>I've saved them So if you're curious and you want to hear them,
131
00:08:10.575 --> 00:08:13.449
<v SPEAKER_00>you should just keep watching until the end of the video.
132
00:08:13.499 --> 00:08:18.496
<v SPEAKER_00>But in the meantime, I'm going to give you my estimate of when we're going to have such AIs.
133
00:08:18.546 --> 00:08:22.619
<v SPEAKER_00>If I had to pick my median year for when automated researchers will be as good
134
00:08:22.619 --> 00:08:28.525
<v SPEAKER_00>as the very best human AI researchers at doing AI research, I'd guess 2028.
135
00:08:28.525 --> 00:08:31.643
<v SPEAKER_00>And that's assuming that the AI labs go full steam ahead
136
00:08:31.643 --> 00:08:36.206
<v SPEAKER_00>and don't slow themselves down intentionally or aren't slowed down by a government.
137
00:08:36.206 --> 00:08:41.380
<v SPEAKER_00>Why do I think that AIs could get this good within every domain
138
00:08:41.440 --> 00:08:45.075
<v SPEAKER_00>where we can check answers and give AIs thousands of rounds of practice,
139
00:08:45.125 --> 00:08:49.569
<v SPEAKER_00>for example, competitive programming contests or well-scoped open math problems,
140
00:08:49.812 --> 00:08:52.336
<v SPEAKER_00>they've gone from worse than most humans
141
00:08:52.336 --> 00:08:58.445
<v SPEAKER_00>And as I'll argue after the conclusion,
142
00:08:59.136 --> 00:09:02.351
<v SPEAKER_00>AI research has exactly the same verifiable properties.
143
00:09:02.912 --> 00:09:06.357
<v SPEAKER_00>Of course, a big part of what makes the top human AI researchers really good
144
00:09:06.377 --> 00:09:08.500
<v SPEAKER_00>at their job can't be directly verified.
145
00:09:08.500 --> 00:09:09.946
<v SPEAKER_00>Trained on.
146
00:09:11.306 --> 00:09:16.661
<v SPEAKER_00>OpenAI's model was obviously not trained
147
00:09:16.661 --> 00:09:22.137
<v SPEAKER_00>by solving other Millennium Prize problems.
148
00:09:22.860 --> 00:09:28.541
<v SPEAKER_00> It was trained on lots of less ambitious, more tractable math problems.
149
00:09:29.121 --> 00:09:32.622
<v SPEAKER_00>And from those, it generalized all the way to solving a problem
150
00:09:32.902 --> 00:09:35.069
<v SPEAKER_00>which no human had ever cracked before.
151
00:09:35.262 --> 00:09:37.093
<v SPEAKER_00>I'd expect the same in AI research,
152
00:09:37.143 --> 00:09:39.533
<v SPEAKER_00>where the combination of thousands of rounds of practice
153
00:09:39.583 --> 00:09:41.194
<v SPEAKER_00>on verifiable research tasks,
154
00:09:41.503 --> 00:09:46.059
<v SPEAKER_00>plus the fact that each new generation of models is broadly smarter than the last,
155
00:09:46.344 --> 00:09:49.455
<v SPEAKER_00>will make models excellent even at the parts of AI research
156
00:09:49.505 --> 00:09:51.116
<v SPEAKER_00>that we can't directly check.
157
00:09:51.425 --> 00:09:54.119
<v SPEAKER_00>Now, I want to be clear that there's a pretty decent chance
158
00:09:54.169 --> 00:09:58.135
<v SPEAKER_00>that hitting this milestone takes longer because some important parts
159
00:09:58.155 --> 00:10:00.322
<v SPEAKER_00>of AI research remain hard to automate.
160
00:10:00.679 --> 00:10:04.012
<v SPEAKER_00>This is just a very hard thing to try to predict in advance,
161
00:10:04.104 --> 00:10:07.639
<v SPEAKER_00>and I'd guess that there's at least a 25% chance That it doesn't happen
162
00:10:07.689 --> 00:10:09.332
<v SPEAKER_00>until after 2032.
163
00:10:09.852 --> 00:10:13.167
<v SPEAKER_00>But conversely, I also think that things could happen much faster
164
00:10:13.217 --> 00:10:15.160
<v SPEAKER_00>and we hit this milestone in 2027.
165
00:10:15.641 --> 00:10:18.075
<v SPEAKER_00>Some of the most well-informed researchers I know,
166
00:10:18.125 --> 00:10:20.788
<v SPEAKER_00>people who have a very good track record of making predictions
167
00:10:20.829 --> 00:10:26.576
<v SPEAKER_00>over the last Expect AIs to beat the best humans at AI research as early
168
00:10:26.676 --> 00:10:27.676
<v SPEAKER_00>as next year.
169
00:10:27.917 --> 00:10:32.823
<v SPEAKER_00>And 2027 is also the straightforward implication of putting the new report for Meter
170
00:10:33.224 --> 00:10:37.178
<v SPEAKER_00>that says that Anthropics' rate of AI progress has doubled from a year ago
171
00:10:37.228 --> 00:10:38.506
<v SPEAKER_00>into a take-offs model.
172
00:10:38.870 --> 00:10:43.005
<v SPEAKER_00>As former guest Ajay Khotra put it in a blog post about this report, quote,
173
00:10:43.055 --> 00:10:46.840
<v SPEAKER_00>if we take at face value that AI is now nearly doubling the rate
174
00:10:46.920 --> 00:10:51.087
<v SPEAKER_00>of AI capabilities progress and assume that acceleration from AI is smooth,
175
00:10:51.325 --> 00:10:55.825
<v SPEAKER_00>this naively implies that we would reach extreme superintelligence within a year,
176
00:10:56.171 --> 00:11:00.997
<v SPEAKER_00>end quote. So the reason my median year is not 2027 is just that I'm uncertain
177
00:11:01.037 --> 00:11:03.610
<v SPEAKER_00>about how accurate this kind of straightforward modeling is.
178
00:11:03.660 --> 00:11:07.625
<v SPEAKER_00>But we should not be surprised and we should be ready for a world in which we get
179
00:11:07.645 --> 00:11:09.367
<v SPEAKER_00>to this milestone next year.
180
00:11:14.209 --> 00:11:17.995
<v SPEAKER_00>Once AI is as good as the best humans at AI research,
181
00:11:18.536 --> 00:11:22.480
<v SPEAKER_00>algorithmic progress will get a lot faster for three important reasons.
182
00:11:22.902 --> 00:11:24.735
<v SPEAKER_00>One, the AIs will be much faster.
183
00:11:24.785 --> 00:11:26.841
<v SPEAKER_00>Two, each of them will be very smart.
184
00:11:26.908 --> 00:11:29.021
<v SPEAKER_00>And three, there will be a lot more of them.
185
00:11:29.071 --> 00:11:30.263
<v SPEAKER_00>Let's start with faster first.
186
00:11:30.313 --> 00:11:33.978
<v SPEAKER_00>Today's AIs already do work at about 10 times human speed,
187
00:11:34.399 --> 00:11:37.333
<v SPEAKER_00>and automated researchers would also be working around the clock,
188
00:11:37.383 --> 00:11:39.716
<v SPEAKER_00>nights and weekends included. As a result,
189
00:11:39.947 --> 00:11:44.060
<v SPEAKER_00>each individual automated researcher will be cramming roughly 50 times more work
190
00:11:44.110 --> 00:11:46.796
<v SPEAKER_00>Every calendar week than a human researcher can do.
191
00:11:46.796 --> 00:11:51.777
<v SPEAKER_00>Of course, that doesn't mean AI progress will immediately accelerate 50x.
192
00:11:51.777 --> 00:11:55.981
<v SPEAKER_00>Those automated researchers would still be bottlenecked by compute for experiments
193
00:11:55.981 --> 00:12:00.490
<v SPEAKER_00>which aren't running any faster so there There would be diminishing returns but even
194
00:12:00.490 --> 00:12:04.870
<v SPEAKER_00>with extremely steep diminishing returns this alone would make algorithmic progress
195
00:12:04.870 --> 00:12:09.730
<v SPEAKER_00>proceed many times faster than it And this is before we come for the fact
196
00:12:09.730 --> 00:12:11.897
<v SPEAKER_00>that in the scenario I'm talking about,
197
00:12:12.130 --> 00:12:16.570
<v SPEAKER_00>every automated researcher will be at least as good at AI research and engineering
198
00:12:16.570 --> 00:12:18.630
<v SPEAKER_00>as the very best humans today.
199
00:12:19.350 --> 00:12:21.828
<v SPEAKER_00>My sense is that around 80% of the algorithmic progress
200
00:12:21.878 --> 00:12:25.220
<v SPEAKER_00>at a given frontier lab is driven by its 50 top researchers.
201
00:12:25.640 --> 00:12:28.882
<v SPEAKER_00>It's not for nothing that Zuckerberg was willing to pay hundreds of millions
202
00:12:28.922 --> 00:12:31.894
<v SPEAKER_00>of dollars to acquire the best talent in the industry.
203
00:12:31.944 --> 00:12:35.327
<v SPEAKER_00>And so you get another big speedup in algorithmic progress from the fact
204
00:12:35.367 --> 00:12:39.534
<v SPEAKER_00>that every single engineer and researcher in this automated company will be
205
00:12:39.629 --> 00:12:43.452
<v SPEAKER_00>at the level of the very best humans in today's frontier AI labs.
206
00:12:44.112 --> 00:12:47.286
<v SPEAKER_00> And finally, there will be a lot more automated researchers.
207
00:12:47.336 --> 00:12:50.509
<v SPEAKER_00>Now, throwing more workers at a problem isn't always helpful.
208
00:12:50.559 --> 00:12:53.722
<v SPEAKER_00>For example, a swarm of agents probably isn't going to be able to write
209
00:12:53.762 --> 00:12:56.745
<v SPEAKER_00>a great novel much faster than a single agent could.
210
00:12:57.225 --> 00:13:00.379
<v SPEAKER_00>But other tasks lend themselves much more to parallelization.
211
00:13:00.429 --> 00:13:02.461
<v SPEAKER_00>For example, look at this animation that I'm overlaying,
212
00:13:02.511 --> 00:13:05.567
<v SPEAKER_00>which shows a bunch of different clods working together
213
00:13:05.714 --> 00:13:07.658
<v SPEAKER_00>to formalize Fermat's last theorem.
214
00:13:08.117 --> 00:13:11.021
<v SPEAKER_00>This feat had thousands of modular subtasks,
215
00:13:11.361 --> 00:13:13.274
<v SPEAKER_00>each of which could be completed independently
216
00:13:13.324 --> 00:13:17.435
<v SPEAKER_00>and where each agent could locally check whether their work had succeeded.
217
00:13:17.510 --> 00:13:21.666
<v SPEAKER_00>AI research is closer to formalizing a theorem than it is to writing a novel
218
00:13:21.716 --> 00:13:24.689
<v SPEAKER_00>because there's a lot There's a lot of independent modular work to do,
219
00:13:24.739 --> 00:13:27.270
<v SPEAKER_00>and there are verifiable proxies for progress.
220
00:13:27.320 --> 00:13:31.422
<v SPEAKER_00>That means a swarm of agents can try out a thousand different approaches and see
221
00:13:31.462 --> 00:13:35.284
<v SPEAKER_00>which one performs best, and they can do this independently for each different part
222
00:13:35.304 --> 00:13:36.295
<v SPEAKER_00>of the pipeline.
223
00:13:36.345 --> 00:13:41.007
<v SPEAKER_00>AI companies are already made up of dozens of different teams working independently
224
00:13:41.368 --> 00:13:43.590
<v SPEAKER_00>on different parts of model development.
225
00:13:43.689 --> 00:13:46.560
<v SPEAKER_00>One team, for example, improves how the pre-training data is filtered.
226
00:13:46.610 --> 00:13:49.382
<v SPEAKER_00>Another designs a particular kind of synthetic RL environment.
227
00:13:49.432 --> 00:13:52.321
<v SPEAKER_00>Another writes a better attention kernel, and so on.
228
00:13:52.393 --> 00:13:55.748
<v SPEAKER_00>In domains like this, where different streams of work can be done
229
00:13:55.798 --> 00:14:00.606
<v SPEAKER_00>and checked independently, dumping in lots of persistent hill-climbing agents tends
230
00:14:00.626 --> 00:14:02.126
<v SPEAKER_00>to speed up progress a lot.
231
00:14:02.188 --> 00:14:07.005
<v SPEAKER_00>Again, there will be steeply diminishing returns just from adding more parallel researchers.
232
00:14:07.055 --> 00:14:08.396
<v SPEAKER_00>Anyone who's ever worked in the team before knows
233
00:14:08.416 --> 00:14:13.027
<v SPEAKER_00>that having 100,000 collaborators doesn't mean that you'll go 100,000 times faster,
234
00:14:13.318 --> 00:14:15.149
<v SPEAKER_00>probably not even 100 times faster.
235
00:14:15.199 --> 00:14:17.089
<v SPEAKER_00>But given the nature of AI research,
236
00:14:17.139 --> 00:14:20.631
<v SPEAKER_00>it's implausible that you wouldn't be going at least a couple times faster
237
00:14:20.681 --> 00:14:23.625
<v SPEAKER_00>from having orders of magnitude more automated labor.
238
00:14:27.432 --> 00:14:30.193
<v SPEAKER_00>So the combination of faster, smarter,
239
00:14:30.353 --> 00:14:33.914
<v SPEAKER_00>and more automated researchers will speed up AI progress a lot.
240
00:14:34.495 --> 00:14:36.051
<v SPEAKER_00>But will this pace continue?
241
00:14:36.175 --> 00:14:37.508
<v SPEAKER_00>Will it get even faster?
242
00:14:37.756 --> 00:14:38.923
<v SPEAKER_00>Or will it slow down?
243
00:14:39.236 --> 00:14:43.408
<v SPEAKER_00>That question is even more important than what the initial pace actually is.
244
00:14:43.458 --> 00:14:45.069
<v SPEAKER_00>Two competing trends are relevant here,
245
00:14:45.119 --> 00:14:47.897
<v SPEAKER_00>and the subsequent rate of progress will come down
246
00:14:47.960 --> 00:14:50.238
<v SPEAKER_00>to which one ends up being more powerful.
247
00:14:50.321 --> 00:14:54.102
<v SPEAKER_00>On the one hand, because of RSI, automated researchers will
248
00:14:57.300 --> 00:15:00.573
<v SPEAKER_00>On the other hand, AI research will be getting harder and harder as all
249
00:15:00.573 --> 00:15:02.962
<v SPEAKER_00>the easy ideas get eaten away by the swarm.
250
00:15:03.490 --> 00:15:07.540
<v SPEAKER_00>By the way, ideas getting harder to find is a thing that already happens.
251
00:15:07.590 --> 00:15:09.850
<v SPEAKER_00>AI companies have to quadruple their R &D compute
252
00:15:09.850 --> 00:15:13.710
<v SPEAKER_00>and double their workforce every single year just to maintain the same rate
253
00:15:13.710 --> 00:15:14.710
<v SPEAKER_00>of progress.
254
00:15:15.050 --> 00:15:18.160
<v SPEAKER_00>So if the rate at which AI gets smarter is faster than the rate
255
00:15:18.180 --> 00:15:20.069
<v SPEAKER_00>at which ideas get harder to find,
256
00:15:20.243 --> 00:15:23.632
<v SPEAKER_00>then we'd get something called the software-only singularity.
257
00:15:23.769 --> 00:15:26.547
<v SPEAKER_00>In this scenario, even without increasing compute,
258
00:15:26.653 --> 00:15:29.457
<v SPEAKER_00>the AI swarm rapidly makes smarter and smarter versions
259
00:15:29.497 --> 00:15:34.559
<v SPEAKER_00>of But if ideas
260
00:15:34.659 --> 00:15:38.101
<v SPEAKER_00>get harder
261
00:15:38.121 --> 00:15:41.142
<v SPEAKER_00>to find faster than RSI makes AIs better at research,
262
00:15:41.562 --> 00:15:44.340
<v SPEAKER_00>we'd end up with something which I'd call a spark.
263
00:15:44.423 --> 00:15:48.195
<v SPEAKER_00>We'd get something like three to six years of AI progress at the current rate
264
00:15:48.245 --> 00:15:49.689
<v SPEAKER_00>in a single calendar year.
265
00:15:50.065 --> 00:15:53.017
<v SPEAKER_00>And then things would simmer down until we build more compute
266
00:15:53.067 --> 00:15:56.918
<v SPEAKER_00>as even these super genius automated researchers need to run bigger experiments
267
00:15:56.968 --> 00:15:58.999
<v SPEAKER_00>before they can make further breakthroughs.
268
00:15:59.049 --> 00:16:03.023
<v SPEAKER_00>As to which one will actually happen, I think it's basically a coin toss.
269
00:16:03.073 --> 00:16:08.057
<v SPEAKER_00>If pressed, I'd give a 50% chance to the Spark scenario and a 50% chance
270
00:16:08.378 --> 00:16:09.989
<v SPEAKER_00>to the software-only singularity.
271
00:16:10.039 --> 00:16:12.371
<v SPEAKER_00>But to be clear, even in the Spark scenario,
272
00:16:12.421 --> 00:16:15.935
<v SPEAKER_00>where we make something like four years of progress in the first calendar year
273
00:16:15.985 --> 00:16:19.569
<v SPEAKER_00>after we automate AI research, Things would feel insane.
274
00:16:20.030 --> 00:16:25.878
<v SPEAKER_00>There's a jump as big as GPT-3.5 to GPT-6 Astra in just 12 months.
275
00:16:26.359 --> 00:16:30.192
<v SPEAKER_00>To remind you of the scale of progress that this leap would compress,
276
00:16:30.575 --> 00:16:34.265
<v SPEAKER_00>GPT-3.5 was able to ride a passable limerick and autocomplete
277
00:16:34.265 --> 00:16:37.529
<v SPEAKER_00>a trivial Python function, but otherwise it was mostly a useless toy.
278
00:16:37.529 --> 00:16:41.698
<v SPEAKER_00>Whereas Astar can build whole video games from scratch and churns out
279
00:16:41.698 --> 00:16:44.246
<v SPEAKER_00>so many Fields Medal -worthy mathematical contributions
280
00:16:44.246 --> 00:16:46.647
<v SPEAKER_00>that we become totally desensitized.
281
00:16:46.647 --> 00:16:51.112
<v SPEAKER_00>In the last four years, We've gone from a preschooler to a savant intern.
282
00:16:51.452 --> 00:16:56.394
<v SPEAKER_00>If you made another jump that big, but starting in 2027 or 2028,
283
00:16:56.814 --> 00:17:00.696
<v SPEAKER_00>you'd probably get a mine which would be vastly superhuman in domains
284
00:17:00.916 --> 00:17:02.805
<v SPEAKER_00>that are even slightly verifiable.
285
00:17:02.917 --> 00:17:06.309
<v SPEAKER_00>For example, it'd be better than Nvidia at coming up with the next generation
286
00:17:06.359 --> 00:17:07.439
<v SPEAKER_00>of AI accelerators.
287
00:17:07.459 --> 00:17:11.731
<v SPEAKER_00>It would make more money than the current human versions of Citadel and Jane Street
288
00:17:11.781 --> 00:17:13.812
<v SPEAKER_00>if it was given equal access to the market.
289
00:17:13.862 --> 00:17:16.995
<v SPEAKER_00>If you give it remote access through a material science experiment lab,
290
00:17:17.045 --> 00:17:19.007
<v SPEAKER_00>it'd be better than the rest of humanity at finding
291
00:17:19.047 --> 00:17:20.936
<v SPEAKER_00>a room temperature superconductor.
292
00:17:24.291 --> 00:17:27.804
<v SPEAKER_00>Now, at this point, you might say, how will even superintelligence,
293
00:17:27.854 --> 00:17:29.406
<v SPEAKER_00>which is trained in a data center,
294
00:17:29.456 --> 00:17:34.460
<v SPEAKER_00>beat human experts in domains where the basis of that human expertise is years
295
00:17:34.500 --> 00:17:36.602
<v SPEAKER_00>and years of real world experience?
296
00:17:37.062 --> 00:17:41.360
<v SPEAKER_00>The way we're currently making AI smarter is by RL -ing them on tasks that are easy
297
00:17:41.360 --> 00:17:44.082
<v SPEAKER_00>to automatically grade from within a data center.
298
00:17:44.140 --> 00:17:47.510
<v SPEAKER_00>For example, did the million new lines of code that the AI wrote pass to pass all
299
00:17:47.510 --> 00:17:54.194
<v SPEAKER_00>the unit tests? Did the AI to get really good at building a business from scratch?
300
00:17:54.194 --> 00:17:56.934
<v SPEAKER_00>How about winning court cases,
301
00:17:56.934 --> 00:18:01.613
<v SPEAKER_00>or having a profitable day of trading in the markets,
302
00:18:01.613 --> 00:18:05.281
<v SPEAKER_00>or helping a candidate win an election?
303
00:18:05.281 --> 00:18:08.316
<v SPEAKER_00>The rollout here requires interacting with the real world,
304
00:18:08.366 --> 00:18:11.641
<v SPEAKER_00>and you can't recreate it from just within the data center.
305
00:18:11.691 --> 00:18:14.585
<v SPEAKER_00>So how will superintelligence get good at this kind of stuff?
306
00:18:14.635 --> 00:18:15.827
<v SPEAKER_00>Well, let me be clear.
307
00:18:15.877 --> 00:18:20.599
<v SPEAKER_00>I don't think we can just bake the answer to every real world problem into the waste.
308
00:18:20.843 --> 00:18:24.864
<v SPEAKER_00>Rather, my claim is that scaling up RL training will give AIs
309
00:18:25.104 --> 00:18:29.065
<v SPEAKER_00>the abilities necessary to ramp up quickly in new contexts,
310
00:18:29.405 --> 00:18:32.476
<v SPEAKER_00>even in hard-to-verify domains like the ones mentioned above.
311
00:18:32.526 --> 00:18:35.859
<v SPEAKER_00>Getting really good at any complex task requires two things.
312
00:18:36.307 --> 00:18:40.751
<v SPEAKER_00>One is domain-specific knowledge, and the other is a more general set of skills,
313
00:18:41.028 --> 00:18:44.009
<v SPEAKER_00>the kind of capabilities that capable humans have.
314
00:18:44.569 --> 00:18:48.013
<v SPEAKER_00>Like being able to seek out relevant information, make a plan,
315
00:18:48.134 --> 00:18:51.009
<v SPEAKER_00>push forward on that plan through mistakes and obstacles,
316
00:18:51.059 --> 00:18:54.414
<v SPEAKER_00>keep track of what you've learned, and collaborate with other people.
317
00:18:54.464 --> 00:18:58.269
<v SPEAKER_00>During RSI, automated engineers will build tens of thousands
318
00:18:58.309 --> 00:19:01.087
<v SPEAKER_00>of times more environments than we have currently.
319
00:19:01.230 --> 00:19:05.050
<v SPEAKER_00>And these will be Far larger and longer running and higher quality
320
00:19:05.050 --> 00:19:09.550
<v SPEAKER_00>and more open -ended and covering a much wider range than today's
321
00:19:09.550 --> 00:19:14.200
<v SPEAKER_00>in The AIs will learn to make their way through unfathomable amounts
322
00:19:14.200 --> 00:19:17.706
<v SPEAKER_00>of virtual worlds that are each, to today's video games,
323
00:19:17.706 --> 00:19:19.702
<v SPEAKER_00>what a Bugatti is to a horse and buggy.
324
00:19:19.702 --> 00:19:24.213
<v SPEAKER_00>These games will be far more difficult and messy and sprawling and realistic
325
00:19:24.213 --> 00:19:26.936
<v SPEAKER_00>than anything that has ever been made for human entertainment.
326
00:19:26.936 --> 00:19:32.418
<v SPEAKER_00>They will require AIs to cooperate or compete with teams of other AIs
327
00:19:32.418 --> 00:19:33.639
<v SPEAKER_00>over long periods of time.
328
00:19:33.639 --> 00:19:37.110
<v SPEAKER_00>For example, an AI might be dropped into a simulated economy of millions
329
00:19:37.110 --> 00:19:39.035
<v SPEAKER_00>of other AIs and told to co -found a successful company.
330
00:19:39.035 --> 00:19:42.300
<v SPEAKER_00>And it's not like the AI will be stuck just thinking
331
00:19:42.300 --> 00:19:43.770
<v SPEAKER_00>about the ideal corporate structure.
332
00:19:43.820 --> 00:19:46.920
<v SPEAKER_00>It'll go through an evolutionary process that involves centuries
333
00:19:46.920 --> 00:19:51.198
<v SPEAKER_00>of corporate competition to figure out the optimal organizational techniques.
334
00:19:51.552 --> 00:19:56.056
<v SPEAKER_00>The AIs will also train themselves on endless backtests of everything in the history
335
00:19:56.076 --> 00:19:58.918
<v SPEAKER_00>of science and tech and politics and culture.
336
00:19:59.359 --> 00:20:05.284
<v SPEAKER_00>Every discovery, invention, war, election, and quarterly earning that has ever happened.
337
00:20:05.544 --> 00:20:07.836
<v SPEAKER_00>For example, here's one prediction training task.
338
00:20:07.886 --> 00:20:11.038
<v SPEAKER_00>Can the AI figure out general relativity given a training corpus
339
00:20:11.088 --> 00:20:14.011
<v SPEAKER_00>that includes no information beyond 1700,
340
00:20:14.131 --> 00:20:17.687
<v SPEAKER_00>which is far earlier than any human was on track to discover GR?
341
00:20:18.054 --> 00:20:22.476
<v SPEAKER_00>Another task might be, given every single newspaper article until 1962,
342
00:20:22.836 --> 00:20:25.827
<v SPEAKER_00>can AI predict how the Cuban Missile Crisis is going to unfold?
343
00:20:25.877 --> 00:20:29.308
<v SPEAKER_00>And it's not just the training data that these automated researchers will be improving.
344
00:20:29.358 --> 00:20:33.110
<v SPEAKER_00>They will also radically improve the basic learning algorithms themselves
345
00:20:33.160 --> 00:20:36.660
<v SPEAKER_00>through breakthroughs in online learning and sample efficiency,
346
00:20:36.741 --> 00:20:39.912
<v SPEAKER_00>both of which have verifiable proxies, as I'll discuss later.
347
00:20:39.962 --> 00:20:44.724
<v SPEAKER_00>In the same way that humans are much more efficient and effective at learning
348
00:20:44.764 --> 00:20:46.625
<v SPEAKER_00>from data than current LLMs are,
349
00:20:47.025 --> 00:20:51.672
<v SPEAKER_00>Future AIs could be far beyond humans at their learning efficiency.
350
00:20:52.032 --> 00:20:55.708
<v SPEAKER_00>Now, why do I think we'll see lots of transfer from verifiable tasks
351
00:20:55.758 --> 00:20:57.369
<v SPEAKER_00>to these more general skills?
352
00:20:57.501 --> 00:21:02.350
<v SPEAKER_00>Well, one reason is that even at one ten thousandth or a millionth of The scale
353
00:21:02.350 --> 00:21:05.716
<v SPEAKER_00>of RL training that will be happening during the intelligence explosion,
354
00:21:05.716 --> 00:21:08.289
<v SPEAKER_00>we're already seeing lots of generalization.
355
00:21:08.289 --> 00:21:11.960
<v SPEAKER_00>If you point clot code or codex at a project that it's never seen before,
356
00:21:11.960 --> 00:21:15.062
<v SPEAKER_00>it knows how to orient itself and figure out how everything fits together
357
00:21:15.062 --> 00:21:17.084
<v SPEAKER_00>and then tackle an ambitious assignment.
358
00:21:17.084 --> 00:21:20.015
<v SPEAKER_00>Of course, it's hard to measure how much models have improved at tasks
359
00:21:20.015 --> 00:21:24.320
<v SPEAKER_00>that are not easily verifiable because if we could, those tasks would be verifiable.
360
00:21:24.320 --> 00:21:27.950
<v SPEAKER_00>But you can just go talk to a new model and compare it to an old one.
361
00:21:27.971 --> 00:21:32.243
<v SPEAKER_00>In my experience, AIs have gotten much better at things that have very little to do
362
00:21:32.243 --> 00:21:33.706
<v SPEAKER_00>with code or math.
363
00:21:33.706 --> 00:21:37.723
<v SPEAKER_00>For example, helping me research the abstract questions I needed to answer
364
00:21:37.723 --> 00:21:39.140
<v SPEAKER_00>while writing this essay.
365
00:21:39.140 --> 00:21:42.576
<v SPEAKER_00>The other big piece of evidence for transfer is human evolution.
366
00:21:42.576 --> 00:21:46.008
<v SPEAKER_00> Our general purpose mental architecture was developed by evolution.
367
00:21:46.058 --> 00:21:49.947
<v SPEAKER_00>And evolution is an optimization process with a really crude verifier.
368
00:21:50.221 --> 00:21:51.942
<v SPEAKER_00>Did your genes pass on or not?
369
00:21:52.463 --> 00:21:53.833
<v SPEAKER_00>In the ancestral environment,
370
00:21:53.883 --> 00:21:57.439
<v SPEAKER_00>the tasks which influenced that outcome were things like hunting
371
00:21:57.506 --> 00:22:01.173
<v SPEAKER_00>and fending off predators and keeping your standing in your tribe.
372
00:22:01.229 --> 00:22:06.007
<v SPEAKER_00> These are our tiny subset of the kinds of tasks that humans are able to tackle today.
373
00:22:06.195 --> 00:22:09.048
<v SPEAKER_00>Evolution did not specifically optimize us to be able to write
374
00:22:09.098 --> 00:22:12.876
<v SPEAKER_00>a Pulitzer Prize winning biography, or make advanced semiconductors,
375
00:22:13.002 --> 00:22:17.257
<v SPEAKER_00>or lead nations of millions of people, or come up with a new branch of mathematics.
376
00:22:17.307 --> 00:22:22.913
<v SPEAKER_00>But in optimizing us for survival on the Savannah, evolution built a general purpose learner.
377
00:22:23.694 --> 00:22:26.348
<v SPEAKER_00>And in training these AIs, we're running a similar process,
378
00:22:26.398 --> 00:22:30.884
<v SPEAKER_00>except we're doing so deliberately with tasks that are much more closely related
379
00:22:31.285 --> 00:22:34.452
<v SPEAKER_00>to the ones that are needed for success in today's world.
380
00:22:34.550 --> 00:22:39.700
<v SPEAKER_00> And unlike evolution, AI companies are trying to improve transfer during training.
381
00:22:39.900 --> 00:22:43.200
<v SPEAKER_00>For example, by making sure that performance improves on difficult tasks
382
00:22:43.200 --> 00:22:44.791
<v SPEAKER_00>that were held out of trading.
383
00:22:44.791 --> 00:22:49.741
<v SPEAKER_00>If even dumb, blind evolution can get this much transfer out of building a mind
384
00:22:49.741 --> 00:22:54.269
<v SPEAKER_00>that is effective at propagating itself in the savannah then the deliberate effort
385
00:22:54.319 --> 00:22:58.475
<v SPEAKER_00>that AI companies are putting into building a flexible and general intelligence
386
00:22:58.525 --> 00:23:02.551
<v SPEAKER_00>that can rapidly ramp up in new contexts should advance much further.
387
00:23:02.891 --> 00:23:06.770
<v SPEAKER_00>Now, even a super intelligent learner can't figure out everything from inside
388
00:23:06.820 --> 00:23:12.153
<v SPEAKER_00>So even these AIs would need some real -world experience before they can beat
389
00:23:12.153 --> 00:23:12.768
<v SPEAKER_00>the best humans.
390
00:23:12.768 --> 00:23:16.064
<v SPEAKER_00>But I think they'll be able to get that experience much faster than people expect,
391
00:23:16.064 --> 00:23:19.842
<v SPEAKER_00>and that they'll will be able top human experts within months of being deployed.
392
00:23:19.842 --> 00:23:22.607
<v SPEAKER_00>And honestly, one of the things that's guiding my intuition here is that I have
393
00:23:22.607 --> 00:23:26.840
<v SPEAKER_00>a lot of 20 something year old friends who I've watched accomplish incredible things
394
00:23:26.840 --> 00:23:30.973
<v SPEAKER_00>and build world -leading companies and ventures in domains that they entered
395
00:23:30.973 --> 00:23:33.649
<v SPEAKER_00>into with basically zero years of experience.
396
00:23:33.649 --> 00:23:37.989
<v SPEAKER_00>History is full of super competent young people who ran circles around the world
397
00:23:37.989 --> 00:23:39.084
<v SPEAKER_00>that they found themselves in.
398
00:23:39.084 --> 00:23:42.489
<v SPEAKER_00>By the age of 27, Napoleon had stacked victory after victory
399
00:23:42.609 --> 00:23:46.165
<v SPEAKER_00>against far larger armies from the other great powers of Europe.
400
00:23:46.235 --> 00:23:49.459
<v SPEAKER_00>By 25, just two years after he got into the oil business,
401
00:23:49.940 --> 00:23:53.335
<v SPEAKER_00>Rockefeller was running one of the world's largest refineries.
402
00:23:53.385 --> 00:23:58.893
<v SPEAKER_00> Rockefeller and Napoleon needed experience, yes, but only a couple years worth, not decades.
403
00:23:59.274 --> 00:24:02.028
<v SPEAKER_00>And whatever was going on inside these guys' brains,
404
00:24:02.078 --> 00:24:04.856
<v SPEAKER_00>an AI should be able to replicate, or even exceed.
405
00:24:05.183 --> 00:24:10.230
<v SPEAKER_00>There's no reason to think that humans are at the ceiling of learning Furthermore,
406
00:24:10.630 --> 00:24:12.352
<v SPEAKER_00>unlike Napoleon or Rockefeller,
407
00:24:12.533 --> 00:24:16.098
<v SPEAKER_00>AI is going to accumulate years of deployed context in just a few days
408
00:24:16.138 --> 00:24:20.204
<v SPEAKER_00>of calendar time. For example, imagine that you wanted these future AIs to run
409
00:24:20.224 --> 00:24:23.002
<v SPEAKER_00>a Fortune 500 company better than its current CEO.
410
00:24:23.228 --> 00:24:25.361
<v SPEAKER_00> How quickly could the AI ramp up at this job?
411
00:24:25.411 --> 00:24:28.326
<v SPEAKER_00>Well, if you let it shadow that CEO, on its first morning,
412
00:24:28.376 --> 00:24:31.487
<v SPEAKER_00>it could read every email and Slack message and document
413
00:24:31.580 --> 00:24:33.113
<v SPEAKER_00>that the company has ever produced.
414
00:24:33.163 --> 00:24:34.535
<v SPEAKER_00>By the end of its first day,
415
00:24:34.585 --> 00:24:38.680
<v SPEAKER_00>copies of it have interviewed every employee and major client in parallel.
416
00:24:38.730 --> 00:24:42.123
<v SPEAKER_00>Obviously, they wouldn't have access to feedback that arrives after many months of serial time.
417
00:24:42.173 --> 00:24:45.617
<v SPEAKER_00>For example, how well they did on the next quarterly earnings.
418
00:24:45.995 --> 00:24:48.328
<v SPEAKER_00>But even given these kinds of bottlenecks,
419
00:24:48.577 --> 00:24:52.259
<v SPEAKER_00>we should expect these future post-Spark AIs to be able to get
420
00:24:52.299 --> 00:24:56.662
<v SPEAKER_00>to top human performance in all domains within months of being developed.
421
00:24:57.103 --> 00:25:00.545
<v SPEAKER_00>There's still 2028 or 2029 in this median scenario.
422
00:25:01.025 --> 00:25:03.358
<v SPEAKER_00>And remember, even in this Spark scenario,
423
00:25:03.549 --> 00:25:06.271
<v SPEAKER_00>all of this happens in just the first year or two
424
00:25:06.353 --> 00:25:08.409
<v SPEAKER_00>after AI research is fully automated.
425
00:25:08.697 --> 00:25:12.653
<v SPEAKER_00>Things don't just stop there because even if the software progress peters out,
426
00:25:12.703 --> 00:25:17.264
<v SPEAKER_00>AIs will continue stoking the fire by adding more and more compute.
427
00:25:17.264 --> 00:25:22.877
<v SPEAKER_00>Even without help from AIs, global AI compute has been growing roughly 3x a year
428
00:25:22.877 --> 00:25:24.545
<v SPEAKER_00>for the last half decade.
429
00:25:24.545 --> 00:25:29.272
<v SPEAKER_00>And the AIs that come out of this Spark will be jaggedly superhuman
430
00:25:29.272 --> 00:25:32.685
<v SPEAKER_00>at helping us continue scaling up this compute.
431
00:25:32.685 --> 00:25:37.841
<v SPEAKER_00>They'll be extremely good at designing new AI chips and laying out the designs
432
00:25:37.841 --> 00:25:43.603
<v SPEAKER_00>of new fabs, even teleoperating robots to help build parts of fads in data centers.
433
00:25:43.603 --> 00:25:48.455
<v SPEAKER_00>And robots, it takes years to get to the same endpoint
434
00:25:48.455 --> 00:25:54.446
<v SPEAKER_00>that this software -only singularity would have achieved in months.
435
00:25:54.446 --> 00:26:01.395
<v SPEAKER_00>Which is a superintelligence that is to us what we are to chimps.
436
00:26:01.395 --> 00:26:03.296
<v SPEAKER_00>Appendix So earlier, I promised
437
00:26:03.316 --> 00:26:06.470
<v SPEAKER_00>to explain why I think AI research is largely verifiable.
438
00:26:06.520 --> 00:26:07.852
<v SPEAKER_00>So that's where I'll start.
439
00:26:07.902 --> 00:26:12.699
<v SPEAKER_00>After that, I'll go through what I think are the strongest objections to my arguments about RSI.
440
00:26:12.749 --> 00:26:16.605
<v SPEAKER_00>Now, one thing I want to call out at the very top is that because both pre-training
441
00:26:16.655 --> 00:26:19.442
<v SPEAKER_00>and post-training verifiable, and I'll make my argument for why later,
442
00:26:19.492 --> 00:26:24.322
<v SPEAKER_00>So is progress on what is the most galling and important efficiency that AIs have
443
00:26:24.322 --> 00:26:27.383
<v SPEAKER_00>against humans, namely their lack of sample efficiency.
444
00:26:27.383 --> 00:26:30.020
<v SPEAKER_00>If you want a neural network to gain some capability,
445
00:26:30.020 --> 00:26:34.691
<v SPEAKER_00>you have to feed it far more data than it would take a human to learn
446
00:26:34.691 --> 00:26:35.719
<v SPEAKER_00>the exact same thing.
447
00:26:35.719 --> 00:26:38.552
<v SPEAKER_00> But every kind of sample efficiency is measurable.
448
00:26:38.840 --> 00:26:41.301
<v SPEAKER_00>For example, you can measure how much data it takes to reach
449
00:26:41.341 --> 00:26:45.152
<v SPEAKER_00>a given pre-training loss, or how many tasks it takes to reach a given score
450
00:26:45.202 --> 00:26:48.603
<v SPEAKER_00>in an RL environment, or even how much feedback and time
451
00:26:48.943 --> 00:26:53.405
<v SPEAKER_00>within a single session it takes to reach a desired level of performance just
452
00:26:53.425 --> 00:26:54.814
<v SPEAKER_00>from in-context learning.
453
00:26:54.965 --> 00:26:58.717
<v SPEAKER_00>Sample efficiency and online learning are really two sides of the same problem,
454
00:26:58.767 --> 00:27:02.528
<v SPEAKER_00>which is how to learn from real-world data quickly and efficiently.
455
00:27:03.169 --> 00:27:08.169
<v SPEAKER_00> For decades, people have recognized this as the deepest open problem in machine learning.
456
00:27:08.496 --> 00:27:11.107
<v SPEAKER_00>AI is equivalent of a Millennium Prize problem.
457
00:27:11.581 --> 00:27:15.507
<v SPEAKER_00>And mathematics has already shown us what happens to such problems,
458
00:27:15.947 --> 00:27:18.430
<v SPEAKER_00>even when they are very difficult, as Okay,
459
00:27:19.991 --> 00:27:23.362
<v SPEAKER_00>now let's get to why I think that AI progress is largely verifiable.
460
00:27:23.412 --> 00:27:27.814
<v SPEAKER_00>Why progress on sample efficiency or online learning or the other problems
461
00:27:27.874 --> 00:27:30.835
<v SPEAKER_00>in ML is captured by verifiable proxies.
462
00:27:31.295 --> 00:27:34.577
<v SPEAKER_00>There are roughly three broad buckets of AI R&D.
463
00:27:35.117 --> 00:27:38.138
<v SPEAKER_00>Pre-training, post-training, and inference efficiency.
464
00:27:38.795 --> 00:27:43.796
<v SPEAKER_00> And as I'll explain, each has strong verifiable proxies that are easy to train against.
465
00:27:44.316 --> 00:27:48.077
<v SPEAKER_00>And since together, these comprise all of algorithmic progress,
466
00:27:48.498 --> 00:27:51.628
<v SPEAKER_00>that means that AI progress in general is easy to train against,
467
00:27:51.678 --> 00:27:55.980
<v SPEAKER_00>which in some sense shouldn't be that surprising because we can make models better
468
00:27:56.020 --> 00:27:58.030
<v SPEAKER_00>at things that can be tested inside a data center
469
00:27:58.080 --> 00:28:01.413
<v SPEAKER_00>and AI training is literally happening inside a data center.
470
00:28:01.682 --> 00:28:02.903
<v SPEAKER_00>As we talk about these proxies,
471
00:28:02.923 --> 00:28:07.130
<v SPEAKER_00>you should keep in mind that verifiability is valuable for two reasons.
472
00:28:07.630 --> 00:28:12.678
<v SPEAKER_00>So first, it allows AI companies to directly RL a model to get better
473
00:28:12.778 --> 00:28:16.323
<v SPEAKER_00>at the specific parts of AI research through thousands around
474
00:28:17.525 --> 00:28:19.648
<v SPEAKER_00>But the second reason verifiability is important is
475
00:28:19.668 --> 00:28:23.934
<v SPEAKER_00>that these proxies allow each agent to empirically check
476
00:28:24.415 --> 00:28:27.700
<v SPEAKER_00>whether they've beaten some score on a leaderboard
477
00:28:28.020 --> 00:28:29.612
<v SPEAKER_00>before they merged their contributions.
478
00:28:29.662 --> 00:28:32.718
<v SPEAKER_00>And so they can work much more effectively in parallel.
479
00:28:33.298 --> 00:28:36.633
<v SPEAKER_00>Okay, so with that in mind, let's start by talking about pre-training.
480
00:28:36.683 --> 00:28:38.846
<v SPEAKER_00>So as you're building GPT-7,
481
00:28:39.207 --> 00:28:43.651
<v SPEAKER_00>you can RL that model to get better at finding pre-training compute multipliers.
482
00:28:44.014 --> 00:28:48.080
<v SPEAKER_00>For example, you can make an RL objective that GPT-7 has to minimize
483
00:28:50.362 --> 00:28:55.106
<v SPEAKER_00>And once GPT-7 is built,
484
00:28:55.466 --> 00:28:58.577
<v SPEAKER_00>you can now deploy this model or a swarm of these models
485
00:28:58.989 --> 00:29:04.654
<v SPEAKER_00>to figure out how to train a GPT-3 size model to the lowest possible perplexity.
486
00:29:05.354 --> 00:29:07.786
<v SPEAKER_00>And this is because loss on a held out test set,
487
00:29:07.836 --> 00:29:11.960
<v SPEAKER_00>which is the basis of free training research, is extremely easy to verify.
488
00:29:12.805 --> 00:29:16.018
<v SPEAKER_00>Of course, what works at small scale doesn't necessarily work at large scale,
489
00:29:16.068 --> 00:29:18.850
<v SPEAKER_00>and it requires taste to anticipate exactly
490
00:29:18.971 --> 00:29:22.113
<v SPEAKER_00>which small scale improvements will actually bear fruit
491
00:29:22.233 --> 00:29:24.955
<v SPEAKER_00>when they're composed together in a bigger model.
492
00:29:25.116 --> 00:29:27.616
<v SPEAKER_00>But this kind of intuition is also trainable.
493
00:29:27.738 --> 00:29:31.762
<v SPEAKER_00>For example, you can make an RL environment where GPT-7 has to predict
494
00:29:31.822 --> 00:29:34.214
<v SPEAKER_00>whether an algorithmic improvement that it made
495
00:29:34.264 --> 00:29:38.818
<v SPEAKER_00>at the 100 million parameter scale will also hold at the 10 billion parameter scale.
496
00:29:38.868 --> 00:29:42.320
<v SPEAKER_00>And while this taste While the East bench environment is more expensive to RL
497
00:29:42.370 --> 00:29:44.051
<v SPEAKER_00>on than the Nano-GPT speedrun,
498
00:29:44.492 --> 00:29:48.992
<v SPEAKER_00>it's still not that difficult to train on if you have frontier lab-scale compute.
499
00:29:49.234 --> 00:29:52.456
<v SPEAKER_00>So even important parts of research tastes are verifiable.
500
00:29:52.536 --> 00:29:56.969
<v SPEAKER_00>And if you just automated pre-training, you'd already radically speed up AI progress.
501
00:29:57.019 --> 00:29:59.019
<v SPEAKER_00>And there's a couple of reasons why.
502
00:29:59.133 --> 00:30:02.696
<v SPEAKER_00>First is that pre-training leads to very general improvements
503
00:30:02.917 --> 00:30:05.409
<v SPEAKER_00>in the model's intelligence and capabilities.
504
00:30:05.459 --> 00:30:08.291
<v SPEAKER_00>And there's a deep explanation for why this is true,
505
00:30:08.341 --> 00:30:11.494
<v SPEAKER_00>which has to do with the link between compression and intelligence.
506
00:30:11.544 --> 00:30:12.976
<v SPEAKER_00>And if you want to learn more about this, by the way,
507
00:30:13.026 --> 00:30:17.129
<v SPEAKER_00>I highly recommend this excellent video by 3Blue1Brown on the topic that I'll link
508
00:30:17.149 --> 00:30:18.149
<v SPEAKER_00>to below.
509
00:30:18.274 --> 00:30:20.748
<v SPEAKER_00>And the second reason is that as you make pre-training improvements,
510
00:30:20.798 --> 00:30:24.623
<v SPEAKER_00>you can now train a smaller and smaller model that is just as good
511
00:30:24.663 --> 00:30:28.607
<v SPEAKER_00>as a previously larger model, but which trains faster and more cheaply.
512
00:30:28.790 --> 00:30:30.803
<v SPEAKER_00>And this not only speeds up pre-training,
513
00:30:30.853 --> 00:30:31.874
<v SPEAKER_00>but it also means
514
00:30:31.994 --> 00:30:36.901
<v SPEAKER_00>that your experiments RL rollouts atop this base model are now more efficient.
515
00:30:37.422 --> 00:30:40.497
<v SPEAKER_00>And since your automated researchers are just instantiations
516
00:30:40.547 --> 00:30:45.047
<v SPEAKER_00>of this now smaller model, you can now support larger researcher populations too.
517
00:30:45.194 --> 00:30:48.408
<v SPEAKER_00>And the third reason is that because smaller models train faster,
518
00:30:48.458 --> 00:30:50.772
<v SPEAKER_00>This actually tightens the RSI loop itself.
519
00:30:50.822 --> 00:30:54.447
<v SPEAKER_00>During RSI, labs probably won't be doing three month long pre-training runs
520
00:30:54.467 --> 00:30:57.301
<v SPEAKER_00>that are spread out across multiple data center campuses.
521
00:30:57.351 --> 00:31:02.239
<v SPEAKER_00>Instead, the army of automated researchers will be finding algorithmic innovations
522
00:31:02.539 --> 00:31:05.539
<v SPEAKER_00>so quickly that by the time that a giant run finished,
523
00:31:05.681 --> 00:31:09.062
<v SPEAKER_00>it would already have been made obsolete by a much smaller model
524
00:31:09.102 --> 00:31:11.435
<v SPEAKER_00>that first began training only a week ago.
525
00:31:11.762 --> 00:31:14.853
<v SPEAKER_00>It's similar to how if you launch a spaceship to Alpha Centauri
526
00:31:14.903 --> 00:31:18.945
<v SPEAKER_00>with today's technology, it would probably be overtaken in transit by one
527
00:31:18.965 --> 00:31:20.895
<v SPEAKER_00>that was launched a century from now.
528
00:31:20.945 --> 00:31:23.579
<v SPEAKER_00>Furthermore, since you're training smaller models faster,
529
00:31:23.629 --> 00:31:27.084
<v SPEAKER_00>and on a scale where you can run thousands of experiments daily,
530
00:31:27.134 --> 00:31:31.211
<v SPEAKER_00>you won't have to bet that small-scale results will hold up in bigger models.
531
00:31:31.261 --> 00:31:34.761
<v SPEAKER_00>You've already tested at the scale which you'll be training at.
532
00:31:35.667 --> 00:31:38.519
<v SPEAKER_00>What do most models get even at today's parameter sizes?
533
00:31:38.569 --> 00:31:40.841
<v SPEAKER_00>I think there's probably a ton more potential.
534
00:31:40.891 --> 00:31:42.802
<v SPEAKER_00>We are far from the limits of pre-training.
535
00:31:42.852 --> 00:31:46.865
<v SPEAKER_00>For example, the AI Lab Magic recently announced that they pre-trained a model
536
00:31:46.915 --> 00:31:51.068
<v SPEAKER_00>that matches the leading open source-based models today like DeepSeq v4 Pro
537
00:31:51.118 --> 00:31:55.062
<v SPEAKER_00>for just half of the compute that was used to train the original GPT-3,
538
00:31:55.261 --> 00:31:57.483
<v SPEAKER_00>which would roughly cost $500,000 today.
539
00:31:57.763 --> 00:32:01.275
<v SPEAKER_00>Orders of magnitude further improvements seem totally plausible.
540
00:32:01.325 --> 00:32:03.037
<v SPEAKER_00> Now let's talk about post-training.
541
00:32:03.087 --> 00:32:06.341
<v SPEAKER_00>There are three different kinds of verifiable proxies for post-training.
542
00:32:06.391 --> 00:32:08.584
<v SPEAKER_00>First, your automated researchers can try
543
00:32:08.634 --> 00:32:12.798
<v SPEAKER_00>to improve your post-training algorithms such that if you want to RL on a new set
544
00:32:12.818 --> 00:32:16.162
<v SPEAKER_00>of environments, it takes less compute or data or time.
545
00:32:16.563 --> 00:32:18.841
<v SPEAKER_00>All three of which are easily measurable.
546
00:32:19.064 --> 00:32:23.696
<v SPEAKER_00> Second, your automated researchers can work on making models better at learning on the fly.
547
00:32:23.746 --> 00:32:25.497
<v SPEAKER_00>And you can easily measure progress on this.
548
00:32:25.547 --> 00:32:28.819
<v SPEAKER_00>For example, you can measure if you drop your model into an environment
549
00:32:28.869 --> 00:32:30.313
<v SPEAKER_00>that was never trained on.
550
00:32:30.429 --> 00:32:34.441
<v SPEAKER_00>How quickly does it learn what's going on and figure out how to get a good score?
551
00:32:34.491 --> 00:32:37.383
<v SPEAKER_00>And how fast does it get better at a video game that it's never played before?
552
00:32:37.433 --> 00:32:39.864
<v SPEAKER_00>And you can have more real-world examples of this too.
553
00:32:39.914 --> 00:32:41.435
<v SPEAKER_00>If you want to see what these could look like,
554
00:32:41.475 --> 00:32:44.546
<v SPEAKER_00>check out this great benchmark that ByteDance released called EdgeBench
555
00:32:44.596 --> 00:32:45.985
<v SPEAKER_00>for these kinds of tasks.
556
00:32:46.637 --> 00:32:50.423
<v SPEAKER_00>And third, you can just measure AI R&D capability directly.
557
00:32:50.963 --> 00:32:54.098
<v SPEAKER_00>Anthropic, for example, has this internal benchmark called CoBench,
558
00:32:54.148 --> 00:32:57.092
<v SPEAKER_00>which contains around 500 real problems that the researchers
559
00:32:57.132 --> 00:32:59.125
<v SPEAKER_00>and engineers have solved this year.
560
00:32:59.175 --> 00:33:01.731
<v SPEAKER_00>And every benchmark is also an RL environment.
561
00:33:01.978 --> 00:33:04.740
<v SPEAKER_00>And in our environment like this would allow Anthropic
562
00:33:04.780 --> 00:33:09.133
<v SPEAKER_00>to have their models practice redoing the last three to six months of human progress
563
00:33:09.183 --> 00:33:13.350
<v SPEAKER_00>at the frontier. The third big area of AI research is inference efficiency.
564
00:33:13.626 --> 00:33:17.099
<v SPEAKER_00>What this involves is designing your model and the surrounding software
565
00:33:17.149 --> 00:33:18.980
<v SPEAKER_00>to get more juice out of your compute.
566
00:33:19.030 --> 00:33:20.919
<v SPEAKER_00>And this is especially verifiable.
567
00:33:21.271 --> 00:33:25.794
<v SPEAKER_00>For example, you can easily measure GPU utilization or KB cache size per token
568
00:33:26.235 --> 00:33:29.717
<v SPEAKER_00>or total flops in a forward pass or latency and so on.
569
00:33:32.485 --> 00:33:36.501
<v SPEAKER_00>Now I want to deal with the strongest objections to my arguments about RSI.
570
00:33:36.551 --> 00:33:39.045
<v SPEAKER_00>I want to be clear that these bottlenecks are serious,
571
00:33:39.095 --> 00:33:43.251
<v SPEAKER_00>and they do tamp down the probability of the most aggressive possible takeoff.
572
00:33:43.301 --> 00:33:47.902
<v SPEAKER_00>This is why I think we'll probably make something like a GPT 3.5 to GPT 6 size jump
573
00:33:47.902 --> 00:33:52.013
<v SPEAKER_00>in 2028 rather than some crazy overnight singularity that starts tomorrow,
574
00:33:52.570 --> 00:33:56.007
<v SPEAKER_00>But I think these bottlenecks won't be especially crippling,
575
00:33:56.007 --> 00:33:58.373
<v SPEAKER_00>and the neck of the bottle is actually pretty wide.
576
00:33:58.373 --> 00:33:59.474
<v SPEAKER_00>Let me explain why.
577
00:33:59.474 --> 00:34:02.988
<v SPEAKER_00>Okay so the first objection, this is an objection that I had until recently,
578
00:34:02.988 --> 00:34:07.252
<v SPEAKER_00>is that we'll be bottlenecked by continual learning or the lack thereof.
579
00:34:07.580 --> 00:34:10.341
<v SPEAKER_00>I spent the past year and a half arguing that the main thing missing
580
00:34:10.381 --> 00:34:14.642
<v SPEAKER_00>from today's AIs is this ability to learn from on-the-job experience.
581
00:34:15.102 --> 00:34:18.935
<v SPEAKER_00>Every new session is their first day on the job, and in each session,
582
00:34:19.043 --> 00:34:22.924
<v SPEAKER_00>they can only retain a couple hours worth of information so they don't accumulate
583
00:34:22.944 --> 00:34:27.376
<v SPEAKER_00>the kind of feedback and know-how that arrives over the course of weeks or months.
584
00:34:27.426 --> 00:34:32.759
<v SPEAKER_00>Last December, this was my main reason for doubting that we'd automate AI research anytime soon.
585
00:34:33.022 --> 00:34:36.527
<v SPEAKER_00>As I wrote then, somehow this automated researcher is going to figure out
586
00:34:36.547 --> 00:34:40.633
<v SPEAKER_00>the algorithm for HCI, which is a problem that humans have been banging their head
587
00:34:40.673 --> 00:34:42.726
<v SPEAKER_00>against for the better half of a century.
588
00:34:42.776 --> 00:34:46.554
<v SPEAKER_00>While not having the basic learning capabilities that children have,
589
00:34:46.742 --> 00:34:48.174
<v SPEAKER_00>I find this super implausible.
590
00:34:48.224 --> 00:34:49.997
<v SPEAKER_00>But I've somewhat changed my mind on this.
591
00:34:50.047 --> 00:34:52.991
<v SPEAKER_00>Here's why I don't think that the current lack of continual learning
592
00:34:53.011 --> 00:34:57.879
<v SPEAKER_00>in these models will stop full automation of the best AI researchers by 2028.
593
00:34:58.259 --> 00:35:01.294
<v SPEAKER_00>First, AI companies might just solve continual learning by then,
594
00:35:01.344 --> 00:35:03.931
<v SPEAKER_00>with architectures that are much like the ones they already have.
595
00:35:03.931 --> 00:35:08.017
<v SPEAKER_00>Previously, I thought that we were bottlenecked by some crazy breakthroughs
596
00:35:08.017 --> 00:35:12.187
<v SPEAKER_00>that would allow models to update their own weights at the end of every session.
597
00:35:12.187 --> 00:35:15.529
<v SPEAKER_00>But now I think that scaling up in -context learning is enough,
598
00:35:15.529 --> 00:35:18.194
<v SPEAKER_00>and so you'll have sessions that are effectively many months long,
599
00:35:18.194 --> 00:35:22.636
<v SPEAKER_00>and this will allow a single instance to learn effectively on the job.
600
00:35:22.636 --> 00:35:24.117
<v SPEAKER_00>And people have published many,
601
00:35:24.117 --> 00:35:25.936
<v SPEAKER_00>many promising ideas that would let
602
00:35:25.936 --> 00:35:29.024
<v SPEAKER_00>the labs achieve dramatically longer effective context windows.
603
00:35:29.024 --> 00:35:32.235
<v SPEAKER_00>And the second reason is that you might not need a continual learner
604
00:35:32.285 --> 00:35:33.841
<v SPEAKER_00>to solve continual learning.
605
00:35:34.146 --> 00:35:38.488
<v SPEAKER_00>As I explained earlier, online learning is an ML research problem with clean,
606
00:35:38.528 --> 00:35:39.584
<v SPEAKER_00>verifiable proxies.
607
00:35:40.048 --> 00:35:42.599
<v SPEAKER_00>If you'd asked me two years ago, which would be harder to solve,
608
00:35:42.649 --> 00:35:44.649
<v SPEAKER_00>Navier Stokes or continual learning,
609
00:35:44.710 --> 00:35:47.822
<v SPEAKER_00>it wouldn't have been obvious to me that the answer was Navier Stokes.
610
00:35:47.872 --> 00:35:51.065
<v SPEAKER_00>Now, of course, it turns out that Continual learning did turn out to be harder,
611
00:35:51.115 --> 00:35:53.288
<v SPEAKER_00>given the fact that the labs haven't cracked it yet.
612
00:35:53.338 --> 00:35:56.122
<v SPEAKER_00>But are we so confident that it's that much harder
613
00:35:56.523 --> 00:36:00.268
<v SPEAKER_00>that the non-online learning models a year or two smarter than the ones
614
00:36:00.288 --> 00:36:04.183
<v SPEAKER_00>that are currently solving Millennium Prize problems won't be able to crack it?
615
00:36:04.233 --> 00:36:06.507
<v SPEAKER_00> Even if they're amnesiacs like the current models are?
616
00:36:06.557 --> 00:36:09.351
<v SPEAKER_00>These models are out here solving Millennium Prize problems
617
00:36:09.401 --> 00:36:13.357
<v SPEAKER_00>while still being these derpy savant interns that have no long-term memory.
618
00:36:13.407 --> 00:36:18.574
<v SPEAKER_00>It's like watching somebody do cartwheels down the track and still keep pace with Usain Bolt.
619
00:36:19.155 --> 00:36:26.062
<v SPEAKER_00>Now, all this being said,
620
00:36:26.342 --> 00:36:27.653
<v SPEAKER_00>I think there is a serious chance
621
00:36:27.703 --> 00:36:30.756
<v SPEAKER_00>that we don't solve continual learning within the next few years,
622
00:36:30.806 --> 00:36:34.600
<v SPEAKER_00>and that models are not able to compensate for this missing capability
623
00:36:34.650 --> 00:36:36.141
<v SPEAKER_00>through their other advantages.
624
00:36:36.191 --> 00:36:38.494
<v SPEAKER_00>That's why I put a 25% probability
625
00:36:38.794 --> 00:36:43.739
<v SPEAKER_00>that we won't automate ILIA-level top human researchers until after 2032.
626
00:36:44.868 --> 00:36:47.993
<v SPEAKER_00>One important objection people have is that we'll be bottlenecked by finding
627
00:36:48.033 --> 00:36:49.644
<v SPEAKER_00>the right verifiable proxies.
628
00:36:49.836 --> 00:36:53.451
<v SPEAKER_00>All the verifiable proxies that I've listed above assume the current paradigm,
629
00:36:53.501 --> 00:36:57.597
<v SPEAKER_00>they would argue, but figuring out what objective to verify in the first place,
630
00:36:57.647 --> 00:36:59.650
<v SPEAKER_00>choosing which hill to have GPT-6,
631
00:37:02.500 --> 00:37:03.110
<v SPEAKER_00>research.
632
00:37:03.160 --> 00:37:06.970
<v SPEAKER_00>This is what one might call research taste, and how are you going to train for that?
633
00:37:07.020 --> 00:37:10.180
<v SPEAKER_00>Before 2018, almost nobody was saying that minimizing loss
634
00:37:10.180 --> 00:37:14.090
<v SPEAKER_00>on next token prediction is going to be the most tractable path to AI progress.
635
00:37:14.140 --> 00:37:18.215
<v SPEAKER_00>So nobody would have bothered to build nano -GPT style speedrun environments
636
00:37:18.215 --> 00:37:21.827
<v SPEAKER_00>where the agent swarm has to minimize how much time it takes to get
637
00:37:21.827 --> 00:37:23.226
<v SPEAKER_00>to a certain pre -training loss.
638
00:37:23.226 --> 00:37:26.525
<v SPEAKER_00>Wouldn't there be multiple new paradigms that we have to cross to get from here
639
00:37:26.525 --> 00:37:30.973
<v SPEAKER_00>to superintelligence? And won't each new paradigm require some associated proxy
640
00:37:30.973 --> 00:37:32.873
<v SPEAKER_00>that we don't know ex ante?
641
00:37:32.873 --> 00:37:36.360
<v SPEAKER_00>How will the automated researchers find these during RSI?
642
00:37:36.360 --> 00:37:38.385
<v SPEAKER_00>I have two responses to this objection.
643
00:37:38.385 --> 00:37:41.410
<v SPEAKER_00>First, the transformer was visible on, in fact,
644
00:37:41.470 --> 00:37:44.554
<v SPEAKER_00>invented to beat the existing translation benchmarks.
645
00:37:45.055 --> 00:37:49.952
<v SPEAKER_00>A similar story is true for reasoning models and the pre-existing coding and math benchmarks.
646
00:37:50.002 --> 00:37:53.658
<v SPEAKER_00>Proxies made before a paradigm leap seem perfectly capable
647
00:37:53.658 --> 00:37:55.178
<v SPEAKER_00>of capturing large step changes in performance.
648
00:37:55.178 --> 00:37:59.530
<v SPEAKER_00>This is because AI learning algorithms are quite general.
649
00:37:59.891 --> 00:38:04.723
<v SPEAKER_00>And second, it's not that difficult to come up with paradigm-agnostic outer-loop proxies.
650
00:38:04.773 --> 00:38:08.165
<v SPEAKER_00>For example, how many Millennium Prize problems does your new model solve?
651
00:38:08.215 --> 00:38:10.867
<v SPEAKER_00>And if you train your model on data before 1905,
652
00:38:10.917 --> 00:38:13.648
<v SPEAKER_00>how long does it take before it discovers general relativity?
653
00:38:13.698 --> 00:38:17.142
<v SPEAKER_00>How fast does it master totally unseen video games? And so on.
654
00:38:17.680 --> 00:38:21.151
<v SPEAKER_00>All in all, I think the other objections to the impact of RSI are much stronger,
655
00:38:21.201 --> 00:38:25.323
<v SPEAKER_00>and I'd be very surprised if this ended up being the reason that RSI was not
656
00:38:25.363 --> 00:38:28.674
<v SPEAKER_00>a big deal. The other big bottleneck that people point out is data.
657
00:38:28.724 --> 00:38:31.375
<v SPEAKER_00>Isn't data one of the main inputs into AI progress?
658
00:38:31.425 --> 00:38:34.814
<v SPEAKER_00>How will RSI happen without that scaling up at the same rate?
659
00:38:35.106 --> 00:38:38.157
<v SPEAKER_00>My answer is that data will continue growing during RSI,
660
00:38:38.207 --> 00:38:40.540
<v SPEAKER_00>but the AIs will be the ones compiling it.
661
00:38:40.764 --> 00:38:44.680
<v SPEAKER_00>Producing better training data for both pre-training and post-training is itself
662
00:38:44.730 --> 00:38:47.985
<v SPEAKER_00>an ML research problem, and AIs are getting increasingly better
663
00:38:48.035 --> 00:38:49.187
<v SPEAKER_00>at doing it themselves.
664
00:38:49.237 --> 00:38:52.692
<v SPEAKER_00>Now, it is true that data is an extremely important input into AI progress.
665
00:38:52.742 --> 00:38:55.105
<v SPEAKER_00>Together with Jerry Hahn, who's a student at Princeton,
666
00:38:55.125 --> 00:38:59.612
<v SPEAKER_00>I actually did We found that for pre-training, over the last six years,
667
00:39:00.012 --> 00:39:03.227
<v SPEAKER_00>more than three times the algorithmic progress has come from data improvements
668
00:39:03.277 --> 00:39:04.610
<v SPEAKER_00>than model improvements.
669
00:39:04.799 --> 00:39:07.884
<v SPEAKER_00>However, I don't think that people realize that these data improvements
670
00:39:07.924 --> 00:39:14.924
<v SPEAKER_00>in pre-training are very much in line with you next time.
671
00:39:15.930 --> 00:39:19.970
<v SPEAKER_00>Data empirically lead to lower loss on a held -out corpus.
672
00:39:20.170 --> 00:39:23.114
<v SPEAKER_00>A similar thing seems to be increasingly true for RL.
673
00:39:23.270 --> 00:39:24.850
<v SPEAKER_00>DeepSeq just published a paper where they talk
674
00:39:24.850 --> 00:39:27.040
<v SPEAKER_00>about how they post -strain their new model.
675
00:39:27.090 --> 00:39:31.306
<v SPEAKER_00>They say that changes to the basic RL algorithm have not mattered nearly as much
676
00:39:31.356 --> 00:39:35.039
<v SPEAKER_00>and that, quote, systematic improvements in the scale, diversity,
677
00:39:35.179 --> 00:39:39.962
<v SPEAKER_00>and verifiability of synthesized data and environments account for essentially all
678
00:39:40.002 --> 00:39:41.835
<v SPEAKER_00>of the observed gains, end quote.
679
00:39:41.964 --> 00:39:45.616
<v SPEAKER_00>And the way in which these environments are made is itself getting more and more automated.
680
00:39:45.666 --> 00:39:50.710
<v SPEAKER_00>They write, quote, we invest in large-scale automated pipelines for data synthesis
681
00:39:50.790 --> 00:39:52.401
<v SPEAKER_00>and environment construction.
682
00:39:52.731 --> 00:39:53.993
<v SPEAKER_00>Now,
683
00:39:54.353 --> 00:40:00.199
<v SPEAKER_00>I want to talk
684
00:40:00.239 --> 00:40:03.292
<v SPEAKER_00>about the idea that AI progress will be bottlenecked by experiments.
685
00:40:03.342 --> 00:40:07.125
<v SPEAKER_00>So earlier, I made this extended analogy between the current acceleration
686
00:40:07.145 --> 00:40:10.559
<v SPEAKER_00>in mathematics and what we should expect to happen in AI research.
687
00:40:10.609 --> 00:40:14.062
<v SPEAKER_00>But there is one big difference between AI research and mathematics.
688
00:40:14.112 --> 00:40:18.168
<v SPEAKER_00>In In math, you can simply reason your way with pen and paper to new discoveries,
689
00:40:18.218 --> 00:40:22.574
<v SPEAKER_00>whereas in AI research, you need to run actual experiments to validate your ideas,
690
00:40:22.624 --> 00:40:24.466
<v SPEAKER_00>and these to compute and time.
691
00:40:24.767 --> 00:40:27.300
<v SPEAKER_00>And as the number of automated researchers grows,
692
00:40:27.350 --> 00:40:31.718
<v SPEAKER_00>each gets access to a smaller and smaller slice of the total experiment compute pie.
693
00:40:31.718 --> 00:40:36.106
<v SPEAKER_00>My answer to this is that each agent will still get access to a ton of compute,
694
00:40:36.197 --> 00:40:37.027
<v SPEAKER_00>basically.
695
00:40:37.077 --> 00:40:41.030
<v SPEAKER_00>Frontier Labs have been more than quadrupling their compute every single year.
696
00:40:41.080 --> 00:40:44.201
<v SPEAKER_00>And if this trend continues, then by the end of 2027,
697
00:40:44.602 --> 00:40:46.983
<v SPEAKER_00>OpenAI could almost give 10,000 agents,
698
00:40:47.203 --> 00:40:50.575
<v SPEAKER_00>so the amount that were involved in solving the Millennium Prize problem,
699
00:40:50.625 --> 00:40:55.308
<v SPEAKER_00>each enough compute to run a GPT-3 size training run every single day.
700
00:40:55.968 --> 00:40:58.050
<v SPEAKER_00>Keep in mind that the final model,
701
00:40:58.270 --> 00:41:04.075
<v SPEAKER_00>trained in the original Transformer paper in 2017, took three days on eight P100s,
702
00:41:04.456 --> 00:41:07.469
<v SPEAKER_00>which would cost about 50 bucks if you went to rent it today,
703
00:41:07.519 --> 00:41:10.962
<v SPEAKER_00>or about one ten-thousandth of the training compute of GPT-3.
704
00:41:11.562 --> 00:41:15.485
<v SPEAKER_00>If the top human AI researchers, like Norm Shazir and Elia Satskiver,
705
00:41:15.885 --> 00:41:20.052
<v SPEAKER_00>had enough experiment compute to train a GPT-3 size model every single day,
706
00:41:20.589 --> 00:41:22.680
<v SPEAKER_00>they might make slower progress than they currently do,
707
00:41:22.730 --> 00:41:25.512
<v SPEAKER_00>but it would be extremely surprising to me if they failed
708
00:41:25.532 --> 00:41:29.175
<v SPEAKER_00>to make meaningful progress altogether and just sat down and started complaining
709
00:41:29.215 --> 00:41:31.104
<v SPEAKER_00>about how small their cluster was.
710
00:41:31.255 --> 00:41:33.726
<v SPEAKER_00>Now, how productive do you think an AI lab would be
711
00:41:33.776 --> 00:41:35.856
<v SPEAKER_00>if it had 10,000 great researchers,
712
00:41:36.336 --> 00:41:39.836
<v SPEAKER_00>each with this much compute and each thinking 10 times as fast?
713
00:41:39.897 --> 00:41:42.267
<v SPEAKER_00>You wouldn't want to write a check to this Neolab?
714
00:41:42.317 --> 00:41:46.038
<v SPEAKER_00>The nature of research and experimentation at the labs today reflects
715
00:41:46.058 --> 00:41:49.779
<v SPEAKER_00>that researcher time is extremely scarce relative to compute.
716
00:41:50.259 --> 00:41:54.510
<v SPEAKER_00>Top AI researchers individually get paid hundreds of millions of dollars a year.
717
00:41:54.560 --> 00:41:57.291
<v SPEAKER_00>So the way labs use compute today tells us very little
718
00:41:57.341 --> 00:42:01.785
<v SPEAKER_00>about how efficiently they could use it if compute, rather than researcher time,
719
00:42:02.043 --> 00:42:04.284
<v SPEAKER_00>was the key bottleneck. There are two main ways
720
00:42:04.324 --> 00:42:08.475
<v SPEAKER_00>in which the RSI agent swarm will use experiment compute much more efficiently
721
00:42:08.525 --> 00:42:10.192
<v SPEAKER_00>than researchers today use it.
722
00:42:10.306 --> 00:42:13.250
<v SPEAKER_00> First, immediately they can trade labor for compute.
723
00:42:13.471 --> 00:42:17.415
<v SPEAKER_00>To save valuable researcher time, experiments today are, and should be,
724
00:42:17.737 --> 00:42:19.237
<v SPEAKER_00>very wasteful with compute.
725
00:42:19.480 --> 00:42:23.646
<v SPEAKER_00>So instead of painstakingly setting up and carefully monitoring tons
726
00:42:23.686 --> 00:42:25.799
<v SPEAKER_00>of small-scale pre-training experiments,
727
00:42:25.849 --> 00:42:30.506
<v SPEAKER_00>A human researcher today might instead kick off a couple of huge multi-agent RL runs
728
00:42:30.556 --> 00:42:31.487
<v SPEAKER_00>in parallel.
729
00:42:31.537 --> 00:42:35.393
<v SPEAKER_00>But if you're bottlenecked by experiment compute, you can just do more of the former.
730
00:42:35.443 --> 00:42:38.237
<v SPEAKER_00>And when those automated researchers are doing an RL run,
731
00:42:38.287 --> 00:42:42.269
<v SPEAKER_00>they could read every single rollout transfer And immediately pause and rebuild
732
00:42:42.269 --> 00:42:44.700
<v SPEAKER_00>the whole environment if some task is broken.
733
00:42:44.750 --> 00:42:47.710
<v SPEAKER_00>They could be doing crazy amounts of small -scale ablations of their models
734
00:42:47.710 --> 00:42:52.880
<v SPEAKER_00>to make them oh And when a team of agents decides to combine their compute together
735
00:42:52.880 --> 00:42:54.800
<v SPEAKER_00>in order to do a much bigger run,
736
00:42:55.020 --> 00:42:58.280
<v SPEAKER_00>they could spend many subjective decades designing
737
00:42:58.280 --> 00:43:00.447
<v SPEAKER_00>the most informative pooled experiment.
738
00:43:01.060 --> 00:43:02.298
<v SPEAKER_00>And once it's done running,
739
00:43:02.348 --> 00:43:06.041
<v SPEAKER_00>they could spend further subjective decades comprehensively analyzing it
740
00:43:06.091 --> 00:43:07.823
<v SPEAKER_00>before designing a new experiment.
741
00:43:07.873 --> 00:43:12.717
<v SPEAKER_00>The other big way that this huge agent swarm could remain productive despite
742
00:43:12.737 --> 00:43:16.079
<v SPEAKER_00>the fact that each individual copy will have access to less compute Is
743
00:43:16.119 --> 00:43:20.182
<v SPEAKER_00>that these automated researchers could come up with a better science for learning
744
00:43:20.202 --> 00:43:21.753
<v SPEAKER_00>from small scale experiments.
745
00:43:21.803 --> 00:43:24.174
<v SPEAKER_00>Scaling laws themselves are a good example of this.
746
00:43:24.224 --> 00:43:26.676
<v SPEAKER_00>The GPT-4 paper says that they were able to predict
747
00:43:26.726 --> 00:43:31.129
<v SPEAKER_00>the model's final loss using models trained with 10,000 x less compute.
748
00:43:31.729 --> 00:43:33.250
<v SPEAKER_00>One of the things that the smarter
749
00:43:33.290 --> 00:43:35.671
<v SPEAKER_00>and faster automated company could be doing is trying
750
00:43:35.691 --> 00:43:38.473
<v SPEAKER_00>to discover more scaling phenomenon like MuP,
751
00:43:38.733 --> 00:43:43.066
<v SPEAKER_00>which lets researchers anticipate the optimal hyperparameters for a larger run
752
00:43:43.415 --> 00:43:45.016
<v SPEAKER_00>from 100x smaller model.
753
00:43:45.416 --> 00:43:47.748
<v SPEAKER_00>How many more similar discoveries like this are there?
754
00:43:47.798 --> 00:43:51.010
<v SPEAKER_00>I remember chatting to an AI researcher who thought that learning
755
00:43:51.060 --> 00:43:54.231
<v SPEAKER_00>from extremely small neural networks could be incredibly informative.
756
00:43:54.281 --> 00:43:59.184
<v SPEAKER_00>He put it this way, the gods above must work from the same principles as the ants below.
757
00:44:01.383 --> 00:44:05.999
<v SPEAKER_00> I want to thank my friends who paired with me through significant parts of writing this essay.
758
00:44:06.049 --> 00:44:09.172
<v SPEAKER_00>Max Ferenc, Gabe Freed, and Thomas Larson.
759
00:44:10.013 --> 00:44:13.127
<v SPEAKER_00>I'll see you on the next essay about superintelligence, but in the meantime,
760
00:44:13.177 --> 00:44:16.288
<v SPEAKER_00>if you want to get notified when that video essay drops,
761
00:44:16.481 --> 00:44:18.037
<v SPEAKER_00>please subscribe on YouTube.
762
00:44:18.183 --> 00:44:20.072
<v SPEAKER_00>All right, I'll see you next time.
763
00:44:20.072 --> 00:44:26.064
[music]
