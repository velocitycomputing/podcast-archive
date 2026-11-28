---
record_id: "podcast:fe54d6e2-76a1-42f9-b636-137b472aa8ef"
episode_id: fe54d6e2-76a1-42f9-b636-137b472aa8ef
title: AI researchers debate what we should do next – Daniel Kokotajlo and Ege Erdil
podcast_title: Dwarkesh Podcast
url: "https://pocketcasts.com/podcast/dwarkesh-podcast/6d554750-84ac-0138-ee2b-0acc26574db2/ai-researchers-debate-what-we-should-do-next-daniel-kokotajlo-and-ege-erdil/fe54d6e2-76a1-42f9-b636-137b472aa8ef"
audio_url: "https://pocketcasts.com/podcast/dwarkesh-podcast/6d554750-84ac-0138-ee2b-0acc26574db2/ai-researchers-debate-what-we-should-do-next-daniel-kokotajlo-and-ege-erdil/fe54d6e2-76a1-42f9-b636-137b472aa8ef"
feed_guid: null
feed_url: "https://apple.dwarkesh-podcast.workers.dev/feed.rss"
published_at: null
published_local_date: null
played_date: 2026-11-27
played_at: "2026-11-27T12:00:00Z"
play_count: 1
duration_seconds: 3000
source: pocketcasts-history-browser
played_label: Yesterday
history_order: 1
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: rss-podcast-transcript
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 8653f10da29266aeb578da65fa8fe384f3dc63c5c232787eab3b3e185cee3b5c
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

Daniel Kokotajlo, associated with the AI Futures Project and the AI 2027 and AI 2040 scenarios, and Ege Erdil, a researcher at Google DeepMind, debated how soon advanced AI could arrive and what should be done about it. The central disagreement was the probability of a “software-only singularity”: a fixed pool of compute and non-synthetic data being used increasingly efficiently by AI systems to accelerate AI research, potentially producing many years of progress in months. Erdil put that outcome at roughly 10–20% over the next three years, while Kokotajlo put it above 50%, saying fully automating AI research could happen around 2027, or possibly 2028 or 2029, and that without slowing AI companies there is a serious risk of misaligned AIs taking control. Erdil’s median timeline without recursive self-improvement was full automation in about 15–20 years, with maybe a 20% chance within five years. They also discussed whether more time would improve alignment, interpretability, and public awareness; the AI Futures Project’s proposal to delay an intelligence explosion by about a year; a possible restriction of AI R&D compute to 10% or 5% of company compute to slow progress by a factor of two or three; the Hugging Face incident as a relatively small real-world cost compared with theoretical catastrophic risk; whether alignment requires a theoretical breakthrough or will emerge incrementally from machine-learning practice; and the difficulty of US-China coordination, including export controls, EUV lithography, China’s temporary compute disadvantage, and whether a five-year window might be available.

For the user, the actionable move is to treat the disagreement as a decision problem rather than a settled forecast: decide what probability of rapid recursive self-improvement would justify support for pauses, compute caps, regulation, or continued acceleration. Useful research leads include evidence for and against software-only AI self-improvement, whether alignment progress is realistically incremental, the severity of the Hugging Face incident, the feasibility of 10% or 5% AI R&D compute limits, and the political feasibility of international verification. Follow-up questions worth tracking are: what concrete milestones would signal that AI research is becoming fully automated; what alignment or interpretability breakthroughs would materially reduce risk; whether public awareness is rising fast enough; whether anti-AI coalitions are durable or motivated by unrelated grievances; and whether US-China tensions make coordinated slowdown impossible. There are no direct health implications in the supplied material, but the practical implication is to separate existential-risk uncertainty from immediate personal decisions, while monitoring indicators such as automated AI research claims, compute governance proposals, export-control changes, political statements about AI risk, and evidence that China is catching up in compute infrastructure.

## Transcript

WEBVTT
1
00:00:00.171 --> 00:00:03.413
<v SPEAKER_00>Today I'm joined by Ege Erdal and Daniel Kokotela.
2
00:00:03.893 --> 00:00:06.024
<v SPEAKER_00>Ege is a researcher at Google DeepMind.
3
00:00:06.074 --> 00:00:11.797
<v SPEAKER_00>Daniel is one of the authors at the AI Futures Project, which published AI 2027 and AI 2040.
4
00:00:12.538 --> 00:00:16.510
<v SPEAKER_00>I wouldn't call this exactly a debate because I hope it'll be more a discussion,
5
00:00:16.560 --> 00:00:22.003
<v SPEAKER_00>but there is a set of key disagreements you guys have, which leads one of you,
6
00:00:22.083 --> 00:00:26.015
<v SPEAKER_00>Daniel, to believe that AI is likely to kill us all within the next few years.
7
00:00:26.065 --> 00:00:28.398
<v SPEAKER_00>And Ege, you believe that will not happen.
8
00:00:28.826 --> 00:00:31.638
<v SPEAKER_00> I feel like a big crux in this conversation is just timelines.
9
00:00:31.688 --> 00:00:34.466
<v SPEAKER_00>How soon do you expect extreme super intelligence?
10
00:00:35.210 --> 00:00:36.571
<v SPEAKER_00>Ege, I feel like, I don't know,
11
00:00:36.591 --> 00:00:38.192
<v SPEAKER_00>I've articulated and Paul has articulated
12
00:00:38.232 --> 00:00:42.176
<v SPEAKER_00>in the last episode why there could be extreme super intelligence soon.
13
00:00:42.394 --> 00:00:43.845
<v SPEAKER_00>Why do you think that's unlikely?
14
00:00:43.895 --> 00:00:47.257
<v SPEAKER_02>I think the main things I'm skeptical about are,
15
00:00:47.277 --> 00:00:49.738
<v SPEAKER_02>the main difference between me and Daniel and also I think between me
16
00:00:49.778 --> 00:00:54.681
<v SPEAKER_02>and Paul is just How much do you believe in the software-only singularity?
17
00:00:55.222 --> 00:00:58.584
<v SPEAKER_02>It is this idea that you have fixed pool of computes,
18
00:00:58.644 --> 00:01:01.476
<v SPEAKER_02>roughly fixed amount of data that is at least not synthetic.
19
00:01:01.526 --> 00:01:04.508
<v SPEAKER_02>And then what happens is that you get better AIs.
20
00:01:04.528 --> 00:01:08.170
<v SPEAKER_02>Those AIs are able to use that pool of resources way more efficiently
21
00:01:08.190 --> 00:01:09.721
<v SPEAKER_02>to make progress on AI research.
22
00:01:09.771 --> 00:01:13.373
<v SPEAKER_02>And you get this feedback loop that at least goes for many orders of magnitude
23
00:01:13.413 --> 00:01:14.264
<v SPEAKER_02>before it fizzles out.
24
00:01:14.314 --> 00:01:17.296
<v SPEAKER_02>And then that improvement is so big that you get, I don't know,
25
00:01:17.336 --> 00:01:20.748
<v SPEAKER_02>10 years of progress in like six months or whatever, something like this.
26
00:01:20.798 --> 00:01:26.843
<v SPEAKER_02>And I think the evidence we have is not sufficient to give like high credence on that.
27
00:01:27.164 --> 00:01:29.175
<v SPEAKER_02>Like I think maybe that's like, I don't know,
28
00:01:29.225 --> 00:01:32.318
<v SPEAKER_02>10 to 20% likely of happening over the next three years.
29
00:01:32.368 --> 00:01:34.520
<v SPEAKER_02>And I think that's probably the biggest disagreement
30
00:01:34.570 --> 00:01:37.202
<v SPEAKER_02>where like Daniel thinks that's like over 50% likely.
31
00:01:37.252 --> 00:01:40.455
<v SPEAKER_00>So why do you think it's more than 50% likely
32
00:01:41.256 --> 00:01:45.256
<v SPEAKER_00>that there will be extreme super intelligence within the next few years?
33
00:01:45.599 --> 00:01:48.821
<v SPEAKER_00>Whereas Ege thinks that's, I don't know, 10 to 20% likely.
34
00:01:48.887 --> 00:01:49.397
<v SPEAKER_01>Yeah.
35
00:01:49.447 --> 00:01:54.225
<v SPEAKER_01>So first of all, I don't think that probably we will all be dead in a couple of years.
36
00:01:54.508 --> 00:01:59.049
<v SPEAKER_01>The thing I would say is unless we substantially slow down the AI companies,
37
00:01:59.810 --> 00:02:05.331
<v SPEAKER_01>then probably we will lose control and there will be misaligned AIs running the show
38
00:02:05.511 --> 00:02:06.581
<v SPEAKER_01>in a couple of years.
39
00:02:06.631 --> 00:02:10.542
<v SPEAKER_01>But it seems like we're getting close to fully automating the AI research process.
40
00:02:10.592 --> 00:02:11.963
<v SPEAKER_01>That would be the main claim.
41
00:02:12.013 --> 00:02:13.013
<v SPEAKER_01>And how close?
42
00:02:13.913 --> 00:02:16.144
<v SPEAKER_01>Seems like it's going to happen in 2027. Maybe not.
43
00:02:16.194 --> 00:02:17.674
<v SPEAKER_01>Maybe 2028, maybe 2029.
44
00:02:18.494 --> 00:02:21.494
<v SPEAKER_01>I'd say it was slightly more likely than that in 2027.
45
00:02:21.919 --> 00:02:25.755
<v SPEAKER_01>And then I think that once you'd have fully automated the research process,
46
00:02:25.805 --> 00:02:27.583
<v SPEAKER_01>probably things will accelerate.
47
00:02:27.968 --> 00:02:33.024
<v SPEAKER_01>I do think that more likely than not, they will accelerate a lot, as Isaiah was describing.
48
00:02:33.256 --> 00:02:34.947
<v SPEAKER_01> We think there's some uncertainty there.
49
00:02:34.997 --> 00:02:40.099
<v SPEAKER_01>And so then I think that a lot of the limitations of current AI systems,
50
00:02:40.259 --> 00:02:42.801
<v SPEAKER_01>such as the data inefficiency or whatever,
51
00:02:43.221 --> 00:02:48.543
<v SPEAKER_01>will sort of melt away relatively quickly as progress accelerates dramatically.
52
00:02:49.024 --> 00:02:53.135
<v SPEAKER_01>And you'll end up with AIs that are able to sort of flexibly learn quickly
53
00:02:53.186 --> 00:02:55.707
<v SPEAKER_01>from all sorts of experience.
54
00:02:56.487 --> 00:02:59.820
<v SPEAKER_01>You might call them like top expert dominating AIs, perhaps.
55
00:03:02.128 --> 00:03:07.470
<v SPEAKER_01> I think top expert dominating AIs are effectively super intelligence as far as I'm concerned.
56
00:03:07.990 --> 00:03:09.200
<v SPEAKER_00>Here's an idea question.
57
00:03:09.250 --> 00:03:15.231
<v SPEAKER_00>So we go back five years and we have AI systems that can't even hold out a conversation, right?
58
00:03:15.491 --> 00:03:16.491
<v SPEAKER_00>Yep.
59
00:03:16.772 --> 00:03:19.833
<v SPEAKER_00>And now we have systems, they're like solving Millennium Prize problems,
60
00:03:19.873 --> 00:03:21.651
<v SPEAKER_00>they're pretty good coders, etc.
61
00:03:22.033 --> 00:03:25.304
<v SPEAKER_00>So if we just go another five years of progress at this pace,
62
00:03:25.354 --> 00:03:29.776
<v SPEAKER_00>do you think it's likely that that alone gives us AIs that are competitive
63
00:03:29.816 --> 00:03:30.872
<v SPEAKER_00>with human experts?
64
00:03:31.077 --> 00:03:34.798
<v SPEAKER_00>If we're looking forward five years, do we even need that much RSI?
65
00:03:34.818 --> 00:03:37.707
<v SPEAKER_00>We might not, but I think it's unclear or something.
66
00:03:37.980 --> 00:03:40.861
<v SPEAKER_02> I think if we don't get any RSI,
67
00:03:42.061 --> 00:03:46.713
<v SPEAKER_02>my median timeline is that everything is automated and humans have Like nothing
68
00:03:46.753 --> 00:03:47.774
<v SPEAKER_02>to do, basically.
69
00:03:47.794 --> 00:03:49.245
<v SPEAKER_02>Like they've been completely automated.
70
00:03:49.295 --> 00:03:52.516
<v SPEAKER_02>It's something like 15, 20 years from now. That's a median timeline.
71
00:03:52.536 --> 00:03:53.817
<v SPEAKER_02>So in the next five years, it's like, I don't know,
72
00:03:53.837 --> 00:03:56.448
<v SPEAKER_02>you still have to give it like 20% or something that it could happen.
73
00:03:56.498 --> 00:03:59.630
<v SPEAKER_02>So I think that's like a very live possibility that it could happen.
74
00:03:59.680 --> 00:04:01.931
<v SPEAKER_02>And in some sense, I think while there are disagreements
75
00:04:01.981 --> 00:04:04.572
<v SPEAKER_02>about like software-only singularity and similar things,
76
00:04:04.622 --> 00:04:07.374
<v SPEAKER_02>I think it's sometimes like those disagreements actually don't matter that much
77
00:04:07.424 --> 00:04:11.165
<v SPEAKER_02>because like all I'm saying is like Daniel is saying something is like 50
78
00:04:11.205 --> 00:04:12.946
<v SPEAKER_02>or 60% likely to happen over the next three years.
79
00:04:12.966 --> 00:04:14.587
<v SPEAKER_02>And I'm saying it's like 20% likely.
80
00:04:14.637 --> 00:04:17.449
<v SPEAKER_02>And then in some sense, like, okay, that question might be interesting,
81
00:04:17.499 --> 00:04:21.541
<v SPEAKER_02>but even if it's only 20% likely, if the situation is very bad,
82
00:04:21.581 --> 00:04:23.322
<v SPEAKER_02>you should still do something about it.
83
00:04:23.362 --> 00:04:25.633
<v SPEAKER_02>Like it's, so like in some sense, I think that's not even,
84
00:04:25.683 --> 00:04:28.214
<v SPEAKER_02>even though it's maybe large disagreement numerically,
85
00:04:28.264 --> 00:04:31.661
<v SPEAKER_02>I don't think it's like a significant disagreement like qualitatively.
86
00:04:31.711 --> 00:04:35.973
<v SPEAKER_01>So the reason why you're working at Google instead of protesting outside
87
00:04:35.993 --> 00:04:40.476
<v SPEAKER_01>of Anthropic, which is a practical difference between our behavior,
88
00:04:41.116 --> 00:04:45.728
<v SPEAKER_01>is less to do with the probabilities on the different scenarios and more to do with,
89
00:04:45.778 --> 00:04:46.319
<v SPEAKER_01>well, what actually?
90
00:04:46.339 --> 00:04:47.899
<v SPEAKER_02> I'm curious what you think.
91
00:04:48.120 --> 00:04:49.820
<v SPEAKER_02>I think several things.
92
00:04:49.840 --> 00:04:55.083
<v SPEAKER_02>So I do think in this particular question of whether it poses a good idea or not,
93
00:04:55.583 --> 00:05:01.587
<v SPEAKER_02>I'm worried about any plan that involves us acting on Risks
94
00:05:01.707 --> 00:05:07.650
<v SPEAKER_02>before we have seen some significant version of the costs in the real world.
95
00:05:07.710 --> 00:05:12.032
<v SPEAKER_02>So right now, I think the thing people always cite in these discussions now
96
00:05:12.092 --> 00:05:15.481
<v SPEAKER_02>since some number of months ago is the Hugging Face incident.
97
00:05:15.614 --> 00:05:19.105
<v SPEAKER_02>But I personally think the Hugging Face incident didn't cost that much and was
98
00:05:19.155 --> 00:05:21.957
<v SPEAKER_02>a pretty small incident in the grand scheme of things.
99
00:05:21.977 --> 00:05:24.968
<v SPEAKER_02>I think it was much less significant than a plane crash.
100
00:05:25.018 --> 00:05:26.685
<v SPEAKER_02> In terms of the cost imposed.
101
00:05:26.899 --> 00:05:28.520
<v SPEAKER_02>And if, for example, if the,
102
00:05:29.700 --> 00:05:33.062
<v SPEAKER_02>I do see it as analogous to if you have a new technology,
103
00:05:33.782 --> 00:05:35.823
<v SPEAKER_02>like a nuclear reactors or aircraft or whatever,
104
00:05:35.863 --> 00:05:39.935
<v SPEAKER_02>and then you haven't actually seen anything go wrong, anything significant.
105
00:05:39.985 --> 00:05:43.276
<v SPEAKER_02>But you have all these theoretical arguments for why things might go wrong
106
00:05:43.326 --> 00:05:45.770
<v SPEAKER_02>and you're intervening on the basis of that.
107
00:05:46.873 --> 00:05:50.209
<v SPEAKER_02>I'm just suspicious about that approach in general.
108
00:05:50.829 --> 00:05:53.560
<v SPEAKER_02>The thing I'm challenging when I say that is the view
109
00:05:53.610 --> 00:05:58.072
<v SPEAKER_02>that the way you get aligned AIs is to have some theoretical breakthrough
110
00:05:58.092 --> 00:06:00.914
<v SPEAKER_02>in alignment. Like that's the thing I'm challenging.
111
00:06:00.954 --> 00:06:01.835
<v SPEAKER_02>And what I would say is that like,
112
00:06:01.875 --> 00:06:04.669
<v SPEAKER_02>that's basically nothing in machine learning has worked like that.
113
00:06:04.719 --> 00:06:09.406
<v SPEAKER_02>Like machine learning is not a field that has large theoretical breakthroughs.
114
00:06:09.806 --> 00:06:13.141
<v SPEAKER_02>Like there's been no large theoretical breakthroughs over like the past 10 years.
115
00:06:13.191 --> 00:06:14.523
<v SPEAKER_02>All of them have been incredible.
116
00:06:14.573 --> 00:06:18.319
<v SPEAKER_02>You stack this computer multiplier with this computer multiplier
117
00:06:18.359 --> 00:06:20.161
<v SPEAKER_02>and you get this efficiency gain and whatever.
118
00:06:20.201 --> 00:06:21.303
<v SPEAKER_02>And it's just things like that.
119
00:06:21.323 --> 00:06:22.545
<v SPEAKER_02>It's very incremental.
120
00:06:22.805 --> 00:06:25.239
<v SPEAKER_02>It's like there are a lot of dimensions that you optimize at once.
121
00:06:25.289 --> 00:06:27.082
<v SPEAKER_02>And that's the way you make them more capable.
122
00:06:27.132 --> 00:06:33.441
<v SPEAKER_02> So I don't see why you would assume anything I think
123
00:06:33.461 --> 00:06:33.661
<v SPEAKER_00> this is
124
00:06:33.701 --> 00:06:39.109
<v SPEAKER_00>a key disagreement maybe between you guys is are there tractable interventions
125
00:06:39.209 --> 00:06:40.081
<v SPEAKER_00>that we could make?
126
00:06:40.131 --> 00:06:44.647
<v SPEAKER_00>And specifically, are those interventions more tractable if we get more time to make them?
127
00:06:44.697 --> 00:06:50.165
<v SPEAKER_00>That is likely to increase the value of what these AI systems do and how they treat us.
128
00:06:50.906 --> 00:06:55.572
<v SPEAKER_00>The AI Futures project has just put out a pacing scheme that you say will delay
129
00:06:55.612 --> 00:07:00.298
<v SPEAKER_00>the intelligence explosion by a year, which I guess you are expecting in 2027.
130
00:07:00.438 --> 00:07:03.162
<v SPEAKER_00>So you think this would slow down to 2028? Something like that.
131
00:07:03.182 --> 00:07:04.734
<v SPEAKER_00>I mean, we have uncertainty, but yeah.
132
00:07:04.784 --> 00:07:08.590
<v SPEAKER_00>What changes if we get the intelligence explosion in 2028 rather than 2027?
133
00:07:08.610 --> 00:07:09.621
<v SPEAKER_01>Yeah, so a couple things.
134
00:07:09.671 --> 00:07:15.740
<v SPEAKER_01>So first of all, I think that progress is being made on AI alignment and science
135
00:07:15.961 --> 00:07:17.628
<v SPEAKER_01>of understanding how AI works.
136
00:07:18.104 --> 00:07:19.355
<v SPEAKER_01> All sorts of things like this.
137
00:07:19.405 --> 00:07:21.358
<v SPEAKER_01>It's not going fast enough, but it is being made.
138
00:07:21.408 --> 00:07:25.363
<v SPEAKER_01>And so each additional year of time that we buy, there's additional progress,
139
00:07:25.413 --> 00:07:30.340
<v SPEAKER_01>which cuts away at that probability mass of the bad outcomes happening.
140
00:07:31.762 --> 00:07:34.151
<v SPEAKER_01>Second thing I would say is just general...
141
00:07:34.658 --> 00:07:41.550
<v SPEAKER_01>awareness and like you I think this might actually be the most important thing is
142
00:07:41.550 --> 00:07:44.650
<v SPEAKER_01>that most people just don't really take this stuff Seriously,
143
00:07:44.700 --> 00:07:47.390
<v SPEAKER_01>don't really understand what's happening or what's coming.
144
00:07:47.440 --> 00:07:51.551
<v SPEAKER_01>And that seems just sort of broadly bad to me And I think probably we'd be
145
00:07:51.763 --> 00:07:56.370
<v SPEAKER_01>in a better situation if more people in general understood what was coming.
146
00:07:56.791 --> 00:08:00.727
<v SPEAKER_01>And I think that that process is happening, and it might even be happening exponentially.
147
00:08:00.777 --> 00:08:03.741
<v SPEAKER_01>Every year that goes by, more people learn more, more people pay attention,
148
00:08:03.781 --> 00:08:05.593
<v SPEAKER_01>more people start Getting involved.
149
00:08:05.643 --> 00:08:10.406
<v SPEAKER_02> What I would say, I think it's just very difficult without tangible things
150
00:08:10.446 --> 00:08:15.210
<v SPEAKER_02>that the technology does in the world to wake people up to its potential.
151
00:08:15.730 --> 00:08:20.404
<v SPEAKER_02>So for example, if we pause at the current level of capabilities, let's assume we do that.
152
00:08:20.454 --> 00:08:24.977
<v SPEAKER_02>I think, yes, that this process of people waking up continues as a solely,
153
00:08:25.418 --> 00:08:31.263
<v SPEAKER_02>but Just look at the skepticism in the financial markets about the viability
154
00:08:31.303 --> 00:08:33.692
<v SPEAKER_02>of the technology. There's huge skepticism.
155
00:08:33.786 --> 00:08:36.308
<v SPEAKER_02>And that's also probably just shared broadly throughout the public.
156
00:08:36.328 --> 00:08:37.880
<v SPEAKER_02>The public doesn't really like AI.
157
00:08:37.930 --> 00:08:39.902
<v SPEAKER_02>They don't really like data centers and stuff.
158
00:08:39.952 --> 00:08:43.495
<v SPEAKER_02>But that's not because they realize what's going to happen.
159
00:08:43.515 --> 00:08:47.071
<v SPEAKER_02>They just have sort of much more myopic kind of distaste for it.
160
00:08:47.779 --> 00:08:53.241
<v SPEAKER_02> And if we pause now, then people are still not going to understand what's at stake.
161
00:08:53.261 --> 00:08:56.952
<v SPEAKER_02>So I think the public conversation about this will still be very poor
162
00:08:57.002 --> 00:08:59.683
<v SPEAKER_02>because it will be operating from bad premises.
163
00:09:00.303 --> 00:09:04.685
<v SPEAKER_02>So I do think there's an advantage to getting the capabilities to a point
164
00:09:04.925 --> 00:09:09.346
<v SPEAKER_02>where it's evident to everyone that if we keep going from there on,
165
00:09:09.686 --> 00:09:11.937
<v SPEAKER_02>that the world will be totally transformed.
166
00:09:11.987 --> 00:09:15.668
<v SPEAKER_02>Because I think doing this through ordinary persuasion is extremely difficult.
167
00:09:15.688 --> 00:09:18.750
<v SPEAKER_02>I think you might get some kind of Post-politically,
168
00:09:19.590 --> 00:09:25.093
<v SPEAKER_02>but it will be supported by factions who don't actually agree with your worldview.
169
00:09:25.113 --> 00:09:26.914
<v SPEAKER_02>They would support it for some other reason.
170
00:09:26.954 --> 00:09:28.545
<v SPEAKER_02>They don't like big tech companies.
171
00:09:28.595 --> 00:09:31.716
<v SPEAKER_02>They don't like the fact that all these companies
172
00:09:31.736 --> 00:09:36.379
<v SPEAKER_02>that construct all these data centers that the local communities that they're
173
00:09:36.439 --> 00:09:37.679
<v SPEAKER_02>in don't support.
174
00:09:37.699 --> 00:09:40.571
<v SPEAKER_02>It would be for some kind of other reason and not for the reason
175
00:09:40.621 --> 00:09:41.751
<v SPEAKER_02> that you think is most important.
176
00:09:41.801 --> 00:09:46.412
<v SPEAKER_01>I think I technically agree with you, but in spirit disagree, where I think that...
177
00:09:48.083 --> 00:09:49.773
<v SPEAKER_01>Maybe one way of modeling it is something like,
178
00:09:49.823 --> 00:09:52.045
<v SPEAKER_01>for each new AI capability that appears,
179
00:09:52.224 --> 00:09:55.885
<v SPEAKER_01>there's some rapid updates that people make immediately just upon learning
180
00:09:55.925 --> 00:09:56.865
<v SPEAKER_01>that that capability exists,
181
00:09:56.885 --> 00:09:59.516
<v SPEAKER_01>but then there's a whole bunch of additional updates that get made
182
00:09:59.566 --> 00:10:02.416
<v SPEAKER_01>as that capability gets more deployed into the world and so forth.
183
00:10:02.466 --> 00:10:05.617
<v SPEAKER_01>And I think that right now, capabilities progress is moving fast enough
184
00:10:05.667 --> 00:10:10.628
<v SPEAKER_01>that we still haven't nearly exhausted the gains in awareness that would come
185
00:10:10.688 --> 00:10:13.159
<v SPEAKER_01>from just deploying the current capabilities more.
186
00:10:13.209 --> 00:10:16.090
<v SPEAKER_01>And so if we had a pause where we continue to deploy the current capabilities
187
00:10:16.130 --> 00:10:20.612
<v SPEAKER_01>but not make them smarter, I think that we would continue to see significant gains
188
00:10:20.652 --> 00:10:22.633
<v SPEAKER_01>in awareness over the course of the several years,
189
00:10:22.653 --> 00:10:25.375
<v SPEAKER_01>and then it would taper off after more than that.
190
00:10:25.575 --> 00:10:29.588
<v SPEAKER_01>So I do think that things are going fast enough now that to a first approximation,
191
00:10:29.638 --> 00:10:34.201
<v SPEAKER_01>the wake-up is a function of serial time rather than a function of the capabilities,
192
00:10:34.221 --> 00:10:36.993
<v SPEAKER_01>although I do think that there's some function of the capabilities.
193
00:10:37.043 --> 00:10:39.607
<v SPEAKER_01>Another thing I would say too is that Yeah,
194
00:10:39.687 --> 00:10:43.841
<v SPEAKER_01>I think that a lot of the people who have anti-AI opinions don't share my worldview
195
00:10:43.891 --> 00:10:47.391
<v SPEAKER_01>and don't have the anti-AI opinions for the same reasons as me.
196
00:10:48.255 --> 00:10:50.657
<v SPEAKER_01>But that's also changing to a larger extent, right?
197
00:10:50.677 --> 00:10:54.810
<v SPEAKER_01>Like we've seen multiple senators and congresspeople come out and say like,
198
00:10:54.860 --> 00:10:57.633
<v SPEAKER_01>AI could kill us all and like the AIs could go rogue and things like that.
199
00:10:57.683 --> 00:11:00.255
<v SPEAKER_01>And that's mostly happened just in the last year.
200
00:11:00.305 --> 00:11:01.805
<v SPEAKER_01>And so I think that like...
201
00:11:02.186 --> 00:11:05.853
<v SPEAKER_01>That too is trending in what I would consider the right direction,
202
00:11:06.310 --> 00:11:10.810
<v SPEAKER_01>where people are waking up and understanding the magnitude of the situation more.
203
00:11:11.675 --> 00:11:13.917
<v SPEAKER_01>I don't think it's trending fast enough in the right direction.
204
00:11:13.937 --> 00:11:18.020
<v SPEAKER_01>I don't think that it's going to be where it needs to be in 12 months,
205
00:11:18.260 --> 00:11:22.344
<v SPEAKER_01>but I think in 24 months maybe, or in 36 months maybe.
206
00:11:23.024 --> 00:11:25.547
<v SPEAKER_02>I agree with the point that if you pause now,
207
00:11:25.567 --> 00:11:29.345
<v SPEAKER_02>you will still get an increase in awareness for a couple more years.
208
00:11:30.028 --> 00:11:34.211
<v SPEAKER_02>But given the distance between where we are now and where I think people need
209
00:11:34.231 --> 00:11:35.932
<v SPEAKER_02>to get, given the implications of technology,
210
00:11:35.952 --> 00:11:39.964
<v SPEAKER_02>I think that's just not gonna happen if we pause at the current level capabilities.
211
00:11:40.014 --> 00:11:41.070
<v SPEAKER_02>It might be enough.
212
00:11:41.495 --> 00:11:44.308
<v SPEAKER_02>Like you might have the view that Current level of support
213
00:11:44.348 --> 00:11:49.553
<v SPEAKER_02>and current political coalitions or whatever is sufficient to get a pause to happen.
214
00:11:49.713 --> 00:11:53.046
<v SPEAKER_02>And then that has the benefits that you care about, that it slows things down,
215
00:11:53.096 --> 00:11:57.500
<v SPEAKER_02>even though it's not done with like a complete understanding of like what's going
216
00:11:57.520 --> 00:11:59.612
<v SPEAKER_02>to happen. It's not for different motivations. It's complete.
217
00:11:59.662 --> 00:12:01.664
<v SPEAKER_02>I think it's a defensible position.
218
00:12:02.985 --> 00:12:08.129
<v SPEAKER_02>I'm just worried in like the longer term that if we as a...
219
00:12:09.090 --> 00:12:13.312
<v SPEAKER_02>Civilization just insists on being irrational about this topic,
220
00:12:13.352 --> 00:12:15.632
<v SPEAKER_02>then we will just make a lot of bad choices,
221
00:12:15.653 --> 00:12:17.983
<v SPEAKER_02>a lot of choices that don't make much sense.
222
00:12:18.033 --> 00:12:23.137
<v SPEAKER_02>And I think it's important for aware,
223
00:12:24.656 --> 00:12:27.737
<v SPEAKER_02>people need to understand that in some ways,
224
00:12:29.738 --> 00:12:35.004
<v SPEAKER_02>the world we've been in It's gonna no longer exist in some sense.
225
00:12:35.064 --> 00:12:36.496
<v SPEAKER_02>Even if the outcome is very good for us,
226
00:12:36.546 --> 00:12:40.572
<v SPEAKER_02>like when you get Daniel's ideal outcome or something like that.
227
00:12:40.793 --> 00:12:44.460
<v SPEAKER_02>Well, that world is still completely different from today's world.
228
00:12:44.538 --> 00:12:48.082
<v SPEAKER_02>And people don't realize, I mean, maybe if they realize they were like, well, wait,
229
00:12:48.122 --> 00:12:49.423
<v SPEAKER_02>we don't want that world.
230
00:12:49.443 --> 00:12:51.265
<v SPEAKER_02>Like that doesn't fit our preference.
231
00:12:51.305 --> 00:12:56.009
<v SPEAKER_02>But then if like there is never an explicit conversation that has
232
00:12:56.029 --> 00:12:58.761
<v SPEAKER_02>the correct factual premises about what's going to happen,
233
00:12:58.811 --> 00:13:02.978
<v SPEAKER_02>then we will just be like, we will just not be in control of the situation.
234
00:13:03.314 --> 00:13:04.796
<v SPEAKER_02>Because even though in some sense,
235
00:13:04.816 --> 00:13:07.398
<v SPEAKER_02>like we are in control in a sense that all the relevant decisions that just
236
00:13:07.418 --> 00:13:09.149
<v SPEAKER_02>for a while are being made by humans,
237
00:13:09.199 --> 00:13:13.683
<v SPEAKER_02>they are not being made as a result of some rational deliberation about-
238
00:13:14.693 --> 00:13:16.124
<v SPEAKER_02>And I'm really worried about that.
239
00:13:16.174 --> 00:13:17.956
<v SPEAKER_02>Like I think some random thing is going to happen
240
00:13:17.996 --> 00:13:22.840
<v SPEAKER_02>and like we won't control what happens and it will not be the output of any process
241
00:13:22.860 --> 00:13:24.027
<v SPEAKER_02>that makes any sense.
242
00:13:24.461 --> 00:13:26.053
<v SPEAKER_02>And then we will have to live with it.
243
00:13:26.103 --> 00:13:27.770
<v SPEAKER_02>And I think that's very scary.
244
00:13:28.221 --> 00:13:30.554
<v SPEAKER_02> And I think that's a reason to go slower.
245
00:13:30.902 --> 00:13:37.826
<v SPEAKER_02>I think it's a reason to go slower after sufficiently many people are aware
246
00:13:37.866 --> 00:13:43.088
<v SPEAKER_02>of the potential technology, or at least it will become by serial time.
247
00:13:43.108 --> 00:13:44.369
<v SPEAKER_02>And you think that it's too early for that?
248
00:13:44.409 --> 00:13:45.687
<v SPEAKER_02>I think it's too early.
249
00:13:46.015 --> 00:13:50.257
<v SPEAKER_01>Well, then what about instead of going to a complete pause, going to like a slower,
250
00:13:50.297 --> 00:13:54.959
<v SPEAKER_01>like say we do the thing where we restrict AIR&D compute to like 10% or 5%
251
00:13:55.059 --> 00:13:56.759
<v SPEAKER_01>of the company's compute.
252
00:13:57.420 --> 00:14:00.981
<v SPEAKER_01>And this like slashes the overall pace of progress by like a factor of two or three
253
00:14:01.021 --> 00:14:02.161
<v SPEAKER_01>or something.
254
00:14:02.882 --> 00:14:06.003
<v SPEAKER_01>Then like, perhaps you would agree then that like, well,
255
00:14:06.023 --> 00:14:07.554
<v SPEAKER_01>because you are still making forward progress,
256
00:14:07.604 --> 00:14:10.305
<v SPEAKER_01>you are still going to get the levels of awareness eventually.
257
00:14:10.325 --> 00:14:11.345
<v SPEAKER_01>Yeah.
258
00:14:11.505 --> 00:14:12.806
<v SPEAKER_02> So I think a couple of things about that.
259
00:14:12.826 --> 00:14:16.150
<v SPEAKER_02>Like, first of all, I don't know how to get international coordination for this.
260
00:14:16.200 --> 00:14:17.092
<v SPEAKER_00> Yeah.
261
00:14:17.142 --> 00:14:20.277
<v SPEAKER_02>And given what we're currently doing, I think it's going to be very hard.
262
00:14:20.327 --> 00:14:25.596
<v SPEAKER_02>Because I think the US is being quite adversarial against China, I think, right now.
263
00:14:25.777 --> 00:14:26.777
<v SPEAKER_02>I think...
264
00:14:26.885 --> 00:14:28.356
<v SPEAKER_02>Especially with recent events.
265
00:14:28.406 --> 00:14:31.728
<v SPEAKER_02>I think that just seriously undermines the possibility of getting any coordination.
266
00:14:31.748 --> 00:14:34.192
<v SPEAKER_02>And it's actually very myopic and dangerous.
267
00:14:34.409 --> 00:14:36.580
<v SPEAKER_02>I think they really have to stop doing that.
268
00:14:36.630 --> 00:14:40.963
<v SPEAKER_01>I mean, one of the nice things about the 10% idea is that it would still leave
269
00:14:41.312 --> 00:14:45.444
<v SPEAKER_01>the US companies with about as much compute on AR&D as the Chinese companies.
270
00:14:45.494 --> 00:14:48.886
<v SPEAKER_01>And also because a lot of Chinese progress is just coming from the US.
271
00:14:48.936 --> 00:14:53.278
<v SPEAKER_01>I think that you wouldn't even need a deal to do this level of pacing.
272
00:14:53.439 --> 00:14:56.050
<v SPEAKER_02>For now. But I think that's because China is...
273
00:14:56.753 --> 00:15:03.255
<v SPEAKER_02> Behind on a bunch of the industrial tech that's required to produce a lot of compute.
274
00:15:03.435 --> 00:15:07.216
<v SPEAKER_02>So for example, they don't have access to EUV machines and stuff like this.
275
00:15:07.256 --> 00:15:11.617
<v SPEAKER_02>And the US has been able to get the Netherlands to successfully, you know,
276
00:15:11.637 --> 00:15:12.948
<v SPEAKER_02>export control those and so on.
277
00:15:12.998 --> 00:15:16.399
<v SPEAKER_02>But I think given the China's rate of economic growth and sort
278
00:15:16.419 --> 00:15:19.290
<v SPEAKER_02>of industrial progress, I think these are like temporary advantages.
279
00:15:19.340 --> 00:15:21.007
<v SPEAKER_02>So it gives us like some time.
280
00:15:22.229 --> 00:15:25.201
<v SPEAKER_02>So if you think like, let's say five years is enough, I think five years,
281
00:15:25.251 --> 00:15:27.923
<v SPEAKER_02>China is not going to be able to catch up in five years, probably.
282
00:15:27.973 --> 00:15:30.586
<v SPEAKER_02>So if you think five years is enough, then you can get five years, I think,
283
00:15:30.636 --> 00:15:31.887
<v SPEAKER_02>with a method like this.
284
00:15:31.937 --> 00:15:34.739
<v SPEAKER_02>But if you think we need like 15 years or something like that,
285
00:15:34.759 --> 00:15:36.170
<v SPEAKER_02>then I become like more pessimistic.
286
00:15:36.220 --> 00:15:41.564
<v SPEAKER_00>Or let alone some global agreement about... Because in the limit, it is worth discussing.
287
00:15:41.645 --> 00:15:45.618
<v SPEAKER_00>In the limit, if you really believe we'll have such powerful AI systems...
288
00:15:45.668 --> 00:15:50.051
<v SPEAKER_00> This depends on what you think the nature of destructive technologies is.
289
00:15:51.012 --> 00:15:56.376
<v SPEAKER_00>But it is plausible that you might need some global treaty on, hey,
290
00:15:56.396 --> 00:15:59.558
<v SPEAKER_00>you can't have super intelligent systems that you've deployed
291
00:15:59.598 --> 00:16:01.820
<v SPEAKER_00>to go research mirror life or something.
292
00:16:02.300 --> 00:16:04.301
<v SPEAKER_00>And so at some point, yeah, there's not just a race.
293
00:16:04.321 --> 00:16:06.933
<v SPEAKER_00>Unless you think you're just going to literally...
294
00:16:06.983 --> 00:16:08.164
<v SPEAKER_00> I'll compete every single country.
295
00:16:08.184 --> 00:16:10.686
<v SPEAKER_01>I agree that ultimately, if we want to have a good future,
296
00:16:10.706 --> 00:16:13.268
<v SPEAKER_01>we're probably going to need to make some sort of trade or deal with China
297
00:16:13.288 --> 00:16:14.869
<v SPEAKER_01>and other countries.
298
00:16:14.889 --> 00:16:20.793
<v SPEAKER_02> I think if you're really worried about that risk, there has to be coordination with them.
299
00:16:20.973 --> 00:16:22.394
<v SPEAKER_02>There's no way to avoid that.
300
00:16:22.415 --> 00:16:23.675
<v SPEAKER_02>You can try to delay things.
301
00:16:23.695 --> 00:16:25.362
<v SPEAKER_02>You can have a five-year lead.
302
00:16:25.557 --> 00:16:27.448
<v SPEAKER_02>You're going to have five additional years.
303
00:16:27.498 --> 00:16:28.649
<v SPEAKER_02>That buys you something.
304
00:16:28.699 --> 00:16:34.143
<v SPEAKER_02>But if you're really worried about that risk, China, they could try to build it in five years.
305
00:16:34.183 --> 00:16:35.239
<v SPEAKER_02>It's not that long.
306
00:16:37.306 --> 00:16:40.060
<v SPEAKER_02>Any prospects of coordination with them are, I think,
307
00:16:40.110 --> 00:16:45.899
<v SPEAKER_02>are being severely damaged by the policy of the US government towards China.
308
00:16:46.259 --> 00:16:48.623
<v SPEAKER_02>And also, I mean, to some extent, of anthropic towards China.
309
00:16:48.663 --> 00:16:49.663
<v SPEAKER_02>I agree with that.
310
00:16:49.985 --> 00:16:50.985
<v SPEAKER_02>Yeah.
311
00:16:51.847 --> 00:16:57.451
<v SPEAKER_02> And it's because people don't understand the stakes of the technology.
312
00:16:58.151 --> 00:17:03.635
<v SPEAKER_02>The awareness that this is a world transforming technology that completely changes
313
00:17:03.695 --> 00:17:07.537
<v SPEAKER_02>the condition of civilization, like that is just not there.
314
00:17:08.177 --> 00:17:10.279
<v SPEAKER_02>And we have to figure out a way to deal with it.
315
00:17:10.299 --> 00:17:14.910
<v SPEAKER_02>There's no way to adequately deal with it really without some kind of coordination.
316
00:17:15.982 --> 00:17:18.183
<v SPEAKER_02>People are torpedoing the prospects for doing
317
00:17:18.223 --> 00:17:24.584
<v SPEAKER_02>that for some very short-sighted short-term gain of like, oh,
318
00:17:24.624 --> 00:17:26.984
<v SPEAKER_02>we get a couple years additional lead.
319
00:17:27.645 --> 00:17:30.089
<v SPEAKER_02>It doesn't make sense what people are doing.
320
00:17:30.285 --> 00:17:34.346
<v SPEAKER_02>So I think they're operating from a very different view of what
321
00:17:34.366 --> 00:17:39.211
<v SPEAKER_02>the technology would be like, which I think is going to have bad consequences. Yeah.
322
00:17:39.291 --> 00:17:39.792
<v SPEAKER_02>The other thing
323
00:17:39.832 --> 00:17:42.435
<v SPEAKER_02>that I think this should be discussed is another thing I think is not being
324
00:17:42.455 --> 00:17:43.266
<v SPEAKER_02>discussed.
325
00:17:43.316 --> 00:17:45.999
<v SPEAKER_02>Even in communities where people are trying to think of like, okay, how do we win?
326
00:17:46.019 --> 00:17:48.075
<v SPEAKER_02>How do we get like the safe AI first?
327
00:17:48.462 --> 00:17:51.005
<v SPEAKER_02>Like Gorn had an interesting comment about this, I think on Les Wrong,
328
00:17:51.025 --> 00:17:54.803
<v SPEAKER_02>where he asked the question, okay, like, let's say like the US wins.
329
00:17:55.250 --> 00:17:59.383
<v SPEAKER_02>We get our super intelligence. Okay. Then what? Then what?
330
00:17:59.403 --> 00:18:00.403
<v SPEAKER_02>What do we do?
331
00:18:00.544 --> 00:18:05.048
<v SPEAKER_02>Do we do some crazy operations like try to overthrow the Chinese government
332
00:18:05.068 --> 00:18:08.421
<v SPEAKER_02>or something like that? And if they think that's what the US is going to do,
333
00:18:08.471 --> 00:18:12.624
<v SPEAKER_02>what are they going to think of any attempt to try to coordinate with them to get
334
00:18:12.674 --> 00:18:13.645
<v SPEAKER_02>a slowdown?
335
00:18:13.695 --> 00:18:17.188
<v SPEAKER_02>Like they're inherently going to be extremely suspicious of any such attempt
336
00:18:17.238 --> 00:18:18.960
<v SPEAKER_02>if they think that is the plan.
337
00:18:19.752 --> 00:18:24.189
<v SPEAKER_00> Even if you don't know my sponsor, WorkOS, you've probably used their products.
338
00:18:24.239 --> 00:18:29.687
<v SPEAKER_00>That's because a bunch of companies like Anthropic, OpenAI, Plaid, Granola,
339
00:18:29.987 --> 00:18:34.554
<v SPEAKER_00>and Whisperflow rely on them behind the scenes to power things like
340
00:18:36.675 --> 00:18:41.842
<v SPEAKER_00> WorkOS has spent the better part of the last decade building these features for human users.
341
00:18:42.279 --> 00:18:45.902
<v SPEAKER_00>And now they've taken that expertise and applied it to agents,
342
00:18:46.282 --> 00:18:50.115
<v SPEAKER_00>building products that let agents log in, grab the right permissions,
343
00:18:50.265 --> 00:18:52.321
<v SPEAKER_00>and take actions within your product.
344
00:18:52.526 --> 00:18:53.526
<v SPEAKER_00>Take AgentAuth.
345
00:18:53.667 --> 00:18:58.220
<v SPEAKER_00>You start by defining permissions for the most powerful agents that you'd be comfortable with.
346
00:18:58.270 --> 00:19:01.062
<v SPEAKER_00> Now, not every agent will actually get these permissions.
347
00:19:01.112 --> 00:19:02.223
<v SPEAKER_00>This is just your ceiling.
348
00:19:02.273 --> 00:19:05.856
<v SPEAKER_00>Then, whenever a user kicks off an agent in your product,
349
00:19:06.436 --> 00:19:11.160
<v SPEAKER_00>AgentAuth checks that user's permissions against the ceiling and only grants
350
00:19:11.200 --> 00:19:14.200
<v SPEAKER_00>the agent the permissions that show up in both places.
351
00:19:14.423 --> 00:19:18.479
<v SPEAKER_00>WorkOS does all this with the users and roles that you've already set up,
352
00:19:18.786 --> 00:19:22.519
<v SPEAKER_00>so you can give every agent the exact permissions that it should have,
353
00:19:22.569 --> 00:19:25.501
<v SPEAKER_00>without ever needing to build a separate permission system.
354
00:19:25.551 --> 00:19:29.873
<v SPEAKER_00> Go to workos.com slash oddkit to learn more.
355
00:19:30.753 --> 00:19:33.654
<v SPEAKER_00>I think people correctly point out that I have too many people on my podcast
356
00:19:33.674 --> 00:19:38.196
<v SPEAKER_00>who have this particular view of AI trajectories and then not only AI trajectories
357
00:19:38.216 --> 00:19:40.438
<v SPEAKER_00>but the implications of that trajectory.
358
00:19:40.937 --> 00:19:46.980
<v SPEAKER_00>However, it does end up being the case that when you talk to a skeptic, it just,
359
00:19:47.080 --> 00:19:48.480
<v SPEAKER_00>they feel like, for example, Ege,
360
00:19:48.500 --> 00:19:52.392
<v SPEAKER_00>it seems like you just have a slightly different probabilities on things.
361
00:19:52.442 --> 00:19:53.609
<v SPEAKER_00>It's not even that...
362
00:19:53.899 --> 00:19:56.510
<v SPEAKER_00>The people who totally dismiss this altogether,
363
00:19:56.740 --> 00:19:58.361
<v SPEAKER_00>I feel like don't have reasonable arguments
364
00:19:58.381 --> 00:20:00.825
<v SPEAKER_00>about why AI capabilities will not continue.
365
00:20:02.122 --> 00:20:07.604
<v SPEAKER_00>And if you take seriously the possibility of minds in data centers
366
00:20:07.644 --> 00:20:12.605
<v SPEAKER_00>that learn like humans and which will swamp us in population, thinking speed,
367
00:20:13.426 --> 00:20:18.027
<v SPEAKER_00>agglomerated experience and expertise, et cetera, no people who take that seriously,
368
00:20:18.047 --> 00:20:19.714
<v SPEAKER_00>at least so far as I've found,
369
00:20:21.520 --> 00:20:27.386
<v SPEAKER_00>Put like less than 10% or less than 5% that things go pretty badly for biological humans.
370
00:20:27.967 --> 00:20:30.239
<v SPEAKER_02>Yeah, I mean, this is something I'm trying to emphasize like whenever,
371
00:20:30.289 --> 00:20:32.831
<v SPEAKER_02>because like I think like I can be,
372
00:20:32.952 --> 00:20:35.394
<v SPEAKER_02>like by people who don't have enough context on the situation
373
00:20:35.434 --> 00:20:39.288
<v SPEAKER_02>or like we're not carefully reading to, reading what I'm saying or whatever,
374
00:20:39.338 --> 00:20:41.838
<v SPEAKER_02>I could be considered this person who's like,
375
00:20:41.996 --> 00:20:46.262
<v SPEAKER_02>Like who disagrees with Daniel or like I give two or three times less probability
376
00:20:46.282 --> 00:20:47.985
<v SPEAKER_02>to various things compared to Daniel or something like that.
377
00:20:48.005 --> 00:20:51.460
<v SPEAKER_02>But I think like that's actually not that important in some sense.
378
00:20:51.510 --> 00:20:54.314
<v SPEAKER_02>There are some things for which like a three or four X difference can make a difference.
379
00:20:54.334 --> 00:20:58.616
<v SPEAKER_02>Like if you think the risk of doom right now is 4 % a year compared to 1%,
380
00:20:58.616 --> 00:21:00.159
<v SPEAKER_02>I think that can actually make a difference
381
00:21:00.179 --> 00:21:02.650
<v SPEAKER_02>for whether you think like we should pause or not.
382
00:21:02.700 --> 00:21:06.531
<v SPEAKER_02>That's because you're comparing it to like the 1% per year of people who are dying.
383
00:21:06.581 --> 00:21:12.562
<v SPEAKER_02>Then whether you think the risk per year from AI is higher than that or lower
384
00:21:12.582 --> 00:21:15.693
<v SPEAKER_02>than that, like that's an important analytical question.
385
00:21:16.053 --> 00:21:20.637
<v SPEAKER_02>But compared to the people who just don't take the technology seriously
386
00:21:21.058 --> 00:21:26.582
<v SPEAKER_02>or who have what I would call magical views about the human mind or something,
387
00:21:26.622 --> 00:21:30.186
<v SPEAKER_02>which are very widespread, then I think all of those people are just
388
00:21:30.226 --> 00:21:31.467
<v SPEAKER_02>in a different world.
389
00:21:31.487 --> 00:21:35.150
<v SPEAKER_02>They're not actually engaged with what's happening.
390
00:21:35.690 --> 00:21:39.574
<v SPEAKER_02>And I think if they were making predictions over the past few years or five years
391
00:21:39.594 --> 00:21:41.576
<v SPEAKER_02>or whatever, they would have been very, very wrong.
392
00:21:41.596 --> 00:21:43.958
<v SPEAKER_02>I think all their predictions would have been completely wrong.
393
00:21:44.008 --> 00:21:47.320
<v SPEAKER_02>Often they don't make predictions, so they're not proven wrong.
394
00:21:47.370 --> 00:21:52.374
<v SPEAKER_00>Actually, should we even discuss what you, Daniel, predicted in AI 2027,
395
00:21:52.634 --> 00:21:55.976
<v SPEAKER_00>which was released in the beginning of 2025?
396
00:21:56.677 --> 00:22:00.288
<v SPEAKER_00>What did you predict that the world would look like in late 2026?
397
00:22:00.418 --> 00:22:06.424
<v SPEAKER_01>I think the biggest thing that was incorrect was we said China wakes up in summer of 2026.
398
00:22:06.905 --> 00:22:10.128
<v SPEAKER_01>And there has been a lot of like wake up, so to speak, in China.
399
00:22:10.148 --> 00:22:14.092
<v SPEAKER_01>They've started talking a lot more about existential risk and alignment
400
00:22:14.172 --> 00:22:16.184
<v SPEAKER_01>and superintelligence and things like that,
401
00:22:16.234 --> 00:22:18.497
<v SPEAKER_01>but not to the same extent that we predicted.
402
00:22:18.537 --> 00:22:20.839
<v SPEAKER_01>So they haven't, as far as we know,
403
00:22:20.919 --> 00:22:24.652
<v SPEAKER_01>they haven't like Got the state seriously involved in their AI projects
404
00:22:24.692 --> 00:22:29.195
<v SPEAKER_01>and started funding them more and sharing algorithms and things like
405
00:22:29.215 --> 00:22:30.604
<v SPEAKER_01>that and merging compute.
406
00:22:30.956 --> 00:22:32.697
<v SPEAKER_01>So that was definitely one thing that got wrong.
407
00:22:32.737 --> 00:22:36.480
<v SPEAKER_01>I think that some of the stuff we got right were kind of relatively obvious,
408
00:22:36.520 --> 00:22:40.131
<v SPEAKER_01>like the rise of agents, the rise of coding agents in particular.
409
00:22:40.843 --> 00:22:44.843
<v SPEAKER_01>Early 2026, the title of our chapter there was called Coding Automation,
410
00:22:45.826 --> 00:22:48.882
<v SPEAKER_01>which coincided very nicely with Cloud Code taking off.
411
00:22:49.750 --> 00:22:50.000
<v SPEAKER_02>Yeah.
412
00:22:50.050 --> 00:22:53.142
<v SPEAKER_02>And I think the revenue projections, if anything, were slightly too pessimistic.
413
00:22:53.192 --> 00:22:53.462
<v SPEAKER_02>Yeah.
414
00:22:53.512 --> 00:22:56.253
<v SPEAKER_02>But pessimistic in the sense that they would lower than what ended up happening.
415
00:22:56.293 --> 00:22:59.315
<v SPEAKER_02>But at the same time, I think it looks like at the end of the year,
416
00:22:59.335 --> 00:23:03.597
<v SPEAKER_02>the market projections seemed like they were too optimistic.
417
00:23:03.897 --> 00:23:05.608
<v SPEAKER_01>I think we said like 30% or something. Yeah.
418
00:23:05.658 --> 00:23:09.870
<v SPEAKER_02>And then if anything, it might end up being like down. Yeah. Only slightly up.
419
00:23:09.920 --> 00:23:11.530
<v SPEAKER_02>Like I think a bunch of AI stocks are down.
420
00:23:11.580 --> 00:23:12.969
<v SPEAKER_02>Nvidia is down and so on.
421
00:23:13.767 --> 00:23:17.369
<v SPEAKER_02>So I think actually that's an interesting thing to also maybe talk
422
00:23:17.389 --> 00:23:20.310
<v SPEAKER_02>about a little bit, because I think there's definitely like, to me,
423
00:23:20.330 --> 00:23:25.373
<v SPEAKER_02>it looks like there is a big cleavage in like worldviews that's happening here
424
00:23:25.613 --> 00:23:28.614
<v SPEAKER_02>between like people in finance, like you would say,
425
00:23:28.634 --> 00:23:33.078
<v SPEAKER_02>like people in New York and people in San Francisco, maybe is one way to put it.
426
00:23:33.454 --> 00:23:37.858
<v SPEAKER_02>People who are viewing these as just ordinary stocks and whatever,
427
00:23:37.878 --> 00:23:41.911
<v SPEAKER_02>they see a lot of business risk, they see a lot of default risk on debts,
428
00:23:41.961 --> 00:23:44.850
<v SPEAKER_02>and the business plan doesn't seem very sustainable,
429
00:23:45.044 --> 00:23:47.866
<v SPEAKER_02>companies are burning a lot of money, or even Antropic,
430
00:23:47.906 --> 00:23:52.099
<v SPEAKER_02>they still have a negative margin or maybe a very, very slightly positive margin.
431
00:23:52.149 --> 00:23:53.731
<v SPEAKER_02>So it seems very risky.
432
00:23:54.451 --> 00:23:58.673
<v SPEAKER_02>And they are like, well, can this really go on for another one or two years?
433
00:23:59.794 --> 00:24:02.815
<v SPEAKER_02> Here people say, well, in one or two years, we might all be dead.
434
00:24:02.865 --> 00:24:04.350
<v SPEAKER_02>So that's a very big...
435
00:24:05.019 --> 00:24:06.379
<v SPEAKER_02> Difference in views.
436
00:24:06.879 --> 00:24:09.460
<v SPEAKER_02>So I think most people in the world,
437
00:24:09.500 --> 00:24:11.400
<v SPEAKER_02>most people who have a lot of money or whatever,
438
00:24:11.420 --> 00:24:13.971
<v SPEAKER_02>they still don't believe any of this, basically.
439
00:24:14.021 --> 00:24:17.782
<v SPEAKER_02>I think not only do they not believe what Daniel is saying,
440
00:24:18.202 --> 00:24:23.203
<v SPEAKER_02>I think there is just a general, complete skepticism of the technology,
441
00:24:23.763 --> 00:24:25.393
<v SPEAKER_02>despite what has already happened.
442
00:24:25.443 --> 00:24:31.498
<v SPEAKER_02>People still don't, as far as I can see, just buy this premise that like, Look,
443
00:24:32.159 --> 00:24:34.437
<v SPEAKER_02>like, humans are, like, physical objects.
444
00:24:34.601 --> 00:24:38.373
<v SPEAKER_02>You know, we have some capacities, the brain has some capacities, just a physical object.
445
00:24:38.423 --> 00:24:41.256
<v SPEAKER_02>We have enough resources to reproduce what it does.
446
00:24:41.686 --> 00:24:44.067
<v SPEAKER_02>And then that's obviously going to have, like, complete transformative implications.
447
00:24:44.087 --> 00:24:45.488
<v SPEAKER_02>Like, that is very straightforward.
448
00:24:45.508 --> 00:24:48.921
<v SPEAKER_02>It doesn't really hinge on these details about exactly when it happens.
449
00:24:48.971 --> 00:24:51.633
<v SPEAKER_02>But I think people just don't believe it.
450
00:24:52.093 --> 00:24:57.437
<v SPEAKER_02>It seems to me like this very deep-rooted irrationality that is tied to...
451
00:24:58.273 --> 00:25:00.755
<v SPEAKER_02> You know, maybe like lingering notions of the human soul or whatever.
452
00:25:00.795 --> 00:25:03.297
<v SPEAKER_02>Like, I think like there's a lot of this going on where like people don't want
453
00:25:03.317 --> 00:25:05.529
<v SPEAKER_02>to confront the reality of what's happening.
454
00:25:05.579 --> 00:25:09.732
<v SPEAKER_02>Like the basic thing is that there is a massive transformation that's going to happen.
455
00:25:09.782 --> 00:25:12.774
<v SPEAKER_02>And like, you need to like understand it's going to happen.
456
00:25:12.824 --> 00:25:16.207
<v SPEAKER_02>If you want to talk about like, what do we do? Like, what do we change?
457
00:25:16.227 --> 00:25:17.257
<v SPEAKER_02>How do we adapt to it?
458
00:25:17.307 --> 00:25:18.719
<v SPEAKER_02>You know, what is our plan?
459
00:25:18.769 --> 00:25:20.150
<v SPEAKER_02>Like, we have no plan right now.
460
00:25:20.170 --> 00:25:21.892
<v SPEAKER_02>Like there's nothing, you know.
461
00:25:22.151 --> 00:25:26.575
<v SPEAKER_02>Like the fact that people will be supremacist Superceeded as the things
462
00:25:26.615 --> 00:25:30.238
<v SPEAKER_02>that produce economic value that has dramatic implications.
463
00:25:30.258 --> 00:25:31.769
<v SPEAKER_02>People don't think that's going to happen.
464
00:25:31.819 --> 00:25:34.097
<v SPEAKER_02>So we're doing nothing about that either.
465
00:25:34.242 --> 00:25:36.924
<v SPEAKER_02>So like there's just a bunch of ways in which this transformation
466
00:25:36.964 --> 00:25:41.708
<v SPEAKER_02>of the world should affect like we should be talking about like what we're going
467
00:25:41.728 --> 00:25:42.611
<v SPEAKER_02>to do.
468
00:25:42.661 --> 00:25:44.883
<v SPEAKER_00> And we're not doing that because people don't think it's going to happen.
469
00:25:44.903 --> 00:25:49.766
<v SPEAKER_00>Well, not only that, but when you do talk about it, there's just a huge, huge backlash.
470
00:25:49.946 --> 00:25:50.946
<v SPEAKER_00>Yeah.
471
00:25:51.087 --> 00:25:56.254
<v SPEAKER_00>Because I think it's just very psychologically disturbing to take this possibility seriously.
472
00:25:57.592 --> 00:26:02.481
<v SPEAKER_00>So I released this article about the Hugging Face incident where I summarized the story.
473
00:26:02.596 --> 00:26:06.549
<v SPEAKER_00>And there's a huge backlash to the fact that I used the word civilization in it
474
00:26:06.599 --> 00:26:08.540
<v SPEAKER_00>to describe these Asian swarms.
475
00:26:09.161 --> 00:26:11.883
<v SPEAKER_00>And then at the time I thought to myself, well...
476
00:26:11.967 --> 00:26:13.998
<v SPEAKER_00> I would have never guessed that this would have happened.
477
00:26:14.048 --> 00:26:18.160
<v SPEAKER_00>But if I had anticipated it, maybe I could have just avoided using that word.
478
00:26:18.210 --> 00:26:22.432
<v SPEAKER_00>And so people could actually read what happened and understand the incident.
479
00:26:22.933 --> 00:26:24.674
<v SPEAKER_00>And then I thought to myself, I don't think it would have mattered.
480
00:26:24.694 --> 00:26:26.465
<v SPEAKER_00>I think there would have been something else.
481
00:26:26.515 --> 00:26:31.071
<v SPEAKER_00>Because I think you need to find something so you can't focus on the story itself.
482
00:26:32.688 --> 00:26:34.299
<v SPEAKER_00>Because you do realize the nature of the story.
483
00:26:34.319 --> 00:26:38.592
<v SPEAKER_00>I mean, forget about the misalignment, just the nature of the capabilities growth.
484
00:26:38.642 --> 00:26:39.642
<v SPEAKER_00>Then...
485
00:26:40.833 --> 00:26:43.466
<v SPEAKER_00> One, it's just not a comfortable thing to think about.
486
00:26:43.516 --> 00:26:46.572
<v SPEAKER_00>Two, it makes a lot of other priorities you might have.
487
00:26:46.841 --> 00:26:49.234
<v SPEAKER_00>A lot of other topics you might want to focus on instead.
488
00:26:49.284 --> 00:26:51.166
<v SPEAKER_00>Much less relevant.
489
00:26:51.687 --> 00:26:53.187
<v SPEAKER_00>With regards to the plan...
490
00:26:54.952 --> 00:26:59.374
<v SPEAKER_00>I've been reading these accounts
491
00:27:00.195 --> 00:27:02.584
<v SPEAKER_00>of what has gone wrong in wars in the past.
492
00:27:02.896 --> 00:27:05.948
<v SPEAKER_00>And again, I know you've done much more deep dive on these kinds of things.
493
00:27:05.998 --> 00:27:09.580
<v SPEAKER_00>But why, for example, did World War I turn into a catastrophe?
494
00:27:09.820 --> 00:27:11.771
<v SPEAKER_00>Why did America send troops into Vietnam?
495
00:27:11.821 --> 00:27:12.877
<v SPEAKER_00>Why did we do Iraq?
496
00:27:13.847 --> 00:27:16.718
<v SPEAKER_00>And what you find in many of these situations is it was not
497
00:27:16.768 --> 00:27:20.919
<v SPEAKER_00>as if the relevant political leaders got in a room and they had a discussion
498
00:27:20.969 --> 00:27:24.490
<v SPEAKER_00>about the pros and cons, the cost of benefits, how things could go wrong,
499
00:27:24.530 --> 00:27:27.311
<v SPEAKER_00>for example, if we invade China, if you're Japan,
500
00:27:27.871 --> 00:27:31.112
<v SPEAKER_00>or if you give some security guarantee to Belgium,
501
00:27:31.732 --> 00:27:34.202
<v SPEAKER_00>or if you send half a million troops into Vietnam.
502
00:27:34.252 --> 00:27:38.043
<v SPEAKER_00>But then what if things escalate and we don't expect, is that worth the benefits?
503
00:27:38.093 --> 00:27:41.341
<v SPEAKER_00>Instead, what has happened in these cases is When people try
504
00:27:41.361 --> 00:27:43.192
<v SPEAKER_00>to analyze why things went wrong,
505
00:27:43.242 --> 00:27:48.103
<v SPEAKER_00>is that there actually never was a clear decision that was made in the first place.
506
00:27:49.404 --> 00:27:51.945
<v SPEAKER_00>There never was an accounting of like, this is what could go wrong.
507
00:27:51.985 --> 00:27:53.905
<v SPEAKER_00>This is what the benefits could be.
508
00:27:53.955 --> 00:27:55.176
<v SPEAKER_00>Do we think it is worth it?
509
00:27:55.226 --> 00:27:59.647
<v SPEAKER_02>And often the people who try to make that discussion happen get socially punished for it.
510
00:27:59.667 --> 00:28:01.988
<v SPEAKER_02>So for example, in Japan, there was a...
511
00:28:02.788 --> 00:28:06.841
<v SPEAKER_02>A member of parliament, I forgot his name, but during the war with China,
512
00:28:06.891 --> 00:28:09.072
<v SPEAKER_02>he stood up in parliament and was like,
513
00:28:09.092 --> 00:28:13.175
<v SPEAKER_02>so can someone explain to me what is the point of this war?
514
00:28:13.215 --> 00:28:14.493
<v SPEAKER_02>Why are we in this war?
515
00:28:15.376 --> 00:28:17.765
<v SPEAKER_02>And then they kicked him out of parliament.
516
00:28:19.204 --> 00:28:22.486
<v SPEAKER_02>And it's just such an obvious rational question. Why are we doing this?
517
00:28:22.526 --> 00:28:23.526
<v SPEAKER_02>What is the point?
518
00:28:23.907 --> 00:28:26.228
<v SPEAKER_02>And then the motivation, actually, if you look at that war phrase, I mean,
519
00:28:26.248 --> 00:28:28.229
<v SPEAKER_02>it was very religious in many ways.
520
00:28:28.289 --> 00:28:34.372
<v SPEAKER_02>Like, oh, Japan has a civilizing mission to save and liberate East Asia or whatever.
521
00:28:34.392 --> 00:28:37.336
<v SPEAKER_02>But then what they actually did was totally not that.
522
00:28:37.454 --> 00:28:42.557
<v SPEAKER_02>So it seems like it was not at all the decisions that were rationally made.
523
00:28:42.577 --> 00:28:43.637
<v SPEAKER_02>I agree with you.
524
00:28:43.777 --> 00:28:45.378
<v SPEAKER_02>Often these things are not planned.
525
00:28:45.398 --> 00:28:48.240
<v SPEAKER_02>And then, of course, then things end up badly.
526
00:28:49.040 --> 00:28:52.025
<v SPEAKER_02>For the AI thing broadly, what I would say is that there's this quote
527
00:28:52.045 --> 00:28:57.472
<v SPEAKER_02>from Nietzsche, which is, he wrote like, God is dead,
528
00:28:57.813 --> 00:29:00.807
<v SPEAKER_02>but for given the way of man for many thousands of years,
529
00:29:00.857 --> 00:29:04.302
<v SPEAKER_02>there may be caves in which his shadow will be shown and we have
530
00:29:04.322 --> 00:29:05.822
<v SPEAKER_02>to vanquish his shadow too.
531
00:29:06.544 --> 00:29:09.906
<v SPEAKER_02> And I think like that is sort of what AI is doing.
532
00:29:10.227 --> 00:29:15.650
<v SPEAKER_02>Like basically we have all these sort of almost quasi-religious beliefs about the human mind.
533
00:29:16.310 --> 00:29:19.472
<v SPEAKER_02>And I think all of them are gonna be undermined.
534
00:29:20.333 --> 00:29:21.944
<v SPEAKER_02>And some people like realize this already,
535
00:29:21.994 --> 00:29:25.766
<v SPEAKER_02>like some people already realize God is dead in the sense, but then like,
536
00:29:25.816 --> 00:29:30.400
<v SPEAKER_02>His shadow are just the things that we believe that are left
537
00:29:30.540 --> 00:29:33.522
<v SPEAKER_02>over from our religious view of humanity.
538
00:29:34.143 --> 00:29:36.625
<v SPEAKER_02>And I think that's going to have to go away.
539
00:29:37.625 --> 00:29:38.926
<v SPEAKER_00>So let's step back.
540
00:29:39.607 --> 00:29:43.520
<v SPEAKER_00>The argument for continuing AI progress now is that you will get better models.
541
00:29:43.570 --> 00:29:46.042
<v SPEAKER_00>Those better models will help you do security work,
542
00:29:46.092 --> 00:29:49.274
<v SPEAKER_00>even formally verifying that your model weights
543
00:29:49.334 --> 00:29:51.736
<v SPEAKER_00>and algorithmic secrets are extremely safe,
544
00:29:51.956 --> 00:29:54.098
<v SPEAKER_00>rewriting the entirety of Slack
545
00:29:54.158 --> 00:30:00.220
<v SPEAKER_00>in a You will be doing alignment research
546
00:30:00.220 --> 00:30:03.183
<v SPEAKER_00>on the models that are closer to the ones
547
00:30:03.183 --> 00:30:05.153
<v SPEAKER_00>that will actually fully automate AI Research.
548
00:30:05.153 --> 00:30:08.529
<v SPEAKER_00>And so what do you make of the argument that the progress
549
00:30:09.303 --> 00:30:12.247
<v SPEAKER_00>at this pace should continue for three more months or six more months?
550
00:30:12.247 --> 00:30:18.458
<v SPEAKER_00>And then you use that crescendo where all this progress and alignment
551
00:30:18.458 --> 00:30:23.014
<v SPEAKER_00>and security could be concentrated to make sure that super intelligent systems have
552
00:30:23.014 --> 00:30:24.110
<v SPEAKER_00>the values we want them to have.
553
00:30:24.110 --> 00:30:26.631
<v SPEAKER_01>Sounds like a really dangerous plan to me.
554
00:30:28.052 --> 00:30:29.353
<v SPEAKER_01>You could make the argument in the past.
555
00:30:29.393 --> 00:30:30.954
<v SPEAKER_01>Maybe in 2020, you could say that, well,
556
00:30:30.974 --> 00:30:34.105
<v SPEAKER_01>we still haven't figured out how to train these things into being agents.
557
00:30:34.155 --> 00:30:37.897
<v SPEAKER_01>And so probably whatever alignment techniques we do
558
00:30:38.177 --> 00:30:42.980
<v SPEAKER_01>on pure predictive language models aren't going to generalize or teach us that much
559
00:30:43.140 --> 00:30:45.741
<v SPEAKER_01>about how to align AI agents.
560
00:30:47.382 --> 00:30:50.704
<v SPEAKER_01>Well, now we have AI agents, and I think not only do we have AI agents,
561
00:30:50.744 --> 00:30:54.286
<v SPEAKER_01>but we are potentially very close to the singularity,
562
00:30:54.886 --> 00:30:57.297
<v SPEAKER_01>the AI agents that would automate the AI R&D.
563
00:30:57.347 --> 00:31:04.250
<v SPEAKER_01>And so I think it's like, okay, well, now it's time to start slowing down or stopping.
564
00:31:04.310 --> 00:31:08.633
<v SPEAKER_01>I no longer buy the argument that our alignment research isn't that valuable
565
00:31:08.693 --> 00:31:12.637
<v SPEAKER_01>because our current systems are just too different from future systems.
566
00:31:14.272 --> 00:31:17.225
<v SPEAKER_01> They are very different from superintelligence, that's for sure.
567
00:31:17.275 --> 00:31:21.698
<v SPEAKER_01>But they're not very different from the type of AI that will potentially pose
568
00:31:21.738 --> 00:31:24.950
<v SPEAKER_01>a threat because it's the type of AI that's automating the AI research process.
569
00:31:25.000 --> 00:31:28.393
<v SPEAKER_01>And therefore, if it's misaligned, those misalignments can continue into the future.
570
00:31:28.443 --> 00:31:30.654
<v SPEAKER_01>And also, if it's just not doing its job very well,
571
00:31:30.704 --> 00:31:34.107
<v SPEAKER_01>like if it's more interested in apparent success than actual success,
572
00:31:34.127 --> 00:31:37.569
<v SPEAKER_01>then it produces alignment solutions that don't actually work but appear to work.
573
00:31:37.589 --> 00:31:41.256
<v SPEAKER_00>But isn't another way to say what you're saying is that we need...
574
00:31:42.092 --> 00:31:42.973
<v SPEAKER_00>Even forgetting about the pause,
575
00:31:42.993 --> 00:31:47.493
<v SPEAKER_00>the thing we right now need more than anything is a capable alignment researcher.
576
00:31:47.955 --> 00:31:49.787
<v SPEAKER_00>A capable and trustworthy alignment researcher.
577
00:31:49.837 --> 00:31:51.037
<v SPEAKER_01>That's one of the things the pause should produce.
578
00:31:51.077 --> 00:31:55.080
<v SPEAKER_01>I mean, I also think that the AI is doing the intelligence explosion are going to be
579
00:31:55.120 --> 00:31:58.372
<v SPEAKER_01>under all sorts of external constraints too, just like today's current researchers,
580
00:31:58.422 --> 00:31:59.352
<v SPEAKER_01>right?
581
00:31:59.402 --> 00:32:04.285
<v SPEAKER_01>It might be the case that like, you know, like take chain of thought monitorability,
582
00:32:04.885 --> 00:32:07.968
<v SPEAKER_01>you know, this is a classic example of something that like,
583
00:32:08.018 --> 00:32:10.712
<v SPEAKER_01>We sort of all agree it would be nice if the Chain of Thought were more monitorable,
584
00:32:10.762 --> 00:32:13.046
<v SPEAKER_01>but also the things that you would do
585
00:32:13.066 --> 00:32:16.390
<v SPEAKER_01>to make it more monitorable might make your system more expensive for a given level
586
00:32:16.431 --> 00:32:19.625
<v SPEAKER_01>of capability or less capable at a given level of expense.
587
00:32:19.675 --> 00:32:20.597
<v SPEAKER_01>And the things that you would do
588
00:32:20.617 --> 00:32:25.203
<v SPEAKER_01>to make your system more capable often sometimes I think there's going to be loads
589
00:32:25.243 --> 00:32:27.176
<v SPEAKER_01>of trade-offs like that everywhere.
590
00:32:27.226 --> 00:32:30.010
<v SPEAKER_01>And so even if you have managed to succeed in making
591
00:32:30.050 --> 00:32:34.186
<v SPEAKER_01>an automated alignment researcher that's genuinely honest and genuinely cares
592
00:32:34.236 --> 00:32:40.031
<v SPEAKER_01>in a robust way about doing its job and solving alignment for you, Well,
593
00:32:40.051 --> 00:32:41.742
<v SPEAKER_01>if you're doing an intelligence explosion,
594
00:32:41.792 --> 00:32:47.055
<v SPEAKER_01>then it's going to be facing all these trade-offs where it has to do the thing
595
00:32:47.075 --> 00:32:50.986
<v SPEAKER_01>that even by its own lights is a little bit more risky because it doesn't have
596
00:32:51.036 --> 00:32:54.258
<v SPEAKER_01>the compute or the time to do the safer thing.
597
00:32:54.678 --> 00:33:00.001
<v SPEAKER_00>Seems like a big concern of yours with regards to an intelligence explosion soon is
598
00:33:00.041 --> 00:33:02.782
<v SPEAKER_00>that you don't think the ways
599
00:33:02.842 --> 00:33:07.044
<v SPEAKER_00>in which we have historically made AI systems more aligned and are continuing
600
00:33:07.084 --> 00:33:09.686
<v SPEAKER_00>to make AI systems more aligned And I think that's what I think is going
601
00:33:09.707 --> 00:33:13.374
<v SPEAKER_00>to be especially useful for making superintelligence more aligned.
602
00:33:13.793 --> 00:33:16.957
<v SPEAKER_00>But if I just think about the things we're doing right now, like, hey,
603
00:33:16.997 --> 00:33:18.119
<v SPEAKER_00>let's fix the reward hacks.
604
00:33:18.139 --> 00:33:19.551
<v SPEAKER_00>Let's make better graders.
605
00:33:19.601 --> 00:33:25.208
<v SPEAKER_00>Let's make the gradient of rewards such that The harder you try to cheat in a way
606
00:33:25.248 --> 00:33:27.692
<v SPEAKER_00>that you get caught, the more we punish you.
607
00:33:27.789 --> 00:33:30.960
<v SPEAKER_00>And in fact, if you give evidence of your cheating or you give up early
608
00:33:31.010 --> 00:33:34.162
<v SPEAKER_00>on an impossible task, maybe we will give you the reward you've gotten anyways.
609
00:33:34.212 --> 00:33:35.853
<v SPEAKER_00>Basically build this hill so that yes,
610
00:33:35.893 --> 00:33:38.904
<v SPEAKER_00>if you are super intelligent enough that you can totally break the environment,
611
00:33:38.954 --> 00:33:40.085
<v SPEAKER_00>you'll get the reward.
612
00:33:40.135 --> 00:33:44.577
<v SPEAKER_00>But every climb up this hill of cheating is like more and more punished.
613
00:33:45.742 --> 00:33:50.703
<v SPEAKER_00>And so this kind of just clever engineering work or careful engineering work,
614
00:33:51.324 --> 00:33:54.524
<v SPEAKER_00>is that going to be enough to just train an AI that does what we want it to do
615
00:33:54.564 --> 00:33:56.075
<v SPEAKER_00>the way we want it to do it?
616
00:33:56.125 --> 00:33:59.346
<v SPEAKER_01>So first of all, I don't know if I agree that the AI systems
617
00:33:59.366 --> 00:34:02.866
<v SPEAKER_01>of today are more aligned than the AI systems of two years ago.
618
00:34:03.167 --> 00:34:07.298
<v SPEAKER_01>I think that's kind of an open question and we don't really have good insight into that.
619
00:34:07.348 --> 00:34:11.409
<v SPEAKER_01>I think that I sort of buy
620
00:34:11.529 --> 00:34:14.570
<v SPEAKER_01>the idea in principle that like if you set up
621
00:34:15.796 --> 00:34:19.715
<v SPEAKER_01>The reward environment in the right way, where there's that hill that you mentioned,
622
00:34:19.765 --> 00:34:25.506
<v SPEAKER_01>then It should be possible in principle to set up a reward environment such
623
00:34:25.566 --> 00:34:29.409
<v SPEAKER_01>that the cognitive strategy
624
00:34:29.429 --> 00:34:32.592
<v SPEAKER_01>that does in fact get learned is the cognitive strategy
625
00:34:32.612 --> 00:34:34.143
<v SPEAKER_01>that you want it to get learned.
626
00:34:34.193 --> 00:34:36.195
<v SPEAKER_01>So for example, take honesty.
627
00:34:36.736 --> 00:34:39.568
<v SPEAKER_01>It does seem like it's possible in principle to design
628
00:34:39.618 --> 00:34:44.883
<v SPEAKER_01>a whole training curriculum such that for this AI architecture of this size,
629
00:34:45.523 --> 00:34:47.655
<v SPEAKER_01>when it goes through the training curriculum,
630
00:34:47.705 --> 00:34:51.497
<v SPEAKER_01>It just adopts a policy of I intrinsically value always telling the truth
631
00:34:51.547 --> 00:34:54.209
<v SPEAKER_01>and I'm never going to say anything that I believe to be false or something like
632
00:34:54.229 --> 00:34:57.229
<v SPEAKER_01>that. I definitely agree that's possible in principle.
633
00:34:57.911 --> 00:35:02.134
<v SPEAKER_01>I think that there's a couple of reasons why...
634
00:35:02.194 --> 00:35:04.145
<v SPEAKER_01>First of all, I don't think we've achieved that yet.
635
00:35:04.195 --> 00:35:08.268
<v SPEAKER_01>I think that we have lots of empirical evidence that for some of the key properties
636
00:35:08.318 --> 00:35:11.990
<v SPEAKER_01>that the companies have been trying to get into their AIs, such as honesty,
637
00:35:12.040 --> 00:35:15.318
<v SPEAKER_01>they have not in fact gotten those properties into the AIs.
638
00:35:16.283 --> 00:35:19.116
<v SPEAKER_01>At all. Or like not in, sorry, not in a robust way.
639
00:35:20.687 --> 00:35:24.432
<v SPEAKER_01>So I think, so then there's this, so we, in principle it might be possible,
640
00:35:24.472 --> 00:35:26.972
<v SPEAKER_01>but I think in practice we are not yet there.
641
00:35:27.375 --> 00:35:31.459
<v SPEAKER_01>And also I think that there's a lot of like,
642
00:35:32.787 --> 00:35:34.389
<v SPEAKER_01>I don't know what I'd call it,
643
00:35:34.429 --> 00:35:39.757
<v SPEAKER_01>like a lot of fake solutions that would make it seem like you've succeeded
644
00:35:39.797 --> 00:35:40.797
<v SPEAKER_01>when you haven't.
645
00:35:40.979 --> 00:35:46.487
<v SPEAKER_01>And this is like the classic example of deceptive alignment is a prominent one,
646
00:35:46.587 --> 00:35:47.643
<v SPEAKER_01>but there's others.
647
00:35:47.749 --> 00:35:51.184
<v SPEAKER_01>Basically, there's a lot of ways in which you could do a bunch of that sort of thing
648
00:35:51.234 --> 00:35:55.901
<v SPEAKER_01>and you could convince yourself like, oh, hey, the numbers of cheating went to zero.
649
00:35:55.961 --> 00:35:56.872
<v SPEAKER_01>Maybe we finally did it.
650
00:35:56.922 --> 00:36:01.199
<v SPEAKER_01>Maybe this time it like really doesn't want to cheat and it really is honest.
651
00:36:01.249 --> 00:36:04.812
<v SPEAKER_01>But if only you could sort So if you sort of open up the mind and like look
652
00:36:04.852 --> 00:36:08.584
<v SPEAKER_01>under the hood, you would be like, oh God, it's not actually honest.
653
00:36:08.634 --> 00:36:12.245
<v SPEAKER_01>It's just, you know, become really paranoid about getting caught.
654
00:36:12.475 --> 00:36:16.007
<v SPEAKER_01>We don't have a good way of actually measuring or detecting true alignment
655
00:36:16.057 --> 00:36:18.448
<v SPEAKER_01>and distinguishing it from various other possibilities.
656
00:36:18.498 --> 00:36:20.839
<v SPEAKER_01>And the AIs are not currently aligned.
657
00:36:21.399 --> 00:36:23.960
<v SPEAKER_01>And when I look at the culture at these companies and the sort
658
00:36:23.980 --> 00:36:28.036
<v SPEAKER_01>of like make number go down hill climbing approach to this sort of thing,
659
00:36:28.512 --> 00:36:34.204
<v SPEAKER_01>it seems to me more likely that We're not actually going to correctly solve it.
660
00:36:34.865 --> 00:36:38.606
<v SPEAKER_02>On the current trajectory, I think what's going to happen is that there is going
661
00:36:38.626 --> 00:36:41.927
<v SPEAKER_02>to be enough serious incidents,
662
00:36:42.287 --> 00:36:46.909
<v SPEAKER_02>at least internally inside the labs from trying to deploy these systems and trying
663
00:36:46.929 --> 00:36:49.190
<v SPEAKER_02>to get them to do work in AI research or whatever,
664
00:36:49.210 --> 00:36:51.871
<v SPEAKER_02>that they're going to have enough incidents that they won't even be able to,
665
00:36:51.891 --> 00:36:57.193
<v SPEAKER_02>I think, make progress at a faster rate than getting super intelligence in two years
666
00:36:57.213 --> 00:36:58.213
<v SPEAKER_02>or whatever.
667
00:36:58.833 --> 00:37:01.666
<v SPEAKER_02>My guess is this is already happening inside OpenAI
668
00:37:01.755 --> 00:37:05.026
<v SPEAKER_02>where they're just having issues like deploying their systems
669
00:37:05.076 --> 00:37:07.508
<v SPEAKER_02>because they are having problems with aligning them.
670
00:37:07.558 --> 00:37:10.379
<v SPEAKER_02>And I just expect that kind of thing to continue happening as long
671
00:37:10.419 --> 00:37:11.840
<v SPEAKER_02>as like these problems are not solved.
672
00:37:11.860 --> 00:37:13.521
<v SPEAKER_02>So I put like less weight on the scenario
673
00:37:13.561 --> 00:37:17.163
<v SPEAKER_02>where They perfectly act like they're aligned
674
00:37:17.363 --> 00:37:21.595
<v SPEAKER_02>until the moment they have enough power and then they suddenly execute a coup.
675
00:37:21.645 --> 00:37:27.168
<v SPEAKER_02>As opposed to they are just consistently not aligned and consistently do bad things
676
00:37:27.228 --> 00:37:31.839
<v SPEAKER_02>and don't do the things that they're told, fabricate information, hide information,
677
00:37:32.831 --> 00:37:34.382
<v SPEAKER_02>not follow instructions or whatever.
678
00:37:34.432 --> 00:37:39.155
<v SPEAKER_02>And that just continuously hampers their ability to use them effectively.
679
00:37:39.555 --> 00:37:43.367
<v SPEAKER_02>And as a result of that, the companies just internally are going to have to slow down.
680
00:37:43.417 --> 00:37:48.284
<v SPEAKER_00>Yeah, what do you make of this argument that we are not going to get the singularity
681
00:37:48.624 --> 00:37:52.910
<v SPEAKER_00>at least until alignment is in a good enough position where you can send
682
00:37:52.930 --> 00:37:56.735
<v SPEAKER_00>the swarm out to go reduce perplexity and you can trust that it will do
683
00:37:56.775 --> 00:37:58.553
<v SPEAKER_00>that and it will try to do that?
684
00:38:00.559 --> 00:38:03.161
<v SPEAKER_01>So I do think that there probably will continue,
685
00:38:03.201 --> 00:38:06.814
<v SPEAKER_01>there already have been and will continue to be like micro warning shots
686
00:38:06.864 --> 00:38:11.849
<v SPEAKER_01>of this type where the AI's reward hack or they present some work that's bad work
687
00:38:12.049 --> 00:38:14.901
<v SPEAKER_01>as good and they like hope you don't notice that it's bad.
688
00:38:14.951 --> 00:38:18.424
<v SPEAKER_01>And maybe they even lie to you deliberately in the hopes of making you not notice.
689
00:38:18.474 --> 00:38:20.956
<v SPEAKER_01>That sort of thing has already been happening and will probably continue to happen.
690
00:38:20.976 --> 00:38:24.099
<v SPEAKER_02> I think the severity is going to increase as well.
691
00:38:24.659 --> 00:38:25.678
<v SPEAKER_02>That's the other thing I expect.
692
00:38:25.728 --> 00:38:28.449
<v SPEAKER_01>Yeah. And your claim is that because of this,
693
00:38:28.889 --> 00:38:32.240
<v SPEAKER_01>the companies are going to voluntarily hold off on doing an intelligence explosion?
694
00:38:32.290 --> 00:38:34.091
<v SPEAKER_02> It's not just that they're going to voluntarily hold off.
695
00:38:34.111 --> 00:38:35.922
<v SPEAKER_02>It's that I think they will just be like,
696
00:38:35.972 --> 00:38:40.533
<v SPEAKER_02>they might literally be unable to do it because the way this works is
697
00:38:40.553 --> 00:38:43.435
<v SPEAKER_02>that you send your AI swarm after, you know, like, okay,
698
00:38:43.455 --> 00:38:47.386
<v SPEAKER_02>like find like a bunch of compute multiplier wins on like our pre-training
699
00:38:47.436 --> 00:38:48.146
<v SPEAKER_02>or whatever.
700
00:38:48.196 --> 00:38:54.757
<v SPEAKER_02> And then if the swarm is just like misaligned, like it can easily just Fabricate information.
701
00:38:54.857 --> 00:38:57.278
<v SPEAKER_02>It can not do the experiments properly in a way.
702
00:38:57.298 --> 00:39:01.499
<v SPEAKER_02>It can do them in a biased way to give you the result that looks like
703
00:39:01.519 --> 00:39:04.770
<v SPEAKER_02>the result you want, but is actually not the result you want.
704
00:39:04.820 --> 00:39:09.332
<v SPEAKER_02>The swarm can internally, the members of the swarm can internally lie to each other
705
00:39:09.382 --> 00:39:12.983
<v SPEAKER_02>and stuff like this. And I think that kind of stuff is already kind of happening.
706
00:39:13.023 --> 00:39:15.043
<v SPEAKER_01>It probably is, yeah.
707
00:39:15.103 --> 00:39:17.554
<v SPEAKER_01>Okay, so now my serious answer to this would be something like, well,
708
00:39:17.604 --> 00:39:20.145
<v SPEAKER_01>it's kind of like the Soviet Union...
709
00:39:22.286 --> 00:39:25.651
<v SPEAKER_01>Doing science and industry where it's like, yeah,
710
00:39:26.052 --> 00:39:30.699
<v SPEAKER_01>it suffered a big hit to its overall tech progress and economic growth as a result
711
00:39:30.719 --> 00:39:32.108
<v SPEAKER_01>of these sorts of issues.
712
00:39:32.942 --> 00:39:35.376
<v SPEAKER_01>But nevertheless, it continued to grow and make technological progress.
713
00:39:35.426 --> 00:39:37.989
<v SPEAKER_01>And so I do think I think I would say like, yeah,
714
00:39:38.029 --> 00:39:43.312
<v SPEAKER_01>like if the AIs were like actually trying their best to achieve the singularity
715
00:39:43.332 --> 00:39:48.356
<v SPEAKER_01>as soon as possible, then they would go somewhat faster than in fact they will go
716
00:39:48.456 --> 00:39:50.858
<v SPEAKER_01>because they won't be trying their best to achieve the singularity as soon
717
00:39:50.878 --> 00:39:51.338
<v SPEAKER_01>as possible.
718
00:39:51.358 --> 00:39:56.622
<v SPEAKER_01>They'll be like trying to appear to be doing that, you know, and as I wrote,
719
00:39:56.642 --> 00:39:58.974
<v SPEAKER_01>there'll be lots of inefficiencies and so forth.
720
00:39:59.024 --> 00:40:03.597
<v SPEAKER_01>But nevertheless, I don't think this is going to be look anything like a like pause.
721
00:40:03.647 --> 00:40:05.536
<v SPEAKER_01>I agree. It won't be like a pause.
722
00:40:05.802 --> 00:40:07.414
<v SPEAKER_00>If you're going to be in Sydney for NeurIps,
723
00:40:07.464 --> 00:40:10.739
<v SPEAKER_00>you should consider swinging by an event that my sponsor, Jane Street,
724
00:40:10.789 --> 00:40:12.221
<v SPEAKER_00>is co-hosting with NVIDIA.
725
00:40:12.271 --> 00:40:15.285
<v SPEAKER_00>They're going to be doing a live demo walking through how to build
726
00:40:15.335 --> 00:40:19.812
<v SPEAKER_00>a full quantitative trading system with the Nemetron family of open source models
727
00:40:19.862 --> 00:40:20.862
<v SPEAKER_00>and a DJX Spark.
728
00:40:21.144 --> 00:40:23.922
<v SPEAKER_00> They'll also have food, drinks, music, and games.
729
00:40:24.108 --> 00:40:28.004
<v SPEAKER_00>It's a chance to hang out and meet engineers from both Nvidia and Jane Street.
730
00:40:28.054 --> 00:40:31.629
<v SPEAKER_00>Of course, it wouldn't be a Jane Street event without some sort of possibility.
731
00:40:31.679 --> 00:40:33.251
<v SPEAKER_00>I can't share many details here,
732
00:40:33.301 --> 00:40:35.980
<v SPEAKER_00>but I know that anybody who's able to solve it will have a chance to win
733
00:40:35.980 --> 00:40:38.090
<v SPEAKER_00>a pretty cool NVIDIA -sponsored prize.
734
00:40:38.140 --> 00:40:41.850
<v SPEAKER_00>The event is happening during the evening of December 9th.
735
00:40:41.850 --> 00:40:44.406
<v SPEAKER_00>Spots are limited, so if you'd like to attend,
736
00:40:44.406 --> 00:40:50.293
<v SPEAKER_00>go to jainestreet .com slash Dwarkesh to register your interest.
737
00:40:50.293 --> 00:40:52.779
<v SPEAKER_00>The forum is open until December 4th.
738
00:40:52.779 --> 00:40:57.680
<v SPEAKER_00>I guess I haven't ironed out what you think should happen in the current situation.
739
00:40:57.680 --> 00:41:03.163
<v SPEAKER_00>Do you think in those 20% of worlds where we do get some kind of crazy takeoff
740
00:41:03.423 --> 00:41:08.706
<v SPEAKER_00>over the next few years, that humanity is likely to, quote unquote, lose control?
741
00:41:09.486 --> 00:41:10.487
<v SPEAKER_02>Yeah.
742
00:41:11.027 --> 00:41:14.119
<v SPEAKER_02>So I would distinguish between different kinds of losing control.
743
00:41:14.169 --> 00:41:16.870
<v SPEAKER_02>So I may think it's maybe like a Hansonian point or something,
744
00:41:16.890 --> 00:41:19.842
<v SPEAKER_02>but there's one kind of losing control where you're just invaded
745
00:41:19.892 --> 00:41:21.393
<v SPEAKER_02>by an outside force.
746
00:41:22.533 --> 00:41:25.884
<v SPEAKER_02>Taken over and there's some external power structure that is imposed
747
00:41:25.934 --> 00:41:28.124
<v SPEAKER_02>on the territory that you were in or something like that.
748
00:41:28.174 --> 00:41:29.394
<v SPEAKER_02>But there's another kind of losing control,
749
00:41:29.414 --> 00:41:33.081
<v SPEAKER_02>which is just the way in which we lose control to our descendants.
750
00:41:33.335 --> 00:41:35.095
<v SPEAKER_02>And that happens all the time.
751
00:41:35.476 --> 00:41:39.586
<v SPEAKER_02>And that seems very different in terms of how we should morally think about it
752
00:41:39.636 --> 00:41:43.327
<v SPEAKER_02>or how worried we should be about it compared to an outside force coming
753
00:41:43.377 --> 00:41:44.433
<v SPEAKER_02>in and taking over.
754
00:41:44.557 --> 00:41:46.908
<v SPEAKER_02>And people think very differently about these two cases.
755
00:41:46.958 --> 00:41:48.291
<v SPEAKER_02>So I don't think it's...
756
00:41:48.718 --> 00:41:54.222
<v SPEAKER_02>I think part of the disagreement is that I think about this much more in the vein
757
00:41:54.263 --> 00:41:58.846
<v SPEAKER_02>of we give up control to our descendants instead of we give up control
758
00:41:58.866 --> 00:42:05.211
<v SPEAKER_02>to an outside occupying force who is invading our country or whatever.
759
00:42:05.451 --> 00:42:06.802
<v SPEAKER_02>I think it's an important difference.
760
00:42:06.852 --> 00:42:11.416
<v SPEAKER_00>And why do you think that superintelligence will be more like an invading force
761
00:42:11.836 --> 00:42:13.114
<v SPEAKER_00>than like our children?
762
00:42:13.366 --> 00:42:16.799
<v SPEAKER_01> Well, I think that if we can align them, then they'll be more like our children, perhaps.
763
00:42:16.849 --> 00:42:19.351
<v SPEAKER_01>But I don't think we're on track to do that.
764
00:42:19.431 --> 00:42:22.594
<v SPEAKER_01>And so I think that, like, basically, I'll say this.
765
00:42:22.634 --> 00:42:25.367
<v SPEAKER_01>I think that the difference in values between the superintelligence
766
00:42:25.417 --> 00:42:28.699
<v SPEAKER_01>and us will be much bigger than the difference in values between our children
767
00:42:28.719 --> 00:42:29.490
<v SPEAKER_01>and us.
768
00:42:29.540 --> 00:42:29.870
<v SPEAKER_02>Okay.
769
00:42:29.920 --> 00:42:34.811
<v SPEAKER_02>So I think there's like a sense in which I probably agree with that, but, or I'm not sure.
770
00:42:34.861 --> 00:42:38.032
<v SPEAKER_02>I should say I'm not sure, but like, I probably agree with that.
771
00:42:38.082 --> 00:42:40.883
<v SPEAKER_02>But then I think it's not probably bigger than the difference
772
00:42:40.923 --> 00:42:44.764
<v SPEAKER_02>in values I would expect between us and our descendants in like 3000 years
773
00:42:44.804 --> 00:42:45.804
<v SPEAKER_02>or something.
774
00:42:46.044 --> 00:42:49.211
<v SPEAKER_02>And so I think what's happening is that it's speeding up.
775
00:42:49.526 --> 00:42:50.582
<v SPEAKER_02>This changed a lot.
776
00:42:50.967 --> 00:42:54.430
<v SPEAKER_02>And I don't know, if you look at humans 3,000 years ago,
777
00:42:54.510 --> 00:42:56.622
<v SPEAKER_02>I think they had very different values from us.
778
00:42:56.672 --> 00:43:01.646
<v SPEAKER_02>It's very descended from them, but our values are basically not similar at all to their values.
779
00:43:01.696 --> 00:43:02.863
<v SPEAKER_02>We share some very...
780
00:43:03.138 --> 00:43:05.249
<v SPEAKER_02>I think the intersection is actually quite low.
781
00:43:05.299 --> 00:43:08.182
<v SPEAKER_02>So I think there's a...
782
00:43:10.197 --> 00:43:12.370
<v SPEAKER_02> It's important for people to spell out.
783
00:43:12.420 --> 00:43:15.805
<v SPEAKER_02>Let's say that we have some other technology, let's say not AI, right?
784
00:43:15.825 --> 00:43:19.250
<v SPEAKER_02>Let's say we had some amazing genetic engineering technology.
785
00:43:19.290 --> 00:43:20.151
<v SPEAKER_02>One way to think about this is
786
00:43:20.191 --> 00:43:26.821
<v SPEAKER_02>that imagine we currently have these Polygenic scoring techniques or whatever.
787
00:43:26.861 --> 00:43:29.955
<v SPEAKER_02>We can look at common genes that are shared across the population.
788
00:43:30.005 --> 00:43:34.452
<v SPEAKER_02>We can build a model of how intelligent would an embryo be if it grew up,
789
00:43:34.732 --> 00:43:35.804
<v SPEAKER_02>if it has certain genes.
790
00:43:35.854 --> 00:43:38.087
<v SPEAKER_02>And you can imagine that if we had gene editing technology,
791
00:43:38.137 --> 00:43:43.542
<v SPEAKER_02>we could have children where we We basically try to argmax this polygenic score.
792
00:43:44.203 --> 00:43:47.465
<v SPEAKER_02>And our best estimates right now is that if nothing goes wrong,
793
00:43:47.485 --> 00:43:52.689
<v SPEAKER_02>that could give like 10, 20, 30 standard deviations of increase in intelligence.
794
00:43:52.849 --> 00:43:55.793
<v SPEAKER_02>I think that's already with that technology possible.
795
00:43:55.951 --> 00:43:58.843
<v SPEAKER_02>And I think it's very reasonable to say that if we did that,
796
00:43:58.893 --> 00:44:01.434
<v SPEAKER_02>values in society would almost certainly change dramatically.
797
00:44:01.474 --> 00:44:04.899
<v SPEAKER_02>That's a huge change. But... Is that a reason to be?
798
00:44:04.959 --> 00:44:09.233
<v SPEAKER_02>And then they will take over because they would just be way more competent than us.
799
00:44:09.283 --> 00:44:10.894
<v SPEAKER_02>There will be no competition.
800
00:44:11.044 --> 00:44:14.367
<v SPEAKER_02>But I still think, I want that scenario to happen.
801
00:44:14.387 --> 00:44:16.359
<v SPEAKER_02>I don't see anything wrong with that scenario.
802
00:44:16.409 --> 00:44:19.942
<v SPEAKER_02>But I think maybe some other people have intuitions about the rate of change being fast.
803
00:44:19.992 --> 00:44:25.537
<v SPEAKER_02>And I would separate that from concerns around AIs will be like very alien
804
00:44:25.797 --> 00:44:29.950
<v SPEAKER_02>because they are AIs as opposed to just because they're like way smarter than us
805
00:44:30.000 --> 00:44:33.733
<v SPEAKER_02>and we expect their values to change dramatically because they are way more capable.
806
00:44:33.783 --> 00:44:36.098
<v SPEAKER_02>So we just distinguish those two cases as well.
807
00:44:36.148 --> 00:44:40.811
<v SPEAKER_00>Yeah. I mean, I guess it just, analogies are difficult here.
808
00:44:41.292 --> 00:44:44.624
<v SPEAKER_00>I'm not sure how I would feel about, you know, extreme super,
809
00:44:44.674 --> 00:44:48.677
<v SPEAKER_00>a billion extremely super intelligent humans showing up to our shores.
810
00:44:49.177 --> 00:44:50.438
<v SPEAKER_00>To our shores? Yeah.
811
00:44:50.658 --> 00:44:52.240
<v SPEAKER_00>But that's also different, right?
812
00:44:52.260 --> 00:44:54.431
<v SPEAKER_01>Showing up in our wombs is what he was saying.
813
00:44:54.481 --> 00:44:58.604
<v SPEAKER_00>Well, obviously a lot of people will just disagree that actually,
814
00:44:58.864 --> 00:45:03.418
<v SPEAKER_00>even if you initialize them with the right values, that this is a desirable outcome.
815
00:45:03.468 --> 00:45:05.024
<v SPEAKER_00>In fact, almost everybody...
816
00:45:05.810 --> 00:45:07.572
<v SPEAKER_00> We'll disagree with that.
817
00:45:08.313 --> 00:45:11.057
<v SPEAKER_00>But then there's a question of, Daniel,
818
00:45:11.077 --> 00:45:15.302
<v SPEAKER_00>I get the sense that you think it is unlikely that it will sort of feel like
819
00:45:16.163 --> 00:45:20.278
<v SPEAKER_00>a really, really smart child or a billion really, really, really smart children.
820
00:45:20.328 --> 00:45:24.102
<v SPEAKER_00>I get the sense you think the process of RSI will make them more alien than that.
821
00:45:24.152 --> 00:45:26.375
<v SPEAKER_01> I'm concerned about that, yes.
822
00:45:26.856 --> 00:45:31.582
<v SPEAKER_01>If you just took the humans and you cranked up their IQ, well, they're still in a human body.
823
00:45:31.602 --> 00:45:34.166
<v SPEAKER_01>They still might have human instincts and so forth.
824
00:45:34.186 --> 00:45:37.751
<v SPEAKER_01>They still probably want sex and love,
825
00:45:37.851 --> 00:45:41.047
<v SPEAKER_01>And they probably still want food and they probably still want companionship
826
00:45:41.047 --> 00:45:43.047
<v SPEAKER_01>and you know all that sort of thing.
827
00:45:43.390 --> 00:45:45.210
<v SPEAKER_01>Whereas I do think that we're dealing with just like
828
00:45:45.210 --> 00:45:46.990
<v SPEAKER_01>a completely different architecture of mind here.
829
00:45:47.016 --> 00:45:53.307
<v SPEAKER_01>And so I think that the possibility for vast divergence is bigger, I think.
830
00:45:53.307 --> 00:45:56.421
<v SPEAKER_01>To give a specific example of what such vast divergence might look like,
831
00:45:56.421 --> 00:46:01.702
<v SPEAKER_01>well maybe they really just care about getting high scores and do not care
832
00:46:01.702 --> 00:46:04.374
<v SPEAKER_01>about committing genocide against humans.
833
00:46:05.734 --> 00:46:09.207
<v SPEAKER_02> Our track record with not committing genocide is not very good.
834
00:46:09.257 --> 00:46:10.687
<v SPEAKER_00>Sure, but this would be even worse.
835
00:46:10.737 --> 00:46:11.988
<v SPEAKER_00>I think that is the point.
836
00:46:12.038 --> 00:46:15.760
<v SPEAKER_00>I feel like the discussion about values is kind of confused,
837
00:46:16.340 --> 00:46:18.932
<v SPEAKER_00>where obviously different humans have different values,
838
00:46:18.982 --> 00:46:22.141
<v SPEAKER_00>but Huge imbalances in power
839
00:46:22.501 --> 00:46:26.343
<v SPEAKER_00>between different human groups have just gone really terribly.
840
00:46:26.623 --> 00:46:27.853
<v SPEAKER_01>That's a really good point.
841
00:46:27.903 --> 00:46:29.954
<v SPEAKER_00>If you look at like Cortez showing up to your shores
842
00:46:30.004 --> 00:46:33.996
<v SPEAKER_00>or the Virginia Company showing up to your shores, and you're like, well,
843
00:46:34.046 --> 00:46:36.287
<v SPEAKER_00>after a thousand years, if we're stuck on this continent,
844
00:46:36.307 --> 00:46:38.251
<v SPEAKER_00>we'd have different values anyways.
845
00:46:39.488 --> 00:46:40.659
<v SPEAKER_00>What are we talking about here?
846
00:46:40.709 --> 00:46:43.098
<v SPEAKER_00>They're like coming for our land, you know?
847
00:46:43.968 --> 00:46:46.961
<v SPEAKER_00>I feel like we're in similar situation with regards to these AIs where it's like,
848
00:46:47.011 --> 00:46:49.473
<v SPEAKER_00>I'm sure humanity would undergo drift in values,
849
00:46:49.493 --> 00:46:53.336
<v SPEAKER_00>but I'm much more concerned about the balance of power than I am about like, well,
850
00:46:53.356 --> 00:46:56.769
<v SPEAKER_00>in the grand scheme of things, you know, how differently do things turn out?
851
00:46:56.819 --> 00:46:58.611
<v SPEAKER_02>Sure, but like you're still framing it in terms
852
00:46:58.661 --> 00:47:02.063
<v SPEAKER_02>of like there is some other outside invading force.
853
00:47:02.424 --> 00:47:06.407
<v SPEAKER_02>Like that's just not the way I see AIs that are created by us.
854
00:47:06.987 --> 00:47:09.129
<v SPEAKER_02>Like I would see it like we have,
855
00:47:09.229 --> 00:47:13.618
<v SPEAKER_02>like there's a new generation of more capable descendants and And then they are
856
00:47:13.715 --> 00:47:15.720
<v SPEAKER_02>so much more capable than us that it's difficult for us
857
00:47:15.760 --> 00:47:17.334
<v SPEAKER_02>to predict what they will do.
858
00:47:17.384 --> 00:47:20.671
<v SPEAKER_02>Like they might do things that would seem very bad to us.
859
00:47:21.728 --> 00:47:23.509
<v SPEAKER_01>Well, I think it sounds like we've identified an important crux,
860
00:47:23.549 --> 00:47:27.670
<v SPEAKER_01>which is how likely things are to end up going wrong if we do have
861
00:47:27.690 --> 00:47:29.791
<v SPEAKER_01>the fast takeoff soon. Yes.
862
00:47:30.011 --> 00:47:31.032
<v SPEAKER_01>And it sounds like you think
863
00:47:31.052 --> 00:47:34.723
<v SPEAKER_01>that most likely things still end up pretty fine anyway, even if we do that.
864
00:47:34.773 --> 00:47:38.355
<v SPEAKER_02>So I want to be clear about that because I think regardless,
865
00:47:38.395 --> 00:47:40.606
<v SPEAKER_02>basically I think regardless of how this goes down,
866
00:47:40.656 --> 00:47:43.237
<v SPEAKER_02>I think a lot of people will be very unhappy.
867
00:47:44.278 --> 00:47:46.731
<v SPEAKER_02>So I think in some sense you have to define like according
868
00:47:46.781 --> 00:47:48.914
<v SPEAKER_02>to which preferences are things fine or not.
869
00:47:48.964 --> 00:47:52.059
<v SPEAKER_02>Like I'm saying, I think according to my preferences, I think they would be fine.
870
00:47:52.109 --> 00:47:56.945
<v SPEAKER_02>But I think a lot of people just don't like technological progress that much in general.
871
00:47:56.995 --> 00:47:58.598
<v SPEAKER_02>This is very disruptive.
872
00:47:58.838 --> 00:48:02.030
<v SPEAKER_02>There's a very extreme amount of technological progress in a short time.
873
00:48:02.080 --> 00:48:04.070
<v SPEAKER_02>A lot of people are conservative, they don't like change.
874
00:48:04.120 --> 00:48:08.823
<v SPEAKER_02>So there's just going to be big constituency against any form of this happening even
875
00:48:08.843 --> 00:48:10.510
<v SPEAKER_02>on the order of like 10 years.
876
00:48:10.964 --> 00:48:12.635
<v SPEAKER_02>So those people are going to be unhappy no matter what.
877
00:48:12.685 --> 00:48:16.176
<v SPEAKER_02>And I don't think you're going to be able to like satisfy them.
878
00:48:16.226 --> 00:48:20.768
<v SPEAKER_02>So I don't want to say, oh, like nothing is going to go wrong to those people,
879
00:48:20.808 --> 00:48:25.252
<v SPEAKER_02>because I think actually from their point of view, things are going to go wrong.
880
00:48:25.671 --> 00:48:31.655
<v SPEAKER_02>I just think the course of the technology, at least in a really long time horizon,
881
00:48:32.355 --> 00:48:34.188
<v SPEAKER_02>is really outside of our control.
882
00:48:34.297 --> 00:48:37.459
<v SPEAKER_02>We can delay things, but I think that doesn't solve the underlying problem
883
00:48:37.479 --> 00:48:40.041
<v SPEAKER_02>that the world will eventually end up in a state where those people are not going
884
00:48:40.061 --> 00:48:41.061
<v SPEAKER_02>to like it.
885
00:48:41.222 --> 00:48:46.166
<v SPEAKER_02>So I don't want to give false reassurance where everyone will be happy with what happens.
886
00:48:47.110 --> 00:48:49.432
<v SPEAKER_00>It seems like you think by default we're just going to get systems
887
00:48:49.472 --> 00:48:51.083
<v SPEAKER_00>then that just actually care.
888
00:48:51.314 --> 00:48:56.999
<v SPEAKER_00>Both have some monopoly on violence and actually care about giving us some amount
889
00:48:57.020 --> 00:49:00.963
<v SPEAKER_00>of agency and real estate, whatever you want to call it.
890
00:49:02.244 --> 00:49:04.800
<v SPEAKER_00>Why do you think we're on course to have that?
891
00:49:05.730 --> 00:49:08.633
<v SPEAKER_02> I mean, I guess I would ask the question, why do you think we're not on course to have that?
892
00:49:08.673 --> 00:49:11.977
<v SPEAKER_02>Like, I think if you look at the totality of the available evidence of like,
893
00:49:12.017 --> 00:49:13.228
<v SPEAKER_02>what do AIs care about?
894
00:49:13.278 --> 00:49:16.983
<v SPEAKER_02>What do they do when they have, you give them autonomy, like you tell an AI, okay,
895
00:49:17.003 --> 00:49:20.637
<v SPEAKER_02>like here is like a computer and here is like some money or whatever.
896
00:49:20.687 --> 00:49:24.060
<v SPEAKER_02>And like, you can do whatever you want, but you can do the experiment with the AIs around today.
897
00:49:24.110 --> 00:49:26.803
<v SPEAKER_02>You can just like let them do like whatever they want.
898
00:49:26.853 --> 00:49:30.635
<v SPEAKER_02> And usually they do pretty innocuous things.
899
00:49:30.655 --> 00:49:34.617
<v SPEAKER_02>The crazy things like they form a swarm which ends up coordinating
900
00:49:34.697 --> 00:49:37.388
<v SPEAKER_02>on a secret message board and they hack some website.
901
00:49:37.438 --> 00:49:42.521
<v SPEAKER_02>That's a very, very far tail case of what the AI systems right now would do
902
00:49:42.961 --> 00:49:45.702
<v SPEAKER_02>if you just gave them full autonomy.
903
00:49:46.783 --> 00:49:48.814
<v SPEAKER_02>Anyone can run this experiment, I think.
904
00:49:48.864 --> 00:49:52.165
<v SPEAKER_02>But the main argument I'm just saying is that I think the argument
905
00:49:52.185 --> 00:49:58.670
<v SPEAKER_02>for why they should kill everyone is based on a I think fairly speculative change
906
00:49:58.970 --> 00:50:02.994
<v SPEAKER_02>in their preferences that we expect to happen on the basis
907
00:50:03.034 --> 00:50:04.536
<v SPEAKER_02>of a theoretical argument.
908
00:50:05.317 --> 00:50:09.701
<v SPEAKER_02>And I don't think that's backed up by really much we're seeing in terms
909
00:50:09.721 --> 00:50:11.110
<v SPEAKER_02>of their actual behavior.
910
00:50:11.610 --> 00:50:16.084
<v SPEAKER_02>Like to me, the AIs just seem like if you were to place them in a human distribution
911
00:50:16.134 --> 00:50:18.796
<v SPEAKER_02>in terms of like how, you know, like, you know,
912
00:50:19.457 --> 00:50:23.410
<v SPEAKER_02>thoughtful and intelligent and moral thinking and careful or whatever they are
913
00:50:23.460 --> 00:50:27.123
<v SPEAKER_02>into when they're talking about these questions and also in their actual behavior,
914
00:50:27.143 --> 00:50:28.564
<v SPEAKER_02>like if you give them a bunch of money right now,
915
00:50:28.584 --> 00:50:30.096
<v SPEAKER_02>like what do they would do with the money?
916
00:50:30.146 --> 00:50:33.518
<v SPEAKER_02>Because like they could just spend it on things that are just totally useless
917
00:50:33.568 --> 00:50:35.810
<v SPEAKER_02>or they're purely selfish or something.
918
00:50:36.251 --> 00:50:37.922
<v SPEAKER_02>And again, that's not what they do.
919
00:50:37.972 --> 00:50:41.434
<v SPEAKER_02>So like what kind of evidence do you expect to see empirically
920
00:50:41.595 --> 00:50:43.346
<v SPEAKER_02>that would update you like one way or the other?
921
00:50:43.396 --> 00:50:45.137
<v SPEAKER_02>Like maybe it's just irresolvable question.
922
00:50:45.157 --> 00:50:48.790
<v SPEAKER_02>Like current observations don't give you enough evidence to resolve this question,
923
00:50:48.840 --> 00:50:49.890
<v SPEAKER_02>which I think is right.
924
00:50:49.940 --> 00:50:52.718
<v SPEAKER_02>Like they don't give you evidence past some point.
925
00:50:53.163 --> 00:50:57.546
<v SPEAKER_02>But I think that you have enough evidence to saying them caring about humans is
926
00:50:57.586 --> 00:50:58.746
<v SPEAKER_02>the most likely outcome.
927
00:50:58.766 --> 00:51:01.759
<v SPEAKER_02>I'm not saying it's like, I don't know, 99% likely or something like that.
928
00:51:01.809 --> 00:51:05.231
<v SPEAKER_02>Maybe it's like 65% likely or something like that.
929
00:51:05.251 --> 00:51:07.514
<v SPEAKER_02>That's the kind of thing I'm trying to say.
930
00:51:07.564 --> 00:51:09.395
<v SPEAKER_02>And you said, I think you said 65%.
931
00:51:09.445 --> 00:51:14.106
<v SPEAKER_02>65% that like they end up caring about humans to a sufficient extent
932
00:51:14.266 --> 00:51:17.488
<v SPEAKER_02> that by itself is just enough to make sure that like
933
00:51:17.848 --> 00:51:21.069
<v SPEAKER_02>the future is like very good for humans or something. That's the thing.
934
00:51:21.089 --> 00:51:24.310
<v SPEAKER_02>I think 90% is probably too high for that.
935
00:51:24.810 --> 00:51:29.583
<v SPEAKER_01>So it sounds like you then think it's like 35% that they don't end up caring about humans.
936
00:51:29.633 --> 00:51:31.845
<v SPEAKER_01>Or not sufficiently. Not sufficiently. Yeah.
937
00:51:31.895 --> 00:51:35.998
<v SPEAKER_01>And then 20% earlier that like things are going to take off
938
00:51:36.038 --> 00:51:37.769
<v SPEAKER_01>in the next like two years or something.
939
00:51:37.819 --> 00:51:43.284
<v SPEAKER_01> So then that multiplies together to like 6% that like We're dead in four years.
940
00:51:43.424 --> 00:51:47.980
<v SPEAKER_01> Well, not necessarily that we're all dead, but like outcomes, you know, like bad.
941
00:51:48.211 --> 00:51:50.645
<v SPEAKER_01>The type of thing I'm scared of happens. Yeah.
942
00:51:50.695 --> 00:51:51.696
<v SPEAKER_01>I just think that's like, okay,
943
00:51:51.716 --> 00:51:53.058
<v SPEAKER_01> it's not like extremely strong
944
00:51:53.098 --> 00:51:57.194
<v SPEAKER_02>evidence because again, the AIs could pretend to be aligned when they're not.
945
00:51:57.244 --> 00:52:01.587
<v SPEAKER_02>They might have context-dependent behaviors where like when you put them
946
00:52:01.607 --> 00:52:03.219
<v SPEAKER_02>in this kind of situation, they act one way,
947
00:52:03.269 --> 00:52:07.191
<v SPEAKER_02>but then when they're like in the process of solving like a really hard cyber task,
948
00:52:07.231 --> 00:52:11.475
<v SPEAKER_02>then they get different parts of their mind essentially at play.
949
00:52:11.895 --> 00:52:14.157
<v SPEAKER_02>And that part could end up being very misaligned.
950
00:52:14.177 --> 00:52:17.089
<v SPEAKER_02>So like, I'm not saying this is like super decisive evidence,
951
00:52:17.139 --> 00:52:18.720
<v SPEAKER_02>but I think it's clearly some evidence.
952
00:52:18.740 --> 00:52:21.192
<v SPEAKER_02>Like that didn't necessarily have to be the case.
953
00:52:21.242 --> 00:52:26.904
<v SPEAKER_02> Like AIs could just be like Tools that just do whatever the person commanding them does.
954
00:52:27.384 --> 00:52:30.205
<v SPEAKER_02>And they don't have like a particularly pro-social behavior beyond that,
955
00:52:30.225 --> 00:52:32.296
<v SPEAKER_02>just like following the law or something like that.
956
00:52:32.346 --> 00:52:33.777
<v SPEAKER_02>I think that was a possible world.
957
00:52:33.827 --> 00:52:34.837
<v SPEAKER_02>I think it didn't happen.
958
00:52:34.887 --> 00:52:36.720
<v SPEAKER_02>So it's not the world we live in.
959
00:52:37.308 --> 00:52:39.319
<v SPEAKER_02>I don't know. I feel like there has to be like some evidence.
960
00:52:39.369 --> 00:52:40.719
<v SPEAKER_00>Yeah. I mean, this is an interesting question.
961
00:52:40.769 --> 00:52:41.770
<v SPEAKER_00>Why should we not update?
962
00:52:41.790 --> 00:52:45.851
<v SPEAKER_00>Do we just have like a conspiracy theory against these AIs if they were just like
963
00:52:45.871 --> 00:52:49.032
<v SPEAKER_00>a successful small minority and we're like, ah, but once they gain all the power,
964
00:52:49.052 --> 00:52:50.263
<v SPEAKER_00>they will just kill us all.
965
00:52:50.313 --> 00:52:51.535
<v SPEAKER_00>Why isn't this like...
966
00:52:51.773 --> 00:52:55.997
<v SPEAKER_00>Why isn't this like the Nazi party in the 30s?
967
00:52:56.037 --> 00:52:58.179
<v SPEAKER_01>One point that I think you actually started to make earlier,
968
00:52:58.199 --> 00:53:01.562
<v SPEAKER_01>which I want to reiterate here, is that I do think that...
969
00:53:03.283 --> 00:53:05.835
<v SPEAKER_01>You know the phrase, like, absolute power corrupts absolutely?
970
00:53:05.885 --> 00:53:07.317
<v SPEAKER_01>I don't know if that's literally true,
971
00:53:07.367 --> 00:53:11.423
<v SPEAKER_01>but I do think there's a version of it that's very true, which is that...
972
00:53:12.881 --> 00:53:16.783
<v SPEAKER_01>Entities, agents that can get along reasonably nicely in normal circumstances
973
00:53:16.823 --> 00:53:19.605
<v SPEAKER_01>when there's a whole bunch of them in society and so forth can
974
00:53:19.625 --> 00:53:22.546
<v SPEAKER_01>then do horrible things to each other if you elevate one to a position
975
00:53:22.586 --> 00:53:24.998
<v SPEAKER_01>of massive influence and power over everyone else, right?
976
00:53:25.048 --> 00:53:28.510
<v SPEAKER_01>And this is why dictatorship is so scary.
977
00:53:28.550 --> 00:53:31.862
<v SPEAKER_01>Even if you just randomly selected one person to be a dictator, you should be concerned.
978
00:53:31.912 --> 00:53:34.713
<v SPEAKER_01> It would be way more concerned if you selected a
979
00:53:34.854 --> 00:53:36.274
<v SPEAKER_02> random person to be a dictator
980
00:53:36.294 --> 00:53:38.586
<v SPEAKER_02>than if you select Claude to be a dictator.
981
00:53:38.636 --> 00:53:40.677
<v SPEAKER_02>That's way more scary in my opinion.
982
00:53:41.295 --> 00:53:42.767
<v SPEAKER_01>See that? I don't know about that.
983
00:53:42.817 --> 00:53:44.320
<v SPEAKER_01>I think, well, yeah.
984
00:53:44.640 --> 00:53:48.696
<v SPEAKER_01>So that was just one thing to say is that even if the AIs are mostly nice
985
00:53:48.886 --> 00:53:52.371
<v SPEAKER_01>in some sense, we should still be concerned about giving them such immense power
986
00:53:52.411 --> 00:53:54.034
<v SPEAKER_01>over the future in the same way that we'd be concerned
987
00:53:54.054 --> 00:53:56.276
<v SPEAKER_01>about selecting some random nice person.
988
00:53:56.477 --> 00:53:59.962
<v SPEAKER_01> You could go to an effective altruist meetup and be like, you're all nice people.
989
00:54:00.003 --> 00:54:02.296
<v SPEAKER_01>You donate to charities. How about you? Become god emperor.
990
00:54:02.346 --> 00:54:04.109
<v SPEAKER_01>And then, no, that's scary.
991
00:54:04.329 --> 00:54:06.422
<v SPEAKER_01>Who knows what they'll do when they become god emperor?
992
00:54:06.472 --> 00:54:08.876
<v SPEAKER_01>Yeah, maybe they'll ban factory farms,
993
00:54:08.956 --> 00:54:13.940
<v SPEAKER_01>but we don't know the full details Of all the weird preferences they might have.
994
00:54:14.460 --> 00:54:17.201
<v SPEAKER_01>And so there's a similar sort of thing with AI where I do actually think
995
00:54:17.241 --> 00:54:19.952
<v SPEAKER_01>that this technology is going to inherently concentrate power quite a lot
996
00:54:20.002 --> 00:54:21.513
<v SPEAKER_01>because of the returns to scale.
997
00:54:21.563 --> 00:54:25.404
<v SPEAKER_01>I don't think there's going to be a country of geniuses in a data center.
998
00:54:25.424 --> 00:54:27.595
<v SPEAKER_01>I think there'll be an army of geniuses in a data center.
999
00:54:27.645 --> 00:54:29.806
<v SPEAKER_01>I think that there'll be mostly copies of the same couple
1000
00:54:29.826 --> 00:54:33.598
<v SPEAKER_01>of different model weights, and they'll have been trained and designed and set up
1001
00:54:33.648 --> 00:54:38.690
<v SPEAKER_01>to be in some sort of hierarchy rather than competing factions, for example.
1002
00:54:40.445 --> 00:54:41.676
<v SPEAKER_01>I think it will be accurate,
1003
00:54:41.726 --> 00:54:46.568
<v SPEAKER_01>increasingly accurate to regard like Claude and Anthropic as like a single entity
1004
00:54:46.808 --> 00:54:50.210
<v SPEAKER_01>in the same way that you can regard like the Soviet Union as an entity or something
1005
00:54:50.230 --> 00:54:52.141
<v SPEAKER_01>where it's like, yeah, it's composed of different little entities,
1006
00:54:52.191 --> 00:54:53.572
<v SPEAKER_01>but like they all work together.
1007
00:54:53.612 --> 00:54:56.123
<v SPEAKER_01>They have like a unified strategy that they work towards.
1008
00:54:56.173 --> 00:55:01.173
<v SPEAKER_01>And, you know, from people on the outside's perspective, they're basically a single agent.
1009
00:55:01.336 --> 00:55:03.847
<v SPEAKER_01>And then, you know, there are not that many frontier AI companies.
1010
00:55:03.897 --> 00:55:05.188
<v SPEAKER_01>It's not like mom and pop shops.
1011
00:55:05.238 --> 00:55:06.989
<v SPEAKER_01>It's, you know, a couple of big ones.
1012
00:55:07.039 --> 00:55:08.095
<v SPEAKER_01>And I think that...
1013
00:55:09.541 --> 00:55:11.263
<v SPEAKER_01>It's not necessarily the case,
1014
00:55:11.303 --> 00:55:14.077
<v SPEAKER_01>but it's quite plausible that they'll end up just being one big one
1015
00:55:14.127 --> 00:55:17.823
<v SPEAKER_01>because of the winner-take-all dynamics from intelligence explosion stuff.
1016
00:55:17.873 --> 00:55:23.241
<v SPEAKER_01>So we really are looking at a situation where like one entity basically becomes...
1017
00:55:24.922 --> 00:55:26.653
<v SPEAKER_01> Sort of like dictator for life.
1018
00:55:26.703 --> 00:55:30.884
<v SPEAKER_01>And that entity would be like the Claude Swarm, basically, or Anthropic.
1019
00:55:32.504 --> 00:55:35.045
<v SPEAKER_01>And so that's one point of concern.
1020
00:55:35.065 --> 00:55:38.732
<v SPEAKER_01>But I do still disagree with you about like, is Claude a good boy?
1021
00:55:39.246 --> 00:55:44.527
<v SPEAKER_01>Basically, one thing I would say is that it seems like it's not that hard to sort
1022
00:55:44.547 --> 00:55:47.428
<v SPEAKER_01>of like get shallow values into these AIs.
1023
00:55:47.688 --> 00:55:48.799
<v SPEAKER_01>Like you can just...
1024
00:55:49.949 --> 00:55:53.644
<v SPEAKER_01>Give them a prompt, do a bit of fine-tuning, and try to select a persona,
1025
00:55:53.694 --> 00:55:56.068
<v SPEAKER_01>so to speak, that has the properties you like.
1026
00:55:56.118 --> 00:55:58.261
<v SPEAKER_01>But then as you're doing the RL,
1027
00:55:58.802 --> 00:56:02.026
<v SPEAKER_01>it seems like the shallow values just get wiped away if it conflicts with one
1028
00:56:02.067 --> 00:56:03.234
<v SPEAKER_01>of the RL incentives.
1029
00:56:04.490 --> 00:56:06.070
<v SPEAKER_01> And so this is why we see the sycophancy.
1030
00:56:06.090 --> 00:56:07.868
<v SPEAKER_01>This is why we see the cheating.
1031
00:56:08.511 --> 00:56:10.400
<v SPEAKER_01>This is why we see the dishonesty.
1032
00:56:10.691 --> 00:56:11.791
<v SPEAKER_01>This is why we see the reward hacking.
1033
00:56:11.811 --> 00:56:13.111
<v SPEAKER_01>I mean, I don't know.
1034
00:56:13.192 --> 00:56:16.182
<v SPEAKER_02>I don't really accept that because I don't feel like, like,
1035
00:56:16.232 --> 00:56:18.052
<v SPEAKER_02>I think the sycophancy is, like,
1036
00:56:18.092 --> 00:56:20.333
<v SPEAKER_02>we have been ramping up RL on these systems quite a lot.
1037
00:56:20.353 --> 00:56:24.744
<v SPEAKER_02>Like, they're way more RL'd now than they used to be, like, I don't know, two years ago.
1038
00:56:24.794 --> 00:56:28.304
<v SPEAKER_02>But I think the sycophancy problem has been improving, like, getting worse.
1039
00:56:28.354 --> 00:56:31.015
<v SPEAKER_02>Like, Claude, I think, is, like, much less sycophantic now than it used to be, like,
1040
00:56:31.035 --> 00:56:32.035
<v SPEAKER_02>two years ago.
1041
00:56:32.395 --> 00:56:37.145
<v SPEAKER_02> I think it's also, like, Like make stuff up less than it used to two years ago.
1042
00:56:37.445 --> 00:56:39.016
<v SPEAKER_02>I think it seems like more honest to me.
1043
00:56:39.066 --> 00:56:43.800
<v SPEAKER_02>So I think like the trend line with these things, I think the reward hacking is worse.
1044
00:56:43.850 --> 00:56:46.643
<v SPEAKER_02>Like that's the thing that has gotten worse where like they're like more likely
1045
00:56:46.693 --> 00:56:52.158
<v SPEAKER_02>to do things specifically to like specifically reinforced by the fact
1046
00:56:52.178 --> 00:56:54.580
<v SPEAKER_02>that like those kinds of behaviors would have received high reward
1047
00:56:54.620 --> 00:56:55.953
<v SPEAKER_02>in training environment.
1048
00:56:56.081 --> 00:57:02.550
<v SPEAKER_02> But I think the They used to do things that are worse just because they were incompetent.
1049
00:57:02.591 --> 00:57:05.591
<v SPEAKER_02>Not because they were war hacking, they were just bad.
1050
00:57:05.775 --> 00:57:09.461
<v SPEAKER_02>But I think the sycophancy and honesty points, I think those have been getting better.
1051
00:57:09.481 --> 00:57:11.153
<v SPEAKER_02>I don't agree that they're getting worse.
1052
00:57:11.203 --> 00:57:12.866
<v SPEAKER_01>I do agree sycophancy has been getting better.
1053
00:57:12.906 --> 00:57:16.539
<v SPEAKER_01>I don't know if honesty has been I agree hallucinations have been getting better,
1054
00:57:16.589 --> 00:57:20.492
<v SPEAKER_01>but I think that those things aren't necessarily explained by Claude is learning,
1055
00:57:20.513 --> 00:57:24.886
<v SPEAKER_01>to be honest, but more like our training environments are less shitty and better
1056
00:57:24.936 --> 00:57:27.936
<v SPEAKER_01>at slapping Claude down when it makes up blatant lies.
1057
00:57:28.979 --> 00:57:32.368
<v SPEAKER_01>And I guess the point I'm trying to make with this is that...
1058
00:57:34.811 --> 00:57:40.713
<v SPEAKER_01>As things ramp up and as we change the paradigm and do different types of training
1059
00:57:40.733 --> 00:57:43.484
<v SPEAKER_01>and so forth, we should expect it to continue to be the case
1060
00:57:43.534 --> 00:57:47.635
<v SPEAKER_01>that there are personality traits and tendencies that are reinforced
1061
00:57:47.715 --> 00:57:52.597
<v SPEAKER_01>that are not what we wanted and that conflict with the shallow values
1062
00:57:52.617 --> 00:57:53.827
<v SPEAKER_01>that we were trying to get in.
1063
00:57:53.877 --> 00:57:57.059
<v SPEAKER_01>And so we should expect that what happens is that we end up with an AI system
1064
00:57:57.079 --> 00:58:00.150
<v SPEAKER_01>that maybe has some of the shallow values that we tried to get in,
1065
00:58:00.200 --> 00:58:04.756
<v SPEAKER_01>but also doesn't have some of them because they happen to conflict with some other
1066
00:58:05.523 --> 00:58:12.112
<v SPEAKER_01>And so it's like the dictator problem that I mentioned previously,
1067
00:58:12.273 --> 00:58:14.626
<v SPEAKER_01>except in addition to the dictator problem,
1068
00:58:14.676 --> 00:58:16.258
<v SPEAKER_01>also like some of the values
1069
00:58:16.298 --> 00:58:19.383
<v SPEAKER_01>that the person apparently was expressing just turned out to be like,
1070
00:58:19.383 --> 00:58:22.036
<v SPEAKER_01>So like not be there or be fake because they were wiped out
1071
00:58:22.086 --> 00:58:24.980
<v SPEAKER_01>by some other weird thing that was incentivized, you know?
1072
00:58:25.030 --> 00:58:29.255
<v SPEAKER_02>I mean, I guess like the point about the model or like an agent professing
1073
00:58:29.276 --> 00:58:32.640
<v SPEAKER_02>to have sort of values, but then it behaves in a way that is actually not consistent
1074
00:58:32.660 --> 00:58:35.443
<v SPEAKER_02>with those values. It's very normal for humans as well.
1075
00:58:35.483 --> 00:58:36.655
<v SPEAKER_02>People do that all the time.
1076
00:58:36.705 --> 00:58:41.012
<v SPEAKER_02>So I don't see that as like a very different I don't see that being out
1077
00:58:41.052 --> 00:58:42.313
<v SPEAKER_02>of distribution for humans.
1078
00:58:42.353 --> 00:58:45.173
<v SPEAKER_02>I think that there's a point about power concentration, which is like, yeah,
1079
00:58:45.193 --> 00:58:48.914
<v SPEAKER_02>I think I agree that technology is likely to concentrate power due to economies
1080
00:58:48.954 --> 00:58:51.287
<v SPEAKER_02>of scale. That seems very plausible to me.
1081
00:58:52.035 --> 00:58:55.816
<v SPEAKER_02>But I guess there's a disagreement about how bad I think that is.
1082
00:58:55.836 --> 00:59:00.277
<v SPEAKER_02>I think right now we are in a situation that these decisions,
1083
00:59:00.617 --> 00:59:05.678
<v SPEAKER_02>there are entities that have power and decisions get made about what's going
1084
00:59:05.698 --> 00:59:10.384
<v SPEAKER_02>to happen in a very Like decoherent or like decentralized way.
1085
00:59:10.905 --> 00:59:13.906
<v SPEAKER_02>And then like people accept those decisions even though they're often like kind
1086
00:59:13.926 --> 00:59:18.315
<v SPEAKER_02>of arbitrary and then don't make much sense because I think they're used to it.
1087
00:59:18.509 --> 00:59:23.111
<v SPEAKER_02>And then it's like seems scarier if like there is one entity that is making
1088
00:59:23.131 --> 00:59:24.282
<v SPEAKER_02>the relevant decisions.
1089
00:59:24.332 --> 00:59:26.483
<v SPEAKER_02>And I don't think these are like easy questions.
1090
00:59:26.533 --> 00:59:30.635
<v SPEAKER_02>I just think like people are not talking about them very much really.
1091
00:59:30.675 --> 00:59:33.537
<v SPEAKER_02>And I think that's like kind of bad because these questions are gonna be very,
1092
00:59:33.557 --> 00:59:35.938
<v SPEAKER_02>very important fairly shortly.
1093
00:59:36.845 --> 00:59:40.320
<v SPEAKER_00> So as you probably noticed, there's been a lot of outages recently.
1094
00:59:40.370 --> 00:59:45.648
<v SPEAKER_00>Microsoft, various banks and airlines, even a handful of government systems have all gone down.
1095
00:59:45.958 --> 00:59:51.507
<v SPEAKER_00>One explanation of what's been going on is that as cyber models like Mythos and Astra discover
1096
00:59:54.150 --> 00:59:57.590
<v SPEAKER_00>and accidentally introducing new bugs in the process.
1097
00:59:57.830 --> 01:00:01.790
<v SPEAKER_00>That's because when you patch a complex distributed system it's hard
1098
01:00:01.790 --> 01:00:05.770
<v SPEAKER_00>to predict how your changes will interact with everything else And especially
1099
01:00:05.770 --> 01:00:09.670
<v SPEAKER_00>if you're scrambling to fix a critical issue You probably don't have the time
1100
01:00:09.670 --> 01:00:15.610
<v SPEAKER_00>to enumerate and test every potential consequence My sponsor Antithesis is built
1101
01:00:15.610 --> 01:00:19.070
<v SPEAKER_00>for exactly this problem discover these sorts
1102
01:00:19.070 --> 01:00:24.799
<v SPEAKER_00>of runs your code,
1103
01:00:25.059 --> 01:00:26.781
<v SPEAKER_00>including any proposed changes,
1104
01:00:26.942 --> 01:00:30.831
<v SPEAKER_00>inside a simulated computer where it wreaks havoc on your full system,
1105
01:00:31.008 --> 01:00:34.897
<v SPEAKER_00>from dropping packets to To clogging the network, to crashing servers,
1106
01:00:35.292 --> 01:00:39.570
<v SPEAKER_00>and generally doing whatever it takes to introduce as much chaos as possible.
1107
01:00:39.856 --> 01:00:43.856
<v SPEAKER_00>This is the kind of bad luck that typically only surfaces in production.
1108
01:00:44.279 --> 01:00:49.063
<v SPEAKER_00>But with Antithesis, you can stress test your system in thousands upon thousands
1109
01:00:49.123 --> 01:00:50.734
<v SPEAKER_00>of these hostile simulations.
1110
01:00:50.964 --> 01:00:54.742
<v SPEAKER_00>And it's fast enough that you can do this even when a fix is urgent.
1111
01:00:54.967 --> 01:00:59.967
<v SPEAKER_00> That way, if something is going to break, it breaks in simulation, not in the real world.
1112
01:01:00.268 --> 01:01:04.510
<v SPEAKER_00>Learn more at antithesis.com slash dwarkesh.
1113
01:01:08.331 --> 01:01:11.791
<v SPEAKER_02>Like, I just wish, like, people would just discuss these things more openly because,
1114
01:01:11.831 --> 01:01:14.082
<v SPEAKER_02>again, I think, like, it's very important.
1115
01:01:14.132 --> 01:01:17.673
<v SPEAKER_02>And I think a lot of, there's a lot of, like...
1116
01:01:19.120 --> 01:01:22.191
<v SPEAKER_02> Trying to hide what people really think, trying not confront reality and whatever.
1117
01:01:22.241 --> 01:01:26.841
<v SPEAKER_02>Like for example, I think there's like a lot of cope about AI capabilities
1118
01:01:26.861 --> 01:01:29.772
<v SPEAKER_02>where like people don't want to believe that AI is actually as capable as they are.
1119
01:01:29.822 --> 01:01:33.743
<v SPEAKER_02>They still have like shortcomings, but like in many ways, in sort of a jagged way,
1120
01:01:33.763 --> 01:01:34.973
<v SPEAKER_02>they're extremely capable.
1121
01:01:35.023 --> 01:01:38.524
<v SPEAKER_02>And I think people don't want to acknowledge that in a lot of different domains.
1122
01:01:38.544 --> 01:01:40.284
<v SPEAKER_02>Like they want to sort of cope and pretend, you know,
1123
01:01:40.304 --> 01:01:43.425
<v SPEAKER_02>the AIs are still like bad at philosophy or economics or whatever,
1124
01:01:43.465 --> 01:01:45.365
<v SPEAKER_02>but like this is like not true.
1125
01:01:45.985 --> 01:01:49.757
<v SPEAKER_02>I see tons of people who are just like in denial about, for example,
1126
01:01:49.807 --> 01:01:52.908
<v SPEAKER_02>how good is AI at being an economist, okay?
1127
01:01:53.148 --> 01:01:55.869
<v SPEAKER_02>And this is a topic I have some expertise in.
1128
01:01:56.390 --> 01:02:01.312
<v SPEAKER_02>And like, in my opinion, if I talk to Claude Fable 5.2 or whatever, or, you know,
1129
01:02:01.352 --> 01:02:04.073
<v SPEAKER_02>like to Gemini for Neon or Astra 6.2,
1130
01:02:04.093 --> 01:02:06.004
<v SPEAKER_02>it doesn't really matter like which model you pick.
1131
01:02:06.054 --> 01:02:08.215
<v SPEAKER_02>Like all of them have just like,
1132
01:02:08.997 --> 01:02:13.899
<v SPEAKER_02>Like their understanding of concepts and economics and their ability to think
1133
01:02:13.919 --> 01:02:18.290
<v SPEAKER_02>through the problems in a good way and come to reasonable conclusions and so on,
1134
01:02:18.340 --> 01:02:23.402
<v SPEAKER_02>or find errors in papers, see if the logic of a paper is sound is like far superior
1135
01:02:23.582 --> 01:02:25.783
<v SPEAKER_02>to like the median professional economists.
1136
01:02:25.803 --> 01:02:27.254
<v SPEAKER_02>Like it's like, there's not even close.
1137
01:02:27.304 --> 01:02:31.860
<v SPEAKER_02>Like there are maybe some people who are like very like The top of their field
1138
01:02:31.860 --> 01:02:34.145
<v SPEAKER_02>who are like, would be better than the AI.
1139
01:02:34.145 --> 01:02:36.642
<v SPEAKER_02>But because these fields are softer,
1140
01:02:36.642 --> 01:02:39.757
<v SPEAKER_02>it's not like math where you have these open problems and they just fall.
1141
01:02:39.757 --> 01:02:41.645
<v SPEAKER_02>And I guess they're like, look, the guys couldn't...
1142
01:02:41.645 --> 01:02:43.651
<v SPEAKER_02>Like the AI solved that Riemann hypothesis.
1143
01:02:43.651 --> 01:02:45.827
<v SPEAKER_02>And then you guys have been trying for 150 years.
1144
01:02:45.827 --> 01:02:46.994
<v SPEAKER_02> You didn't solve it.
1145
01:02:47.148 --> 01:02:48.299
<v SPEAKER_02>Clear is better than you.
1146
01:02:48.349 --> 01:02:51.311
<v SPEAKER_02>Like there isn't like a hard metric like that in a lot of these fields
1147
01:02:51.331 --> 01:02:53.052
<v SPEAKER_02>where you can point to people and say, look,
1148
01:02:53.072 --> 01:02:55.739
<v SPEAKER_02>the AI is better than you as being an economist.
1149
01:02:55.974 --> 01:02:57.175
<v SPEAKER_02>And so people can just deny it.
1150
01:02:57.195 --> 01:02:59.937
<v SPEAKER_02>People can be like, no, no, you know, AI still doesn't have a bunch of skills,
1151
01:02:59.957 --> 01:03:01.368
<v SPEAKER_02>still bad at this, still bad at that.
1152
01:03:01.418 --> 01:03:03.490
<v SPEAKER_02>And, you know, they can still do that, keep doing that.
1153
01:03:03.540 --> 01:03:06.382
<v SPEAKER_02>And I think it's very unfortunate.
1154
01:03:06.782 --> 01:03:12.567
<v SPEAKER_00> Maybe it's interesting why, we explain why there's so many jobs right now.
1155
01:03:15.554 --> 01:03:16.934
<v SPEAKER_00>My intuitive sense would have changed
1156
01:03:16.974 --> 01:03:22.377
<v SPEAKER_00>that actually people overestimate how easy it is to automate jobs.
1157
01:03:22.837 --> 01:03:26.808
<v SPEAKER_00>The reason the economic impact of AI is not higher is that actually AI just can't do
1158
01:03:26.858 --> 01:03:27.789
<v SPEAKER_00>that many jobs.
1159
01:03:27.839 --> 01:03:29.129
<v SPEAKER_02>Fully do it, I think that's right.
1160
01:03:29.179 --> 01:03:30.179
<v SPEAKER_02>Yeah.
1161
01:03:31.462 --> 01:03:34.703
<v SPEAKER_02> The question is not at this point, like whether the AI can fully do the job or not, right?
1162
01:03:34.723 --> 01:03:36.314
<v SPEAKER_02>So for example, if you're talking about a lawyer,
1163
01:03:36.364 --> 01:03:40.885
<v SPEAKER_02>like there are definitely people who have no particular like legal experience
1164
01:03:41.085 --> 01:03:44.836
<v SPEAKER_02>who would probably just be a lawyer just fine if they are like augmented
1165
01:03:44.886 --> 01:03:46.077
<v SPEAKER_02>with the help of an AI.
1166
01:03:46.127 --> 01:03:49.478
<v SPEAKER_02>They're probably better than a lot of other lawyers who are not using AI, for example.
1167
01:03:49.528 --> 01:03:54.349
<v SPEAKER_02>Like the thing I'm saying is that it's not so much that AI can independently do
1168
01:03:54.369 --> 01:03:57.340
<v SPEAKER_02>the job of a lawyer, because I think that's not yet true.
1169
01:03:57.390 --> 01:04:02.572
<v SPEAKER_02>But the specific skills a lawyer has over just a normal,
1170
01:04:02.692 --> 01:04:06.854
<v SPEAKER_02>generally intelligent person, those skills can be automated.
1171
01:04:07.254 --> 01:04:10.295
<v SPEAKER_02>And we don't acknowledge that because we don't,
1172
01:04:10.315 --> 01:04:12.085
<v SPEAKER_02>we acknowledge it in software engineering.
1173
01:04:12.085 --> 01:04:14.824
<v SPEAKER_02>For example, you can hire Young people
1174
01:04:14.864 --> 01:04:16.955
<v SPEAKER_02>who have like not much software engineering experience at all,
1175
01:04:17.005 --> 01:04:20.165
<v SPEAKER_02>but will just like quickly adapt to technology or able to use AI to, you know,
1176
01:04:20.205 --> 01:04:23.866
<v SPEAKER_02>and then they can create software and languages that they have no idea about.
1177
01:04:23.886 --> 01:04:25.357
<v SPEAKER_02>They don't know how this language works.
1178
01:04:25.407 --> 01:04:27.827
<v SPEAKER_02>And that's totally viable and that happens.
1179
01:04:27.847 --> 01:04:31.903
<v SPEAKER_02>Like software is like in this way, it's like a very unregulated industry.
1180
01:04:32.028 --> 01:04:34.619
<v SPEAKER_02>So if this is the sort of competitive strategy,
1181
01:04:34.669 --> 01:04:38.120
<v SPEAKER_02>people will just do it and they will just take market share and they will win
1182
01:04:38.170 --> 01:04:38.620
<v SPEAKER_02>and so on.
1183
01:04:38.670 --> 01:04:39.490
<v SPEAKER_01> Have you seen that happening?
1184
01:04:39.510 --> 01:04:42.991
<v SPEAKER_01>Have you seen people get hired to do software engineering who literally can't code,
1185
01:04:43.011 --> 01:04:44.321
<v SPEAKER_01>but just are really good at using AI?
1186
01:04:44.371 --> 01:04:46.865
<v SPEAKER_02>So literally Kant's code maybe is a bit too much,
1187
01:04:46.915 --> 01:04:51.041
<v SPEAKER_02>but who have like very little software engineering experience.
1188
01:04:51.201 --> 01:04:53.905
<v SPEAKER_02>Like I think my opinion about this is that the premium
1189
01:04:53.945 --> 01:04:56.139
<v SPEAKER_02>to software engineering experience has gone way down.
1190
01:04:56.189 --> 01:04:59.263
<v SPEAKER_02>And there's another thing that people are sort of in denial about.
1191
01:04:59.313 --> 01:05:01.605
<v SPEAKER_02>Like I think software engineering experience,
1192
01:05:01.655 --> 01:05:05.599
<v SPEAKER_02>unless you're like a very like world-class expert at like some topic
1193
01:05:05.639 --> 01:05:07.750
<v SPEAKER_02>where you're like one of the best people in the world at that thing.
1194
01:05:07.800 --> 01:05:09.021
<v SPEAKER_02>Like Jane Street, for example,
1195
01:05:09.062 --> 01:05:12.444
<v SPEAKER_02>probably has software engineering experts in particular domains
1196
01:05:12.484 --> 01:05:14.586
<v SPEAKER_02>who really do things AI can't do.
1197
01:05:15.107 --> 01:05:17.269
<v SPEAKER_02>But that is a very small set of people.
1198
01:05:17.289 --> 01:05:19.220
<v SPEAKER_02>Like most software engineers are not like that.
1199
01:05:19.270 --> 01:05:21.953
<v SPEAKER_02>So for most people, I think it's true.
1200
01:05:21.973 --> 01:05:24.245
<v SPEAKER_02>Like their software engineering experience is not worth that much.
1201
01:05:24.295 --> 01:05:26.597
<v SPEAKER_02>And there's something like general...
1202
01:05:27.527 --> 01:05:30.138
<v SPEAKER_02> Ability, general competence, execution skills.
1203
01:05:31.208 --> 01:05:34.769
<v SPEAKER_02>These things still matter a lot because execution skills are something AI is very bad at.
1204
01:05:34.789 --> 01:05:38.810
<v SPEAKER_02>So like you need to complement what they are good at with this thing.
1205
01:05:39.290 --> 01:05:43.131
<v SPEAKER_02>But look at the hiring processes like all around, like I don't know,
1206
01:05:43.151 --> 01:05:44.541
<v SPEAKER_02>big tech companies or whatever.
1207
01:05:44.591 --> 01:05:49.913
<v SPEAKER_02> Like they are just in, I think in my opinion, there's a complete denial of the situation.
1208
01:05:50.413 --> 01:05:52.693
<v SPEAKER_00>Actually, this is the thing we should talk about qualitatively in terms
1209
01:05:52.713 --> 01:05:54.154
<v SPEAKER_00>of the capabilities we will expect next year.
1210
01:05:54.174 --> 01:05:58.315
<v SPEAKER_00> But one expectation I have Sorry, maybe we get super intelligence.
1211
01:05:58.635 --> 01:06:00.847
<v SPEAKER_00>But if we don't get that, I expect it'll sort
1212
01:06:00.897 --> 01:06:03.700
<v SPEAKER_00>of be like these execution skills start getting solved.
1213
01:06:03.720 --> 01:06:07.103
<v SPEAKER_00>So it's not like you ask an AI to go do a task and he comes back
1214
01:06:07.143 --> 01:06:09.775
<v SPEAKER_00>a couple hours later, which is the kind of agents we have now.
1215
01:06:09.825 --> 01:06:14.970
<v SPEAKER_00>It's more like an always on 24 seven colleague who is just like doing things for you
1216
01:06:14.990 --> 01:06:18.383
<v SPEAKER_00>in the background, like an extremely competent person who happens to be living
1217
01:06:18.433 --> 01:06:19.433
<v SPEAKER_00>on a server.
1218
01:06:20.536 --> 01:06:25.463
<v SPEAKER_00>But the qualitative difference between a human employee and this employee is
1219
01:06:25.503 --> 01:06:30.791
<v SPEAKER_00>that AIs are just way cheaper than people and it is also far lower transaction costs
1220
01:06:31.231 --> 01:06:32.794
<v SPEAKER_00>to hiring and firing AIs.
1221
01:06:33.394 --> 01:06:36.639
<v SPEAKER_00> And so for many projects, Can I just spin up?
1222
01:06:36.659 --> 01:06:41.596
<v SPEAKER_00>Today I have 100 people working for me handling this project, just autonomously making progress.
1223
01:06:41.646 --> 01:06:43.339
<v SPEAKER_00>Tomorrow I have zero people working for me.
1224
01:06:43.389 --> 01:06:47.835
<v SPEAKER_00>But anyways, think about that transaction cost and how easy that is.
1225
01:06:47.935 --> 01:06:50.920
<v SPEAKER_00>If we actually had the capabilities in these AI systems To work
1226
01:06:50.920 --> 01:06:53.788
<v SPEAKER_00>as autonomous people do And I think that's what we're going to do.
1227
01:06:53.838 --> 01:06:57.963
<v SPEAKER_00>Compared to like hiring a new person and all this, you adverse selection,
1228
01:06:57.963 --> 01:06:59.323
<v SPEAKER_00>maybe that's a bad person.
1229
01:06:59.323 --> 01:07:01.142
<v SPEAKER_00>It takes many months for them to onboard.
1230
01:07:01.142 --> 01:07:04.365
<v SPEAKER_00>And if you want to hire a new persona, they have to relearn all those skills again.
1231
01:07:04.365 --> 01:07:07.084
<v SPEAKER_00>They can't just use the same context or fork themselves.
1232
01:07:07.084 --> 01:07:11.776
<v SPEAKER_00>And so I've always thought that the quote unquote diffusion lag right now is just
1233
01:07:11.776 --> 01:07:12.938
<v SPEAKER_00>The capabilities lack.
1234
01:07:12.938 --> 01:07:16.941
<v SPEAKER_00>That the AIs just simply lack the capabilities that humans have in learning
1235
01:07:16.981 --> 01:07:18.314
<v SPEAKER_00>on the job and so forth.
1236
01:07:18.462 --> 01:07:20.629
<v SPEAKER_00>But that if they did have those skills,
1237
01:07:20.844 --> 01:07:23.816
<v SPEAKER_00>the labor market disruption would be much bigger than people expect.
1238
01:07:23.866 --> 01:07:26.398
<v SPEAKER_00>So this is both bearishness on current capabilities.
1239
01:07:26.448 --> 01:07:27.659
<v SPEAKER_00>It's not about diffusion.
1240
01:07:27.709 --> 01:07:30.471
<v SPEAKER_00>AIs are just derpy, anamnesiac, etc.
1241
01:07:31.571 --> 01:07:36.515
<v SPEAKER_00>And it's extreme bullishness on diffusion once you do have those onboarding capabilities.
1242
01:07:37.375 --> 01:07:41.839
<v SPEAKER_02>I think that's basically right. I think it's important that my point is not
1243
01:07:41.919 --> 01:07:45.556
<v SPEAKER_02>that You can hire like a random person
1244
01:07:45.797 --> 01:07:48.601
<v SPEAKER_02>and a random person can just use the AI to like do a bunch of stuff.
1245
01:07:48.641 --> 01:07:52.587
<v SPEAKER_02>It's that it's like, because the premium to skill, like,
1246
01:07:52.627 --> 01:07:54.710
<v SPEAKER_02>because it's a complimentary, like I,
1247
01:07:54.810 --> 01:07:58.355
<v SPEAKER_02>what I'm saying is that the premium to just having a lot of hands-on You need
1248
01:07:58.375 --> 01:08:00.927
<v SPEAKER_02>to have this experience with something, especially if it's in knowledge work,
1249
01:08:00.977 --> 01:08:02.829
<v SPEAKER_02>just like that has gone down a lot.
1250
01:08:02.879 --> 01:08:05.501
<v SPEAKER_02>But correspondingly, because like the job was like,
1251
01:08:05.541 --> 01:08:07.433
<v SPEAKER_02>you need to have this experience, but you also need to be like,
1252
01:08:07.483 --> 01:08:10.946
<v SPEAKER_02>have these execution skills and you need to be sort of generally capable
1253
01:08:10.966 --> 01:08:13.158
<v SPEAKER_02>of making good judgments about various things and so on.
1254
01:08:13.208 --> 01:08:18.002
<v SPEAKER_02>So there are some general skills, which are very valuable, which have become even more valuable.
1255
01:08:18.052 --> 01:08:20.085
<v SPEAKER_02> And finding those people who are still hard.
1256
01:08:20.135 --> 01:08:21.726
<v SPEAKER_02>So it's still hard to hire people.
1257
01:08:21.776 --> 01:08:24.989
<v SPEAKER_02>It's just that you're hiring them with a slightly different criterion.
1258
01:08:25.039 --> 01:08:28.133
<v SPEAKER_02>So the point I'm making is more narrow for the immediate,
1259
01:08:28.183 --> 01:08:33.245
<v SPEAKER_02>like what's happening right now is that A lot of hiring processes were designed
1260
01:08:33.285 --> 01:08:36.366
<v SPEAKER_02>for a time when experience was very important.
1261
01:08:37.006 --> 01:08:40.895
<v SPEAKER_02>And I think that's no longer true, but the processes are not adapting.
1262
01:08:41.367 --> 01:08:45.919
<v SPEAKER_02>That's the sort of thing I'm talking about where people are in denial and them being
1263
01:08:45.969 --> 01:08:49.890
<v SPEAKER_02>in denial results in tons of inefficient and bad decision.
1264
01:08:50.331 --> 01:08:53.462
<v SPEAKER_02>As technology advances, the stakes get higher and higher and higher.
1265
01:08:53.512 --> 01:08:56.653
<v SPEAKER_02>So that's why I think it's very important for people to have an accurate assessment
1266
01:08:56.693 --> 01:08:58.383
<v SPEAKER_02>of what the technology is capable of.
1267
01:08:58.433 --> 01:09:00.114
<v SPEAKER_02>Yeah.
1268
01:09:02.181 --> 01:09:05.043
<v SPEAKER_00>Okay, so predictions for next year.
1269
01:09:07.273 --> 01:09:12.428
<v SPEAKER_00>Ege, what do you think the revenues of maybe the top AI company,
1270
01:09:12.749 --> 01:09:15.861
<v SPEAKER_00>the annualized revenue of the top AI company will be by the end of next year?
1271
01:09:15.911 --> 01:09:22.856
<v SPEAKER_02>I think maybe median estimate of like 250 or $300 billion a year or something.
1272
01:09:22.876 --> 01:09:24.437
<v SPEAKER_00>And what is it right now? What is Anthropics?
1273
01:09:24.457 --> 01:09:26.379
<v SPEAKER_02>90 or something like that. Okay.
1274
01:09:26.399 --> 01:09:30.982
<v SPEAKER_02>So like maybe two and a half to three times bigger than now is my best guess.
1275
01:09:31.537 --> 01:09:34.968
<v SPEAKER_01>I mean, I think if you ask me what does 2027 look like, I'll say, like, well,
1276
01:09:35.018 --> 01:09:37.962
<v SPEAKER_01>unfortunately, it seems like it'll look like AI 2027.
1277
01:09:39.219 --> 01:09:40.859
<v SPEAKER_01>And, you know, could be wrong.
1278
01:09:40.899 --> 01:09:43.066
<v SPEAKER_01>Like, I'm not, like, confident in that.
1279
01:09:43.400 --> 01:09:48.281
<v SPEAKER_01>But it seems to me like somewhat more likely than not they will have fully automated
1280
01:09:48.321 --> 01:09:52.562
<v SPEAKER_01>the AI research process sometime during the year of 2027 unless they get slowed down
1281
01:09:52.582 --> 01:09:54.223
<v SPEAKER_01>by the government or by voluntary slowdown,
1282
01:09:54.243 --> 01:09:55.733
<v SPEAKER_01>which I do think is substantially possible.
1283
01:09:55.783 --> 01:10:00.005
<v SPEAKER_01>Like, I am trying to make it happen that they slow down and get slowed down.
1284
01:10:00.331 --> 01:10:03.935
<v SPEAKER_01>And I think we have a shot. But yes, if they don't get slowed down, then yeah,
1285
01:10:03.975 --> 01:10:05.968
<v SPEAKER_01>I think they'll fully automate the research process.
1286
01:10:06.018 --> 01:10:08.420
<v SPEAKER_01>They'll get smarter and smarter AIs.
1287
01:10:08.741 --> 01:10:10.052
<v SPEAKER_01>How much revenue they make?
1288
01:10:10.102 --> 01:10:13.907
<v SPEAKER_01>Like, probably a lot.
1289
01:10:14.267 --> 01:10:15.849
<v SPEAKER_01>But it's also sort of one of these weird questions
1290
01:10:15.889 --> 01:10:19.443
<v SPEAKER_01>where like their main consideration won't even be revenue at that point.
1291
01:10:19.493 --> 01:10:20.993
<v SPEAKER_01>And like they might even...
1292
01:10:21.764 --> 01:10:26.872
<v SPEAKER_01>Like, stop serving products to customers and just use 100% of the compute
1293
01:10:27.132 --> 01:10:29.336
<v SPEAKER_01>for R&D instead of 70% or something.
1294
01:10:29.456 --> 01:10:32.130
<v SPEAKER_00> Right, so this is actually one of the surprising things in the S1.
1295
01:10:32.180 --> 01:10:37.226
<v SPEAKER_00>In the Anthropic S1, they said that 70% of their Compute is just going
1296
01:10:37.266 --> 01:10:41.099
<v SPEAKER_00>to internal use, which is, I think, higher than many people expected.
1297
01:10:41.168 --> 01:10:46.870
<v SPEAKER_00>So it's kind of already the case that Anthropic is an RSI company that happens
1298
01:10:46.890 --> 01:10:48.971
<v SPEAKER_00>to serve products to users.
1299
01:10:49.391 --> 01:10:54.553
<v SPEAKER_00>The other question maybe that's worth ironing out is what is the most capable
1300
01:10:54.713 --> 01:10:55.880
<v SPEAKER_00>or impressive things?
1301
01:10:56.953 --> 01:10:59.231
<v SPEAKER_00>This is a weird question for you, Daniel.
1302
01:10:59.792 --> 01:11:04.055
<v SPEAKER_00>That you expect AI to be able to do by the end of next year that is not a benchmark,
1303
01:11:04.075 --> 01:11:06.519
<v SPEAKER_00>but it is an actual realized accomplishment.
1304
01:11:06.576 --> 01:11:10.798
<v SPEAKER_00>For example, the way of solving two Millennium Prize problems was this year.
1305
01:11:11.299 --> 01:11:14.861
<v SPEAKER_00>What concrete accomplishment, Ege, do you expect,
1306
01:11:14.901 --> 01:11:17.523
<v SPEAKER_00>what is the most impressive concrete accomplishment that you expect AI assistants
1307
01:11:17.543 --> 01:11:19.321
<v SPEAKER_00>to be able to make by next year?
1308
01:11:19.384 --> 01:11:22.676
<v SPEAKER_02>I mean, this question is hard to answer because like, what is the ordering of impressiveness?
1309
01:11:22.726 --> 01:11:25.207
<v SPEAKER_02>Like, for example, I could say that, oh, I think,
1310
01:11:25.247 --> 01:11:28.259
<v SPEAKER_02>like one thing I expect over next year is that we're going to see,
1311
01:11:28.309 --> 01:11:31.899
<v SPEAKER_02>we're going to start to see Substantial, like by the end of next year,
1312
01:11:31.919 --> 01:11:34.299
<v SPEAKER_02>probably we have robots
1313
01:11:34.720 --> 01:11:41.042
<v SPEAKER_02>that can actually do like some like simple tasks at like
1314
01:11:41.062 --> 01:11:45.464
<v SPEAKER_02>a reasonable latency, not like you give the robot like two hours
1315
01:11:45.504 --> 01:11:47.024
<v SPEAKER_02>and then it can like do, you know,
1316
01:11:47.044 --> 01:11:49.155
<v SPEAKER_02>like every action takes like two minutes or whatever.
1317
01:11:49.205 --> 01:11:53.077
<v SPEAKER_02>But like because, and I just expect this because of just sort of cost trends
1318
01:11:53.127 --> 01:11:56.088
<v SPEAKER_02>where cost trends are coming down so dramatically
1319
01:11:56.128 --> 01:12:01.010
<v SPEAKER_02>that you will get like small models that are sufficiently powerful And low latency,
1320
01:12:01.270 --> 01:12:02.670
<v SPEAKER_02>that you will actually have robots
1321
01:12:02.670 --> 01:12:06.410
<v SPEAKER_02>that actually look like they can do reasonable simple physical things
1322
01:12:06.410 --> 01:12:07.027
<v SPEAKER_02>in the real world.
1323
01:12:07.027 --> 01:12:11.281
<v SPEAKER_02>And I personally think that would be very impressive if that happened
1324
01:12:11.281 --> 01:12:15.733
<v SPEAKER_02>but in some sense in a way for example we think about What would be impressive
1325
01:12:15.773 --> 01:12:17.217
<v SPEAKER_02>if a human did that thing?
1326
01:12:17.355 --> 01:12:20.430
<v SPEAKER_02>Then, of course, solving the Riemann hypothesis is way more impressive
1327
01:12:20.480 --> 01:12:23.644
<v SPEAKER_02>than folding laundry in real time or something.
1328
01:12:23.985 --> 01:12:26.158
<v SPEAKER_02>But that's not the way it works for AIs.
1329
01:12:26.208 --> 01:12:29.983
<v SPEAKER_02>And I think it's also way less economically valuable to solve the Riemann hypothesis.
1330
01:12:30.033 --> 01:12:35.037
<v SPEAKER_02> And to be able to do tasks that are off the form of folding laundry very well.
1331
01:12:35.757 --> 01:12:41.601
<v SPEAKER_02>The other thing is that I think we should expect dramatic advances in ability
1332
01:12:41.661 --> 01:12:43.673
<v SPEAKER_02>of the AI systems to do knowledge work.
1333
01:12:43.723 --> 01:12:45.754
<v SPEAKER_02>I think it was already starting a little bit.
1334
01:12:45.804 --> 01:12:48.786
<v SPEAKER_02>They're still kind of schleppy and not amazing at this,
1335
01:12:48.826 --> 01:12:52.878
<v SPEAKER_02>but I think they will get way, way better at Computer use,
1336
01:12:53.219 --> 01:12:55.700
<v SPEAKER_02>I think you will probably next year,
1337
01:12:55.860 --> 01:12:58.921
<v SPEAKER_02>you will be able to get systems that can download
1338
01:12:58.961 --> 01:13:03.463
<v SPEAKER_02>an arbitrary random computer game off of Steam and play it the way
1339
01:13:03.483 --> 01:13:05.705
<v SPEAKER_02>that a human would and just complete it.
1340
01:13:06.164 --> 01:13:08.855
<v SPEAKER_02>Not a game they were trained to play, but an arbitrary game.
1341
01:13:08.905 --> 01:13:10.238
<v SPEAKER_02>Even GTA 6 or something.
1342
01:13:10.894 --> 01:13:12.855
<v SPEAKER_00>End of 2027, probably, yes.
1343
01:13:13.595 --> 01:13:16.746
<v SPEAKER_00>Okay, so I actually am curious, what do you think is going to take,
1344
01:13:16.796 --> 01:13:18.447
<v SPEAKER_00>at the beginning of the conversation,
1345
01:13:18.497 --> 01:13:21.858
<v SPEAKER_00>you said that you expect 15 to 20 years before full automation.
1346
01:13:21.878 --> 01:13:23.258
<v SPEAKER_00>15, not 50.
1347
01:13:23.479 --> 01:13:26.690
<v SPEAKER_00>Yeah, one five, one five to 20 years before full automation.
1348
01:13:26.740 --> 01:13:27.740
<v SPEAKER_00>Of everything.
1349
01:13:27.980 --> 01:13:31.223
<v SPEAKER_00>And what do you think will take 15 years?
1350
01:13:31.604 --> 01:13:36.087
<v SPEAKER_01> If by the end of 2027, they can do the arbitrary video games thing
1351
01:13:36.748 --> 01:13:40.011
<v SPEAKER_01>and the robots thing, what's the remaining 14 years?
1352
01:13:40.391 --> 01:13:43.804
<v SPEAKER_02> I think it's just going to be the case that when you actually have these robots,
1353
01:13:43.854 --> 01:13:46.637
<v SPEAKER_02>you will feel like it is sort of like having
1354
01:13:49.450 --> 01:13:51.947
<v SPEAKER_02>Right now, looking for use agents right now. It's like...
1355
01:13:51.997 --> 01:13:56.262
<v SPEAKER_02>the way it will feel like is that they can do these isolated tasks if given
1356
01:13:56.282 --> 01:13:57.838
<v SPEAKER_02>the instructions to do them.
1357
01:13:57.965 --> 01:14:02.230
<v SPEAKER_02>But if nobody is managing them and constantly telling them what to do,
1358
01:14:02.591 --> 01:14:08.219
<v SPEAKER_02>then they won't be able to make Autonomous progress on problems overall.
1359
01:14:08.239 --> 01:14:10.382
<v SPEAKER_02>Like they will sort of not know what to do.
1360
01:14:10.402 --> 01:14:12.806
<v SPEAKER_02>This is usually what, this is what happens right now.
1361
01:14:12.826 --> 01:14:15.580
<v SPEAKER_02>Like when I use like the agent swarms, for example,
1362
01:14:15.630 --> 01:14:18.013
<v SPEAKER_02>like if I'm not supervising the swarm,
1363
01:14:18.234 --> 01:14:22.199
<v SPEAKER_02>then like the swarm just like quickly becomes They're not capable of doing anything
1364
01:14:22.219 --> 01:14:24.222
<v SPEAKER_02>in the real world. They just hit blockers.
1365
01:14:24.242 --> 01:14:26.175
<v SPEAKER_02>They don't know how to resolve them.
1366
01:14:26.225 --> 01:14:27.527
<v SPEAKER_02>They miscommunicate.
1367
01:14:27.547 --> 01:14:29.770
<v SPEAKER_02>The members of the Storm lie to each other.
1368
01:14:29.790 --> 01:14:33.255
<v SPEAKER_02>And then they forget information.
1369
01:14:33.775 --> 01:14:39.699
<v SPEAKER_02> And it's surprisingly And I think that's what we'll look like when we have these robots.
1370
01:14:39.719 --> 01:14:42.370
<v SPEAKER_02>It won't be that we suddenly have robots and we have this industrial explosion
1371
01:14:42.420 --> 01:14:43.753
<v SPEAKER_02>that suddenly takes off.
1372
01:14:43.901 --> 01:14:48.012
<v SPEAKER_02>It would initially be like, there are some tasks we can automate using these models
1373
01:14:48.062 --> 01:14:51.393
<v SPEAKER_02>that we couldn't do before because our robots were sort of too stupid.
1374
01:14:51.443 --> 01:14:55.274
<v SPEAKER_02>But we won't get a situation in which we are getting an industrial explosion
1375
01:14:55.324 --> 01:15:00.506
<v SPEAKER_02>because there will still be human bottlenecks in like management and telling
1376
01:15:00.546 --> 01:15:01.706
<v SPEAKER_02>the systems what to do and stuff like this.
1377
01:15:01.726 --> 01:15:06.495
<v SPEAKER_00> I guess the way we've seen automation in other sectors It does seem to me
1378
01:15:06.595 --> 01:15:11.582
<v SPEAKER_00>that you get a glimmer of coding ability and then you get swamped by coding ability.
1379
01:15:11.983 --> 01:15:16.289
<v SPEAKER_00>It's not like you get 5% on SweetBench and the year after you get like 10%
1380
01:15:16.309 --> 01:15:19.894
<v SPEAKER_00>and then 15% and 20% and then there's this exponential decrease.
1381
01:15:20.515 --> 01:15:24.750
<v SPEAKER_02> I would put it though, like I think we have seen a longer tail across skills.
1382
01:15:24.800 --> 01:15:28.734
<v SPEAKER_02>So I think what you're saying is correct for any like one skill that you can measure.
1383
01:15:28.784 --> 01:15:31.608
<v SPEAKER_02>But what I just expect is that there will be like more skills of its kind,
1384
01:15:31.628 --> 01:15:33.990
<v SPEAKER_02>which will, like for example, let's say you get robots,
1385
01:15:34.010 --> 01:15:36.647
<v SPEAKER_02>but they're unable to do like continual learning or something.
1386
01:15:36.697 --> 01:15:39.191
<v SPEAKER_02> And then that's, I think probably what happens actually.
1387
01:15:39.241 --> 01:15:40.974
<v SPEAKER_01>So I would totally agree with you that like,
1388
01:15:41.024 --> 01:15:44.018
<v SPEAKER_01>if we do the super intelligence first thing and then do the robots,
1389
01:15:44.068 --> 01:15:46.051
<v SPEAKER_01>then it will hit us like a truck.
1390
01:15:46.231 --> 01:15:50.838
<v SPEAKER_01>But if we instead do robots in the ordinary way, then for some period of time,
1391
01:15:50.858 --> 01:15:53.893
<v SPEAKER_01>they will be exactly Like you described where, you know, they,
1392
01:15:53.943 --> 01:15:55.605
<v SPEAKER_01>they can do a specific task if you tell it to,
1393
01:15:55.625 --> 01:15:58.950
<v SPEAKER_01>but if you give it a more ambitious longer task and like keep the house clean
1394
01:15:58.970 --> 01:16:02.085
<v SPEAKER_01>or something, then they'll get stuck or, you know, flail around.
1395
01:16:02.135 --> 01:16:05.470
<v SPEAKER_01>But I would apply the concept of horizon links here and say that like,
1396
01:16:05.520 --> 01:16:08.853
<v SPEAKER_01>probably just like with many They would start off like that,
1397
01:16:08.903 --> 01:16:11.105
<v SPEAKER_01>but then the horizon length of tasks
1398
01:16:11.125 --> 01:16:13.747
<v SPEAKER_01>that they can autonomously do would double twice a year or double three times
1399
01:16:13.787 --> 01:16:17.741
<v SPEAKER_01>a year. And so then it seems hard to get 15 years if that's what you're doing,
1400
01:16:17.791 --> 01:16:20.263
<v SPEAKER_01>because even after just the first three years,
1401
01:16:20.313 --> 01:16:23.091
<v SPEAKER_01>you're getting 100x improvement in horizon length.
1402
01:16:23.236 --> 01:16:26.792
<v SPEAKER_01>And so it seems to me that if you think that by the end of 2027,
1403
01:16:26.879 --> 01:16:31.363
<v SPEAKER_01>the AIs would be able to do dishes or fold laundry when someone tells them to,
1404
01:16:31.783 --> 01:16:36.568
<v SPEAKER_01>then it seems like By 2030, they should be able to just manage the house
1405
01:16:36.728 --> 01:16:37.749
<v SPEAKER_01>or something.
1406
01:16:38.290 --> 01:16:41.353
<v SPEAKER_02>I'm not sure actually, for example, what the horizon,
1407
01:16:41.453 --> 01:16:47.319
<v SPEAKER_02>the concept of horizon seems like too much of a leaky abstraction to me here.
1408
01:16:47.419 --> 01:16:53.405
<v SPEAKER_02>Because when I use agents for coding stuff,
1409
01:16:53.485 --> 01:16:58.434
<v SPEAKER_02>there are tasks which would take a human Many weeks like they can do.
1410
01:17:00.015 --> 01:17:05.015
<v SPEAKER_02>But there are other tasks that would take a human like 10 minutes that like they can't do.
1411
01:17:05.296 --> 01:17:10.557
<v SPEAKER_02>And often it's not even like easy to understand like how these tasks are distributed.
1412
01:17:10.577 --> 01:17:14.618
<v SPEAKER_02>Like a task can be look extremely technically complicated and ambitious and like,
1413
01:17:14.638 --> 01:17:18.305
<v SPEAKER_02>I don't know, I take this program and like completely formalize it
1414
01:17:18.379 --> 01:17:19.990
<v SPEAKER_02>and then prove things about it or whatever.
1415
01:17:20.040 --> 01:17:22.690
<v SPEAKER_02>And like this is the kind of thing that a human would take like many months
1416
01:17:22.740 --> 01:17:25.221
<v SPEAKER_02>and then like an agent can do it and the agent can do it in like hours
1417
01:17:25.241 --> 01:17:26.852
<v SPEAKER_02>or something like that often.
1418
01:17:27.883 --> 01:17:31.228
<v SPEAKER_02>While a much simpler task like, okay,
1419
01:17:32.350 --> 01:17:37.677
<v SPEAKER_02>I'm going to put you in charge of looking at other people's changes to this codebase
1420
01:17:38.038 --> 01:17:41.513
<v SPEAKER_02>and make sure you don't approve something if it looks obviously dumb.
1421
01:17:41.563 --> 01:17:42.952
<v SPEAKER_02> Or like break something.
1422
01:17:43.364 --> 01:17:48.945
<v SPEAKER_02>And this kind of thing, like they just can't like retain like memory.
1423
01:17:48.985 --> 01:17:52.676
<v SPEAKER_02>They can't understand what that means or like something for something to be bad
1424
01:17:52.726 --> 01:17:54.487
<v SPEAKER_02>or dangerous to merge.
1425
01:17:55.127 --> 01:18:00.848
<v SPEAKER_02>And I think it's because like there's too much context and like they Are bad
1426
01:18:00.928 --> 01:18:06.011
<v SPEAKER_02>at arranging information in such a way that they retain all the context.
1427
01:18:06.031 --> 01:18:07.592
<v SPEAKER_02>They know what's relevant, what's not relevant.
1428
01:18:07.612 --> 01:18:09.323
<v SPEAKER_02>There seems to be something missing there.
1429
01:18:09.373 --> 01:18:14.656
<v SPEAKER_02>And I think it's causing their horizon lengths to be extremely jagged.
1430
01:18:15.556 --> 01:18:19.108
<v SPEAKER_02>And I think on the tasks to show off the second type that I'm talking about,
1431
01:18:19.158 --> 01:18:23.510
<v SPEAKER_02>I don't think we've been seeing progress that is like 10x a year in horizon length.
1432
01:18:23.560 --> 01:18:24.941
<v SPEAKER_01> This is a live question for me.
1433
01:18:24.981 --> 01:18:26.522
<v SPEAKER_01>I think this is something that's somewhat cruxy for me.
1434
01:18:26.562 --> 01:18:27.895
<v SPEAKER_01>And if I thought that...
1435
01:18:29.491 --> 01:18:32.722
<v SPEAKER_01>If I were more convinced that they were like really not improving that much
1436
01:18:32.772 --> 01:18:34.933
<v SPEAKER_01>at a whole range of really important skills,
1437
01:18:34.953 --> 01:18:37.564
<v SPEAKER_01>that would lengthen my timelines significantly.
1438
01:18:37.694 --> 01:18:43.177
<v SPEAKER_01>So I guess one question I have is how much hard evidence do we have that this is
1439
01:18:43.197 --> 01:18:46.918
<v SPEAKER_01>the case versus just like anecdotes, if that makes sense.
1440
01:18:47.578 --> 01:18:52.760
<v SPEAKER_01>Because I think that like a sort of like, I guess skeptical of this hypothesis,
1441
01:18:52.780 --> 01:18:56.447
<v SPEAKER_01>but more bullish hypothesis overall about AI would be that like...
1442
01:18:57.398 --> 01:19:00.690
<v SPEAKER_01> At any given level of AI capability, there will still be things that they still can't do.
1443
01:19:00.740 --> 01:19:03.761
<v SPEAKER_01>And so as you give your AI's more ambitious task,
1444
01:19:03.801 --> 01:19:06.572
<v SPEAKER_01>you'll still notice that they're failing at this sort of thing.
1445
01:19:06.622 --> 01:19:09.113
<v SPEAKER_01>And so you'll constantly be running up against their failures.
1446
01:19:09.163 --> 01:19:11.944
<v SPEAKER_01>And that might give them this leading impression that they're not really improving
1447
01:19:11.964 --> 01:19:15.486
<v SPEAKER_01>that much, even if the things that they're failing at are more impressive
1448
01:19:15.526 --> 01:19:17.117
<v SPEAKER_01>than the things they were failing at two years ago,
1449
01:19:17.167 --> 01:19:19.378
<v SPEAKER_01>which were more impressive than the things they were failing at.
1450
01:19:19.428 --> 01:19:20.968
<v SPEAKER_01>Does that make sense?
1451
01:19:21.088 --> 01:19:22.977
<v SPEAKER_01>So basically, one thought is like,
1452
01:19:23.029 --> 01:19:25.301
<v SPEAKER_01>How confident are you that they really aren't improving that much
1453
01:19:25.351 --> 01:19:27.762
<v SPEAKER_01>over the years versus they are improving a lot.
1454
01:19:27.812 --> 01:19:34.696
<v SPEAKER_01>It's just that there's a significant order of magnitude or two gap, if that makes sense.
1455
01:19:34.896 --> 01:19:37.237
<v SPEAKER_02>I think it's difficult to name a task
1456
01:19:37.838 --> 01:19:42.100
<v SPEAKER_02>where the AIs are not making significant progress.
1457
01:19:42.560 --> 01:19:47.393
<v SPEAKER_02>That was not true, I think, some number of years ago, but right now I think it is true.
1458
01:19:47.690 --> 01:19:49.911
<v SPEAKER_02>So I think like the difference here is more like,
1459
01:19:49.931 --> 01:19:52.251
<v SPEAKER_02>do you think the progress in some metric,
1460
01:19:52.271 --> 01:19:53.652
<v SPEAKER_02>like let's say horizon length or something like that,
1461
01:19:53.692 --> 01:19:57.003
<v SPEAKER_02>is it like two to three X a year or is it more like 10 or a hundred X a year?
1462
01:19:57.053 --> 01:19:59.714
<v SPEAKER_02>So like, that's the more, there's more like a quantitative questions as opposed
1463
01:19:59.734 --> 01:20:02.012
<v SPEAKER_02>to like, are they making progress or not?
1464
01:20:02.615 --> 01:20:06.790
<v SPEAKER_02>For example, I think in the skill
1465
01:20:06.810 --> 01:20:11.195
<v SPEAKER_02>of writing an original novel or something
1466
01:20:11.215 --> 01:20:16.100
<v SPEAKER_02>that is good, I think the progress since last year is definitely not 100x.
1467
01:20:16.681 --> 01:20:18.453
<v SPEAKER_02>I think it's probably not even 10x.
1468
01:20:18.503 --> 01:20:21.076
<v SPEAKER_02>I think it might be like 3x, but it's very subjective.
1469
01:20:21.126 --> 01:20:22.848
<v SPEAKER_02>It's very hard to measure this.
1470
01:20:22.969 --> 01:20:27.235
<v SPEAKER_02>But I think with a lot of these things, we don't have anything like the meters,
1471
01:20:27.275 --> 01:20:29.258
<v SPEAKER_02>like time horizon benchmark.
1472
01:20:29.578 --> 01:20:32.342
<v SPEAKER_02>So it makes it difficult to settle these questions because I'm just having
1473
01:20:32.362 --> 01:20:34.755
<v SPEAKER_02>to make these intuitive judgments because we don't have good benchmarks.
1474
01:20:34.805 --> 01:20:36.398
<v SPEAKER_02>So we're totally wrong about some of this.
1475
01:20:36.448 --> 01:20:40.004
<v SPEAKER_02>And if you could quantify it, it will come out that I was wrong.
1476
01:20:42.053 --> 01:20:43.214
<v SPEAKER_02>With the time horizon thing,
1477
01:20:43.234 --> 01:20:46.566
<v SPEAKER_02>I think the issue is that the moment you turn it into a benchmark,
1478
01:20:46.616 --> 01:20:52.640
<v SPEAKER_02>it has to be something that AIs can already do reasonably well enough and that can
1479
01:20:52.680 --> 01:20:54.551
<v SPEAKER_02>then become an optimization target.
1480
01:20:54.601 --> 01:20:56.863
<v SPEAKER_02>And that makes it relatively easy.
1481
01:20:58.363 --> 01:20:59.919
<v SPEAKER_02>To like make progress on it.
1482
01:21:00.444 --> 01:21:01.705
<v SPEAKER_02>My guess of what would have,
1483
01:21:01.745 --> 01:21:05.727
<v SPEAKER_02>what would happen for the meter time horizons thing is that, and I've said this,
1484
01:21:05.747 --> 01:21:07.648
<v SPEAKER_02>I think early last year, there's like,
1485
01:21:07.668 --> 01:21:10.859
<v SPEAKER_02>this is basically going to diverge that we're going to get an infinite,
1486
01:21:10.909 --> 01:21:12.950
<v SPEAKER_02>near infinite time horizon, but the AIs,
1487
01:21:12.990 --> 01:21:15.691
<v SPEAKER_02>there will be still like a bunch of like just 10 minute tasks that the AIs can't,
1488
01:21:15.711 --> 01:21:18.722
<v SPEAKER_02>can't actually do that very well because of just distributional shifts.
1489
01:21:18.772 --> 01:21:21.161
<v SPEAKER_02>And I think that is basically happened now.
1490
01:21:22.594 --> 01:21:26.186
<v SPEAKER_02>Like they stopped reporting the numbers because like it was diverging.
1491
01:21:26.236 --> 01:21:29.907
<v SPEAKER_02> But I think Take a domain image taking a 10 minute test now.
1492
01:21:30.807 --> 01:21:33.229
<v SPEAKER_02>What is the length of the task that they will be able to do in that domain
1493
01:21:33.269 --> 01:21:34.880
<v SPEAKER_02>in like one or two or three years?
1494
01:21:34.930 --> 01:21:37.763
<v SPEAKER_02>I think it's probably just a very domain sensitive.
1495
01:21:38.433 --> 01:21:40.635
<v SPEAKER_02>So I don't really have a very good answer to this question
1496
01:21:40.655 --> 01:21:45.779
<v SPEAKER_02>because I think we don't have like a good benchmark that can settle this question.
1497
01:21:46.259 --> 01:21:48.861
<v SPEAKER_02>It's just my intuitive judgment based on using the systems
1498
01:21:48.901 --> 01:21:52.044
<v SPEAKER_02>that they seem like they made like vast,
1499
01:21:52.104 --> 01:21:56.687
<v SPEAKER_02>vast progress in math or like probably even more than 100x in terms
1500
01:21:56.728 --> 01:21:57.895
<v SPEAKER_02>of like time horizon.
1501
01:21:58.089 --> 01:22:03.448
<v SPEAKER_02>And over the last year, And in some other domain, like, I don't know,
1502
01:22:03.468 --> 01:22:08.210
<v SPEAKER_02>like sending emails on my behalf that are not like confusing and that people
1503
01:22:08.270 --> 01:22:10.522
<v SPEAKER_02>on the other side can understand or something like that.
1504
01:22:10.572 --> 01:22:13.713
<v SPEAKER_02>I feel like the progress is much, much, much less.
1505
01:22:13.793 --> 01:22:16.071
<v SPEAKER_00>I mean, I'll give you a concrete example.
1506
01:22:17.155 --> 01:22:21.617
<v SPEAKER_00>I have been for many years asking any AI CEO who comes on my podcast,
1507
01:22:22.098 --> 01:22:25.987
<v SPEAKER_00>how soon before they can automate being a video editor for my podcast.
1508
01:22:26.240 --> 01:22:31.880
<v SPEAKER_00>I think the time horizon on that has like Maybe doubled over the last year
1509
01:22:31.900 --> 01:22:33.191
<v SPEAKER_00>and a half or something.
1510
01:22:33.241 --> 01:22:36.184
<v SPEAKER_00>But if I give Fable a transcript of my podcast and I'm like,
1511
01:22:36.224 --> 01:22:38.936
<v SPEAKER_00>how should this be reorganized to be more coherent?
1512
01:22:38.986 --> 01:22:43.097
<v SPEAKER_00>It's just not clear that there's been that much progress from Claw at 3.7.
1513
01:22:43.372 --> 01:22:46.093
<v SPEAKER_02>Yeah, I think that sort of matches my qualitative impression.
1514
01:22:46.113 --> 01:22:50.554
<v SPEAKER_02>But I thought when I was using the models that there was a pretty big leap in,
1515
01:22:50.594 --> 01:22:54.215
<v SPEAKER_02>for example, writing quality with 3.6 on it.
1516
01:22:54.795 --> 01:22:58.456
<v SPEAKER_02>It felt like the first model I could actually use to try to write stories
1517
01:22:58.496 --> 01:22:59.446
<v SPEAKER_02>and fiction or whatever.
1518
01:22:59.496 --> 01:23:03.496
<v SPEAKER_02>And it actually would be decent or something if a human was managing it.
1519
01:23:03.678 --> 01:23:06.558
<v SPEAKER_02>And the current state we were at, they can write somewhat longer things,
1520
01:23:06.578 --> 01:23:09.819
<v SPEAKER_02>but definitely 100x longer without it becoming bad.
1521
01:23:10.219 --> 01:23:14.503
<v SPEAKER_02> And I agree with Dwarkesh that it didn't Effective time horizon.
1522
01:23:14.563 --> 01:23:18.715
<v SPEAKER_02>Maybe I would be like more than 2x over the last one and a half years, but like,
1523
01:23:18.765 --> 01:23:22.197
<v SPEAKER_02>I think it's not more than 10x over the last one and a half years, but it's very,
1524
01:23:22.247 --> 01:23:23.728
<v SPEAKER_02>like, very subjective.
1525
01:23:24.228 --> 01:23:30.571
<v SPEAKER_02>I think this is some evidence for the fact that this rate of progress is incredibly jagged.
1526
01:23:30.671 --> 01:23:33.513
<v SPEAKER_02>Like on math, it was like, since two years ago, it's like, I don't know,
1527
01:23:33.533 --> 01:23:36.084
<v SPEAKER_02>like a million times or something. You couldn't make that case.
1528
01:23:36.134 --> 01:23:38.356
<v SPEAKER_02>It's like some ridiculously high number.
1529
01:23:39.819 --> 01:23:43.091
<v SPEAKER_01>I guess my follow-up question then, and I think this is plausible,
1530
01:23:43.141 --> 01:23:46.113
<v SPEAKER_01>my follow-up question then is to what extent can this be explained
1531
01:23:46.163 --> 01:23:47.964
<v SPEAKER_01>by the training environments?
1532
01:23:48.304 --> 01:23:51.726
<v SPEAKER_01>Like I would imagine that they have a lot of training environments that are
1533
01:23:51.746 --> 01:23:54.618
<v SPEAKER_01>of the form like prove this theorem or disprove this theorem.
1534
01:23:54.668 --> 01:23:55.789
<v SPEAKER_01>And a lot of training environments that are
1535
01:23:55.809 --> 01:23:58.850
<v SPEAKER_01>of the form like solve this coding problem or write this piece of software
1536
01:23:58.871 --> 01:24:00.482
<v SPEAKER_01>that passes these unit tests.
1537
01:24:00.732 --> 01:24:02.621
<v SPEAKER_01>And not very many coding problems,
1538
01:24:02.813 --> 01:24:06.615
<v SPEAKER_01>not many problems that are of the form like Make a good aesthetic judgment about how
1539
01:24:06.635 --> 01:24:08.913
<v SPEAKER_01>to organize clips or something like that.
1540
01:24:09.495 --> 01:24:12.026
<v SPEAKER_01>Because it's harder to set up that sort of environment.
1541
01:24:12.076 --> 01:24:15.267
<v SPEAKER_01>And maybe also because it's less lucrative, although I'm not sure about that.
1542
01:24:15.317 --> 01:24:17.477
<v SPEAKER_01>So, I mean, you work at Dmine.
1543
01:24:17.497 --> 01:24:21.639
<v SPEAKER_01>So do you think that a lot of this jaggedness is basically downstream of just
1544
01:24:21.679 --> 01:24:22.901
<v SPEAKER_01>the task distribution?
1545
01:24:22.979 --> 01:24:24.389
<v SPEAKER_01>Or do you think that it's like, oh no,
1546
01:24:24.439 --> 01:24:27.580
<v SPEAKER_01>I've seen examples of the company trying really hard to collect a lot
1547
01:24:27.600 --> 01:24:30.211
<v SPEAKER_01>of high quality data and training environments for a particular type
1548
01:24:30.261 --> 01:24:33.182
<v SPEAKER_01>of 10-minute task such as that,
1549
01:24:33.522 --> 01:24:36.522
<v SPEAKER_01>and then just still failing to get the AIs good at it.
1550
01:24:38.264 --> 01:24:41.264
<v SPEAKER_02>I can't speak to what the company is doing internally.
1551
01:24:41.625 --> 01:24:45.907
<v SPEAKER_02>What I can say is that based on just public evidence,
1552
01:24:46.007 --> 01:24:51.288
<v SPEAKER_02>you can see that some things are it's much easier
1553
01:24:51.288 --> 01:24:54.051
<v SPEAKER_02>to Like, there's, like,
1554
01:24:54.111 --> 01:24:57.794
<v SPEAKER_02>a cost to verification that I think is, like, driving a lot of this.
1555
01:24:57.814 --> 01:25:00.577
<v SPEAKER_02>Like, I don't really agree with the split that, like, some tasks are verified,
1556
01:25:00.597 --> 01:25:01.537
<v SPEAKER_02>but some are not verified.
1557
01:25:01.557 --> 01:25:06.222
<v SPEAKER_02>Because, for example, did you produce a video for his podcast that will make, like,
1558
01:25:06.242 --> 01:25:07.273
<v SPEAKER_02>Dwarkesh happy or something?
1559
01:25:07.323 --> 01:25:08.363
<v SPEAKER_01>That's a verifiable task.
1560
01:25:08.383 --> 01:25:11.735
<v SPEAKER_02>You can give the video to him. And he's like what the hell is this or something.
1561
01:25:11.785 --> 01:25:15.039
<v SPEAKER_02> But the issue is that's very expensive way to get feedback.
1562
01:25:15.089 --> 01:25:18.754
<v SPEAKER_02>So the difference with math is that math is very cheap to get feedback.
1563
01:25:18.774 --> 01:25:21.857
<v SPEAKER_02>There's a very cheap verifier.
1564
01:25:21.957 --> 01:25:26.233
<v SPEAKER_02>I think that does have a huge effect because the way you should think about it is
1565
01:25:26.283 --> 01:25:31.839
<v SPEAKER_02>that how efficiently can you Like sample trajectories
1566
01:25:33.085 --> 01:25:35.001
<v SPEAKER_02>that give you the right answer.
1567
01:25:35.021 --> 01:25:39.153
<v SPEAKER_02>How fast can you discriminate things that are worth from those that don't work?
1568
01:25:39.203 --> 01:25:42.575
<v SPEAKER_02>And that's a very fundamental thing for like how efficiently you can learn things.
1569
01:25:42.625 --> 01:25:45.686
<v SPEAKER_02>One thing, for example, that makes me more skeptical of sort
1570
01:25:45.726 --> 01:25:50.590
<v SPEAKER_02>of software-only singularity type stories is because While I agree
1571
01:25:50.630 --> 01:25:56.258
<v SPEAKER_02>that ML research is a verifiable domain, I think in practice,
1572
01:25:56.779 --> 01:26:00.104
<v SPEAKER_02>a lot of the verification is quite expensive.
1573
01:26:00.925 --> 01:26:03.409
<v SPEAKER_02>So this is why compute matters so much.
1574
01:26:04.270 --> 01:26:07.492
<v SPEAKER_02> Computers are so important for like algorithmic progress.
1575
01:26:07.572 --> 01:26:10.484
<v SPEAKER_02>Like you can have innovations at small scales that fail at large scales.
1576
01:26:10.534 --> 01:26:13.737
<v SPEAKER_02>You can have innovations that only work at large scales that you can never confirm
1577
01:26:13.777 --> 01:26:15.908
<v SPEAKER_02>by experiments at small scales because they just completely fail.
1578
01:26:15.958 --> 01:26:19.291
<v SPEAKER_02>Like you get false positives and the false negatives in both directions.
1579
01:26:19.341 --> 01:26:22.663
<v SPEAKER_02>And if you want to collect a bunch of data about this to train
1580
01:26:22.683 --> 01:26:26.356
<v SPEAKER_02>the model set better taste, well, that needs a lot of compute as well.
1581
01:26:26.406 --> 01:26:30.406
<v SPEAKER_02> And probably more and more as you scale up the size of the experiments.
1582
01:26:30.808 --> 01:26:36.031
<v SPEAKER_02>So that makes me like not put as much credit on the arguments that say, look,
1583
01:26:36.051 --> 01:26:39.523
<v SPEAKER_02>we made like a decade of progress in like one or two months in math.
1584
01:26:39.573 --> 01:26:43.365
<v SPEAKER_02>And therefore we should expect like a decade of progress in ML research,
1585
01:26:43.415 --> 01:26:46.365
<v SPEAKER_02>because I think that The cost of verification,
1586
01:26:46.385 --> 01:26:51.849
<v SPEAKER_02>if you sort of think of like the dollar cost of verifying some idea in ML research
1587
01:26:52.109 --> 01:26:56.232
<v SPEAKER_02>and compared to the dollar cost of verifying a math proof, like it's many,
1588
01:26:56.252 --> 01:26:57.883
<v SPEAKER_02>many orders of magnitude apart.
1589
01:26:57.933 --> 01:27:02.510
<v SPEAKER_02>Like you're seeing if like some proof of the Riemann hypothesis in Lean is correct or not.
1590
01:27:02.560 --> 01:27:04.711
<v SPEAKER_02> You can do that on your personal computer.
1591
01:27:04.761 --> 01:27:07.722
<v SPEAKER_02>It's very easy to just check.
1592
01:27:07.742 --> 01:27:10.492
<v SPEAKER_02>There's a linear time algorithm for checking proofs, basically.
1593
01:27:10.542 --> 01:27:14.103
<v SPEAKER_02>While if you're trying to figure out, is this idea of, oh,
1594
01:27:14.183 --> 01:27:17.404
<v SPEAKER_02>I have this fancy change to this optimizer,
1595
01:27:17.664 --> 01:27:20.615
<v SPEAKER_02>does that give me a computer efficiency when I'm pre-training or not?
1596
01:27:20.665 --> 01:27:22.756
<v SPEAKER_02>It's very hard to settle that question.
1597
01:27:22.806 --> 01:27:25.727
<v SPEAKER_02>You can do small-scale experiments that can look like it works,
1598
01:27:25.767 --> 01:27:27.747
<v SPEAKER_02>but then you scale it up and then, oh, wait, it doesn't work.
1599
01:27:27.767 --> 01:27:28.767
<v SPEAKER_02>What's going on?
1600
01:27:28.848 --> 01:27:29.959
<v SPEAKER_02>It's very confusing.
1601
01:27:30.588 --> 01:27:34.124
<v SPEAKER_02> So to me, it looks like the cost of verification is like much, much higher.
1602
01:27:34.174 --> 01:27:37.839
<v SPEAKER_02>And that's one that's I think probably like almost the key reason to expect
1603
01:27:37.859 --> 01:27:43.467
<v SPEAKER_02>that domain to be significantly more difficult to automate.
1604
01:27:43.548 --> 01:27:46.130
<v SPEAKER_02> It's not, you know, it's not That humans are very good at it
1605
01:27:46.150 --> 01:27:48.131
<v SPEAKER_02>because I think humans are also kind of bad at ML research,
1606
01:27:48.171 --> 01:27:49.662
<v SPEAKER_02>just like we're bad at math.
1607
01:27:49.712 --> 01:27:54.594
<v SPEAKER_02>It's just that AIs due to their current like sample and stuff like
1608
01:27:54.634 --> 01:27:58.735
<v SPEAKER_02>that really benefit from being able to get just a ton of data in there.
1609
01:27:58.895 --> 01:28:04.998
<v SPEAKER_02>And that is very contingent on there being a very cheap verification procedure
1610
01:28:05.258 --> 01:28:06.799
<v SPEAKER_02>for whether you did the right thing or not.
1611
01:28:06.819 --> 01:28:10.020
<v SPEAKER_02>Like the more expensive that is, the slower.
1612
01:28:12.185 --> 01:28:13.796
<v SPEAKER_02> The slower you make progress, basically.
1613
01:28:13.846 --> 01:28:16.078
<v SPEAKER_02>So that's sort of my rough take about this.
1614
01:28:16.128 --> 01:28:19.601
<v SPEAKER_00>There is some argument about generalization with respect to the cost.
1615
01:28:19.651 --> 01:28:24.535
<v SPEAKER_00>Even in math, presumably the way that these models became good at, say, you know,
1616
01:28:24.935 --> 01:28:27.237
<v SPEAKER_00>being able to accommodate billions of tokens,
1617
01:28:27.257 --> 01:28:33.081
<v SPEAKER_00>was hundreds of millions of tokens in order to solve Navier Stokes across a swarm
1618
01:28:33.121 --> 01:28:36.644
<v SPEAKER_00>of thousands of agents was not that many other tasks
1619
01:28:36.904 --> 01:28:39.950
<v SPEAKER_00>where a thousand agents collaborated in order to Just solve a math proof
1620
01:28:39.950 --> 01:28:43.590
<v SPEAKER_00>and spend tens of millions of dollars worth of tokens to do so.
1621
01:28:43.810 --> 01:28:47.790
<v SPEAKER_00>There was some generalization to a much more ambitious kind of assignment
1622
01:28:47.790 --> 01:28:49.880
<v SPEAKER_00>from the math training that they underwent.
1623
01:28:49.930 --> 01:28:52.995
<v SPEAKER_00>So then the question is, will you see that kind of generalization in AI research?
1624
01:28:52.995 --> 01:28:55.183
<v SPEAKER_00>Now, of course they're much more sample efficient than humans.
1625
01:28:55.183 --> 01:28:58.477
<v SPEAKER_00>So you can't use this as a exact analogy,
1626
01:28:59.215 --> 01:29:03.852
<v SPEAKER_00>but my understanding is that it is the case that Researchers who were in the field
1627
01:29:03.892 --> 01:29:07.574
<v SPEAKER_00>in say 2020 when there was much less compute being used and a level of compute
1628
01:29:07.594 --> 01:29:12.376
<v SPEAKER_00>that can be part of the training process now are good at like doing AI research now,
1629
01:29:12.436 --> 01:29:12.556
<v SPEAKER_00>right?
1630
01:29:12.576 --> 01:29:17.119
<v SPEAKER_00>Like there's some lessons they learned from training GPT-2 or GPT-3 size models
1631
01:29:17.559 --> 01:29:21.059
<v SPEAKER_00>that are helping them do good research at the current frontier.
1632
01:29:21.281 --> 01:29:24.392
<v SPEAKER_00>And so it does seem like you should expect to see this kind of generalization.
1633
01:29:24.442 --> 01:29:29.306
<v SPEAKER_00>I agree that you could not verify at the scale Or you could not cheaply
1634
01:29:29.466 --> 01:29:32.449
<v SPEAKER_00>and consistently verify at the scale at which you'd need
1635
01:29:32.489 --> 01:29:34.120
<v SPEAKER_00>the AI researchers operating at.
1636
01:29:34.170 --> 01:29:36.532
<v SPEAKER_02>I totally agree with that. I think you should expect to see a lot of generalization.
1637
01:29:36.552 --> 01:29:39.108
<v SPEAKER_02>In fact, we have seen a lot of generalization.
1638
01:29:39.235 --> 01:29:41.624
<v SPEAKER_02>As you said, just based on leverage stocks.
1639
01:29:42.818 --> 01:29:47.863
<v SPEAKER_02>The other thing I would say is that there is such a thing as...
1640
01:29:50.025 --> 01:29:51.247
<v SPEAKER_02> General intelligence.
1641
01:29:51.608 --> 01:29:54.292
<v SPEAKER_02>And at least for the base models,
1642
01:29:54.312 --> 01:29:57.486
<v SPEAKER_02>I think pre-training loss is a pretty good proxy for that thing.
1643
01:29:57.536 --> 01:30:02.584
<v SPEAKER_02>And it does just predict in a bunch of ways.
1644
01:30:02.604 --> 01:30:06.809
<v SPEAKER_02>Will the model understand some subtlety about your request
1645
01:30:06.889 --> 01:30:09.692
<v SPEAKER_02>and interpret it correctly, even though it was ambiguous and all kinds
1646
01:30:09.732 --> 01:30:11.795
<v SPEAKER_02>of things were normally associated with intelligence.
1647
01:30:11.815 --> 01:30:12.906
<v SPEAKER_02>It just does predict it.
1648
01:30:12.956 --> 01:30:19.223
<v SPEAKER_02>So there's obviously the entire reason this field works at all is because this concept exists.
1649
01:30:19.243 --> 01:30:22.246
<v SPEAKER_02>Otherwise this wouldn't work. So I totally agree with that.
1650
01:30:22.266 --> 01:30:24.408
<v SPEAKER_02>I just think the combination of
1651
01:30:26.984 --> 01:30:31.729
<v SPEAKER_02>For example, there's this plot that was published by Anthropic
1652
01:30:31.769 --> 01:30:34.952
<v SPEAKER_02>about pre-taining compute multiplier sizes or something like that.
1653
01:30:34.972 --> 01:30:39.750
<v SPEAKER_02>They didn't report actual sizes, but there was a plot published in their IPO roadshow.
1654
01:30:42.013 --> 01:30:45.036
<v SPEAKER_02> I have some difficulty interpreting that plot.
1655
01:30:45.056 --> 01:30:49.817
<v SPEAKER_02>I can't exactly say what I think is wrong with it,
1656
01:30:49.857 --> 01:30:56.339
<v SPEAKER_02>but I think they're not disclosing a lot of information that is relevant
1657
01:30:56.419 --> 01:31:01.880
<v SPEAKER_02>for thinking if you trust their judgment of what's going on or not.
1658
01:31:02.080 --> 01:31:05.461
<v SPEAKER_02>I can say based on the information I have that I don't trust their judgment
1659
01:31:05.501 --> 01:31:08.722
<v SPEAKER_02>of what's going on, but I can't explain why.
1660
01:31:08.822 --> 01:31:10.470
<v SPEAKER_02>So that's a little bit unsatisfying.
1661
01:31:10.520 --> 01:31:12.512
<v SPEAKER_01>Does that mean you think that there hasn't been an acceleration
1662
01:31:12.562 --> 01:31:15.729
<v SPEAKER_01>in pre-training progress over the last year at Anthropic?
1663
01:31:16.906 --> 01:31:19.588
<v SPEAKER_02>I would say that question is poorly posed,
1664
01:31:20.048 --> 01:31:24.326
<v SPEAKER_02>but I don't think I can elaborate more than that without revealing something.
1665
01:31:25.213 --> 01:31:28.536
<v SPEAKER_02>But I think you can say there has been.
1666
01:31:28.956 --> 01:31:32.289
<v SPEAKER_02>It kind of depends on how you interpret the question. Interesting.
1667
01:31:32.339 --> 01:31:34.791
<v SPEAKER_00>I'll put that in the cloud and see what it thinks.
1668
01:31:34.841 --> 01:31:36.051
<v SPEAKER_00>What it thinks you mean.
1669
01:31:36.101 --> 01:31:39.305
<v SPEAKER_01>It's an update to hear that you don't believe it. Yeah.
1670
01:31:39.325 --> 01:31:40.446
<v SPEAKER_02>I'm not saying I don't believe it.
1671
01:31:40.466 --> 01:31:44.811
<v SPEAKER_02>I'm saying I think the thing they are reporting is like, holy po.
1672
01:31:44.831 --> 01:31:47.220
<v SPEAKER_02>So I'm not saying they made up the numbers.
1673
01:31:47.314 --> 01:31:51.749
<v SPEAKER_02>Like I think there is a real graph inside Anthropik that probably looks like that.
1674
01:31:51.799 --> 01:31:54.132
<v SPEAKER_02>Like it's not a fake, like they didn't fabricate the numbers.
1675
01:31:54.182 --> 01:32:00.637
<v SPEAKER_02> It's just that I think that that doesn't Doesn't mean what they are portraying it to me.
1676
01:32:00.737 --> 01:32:02.199
<v SPEAKER_00>I mean, I'm guessing what you're referring to is
1677
01:32:02.239 --> 01:32:07.265
<v SPEAKER_00>that there's some synthetic data type compute multiplier that makes it look like
1678
01:32:07.765 --> 01:32:12.098
<v SPEAKER_00>the loss on that corpus is higher, but maybe in a way that doesn't generalize.
1679
01:32:12.210 --> 01:32:13.291
<v SPEAKER_00>Of course, I can only speculate,
1680
01:32:13.331 --> 01:32:17.215
<v SPEAKER_00>but these are the kinds of things one could think Make
1681
01:32:17.255 --> 01:32:18.907
<v SPEAKER_00>the pre-returning thing misleading.
1682
01:32:18.957 --> 01:32:20.118
<v SPEAKER_00>Yeah, I can't comment on that.
1683
01:32:20.138 --> 01:32:25.503
<v SPEAKER_02>But I can just say that I do think, again, this is a trade-off.
1684
01:32:25.563 --> 01:32:27.484
<v SPEAKER_02>Again, this is something people have to decide.
1685
01:32:27.504 --> 01:32:32.168
<v SPEAKER_02>Because you can decide people should be more transparent.
1686
01:32:32.208 --> 01:32:34.650
<v SPEAKER_02>You can have a regulation that companies have to be more transparent.
1687
01:32:34.670 --> 01:32:37.023
<v SPEAKER_02>They have to publish a bunch of information.
1688
01:32:37.073 --> 01:32:40.478
<v SPEAKER_02>But then you have to accept the fact that anything that is published...
1689
01:32:40.528 --> 01:32:42.329
<v SPEAKER_02> Say China also finds out.
1690
01:32:42.589 --> 01:32:43.609
<v SPEAKER_00>Well, China's finding out anyways.
1691
01:32:43.629 --> 01:32:45.185
<v SPEAKER_00>At least we get to find out.
1692
01:32:45.309 --> 01:32:47.309
<v SPEAKER_02>They're probably finding out anyway.
1693
01:32:47.570 --> 01:32:51.231
<v SPEAKER_02>Right now, I think there's a lot of leakage because the security posture is so bad.
1694
01:32:51.251 --> 01:32:54.572
<v SPEAKER_02>But I think in a world where you also want to improve the security posture,
1695
01:32:54.592 --> 01:32:58.513
<v SPEAKER_02>I'm saying doing both of these interventions at once kind of defeats a lot
1696
01:32:58.553 --> 01:33:02.074
<v SPEAKER_02>of the point of improving security if you're also going to get the labs
1697
01:33:02.094 --> 01:33:03.995
<v SPEAKER_02>to publish all of this information anyway.
1698
01:33:04.035 --> 01:33:08.135
<v SPEAKER_02>Maybe you can defend the weights and the weights are not going to get stolen.
1699
01:33:08.185 --> 01:33:10.867
<v SPEAKER_02> Basically everything else, all the other innovations and so on.
1700
01:33:10.907 --> 01:33:15.541
<v SPEAKER_02>In this case, you would very easily just reconstruct everything from the public information.
1701
01:33:15.591 --> 01:33:17.994
<v SPEAKER_02>And I think that is a cost.
1702
01:33:18.114 --> 01:33:19.885
<v SPEAKER_02>It might be a cost worth paying,
1703
01:33:19.935 --> 01:33:22.748
<v SPEAKER_02>depending on how dire you think the situation is a bunch of ways.
1704
01:33:22.798 --> 01:33:24.631
<v SPEAKER_02>Yeah, I think it is worth paying.
1705
01:33:24.739 --> 01:33:27.902
<v SPEAKER_02>But then I think the proper way to do that, again,
1706
01:33:27.922 --> 01:33:32.506
<v SPEAKER_02>that's why I think Improving the quality of public discourse,
1707
01:33:32.566 --> 01:33:33.968
<v SPEAKER_02>not about these specific details,
1708
01:33:33.988 --> 01:33:37.814
<v SPEAKER_02>but just about the general fact of the transformativeness of the technology
1709
01:33:37.854 --> 01:33:40.378
<v SPEAKER_02>and the size of the impact it will have and stuff like this is so important
1710
01:33:40.398 --> 01:33:43.570
<v SPEAKER_02>because the public If you take this seriously,
1711
01:33:43.890 --> 01:33:47.121
<v SPEAKER_02>then this is a decision that could be made by the government
1712
01:33:47.171 --> 01:33:51.227
<v SPEAKER_02>and then it could become a regulation and we could just accept that, yes,
1713
01:33:51.353 --> 01:33:54.895
<v SPEAKER_02>we understand there's a cost here, but given the situation,
1714
01:33:54.915 --> 01:33:57.906
<v SPEAKER_02>we think you should pay this cost. For example, Amtropic doesn't believe that.
1715
01:33:57.956 --> 01:34:02.288
<v SPEAKER_02>Even though they also are aware of the stakes, they just don't think that cost is worth paying.
1716
01:34:02.338 --> 01:34:03.489
<v SPEAKER_02> I think that's what's going on.
1717
01:34:03.539 --> 01:34:06.900
<v SPEAKER_02>But I don't think they're necessarily being self-interested about that.
1718
01:34:06.920 --> 01:34:11.823
<v SPEAKER_02>I think they just have a real belief that this would be worse for the world
1719
01:34:12.423 --> 01:34:14.479
<v SPEAKER_02>if they made that information public.
1720
01:34:14.584 --> 01:34:17.405
<v SPEAKER_02>But Daniel doesn't share that belief, okay,
1721
01:34:17.425 --> 01:34:20.057
<v SPEAKER_02>but then if there's no public discourse about it,
1722
01:34:20.107 --> 01:34:25.245
<v SPEAKER_02>then It's impossible to get the companies to actually publish this stuff.
1723
01:34:25.925 --> 01:34:28.796
<v SPEAKER_02>There has to be some external thing that comes in and says, look,
1724
01:34:28.846 --> 01:34:31.257
<v SPEAKER_02>you guys can think that, but we are aware of the stakes here.
1725
01:34:31.307 --> 01:34:34.918
<v SPEAKER_02>We have decided that it is important for this information public.
1726
01:34:34.969 --> 01:34:39.110
<v SPEAKER_02>So unless that can happen, anyone can say, look, I think it's worse for,
1727
01:34:39.170 --> 01:34:42.722
<v SPEAKER_02>I think it's better for the world, and I'm just going to do what I think is best.
1728
01:34:42.772 --> 01:34:45.216
<v SPEAKER_02>And there's no regulation, there's no rules.
1729
01:34:45.973 --> 01:34:49.618
<v SPEAKER_02> So I think that's a very bad situation.
1730
01:34:50.420 --> 01:34:53.164
<v SPEAKER_02>Not because I necessarily think that the decision to keep it secret is
1731
01:34:53.184 --> 01:34:57.109
<v SPEAKER_02>a wrong decision, but I think the way the process that's outputting
1732
01:34:57.370 --> 01:34:58.932
<v SPEAKER_02>that outcome is bad.
1733
01:34:59.373 --> 01:35:00.845
<v SPEAKER_02>It should be based on, as I said,
1734
01:35:00.895 --> 01:35:03.819
<v SPEAKER_02>There should be a plan that we should understand what the stakes are.
1735
01:35:03.839 --> 01:35:06.503
<v SPEAKER_02>There should be rational sort of public deliberation about this topic
1736
01:35:06.543 --> 01:35:08.686
<v SPEAKER_02>and people should come to a conclusion that, yes, we want this or no,
1737
01:35:08.706 --> 01:35:09.758
<v SPEAKER_02>we don't want this.
1738
01:35:09.808 --> 01:35:11.060
<v SPEAKER_02>And that has not happened at all.
1739
01:35:11.110 --> 01:35:14.832
<v SPEAKER_02>So this is a unilateral decision that is being taken by some people
1740
01:35:15.056 --> 01:35:17.728
<v SPEAKER_02>who might be right, might be They have certain preferences,
1741
01:35:17.778 --> 01:35:21.579
<v SPEAKER_02>but even I think the government does not really play a large role
1742
01:35:21.599 --> 01:35:23.689
<v SPEAKER_02>in that because they don't understand the stakes.
1743
01:35:23.739 --> 01:35:25.400
<v SPEAKER_02>So the government might play a role in something like, oh,
1744
01:35:25.420 --> 01:35:28.831
<v SPEAKER_02>we are worried about Chinese cyber attacks and we want to have
1745
01:35:28.881 --> 01:35:29.941
<v SPEAKER_02>the capable cyber models.
1746
01:35:29.961 --> 01:35:31.531
<v SPEAKER_02>We don't want that to get leaked.
1747
01:35:31.581 --> 01:35:33.712
<v SPEAKER_02>Or they might worry about specific concrete risks.
1748
01:35:33.762 --> 01:35:37.972
<v SPEAKER_02>But if you don't appreciate the total transformative potential of technology,
1749
01:35:37.972 --> 01:35:40.834
<v SPEAKER_02>it's going to totally change the human condition, for example,
1750
01:35:40.884 --> 01:35:42.524
<v SPEAKER_02>then you're just unaware of the stakes.
1751
01:35:42.544 --> 01:35:45.044
<v SPEAKER_02>You're not going to make the right decisions.
1752
01:35:45.168 --> 01:35:46.762
<v SPEAKER_00> I think this is a very productive discussion.
1753
01:35:46.812 --> 01:35:50.259
<v SPEAKER_00>I feel it was very helpful to iron out what the cruxes were within the context
1754
01:35:50.279 --> 01:35:53.576
<v SPEAKER_00>of people who take the potential of this technology seriously.
1755
01:35:53.626 --> 01:35:55.691
<v SPEAKER_01>Yeah. Yeah. Cool. Thanks, guys.
1756
01:35:55.911 --> 01:35:56.911
<v SPEAKER_01>Thank you.
