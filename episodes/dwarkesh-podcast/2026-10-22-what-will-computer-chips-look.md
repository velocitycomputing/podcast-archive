---
record_id: "podcast:3f14e485-c5c1-4e29-836f-f078145d8194"
episode_id: 3f14e485-c5c1-4e29-836f-f078145d8194
title: What will computer chips look like in 2045?
podcast_title: Dwarkesh Podcast
url: "https://pocketcasts.com/podcast/dwarkesh-podcast/6d554750-84ac-0138-ee2b-0acc26574db2/what-will-computer-chips-look-like-in-2045/3f14e485-c5c1-4e29-836f-f078145d8194"
audio_url: "https://pocketcasts.com/podcast/dwarkesh-podcast/6d554750-84ac-0138-ee2b-0acc26574db2/what-will-computer-chips-look-like-in-2045/3f14e485-c5c1-4e29-836f-f078145d8194"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-22
played_at: "2026-10-22T12:00:00Z"
play_count: 1
duration_seconds: 4080
source: pocketcasts-history-browser
played_label: October 22
history_order: 47
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: rss-podcast-transcript
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 9cfd9ee86e16584668a64a5c11f339e5b6201be4b82e6787efef86eb9f2e0700
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

Intel’s Chris Auth and the host toured Intel fabs and discussed how AI demand is stressing semiconductor supply, with one speaker saying demand is 40–50% above maximum capacity. The conversation traced Intel’s 14A node development—about three years underway, roughly 2,000 process steps, thousands of wafers per week, and yield improvement via inline metrology, end-of-line electrical test, failure analysis, and TEM cross-sections. It compared Intel’s 10nm delay—target 2016, manufacturing 2018, stock down more than 15%, TSMC up 13%—to lessons about limiting innovation to keep schedule, especially after EUV was not ready; TSMC used EUV in volume manufacturing in 2019 and 5nm in 2020, while Intel’s first EUV products arrived in 2023. It also explained transistor scaling from planar MOS in 1960 to FinFET—lab 1989, Intel production 2011—and gate-all-around—demo 1988, Samsung production 2022—and covered high-NA EUV, moving numerical aperture from 0.33 to 0.55 for about 1.7x smaller features, standard tools around $200 million, high-end tools about twice as expensive, backside power, and why Intel may adopt high-NA while TSMC may prefer double patterning.

Actionable takeaways are mainly research and decision-making leads rather than health advice: track whether Intel 14A hits schedule, yield, and cost targets; monitor ASML high-NA adoption, throughput, defect rates, and cost-per-wafer versus multi-patterning; watch TSMC’s economics and Intel’s backside-power architecture as the key differentiator; and follow maturity gates for 2D materials, CFET, and advanced interconnects. Useful follow-up questions are: what monthly yield gains and defect Pareto are being achieved on 14A; how many litho passes high-NA saves; whether backside power reduces pitch enough to justify high-NA; which customers are committed to 14A; and how tool lead times, materials, and atomic-layer deposition constrain future nodes. For investment or supply-chain decisions, weigh node delay risk, capex intensity, and the possibility that AI compute demand remains above capacity, making capacity, yield, and schedule reliability as important as raw transistor performance.

## Transcript

WEBVTT
1
00:00:00.311 --> 00:00:04.655
<v SPEAKER_01>There's never been as big a shock to the semiconductor industry as the current surge
2
00:00:04.675 --> 00:00:05.917
<v SPEAKER_01>in demand from AI.
3
00:00:06.217 --> 00:00:09.400
<v SPEAKER_02> AI is driving incredible computing demand.
4
00:00:09.740 --> 00:00:13.851
<v SPEAKER_02>Easily 40 to 50% above our maximum capacity, which I've never seen before.
5
00:00:13.912 --> 00:00:17.643
<v SPEAKER_01> Progress in AI has been driven by exponentially increasing compute.
6
00:00:17.693 --> 00:00:18.983
<v SPEAKER_01>To sustain that progress,
7
00:00:19.033 --> 00:00:22.564
<v SPEAKER_01>foundries like Intel will need to manufacture far more leading-edge compute,
8
00:00:22.614 --> 00:00:26.392
<v SPEAKER_01>both by producing more chips and by improving what each chip can do.
9
00:00:26.515 --> 00:00:30.086
<v SPEAKER_01>But the production of these chips is bottlenecked by tools that Intel buys
10
00:00:30.136 --> 00:00:33.677
<v SPEAKER_01>from their suppliers, most famously, ASML's EUV machines.
11
00:00:33.897 --> 00:00:35.947
<v SPEAKER_03>If they don't have the equipment, they can't make the chips here.
12
00:00:35.997 --> 00:00:40.128
<v SPEAKER_01> I spent two days touring Intel's fabs to prepare for these interviews with its leadership.
13
00:00:40.178 --> 00:00:44.430
<v SPEAKER_01>I wanted to understand what it takes to manufacture the world's most advanced chips
14
00:00:44.480 --> 00:00:46.980
<v SPEAKER_01>and how hardware is shaping the future of AI.
15
00:00:47.420 --> 00:00:48.851
<v SPEAKER_01>Okay, I'm joined by Chris Auth,
16
00:00:48.901 --> 00:00:53.352
<v SPEAKER_01>who leads development of all the processes that are currently under manufacturing.
17
00:00:53.402 --> 00:00:56.713
<v SPEAKER_01>The thing I want to understand in more concrete detail is how...
18
00:00:56.763 --> 00:00:59.596
<v SPEAKER_01> The development of a new process actually happens.
19
00:00:59.706 --> 00:01:03.484
<v SPEAKER_01>So if 14A is going to come out in three years or two years from now,
20
00:01:03.649 --> 00:01:05.705
<v SPEAKER_01>what is happening from now till then?
21
00:01:06.211 --> 00:01:08.492
<v SPEAKER_01>And I want you to walk me through as much detail as you can,
22
00:01:08.532 --> 00:01:11.815
<v SPEAKER_01>everything from the level of how is the yield improving?
23
00:01:11.835 --> 00:01:13.246
<v SPEAKER_01>What kind of telemetry do you guys look at?
24
00:01:13.296 --> 00:01:15.448
<v SPEAKER_01>What kind of experiments do you guys run?
25
00:01:15.498 --> 00:01:20.776
<v SPEAKER_01>I want to understand what is going to happen over the next two years as concretely as possible.
26
00:01:20.967 --> 00:01:22.356
<v SPEAKER_00>And if we talk about 14A,
27
00:01:22.888 --> 00:01:27.251
<v SPEAKER_00>14A has actually been in development for about three plus years at this stage.
28
00:01:28.271 --> 00:01:31.973
<v SPEAKER_00>And so quite a bit of free work has been done to get to this stage that it's at right now.
29
00:01:32.013 --> 00:01:35.295
<v SPEAKER_00>And right now we're getting very close to where we're finalizing the process.
30
00:01:35.335 --> 00:01:38.707
<v SPEAKER_00>We're finalizing the tool sets that it will be manufactured on.
31
00:01:38.757 --> 00:01:42.389
<v SPEAKER_00>And we're working on kind of the fine tuning of each of the process steps.
32
00:01:42.439 --> 00:01:45.995
<v SPEAKER_00>There's about 2,000 steps in the factory that you have to go do.
33
00:01:46.341 --> 00:01:50.973
<v SPEAKER_00> And you need to do Really intricate work at each one of those to make sure it's fine-tuned.
34
00:01:51.013 --> 00:01:52.435
<v SPEAKER_00>It can go into manufacturing.
35
00:01:52.455 --> 00:01:55.860
<v SPEAKER_00>It can run thousands of wafers a week on this process,
36
00:01:55.900 --> 00:01:58.113
<v SPEAKER_00>and it can be repeatable every single time.
37
00:01:58.163 --> 00:02:00.397
<v SPEAKER_01>Right now, you might have a certain yield.
38
00:02:00.447 --> 00:02:05.173
<v SPEAKER_01> Walk me through how that increases month over So there's a line running at 14A.
39
00:02:05.614 --> 00:02:09.119
<v SPEAKER_01>What happens from now until next month that will result in the yield changing?
40
00:02:09.139 --> 00:02:10.952
<v SPEAKER_01>How do you identify where the defects are?
41
00:02:11.002 --> 00:02:12.384
<v SPEAKER_00>How do you fix that?
42
00:02:12.404 --> 00:02:15.869
<v SPEAKER_00>So there's a constant process that we go through in identifying defects.
43
00:02:15.889 --> 00:02:18.763
<v SPEAKER_00> And there's kind of two main ways that we'll We'll identify defects.
44
00:02:18.813 --> 00:02:21.077
<v SPEAKER_00>One is we have inline metrology.
45
00:02:21.297 --> 00:02:23.520
<v SPEAKER_00>So we have tools that will look at the wafers and say,
46
00:02:23.560 --> 00:02:26.415
<v SPEAKER_00>ah, there's a defect there, there's a defect there, there's a defect there.
47
00:02:26.465 --> 00:02:32.353
<v SPEAKER_00>And then also at end of line, either electrical test or we sort and see where the fails are.
48
00:02:32.834 --> 00:02:36.676
<v SPEAKER_00> Identify failures, and then we will get analysis on those failures.
49
00:02:36.716 --> 00:02:37.946
<v SPEAKER_00>We'll cross-section it.
50
00:02:37.996 --> 00:02:42.378
<v SPEAKER_00>You were in the TEM lab yesterday, and you saw how you can get cross-sections.
51
00:02:42.398 --> 00:02:43.739
<v SPEAKER_00>You'll get a cross-section of a defect,
52
00:02:43.779 --> 00:02:44.399
<v SPEAKER_00>and from that,
53
00:02:44.439 --> 00:02:45.869
<v SPEAKER_00>you'll be able to say, oh,
54
00:02:45.919 --> 00:02:47.520
<v SPEAKER_00>that defect is between these layers,
55
00:02:47.540 --> 00:02:50.311
<v SPEAKER_00>so it must have come from this section of the flow.
56
00:02:50.361 --> 00:02:54.528
<v SPEAKER_00>Oh, we have inline metrology in that section, which has identified defects.
57
00:02:54.583 --> 00:02:56.874
<v SPEAKER_00>Those are the defects we need to go after.
58
00:02:56.924 --> 00:03:01.813
<v SPEAKER_00>I think what we've learned is that you don't want to do too much innovation in one node.
59
00:03:01.987 --> 00:03:05.699
<v SPEAKER_00> Because the more innovation that you did, the more complex it becomes.
60
00:03:05.749 --> 00:03:09.561
<v SPEAKER_00>And while you'll be able to get that to work, you need to hit a certain schedule.
61
00:03:09.611 --> 00:03:12.382
<v SPEAKER_00>And that's the schedule that your customer ultimately wants.
62
00:03:12.432 --> 00:03:14.293
<v SPEAKER_00>So having that predictable schedule is a key piece.
63
00:03:14.313 --> 00:03:18.625
<v SPEAKER_00>So you've got to figure out how much innovation you can put in in order to meet
64
00:03:18.675 --> 00:03:22.064
<v SPEAKER_00>the customer's requirements in the timeline that they needed.
65
00:03:22.117 --> 00:03:26.409
<v SPEAKER_01>Intel learned how costly that tradeoff can be with delays to its 10 nanometer node,
66
00:03:26.459 --> 00:03:28.848
<v SPEAKER_01>whose original target launch date was 2016,
67
00:03:28.921 --> 00:03:31.588
<v SPEAKER_01>but which didn't begin manufacturing until 2018.
68
00:03:31.717 --> 00:03:31.987
<v SPEAKER_03>You know,
69
00:03:32.037 --> 00:03:34.759
<v SPEAKER_03>usually Intel has been the keeper of Moore's Law,
70
00:03:34.978 --> 00:03:37.759
<v SPEAKER_03>a new cadence of manufacturing every two years.
71
00:03:38.140 --> 00:03:41.211
<v SPEAKER_03>But their last set of products slipped almost four years.
72
00:03:41.261 --> 00:03:47.403
<v SPEAKER_02>Intel today having its worst day in four months, the stock now down more than 15%.
73
00:03:47.723 --> 00:03:54.126
<v SPEAKER_02>I also want to point out Taiwan Semiconductor up 13% off of Intel's bad news.
74
00:03:54.206 --> 00:03:59.428
<v SPEAKER_01>Walk me through what lessons you think Intel has learned from 10 nanometer.
75
00:03:59.668 --> 00:04:03.873
<v SPEAKER_00> 10android was a good example of where we had very aggressive targets.
76
00:04:04.073 --> 00:04:06.936
<v SPEAKER_00>We were doing what was called hyperscaling at the time,
77
00:04:06.976 --> 00:04:10.570
<v SPEAKER_00>so we were scaling much faster than what had been historically done.
78
00:04:10.620 --> 00:04:11.731
<v SPEAKER_00>In order to do that,
79
00:04:12.021 --> 00:04:17.547
<v SPEAKER_00>we came up with all sorts of innovative ideas and how we could achieve that
80
00:04:18.749 --> 00:04:22.171
<v SPEAKER_00>without New tools because the tools weren't ready.
81
00:04:22.711 --> 00:04:26.473
<v SPEAKER_00>And so that put a lot of burden on the process and a lot of burden on the engineers
82
00:04:26.513 --> 00:04:27.403
<v SPEAKER_00>in order to do that.
83
00:04:27.453 --> 00:04:30.455
<v SPEAKER_00>Now, at the end of the day, 10 engineers are great technology.
84
00:04:30.475 --> 00:04:31.415
<v SPEAKER_00>There's world-class yield.
85
00:04:31.435 --> 00:04:33.066
<v SPEAKER_00>There's world-class performance.
86
00:04:33.116 --> 00:04:34.505
<v SPEAKER_00>There's world-class cost.
87
00:04:34.597 --> 00:04:38.048
<v SPEAKER_00>But it took us longer to do that than what we would have liked.
88
00:04:38.098 --> 00:04:42.380
<v SPEAKER_00>And so we've kind of tried to take that learning into future technology nodes
89
00:04:42.420 --> 00:04:42.801
<v SPEAKER_00>and say, hey,
90
00:04:42.821 --> 00:04:45.542
<v SPEAKER_00>we need to limit the amount of innovation we put in there to make sure
91
00:04:45.562 --> 00:04:46.712
<v SPEAKER_00>that we keep it on schedule.
92
00:04:46.762 --> 00:04:48.595
<v SPEAKER_01>What do you think was the main...
93
00:04:49.195 --> 00:04:52.037
<v SPEAKER_01> EUV was probably the big
94
00:04:52.057 --> 00:04:53.678
<v SPEAKER_00> thing.
95
00:04:53.798 --> 00:04:58.820
<v SPEAKER_00>When we started to define 10 nanometer, what the conclusion was, EUV was not ready.
96
00:04:59.600 --> 00:05:02.922
<v SPEAKER_01>EUV is extreme ultraviolet lithography.
97
00:05:03.242 --> 00:05:07.164
<v SPEAKER_01>It prints chip patterns with light at a wavelength of 13.5 nanometers,
98
00:05:07.484 --> 00:05:11.286
<v SPEAKER_01>about 14 times shorter than that emitted by previous tools
99
00:05:11.626 --> 00:05:13.348
<v SPEAKER_01>that chip makers had relied on.
100
00:05:13.506 --> 00:05:17.920
<v SPEAKER_01> The shorter the wavelength, the finer the features that a single exposure can print.
101
00:05:17.970 --> 00:05:21.692
<v SPEAKER_01>But Intel decided this technology wasn't going to be ready in time.
102
00:05:21.793 --> 00:05:24.495
<v SPEAKER_01>TSMC transitioned to EUV much sooner.
103
00:05:25.055 --> 00:05:31.461
<v SPEAKER_01>It put EUV into volume manufacturing in 2019 and ramped it up further on its 5nm node in 2020.
104
00:05:32.383 --> 00:05:36.044
<v SPEAKER_01>Intel's first EUV process did not reach products until 2023,
105
00:05:36.545 --> 00:05:40.588
<v SPEAKER_01>so TSMC had about four more years of experience with these machines.
106
00:05:41.590 --> 00:05:46.838
<v SPEAKER_01>So yesterday we were at the research lab and we're getting a preview of 2D materials
107
00:05:46.878 --> 00:05:49.902
<v SPEAKER_01>and CFET and erythenium interconnects.
108
00:05:50.563 --> 00:05:55.521
<v SPEAKER_01>And I'm curious about how you decide whether that technology is mature enough for the next node.
109
00:05:55.571 --> 00:05:58.634
<v SPEAKER_00>One thing that did also And what's also come out of 10 N is we started to define
110
00:05:58.674 --> 00:06:00.118
<v SPEAKER_00>a set of maturity metrics.
111
00:06:00.415 --> 00:06:03.437
<v SPEAKER_00>And so we use those maturity metrics in a process,
112
00:06:03.678 --> 00:06:04.618
<v SPEAKER_00>what you call phase gate,
113
00:06:04.638 --> 00:06:07.911
<v SPEAKER_00>where we would say to go from pathfinding into development,
114
00:06:07.961 --> 00:06:09.883
<v SPEAKER_00>these are the criteria that we need to go hit.
115
00:06:09.903 --> 00:06:13.215
<v SPEAKER_00>And there's yield criteria, defect criteria, performance criteria.
116
00:06:13.265 --> 00:06:16.548
<v SPEAKER_00>And we need to hit those in order to move to the next set of the flow.
117
00:06:16.568 --> 00:06:19.380
<v SPEAKER_00>And if there's something that doesn't make that, then it misses that.
118
00:06:19.430 --> 00:06:23.763
<v SPEAKER_00>And it goes on to the next technology and we focus on the items that are ready
119
00:06:23.875 --> 00:06:28.191
<v SPEAKER_00>and we can run and put into a process because one of the key things is staying
120
00:06:28.241 --> 00:06:28.891
<v SPEAKER_00>on schedule.
121
00:06:28.941 --> 00:06:33.637
<v SPEAKER_01>Staying on schedule is hard partly because new transistor designs take decades to mature.
122
00:06:33.687 --> 00:06:38.409
<v SPEAKER_01>Modern trip transistors evolved from the planar MOS transistor, demonstrated in 1960.
123
00:06:39.153 --> 00:06:44.153
<v SPEAKER_01> The history of transistors since has been the progression from two dimensions into three.
124
00:06:44.254 --> 00:06:46.585
<v SPEAKER_01>Each development that Chris goes on to describe,
125
00:06:46.635 --> 00:06:50.079
<v SPEAKER_01>from FinFET to gate all around, is a step in that progression.
126
00:06:50.456 --> 00:06:55.512
<v SPEAKER_01>So it'll help to first look at a basic transistor and how its parts have changed over time.
127
00:06:55.597 --> 00:06:57.541
<v SPEAKER_01>A transistor is basically a switch.
128
00:06:58.058 --> 00:06:59.169
<v SPEAKER_01>When it's turned on,
129
00:06:59.238 --> 00:07:01.859
<v SPEAKER_01>it allows current to flow between its two ends,
130
00:07:02.279 --> 00:07:04.612
<v SPEAKER_01>which are called the source and the drain.
131
00:07:05.423 --> 00:07:10.490
<v SPEAKER_01> A piece called a gate sits on top of the silicon between the source and the drain.
132
00:07:11.291 --> 00:07:15.376
<v SPEAKER_01>Applying a positive voltage to the gate turns the switch on because
133
00:07:15.416 --> 00:07:20.043
<v SPEAKER_01>the positive voltage pulls negatively charged electrons in the silicon beneath
134
00:07:20.123 --> 00:07:24.284
<v SPEAKER_01>The electrons collect just beneath that insulation and form a thin conducting path
135
00:07:24.304 --> 00:07:25.225
<v SPEAKER_01>from the source to the drain.
136
00:07:25.265 --> 00:07:26.925
<v SPEAKER_01>This is called the channel.
137
00:07:35.949 --> 00:07:37.005
<v SPEAKER_01>Remove the voltage,
138
00:07:37.110 --> 00:07:41.367
<v SPEAKER_01>and the electrons disperse, the channel disappears, and the switch turns off.
139
00:07:41.417 --> 00:07:42.639
<v SPEAKER_01>As transistors shrank,
140
00:07:42.759 --> 00:07:46.865
<v SPEAKER_01>the source and the drain got so close together that current could flow through
141
00:07:46.905 --> 00:07:50.016
<v SPEAKER_01>the channel even when the switch was supposed to be off.
142
00:07:51.251 --> 00:07:58.251
<v SPEAKER_01> The fix was to give the gate a tighter grip on the channel by touching it from more sides.
143
00:08:00.401 --> 00:08:04.916
<v SPEAKER_01>In the original planar transistor, the gate only touches the channel from the top.
144
00:08:04.966 --> 00:08:09.355
<v SPEAKER_01>The FinFET transistor squeezes the channel into a thin vertical fin of silicon.
145
00:08:09.632 --> 00:08:13.958
<v SPEAKER_01> The gate drapes over the fin, so it controls the channel from three sides.
146
00:08:14.559 --> 00:08:18.024
<v SPEAKER_01>The next progression from there was to cover not only the top and the sides of
147
00:08:18.044 --> 00:08:19.837
<v SPEAKER_01>the channel, but also the bottom.
148
00:08:19.887 --> 00:08:24.283
<v SPEAKER_01>This technology is called Gate All Around, and it slices the channel into thin ribbons.
149
00:08:24.333 --> 00:08:27.365
<v SPEAKER_01> Each of which gets completely wrapped around by the gate.
150
00:08:27.415 --> 00:08:31.749
<v SPEAKER_01>But getting gate all around to work required new materials and new manufacturing steps.
151
00:08:31.799 --> 00:08:33.730
<v SPEAKER_01>To build these floating ribbons of silicon,
152
00:08:33.780 --> 00:08:37.143
<v SPEAKER_01>you first sandwich them between alternating layers of
153
00:08:37.183 --> 00:08:39.016
<v SPEAKER_01>a temporary placeholder material,
154
00:08:39.144 --> 00:08:42.255
<v SPEAKER_01>which holds the space where the gate will eventually go.
155
00:08:42.747 --> 00:08:46.169
<v SPEAKER_01>We use a placeholder because the materials in the real gate wouldn't survive
156
00:08:46.209 --> 00:08:47.920
<v SPEAKER_01>the processing that comes after,
157
00:08:47.970 --> 00:08:51.470
<v SPEAKER_01>which involves baking the wafer at around 1000 degrees Celsius.
158
00:08:52.112 --> 00:08:53.623
<v SPEAKER_01>Once these hot steps are done,
159
00:08:53.673 --> 00:08:57.451
<v SPEAKER_01>chip makers etch away the placeholder, leaving the ribbon suspended.
160
00:08:57.735 --> 00:08:58.735
<v SPEAKER_01> FinFET was
161
00:09:12.717 --> 00:09:17.660
<v SPEAKER_01> It was demonstrated in a lab in 1989 and reached volume production at Intel in 2011.
162
00:09:18.321 --> 00:09:22.763
<v SPEAKER_01>A gate all around transistor had been demonstrated a year earlier in 1988,
163
00:09:23.244 --> 00:09:27.046
<v SPEAKER_01>but Samsung didn't begin producing gate all around chips until 2022.
164
00:09:27.546 --> 00:09:28.546
<v SPEAKER_01>So these ideas,
165
00:09:28.667 --> 00:09:30.167
<v SPEAKER_01>FinFET and gate all around,
166
00:09:30.228 --> 00:09:34.672
<v SPEAKER_01>were developed around the same time, but they reached production a decade apart.
167
00:09:34.891 --> 00:09:39.912
<v SPEAKER_01>I wanted to ask Chris why it took so long to get to this current gate all around technology.
168
00:09:39.962 --> 00:09:42.914
<v SPEAKER_01> Maybe you can walk me through then the process of getting into high volume manufacturing.
169
00:09:42.964 --> 00:09:44.656
<v SPEAKER_01>I want to understand concretely,
170
00:09:44.706 --> 00:09:45.846
<v SPEAKER_01>once you have an idea that, hey,
171
00:09:45.866 --> 00:09:48.028
<v SPEAKER_01>we're going to make the channel smaller,
172
00:09:48.048 --> 00:09:49.548
<v SPEAKER_01>we're going to surround it,
173
00:09:49.909 --> 00:09:54.673
<v SPEAKER_01>all the other problems of material science and figuring out how to not destroy
174
00:09:55.079 --> 00:09:57.495
<v SPEAKER_01>the gate, how do they actually get figured out?
175
00:09:57.535 --> 00:09:58.786
<v SPEAKER_01>Why does it take so long?
176
00:09:58.836 --> 00:10:01.187
<v SPEAKER_00>Gate all around is a good example because back in the 90s,
177
00:10:01.237 --> 00:10:02.088
<v SPEAKER_00>we knew of this idea,
178
00:10:02.138 --> 00:10:05.190
<v SPEAKER_00>but we knew there was going to be these problems on how you put this
179
00:10:05.240 --> 00:10:07.061
<v SPEAKER_00>into high volume manufacturing.
180
00:10:07.321 --> 00:10:08.141
<v SPEAKER_00>And at the same time,
181
00:10:08.161 --> 00:10:11.023
<v SPEAKER_00>there's other things like high K metal gate,
182
00:10:11.523 --> 00:10:15.205
<v SPEAKER_00>there's strained silicon, there's FinFETs that are out there.
183
00:10:15.706 --> 00:10:18.757
<v SPEAKER_00>And so it's kind of like, when's the right time to go and tackle those?
184
00:10:18.807 --> 00:10:19.807
<v SPEAKER_00>Yeah.
185
00:10:20.170 --> 00:10:22.301
<v SPEAKER_00> You don't want to tackle something before you have to.
186
00:10:22.351 --> 00:10:26.502
<v SPEAKER_00>And so if you have these other things that can drive performance, you would go and do that.
187
00:10:26.552 --> 00:10:28.273
<v SPEAKER_00>We went through this path where we did this.
188
00:10:28.293 --> 00:10:29.453
<v SPEAKER_00>We did strain silicon,
189
00:10:29.473 --> 00:10:30.574
<v SPEAKER_00>high K metal gate,
190
00:10:30.694 --> 00:10:34.525
<v SPEAKER_00>we did FinFETs, and then it became, well, we need to do things further.
191
00:10:34.575 --> 00:10:35.265
<v SPEAKER_00>How do we get there?
192
00:10:35.315 --> 00:10:38.836
<v SPEAKER_00>Well, gate all around is really the ultimate transistor out there.
193
00:10:38.856 --> 00:10:42.840
<v SPEAKER_00> Maybe it's time to go and Start tackling some of those issues that you have.
194
00:10:42.880 --> 00:10:43.882
<v SPEAKER_00>And you're right.
195
00:10:43.922 --> 00:10:47.777
<v SPEAKER_00>Now you have to look at how you put Hayek and Metal Gate in with Gate All Round.
196
00:10:47.827 --> 00:10:49.620
<v SPEAKER_00>So it's that innovation that takes time.
197
00:10:49.670 --> 00:10:51.913
<v SPEAKER_00>Sometimes it's you need new materials.
198
00:10:52.213 --> 00:10:55.498
<v SPEAKER_00>Sometimes it's you need different tools.
199
00:10:55.658 --> 00:10:59.729
<v SPEAKER_00> You need a tool in order to be able to do some of the things that you need to go do.
200
00:10:59.779 --> 00:11:01.680
<v SPEAKER_00>And that requires invention from the tool vendors.
201
00:11:01.700 --> 00:11:02.870
<v SPEAKER_00>You have to go to the tool vendor and say, hey,
202
00:11:02.920 --> 00:11:04.461
<v SPEAKER_00>I need a tool that can do X,
203
00:11:04.481 --> 00:11:09.502
<v SPEAKER_00>Y, Z. I need a gas that can deposit this particular material that goes into that.
204
00:11:09.602 --> 00:11:13.303
<v SPEAKER_00>I need a heating chuck that has this characteristic to it.
205
00:11:14.184 --> 00:11:15.684
<v SPEAKER_00>All those things take time.
206
00:11:16.424 --> 00:11:19.565
<v SPEAKER_00>And some of it's iterative, where you have to run a gate all around transition.
207
00:11:19.585 --> 00:11:21.436
<v SPEAKER_00>You say, oh, well, that didn't work.
208
00:11:21.486 --> 00:11:24.375
<v SPEAKER_00>Let me figure out what was wrong with my hypothesis.
209
00:11:25.525 --> 00:11:28.186
<v SPEAKER_00> Try it again with some different structure.
210
00:11:28.426 --> 00:11:33.427
<v SPEAKER_01>How has the nature of R&D changed from the era
211
00:11:33.767 --> 00:11:38.287
<v SPEAKER_01>of just making planar transistors smaller and smaller and just getting the benefits
212
00:11:38.307 --> 00:11:40.863
<v SPEAKER_01>of Denard scaling to the world we're in today?
213
00:11:41.028 --> 00:11:42.968
<v SPEAKER_01>Is it just a totally different kind of R&D process
214
00:11:42.988 --> 00:11:45.499
<v SPEAKER_01>where previously you were just like, let's make things smaller, smaller, smaller.
215
00:11:45.549 --> 00:11:49.340
<v SPEAKER_01>Now you look at all these other facets of performance at the same time and
216
00:11:49.390 --> 00:11:51.946
<v SPEAKER_01>the improvements in size don't come as easily.
217
00:11:52.379 --> 00:11:55.512
<v SPEAKER_01> Walk me through whether there was some crucial change in the R&D process at that point.
218
00:11:55.562 --> 00:11:59.545
<v SPEAKER_00>If you look at the 80s and 90s, yes, it was driven really by Denard scaling, lithography.
219
00:11:59.565 --> 00:12:01.017
<v SPEAKER_00>We just make things smaller,
220
00:12:01.067 --> 00:12:05.751
<v SPEAKER_00>transistors got faster, they got more reliable, and it was very predictable cadence.
221
00:12:06.231 --> 00:12:10.405
<v SPEAKER_00>When we started to hit 2000s, what we saw was that's not good enough anymore.
222
00:12:10.455 --> 00:12:11.586
<v SPEAKER_00>We need to do something different.
223
00:12:11.636 --> 00:12:14.518
<v SPEAKER_00>And to me, it became this golden age of innovation.
224
00:12:14.759 --> 00:12:17.926
<v SPEAKER_00>For each technology node, how are you going to provide...
225
00:12:18.017 --> 00:12:18.617
<v SPEAKER_00> More scaling.
226
00:12:18.637 --> 00:12:20.648
<v SPEAKER_00>How are you going to provide more performance?
227
00:12:20.698 --> 00:12:23.029
<v SPEAKER_00>And so it drove things like strained silicon.
228
00:12:23.079 --> 00:12:24.860
<v SPEAKER_00>It drove high-K metal gates.
229
00:12:24.920 --> 00:12:25.871
<v SPEAKER_00>It drove FinFETs.
230
00:12:25.921 --> 00:12:26.991
<v SPEAKER_00>It got gate all around.
231
00:12:27.041 --> 00:12:28.374
<v SPEAKER_00>It drove backside power.
232
00:12:29.042 --> 00:12:32.084
<v SPEAKER_00>These are things that were in the 80s and 90s.
233
00:12:32.104 --> 00:12:32.844
<v SPEAKER_00>You would be like, oh, no,
234
00:12:32.864 --> 00:12:35.045
<v SPEAKER_00>we're not touching any of that because we just continue to have
235
00:12:35.065 --> 00:12:35.865
<v SPEAKER_00>the same process flow.
236
00:12:35.885 --> 00:12:37.941
<v SPEAKER_00>We just scale it, scale it, scale it.
237
00:12:38.126 --> 00:12:42.889
<v SPEAKER_00>But that's really for somebody like me who's a transistor junkie.
238
00:12:43.009 --> 00:12:45.530
<v SPEAKER_00>It's awesome because now the playbook's open.
239
00:12:46.050 --> 00:12:47.771
<v SPEAKER_00> You can do all sorts of things out there.
240
00:12:47.811 --> 00:12:49.461
<v SPEAKER_00>You can bring in new materials.
241
00:12:49.511 --> 00:12:52.573
<v SPEAKER_00>I mean, just look at the number of materials we used to use in the 90s versus materials.
242
00:12:52.593 --> 00:12:54.426
<v SPEAKER_00>Today, it's probably gone up 10x.
243
00:12:55.153 --> 00:12:56.864
<v SPEAKER_00>And there's a lot of innovation there.
244
00:12:56.914 --> 00:12:58.895
<v SPEAKER_00>There's atomic layer depositions, you know.
245
00:12:58.935 --> 00:13:02.046
<v SPEAKER_00>I mean, just you're controlling atom by atom this stuff.
246
00:13:02.136 --> 00:13:06.998
<v SPEAKER_00>So it's changed a lot how you approach the process as to before it was try
247
00:13:07.018 --> 00:13:08.838
<v SPEAKER_00>to not change anything to now.
248
00:13:08.878 --> 00:13:12.260
<v SPEAKER_00>It's like take the sledgehammer and start just tearing the thing up and come up
249
00:13:12.280 --> 00:13:13.281
<v SPEAKER_00>with some new idea.
250
00:13:13.331 --> 00:13:18.914
<v SPEAKER_01> For 14A, Intel is using a new kind of lithography machine, high NA EUV.
251
00:13:19.654 --> 00:13:25.237
<v SPEAKER_01>It uses the same extreme ultraviolet light as today's EUV machines, but changes the optics.
252
00:13:26.178 --> 00:13:27.879
<v SPEAKER_01>NA, or numerical aperture,
253
00:13:28.259 --> 00:13:33.121
<v SPEAKER_01>is a measure of how wide a cone of light the machine's mirrors can focus onto
254
00:13:33.141 --> 00:13:34.141
<v SPEAKER_01>the wafer.
255
00:13:34.422 --> 00:13:38.758
<v SPEAKER_01> The wider the cone you can focus, the smaller the spot that your light can carve.
256
00:13:38.808 --> 00:13:42.453
<v SPEAKER_01>Standard EUV machines have an NA of 0.33.
257
00:13:42.934 --> 00:13:45.037
<v SPEAKER_01>High NA widens it to 0.55.
258
00:13:45.277 --> 00:13:48.902
<v SPEAKER_01>So high NA can print features about 1.7 times smaller
259
00:13:51.105 --> 00:13:54.220
<v SPEAKER_01>When features are smaller than the lithography machine can print,
260
00:13:54.270 --> 00:13:57.603
<v SPEAKER_01>chip makers have to split the pattern across several passes,
261
00:13:58.056 --> 00:14:00.389
<v SPEAKER_01>each printing a different set of features.
262
00:14:05.888 --> 00:14:08.932
<v SPEAKER_01>These additional pass takes up valuable time on a machine
263
00:14:08.972 --> 00:14:13.528
<v SPEAKER_01>that costs around $200 million, and it introduces another opportunity for defects.
264
00:14:13.979 --> 00:14:16.368
<v SPEAKER_01>High-end machines cost about twice as much,
265
00:14:16.723 --> 00:14:19.377
<v SPEAKER_01>but they can reduce the number of passes that are needed.
266
00:14:19.427 --> 00:14:19.907
<v SPEAKER_01>The question,
267
00:14:19.927 --> 00:14:22.880
<v SPEAKER_01>which determines whether they justify their higher price,
268
00:14:22.930 --> 00:14:27.143
<v SPEAKER_01>is how much more time they save and how much they've reduced their risk of defects.
269
00:14:27.193 --> 00:14:30.656
<v SPEAKER_01>Now you guys are using high NA UV tools for 14A,
270
00:14:30.956 --> 00:14:35.012
<v SPEAKER_01>whereas TSMC has said that they don't make economical sense yet for them.
271
00:14:35.320 --> 00:14:41.525
<v SPEAKER_01>How do you decide whether the next litho tool is the one that is ready to adopt or not?
272
00:14:42.141 --> 00:14:46.603
<v SPEAKER_00>Yeah, and Hyenae is a good example of where because of the architecture
273
00:14:46.663 --> 00:14:50.484
<v SPEAKER_00>of our technology versus TSMCs,
274
00:14:50.544 --> 00:14:54.146
<v SPEAKER_00>we make different conclusions off of the same tool set.
275
00:14:54.406 --> 00:14:55.628
<v SPEAKER_00>We use backside power.
276
00:14:56.107 --> 00:15:00.888
<v SPEAKER_00>That means that you actually alleviate some of the pitch requirements you have on
277
00:15:00.908 --> 00:15:04.820
<v SPEAKER_00>the front side, and that allows you to print that directly with Hyenae.
278
00:15:04.870 --> 00:15:08.846
<v SPEAKER_00>TSMC has to run very tighter pitches because they don't have backside power,
279
00:15:08.896 --> 00:15:12.351
<v SPEAKER_00>and they can't do that with high NA, so they have to use double patterning EV.
280
00:15:12.401 --> 00:15:14.845
<v SPEAKER_00>So for them, it's not very helpful.
281
00:15:15.005 --> 00:15:16.505
<v SPEAKER_00>For us, it is very helpful.
282
00:15:16.587 --> 00:15:17.188
<v SPEAKER_00>Now at 14,
283
00:15:17.228 --> 00:15:18.620
<v SPEAKER_00>we've left it as an option,
284
00:15:18.670 --> 00:15:20.703
<v SPEAKER_00>and it's something that we'll have Chris is referring to
285
00:15:20.753 --> 00:15:21.815
<v SPEAKER_00>a feature called backside power.
286
00:15:21.835 --> 00:15:23.718
<v SPEAKER_00>A chip has two different kinds of wiring.
287
00:15:23.758 --> 00:15:26.412
<v SPEAKER_00> Power lines deliver electricity to the transistors,
288
00:15:26.462 --> 00:15:27.462
<v SPEAKER_01> and they need to
289
00:15:35.454 --> 00:15:38.285
<v SPEAKER_01> Signal lines let the transistors talk to each other.
290
00:15:38.335 --> 00:15:39.166
<v SPEAKER_01>They're much thinner,
291
00:15:39.216 --> 00:15:43.177
<v SPEAKER_01>but they need to be spaced apart so that the signal from one wire doesn't interfere
292
00:15:43.217 --> 00:15:44.508
<v SPEAKER_01>with the signal from another.
293
00:15:44.558 --> 00:15:45.528
<v SPEAKER_01>In the past,
294
00:15:45.578 --> 00:15:48.859
<v SPEAKER_01>all of these power lines and signal lines had to be crammed together on top of
295
00:15:48.879 --> 00:15:49.879
<v SPEAKER_01>the transistors.
296
00:15:50.240 --> 00:15:55.518
<v SPEAKER_01>Intel's newest process moves these power lines below the transistors, to the back of the wafer.
297
00:15:55.782 --> 00:16:00.053
<v SPEAKER_01>This frees up space on top, so the signal lines don't have to be packed as tightly.
298
00:16:00.103 --> 00:16:02.659
<v SPEAKER_01> This change makes high NA worth it for Intel.
299
00:16:02.924 --> 00:16:04.202
<v SPEAKER_01>Without backside power,
300
00:16:04.305 --> 00:16:08.016
<v SPEAKER_01>the wiring is so tight that it would require multiple passes to print,
301
00:16:08.066 --> 00:16:09.066
<v SPEAKER_01>even with high NA.
302
00:16:09.507 --> 00:16:12.648
<v SPEAKER_01>With backside power, a single high NA pass is enough.
303
00:16:13.308 --> 00:16:17.680
<v SPEAKER_01>Outside companies can now commission Intel to manufacture chips that they've designed.
304
00:16:17.730 --> 00:16:19.951
<v SPEAKER_01>They follow Intel's Process Design Kit,
305
00:16:20.251 --> 00:16:25.313
<v SPEAKER_01>or PDK, the menu of what a given process can build, and the rules for building it.
306
00:16:25.962 --> 00:16:28.894
<v SPEAKER_01>Do you need to lock that into your PDK right now for customers who are planning
307
00:16:28.944 --> 00:16:30.365
<v SPEAKER_01>on developing on 14A?
308
00:16:30.706 --> 00:16:32.427
<v SPEAKER_00>It's an option in the PDK today,
309
00:16:32.447 --> 00:16:36.670
<v SPEAKER_00>and we're handling it as a customer-by-customer discussion that we have as to
310
00:16:36.690 --> 00:16:38.581
<v SPEAKER_00>whether or not they want to go down that path or not.
311
00:16:38.631 --> 00:16:39.972
<v SPEAKER_01>So for 18A,
312
00:16:40.433 --> 00:16:44.296
<v SPEAKER_01>there was public reporting that there were delays or issues with the PDK such
313
00:16:44.316 --> 00:16:45.667
<v SPEAKER_01>that some instructions didn't work,
314
00:16:45.717 --> 00:16:49.289
<v SPEAKER_01>and it was difficult for people to use your foundry to build their chips.
315
00:16:49.339 --> 00:16:53.683
<v SPEAKER_01>Tell me about the process of Intel becoming a foundry and then having a PDK
316
00:16:53.723 --> 00:16:55.865
<v SPEAKER_01> that There's
317
00:16:58.536 --> 00:17:01.083
<v SPEAKER_00> definitely a learning curve to how you become a Foundry,
318
00:17:01.133 --> 00:17:04.288
<v SPEAKER_00>and that's something that our competitors have gone through as well.
319
00:17:04.338 --> 00:17:05.910
<v SPEAKER_00>PDK is a good example of that.
320
00:17:05.960 --> 00:17:09.495
<v SPEAKER_00>For decades, we've been an IDM, and we've gone to our product team.
321
00:17:09.545 --> 00:17:10.927
<v SPEAKER_00> And we've shown them our transistor data.
322
00:17:10.947 --> 00:17:12.169
<v SPEAKER_00>And we share that data back and forth.
323
00:17:12.189 --> 00:17:15.134
<v SPEAKER_00>And we haven't had a formal PDK type process.
324
00:17:15.534 --> 00:17:19.500
<v SPEAKER_00>So that's a new process that we've had to go implement on AT&A.
325
00:17:19.580 --> 00:17:22.104
<v SPEAKER_00>And AT&A started out not having a PDK.
326
00:17:22.404 --> 00:17:26.590
<v SPEAKER_00>And so there's definitely a lot The feedback we've got from the customers as
327
00:17:26.630 --> 00:17:30.315
<v SPEAKER_00>to what they expect for quality and maturity of the PDK,
328
00:17:30.396 --> 00:17:32.929
<v SPEAKER_00>what sort of information that they want to see in there.
329
00:17:32.979 --> 00:17:35.823
<v SPEAKER_00>And so we've tried to incorporate that into making sure that,
330
00:17:35.843 --> 00:17:39.065
<v SPEAKER_00>hey, we have a PDK that meets our customers' requirements.
331
00:17:39.308 --> 00:17:43.620
<v SPEAKER_00> That's where we've ended up, is that we're starting to get PDKs that have this.
332
00:17:43.670 --> 00:17:45.580
<v SPEAKER_00>And 14A will have that from the get-go.
333
00:17:45.630 --> 00:17:47.771
<v SPEAKER_00>It has very high-quality PDKs.
334
00:17:47.791 --> 00:17:52.653
<v SPEAKER_00>Again, there's maturity metrics for what is a PDK.5 versus a .9 versus a 1.0.
335
00:17:52.993 --> 00:17:57.935
<v SPEAKER_00>And we're constantly going through and taking customer feedback and incorporating
336
00:17:57.955 --> 00:17:59.788
<v SPEAKER_00>that into the quality of our PDK.
337
00:18:00.857 --> 00:18:04.357
<v SPEAKER_01> For most of its history, Intel's fabs made only Intel's chips.
338
00:18:04.898 --> 00:18:07.649
<v SPEAKER_01>That could be part of what allowed TSMC to gain an edge.
339
00:18:07.699 --> 00:18:11.060
<v SPEAKER_01>Serving many customers gave TSMC more wafers to learn from,
340
00:18:11.440 --> 00:18:14.829
<v SPEAKER_01>more revenue to reinvest, and more pressure to hit deadlines.
341
00:18:15.381 --> 00:18:15.741
<v SPEAKER_01>Basically,
342
00:18:15.781 --> 00:18:19.042
<v SPEAKER_01>all enterprise customers have a shared set of product requirements that you have
343
00:18:19.062 --> 00:18:22.053
<v SPEAKER_01>to meet if you want to even start talking about doing business with them.
344
00:18:22.103 --> 00:18:23.547
<v SPEAKER_01>These are things like SSO,
345
00:18:23.643 --> 00:18:26.894
<v SPEAKER_01>so employees can log into your app with their company accounts,
346
00:18:26.944 --> 00:18:27.944
<v SPEAKER_01>or directory sync,
347
00:18:28.064 --> 00:18:29.715
<v SPEAKER_01>so that whenever someone leaves,
348
00:18:29.765 --> 00:18:33.185
<v SPEAKER_01>their access WorkOS also has versions of these features that are purpose-built
349
00:18:33.205 --> 00:18:33.466
<v SPEAKER_01>for agents,
350
00:18:33.486 --> 00:18:34.126
<v SPEAKER_01>so they can log in,
351
00:18:34.146 --> 00:18:37.757
<v SPEAKER_01>grab the right permissions, and take actions within your product.
352
00:18:59.910 --> 00:19:03.363
<v SPEAKER_01>All of these features can be plugged in with just a few lines of code,
353
00:19:03.413 --> 00:19:06.125
<v SPEAKER_01>so you can add them and get started selling to enterprises.
354
00:19:06.175 --> 00:19:07.457
<v SPEAKER_01>OpenAI, Anthropic,
355
00:19:07.577 --> 00:19:08.688
<v SPEAKER_01>and Thinking Machines,
356
00:19:08.738 --> 00:19:11.127
<v SPEAKER_01>as well as more than 3,000 other companies,
357
00:19:11.600 --> 00:19:15.023
<v SPEAKER_01>all rely on WorkOS to meet their enterprise requirements.
358
00:19:15.503 --> 00:19:19.559
<v SPEAKER_01>If you want to join them, go to workos.com and tell them that I sent you.
359
00:19:20.128 --> 00:19:22.219
<v SPEAKER_01>If a butterfly flapped its wings in the 60s,
360
00:19:22.269 --> 00:19:25.310
<v SPEAKER_01>could you imagine a world where gator all around is not even
361
00:19:25.350 --> 00:19:26.210
<v SPEAKER_01>a word people have heard of,
362
00:19:26.230 --> 00:19:27.291
<v SPEAKER_01>an idea people are familiar with,
363
00:19:27.311 --> 00:19:30.282
<v SPEAKER_01>but people are thinking of an extremely different branch of the tech tree?
364
00:19:30.332 --> 00:19:32.873
<v SPEAKER_01>And how far down the tech tree do you think things could be totally different?
365
00:19:32.893 --> 00:19:35.163
<v SPEAKER_01>Could it be like we're not even using copper?
366
00:19:35.213 --> 00:19:39.315
<v SPEAKER_00>If you look at, say, transistors and interconnects, I think...
367
00:19:40.175 --> 00:19:41.397
<v SPEAKER_00>Where we've gotten to,
368
00:19:42.056 --> 00:19:44.638
<v SPEAKER_00>as far as the transistor and gate all around and it being
369
00:19:44.658 --> 00:19:48.220
<v SPEAKER_00>the ideal transistor structure that I have, I think was somewhat inevitable.
370
00:19:48.240 --> 00:19:51.272
<v SPEAKER_00>As I said, in the 90s, we were already talking about these type of things.
371
00:19:51.322 --> 00:19:54.044
<v SPEAKER_00>Backside power, that one's pretty out there.
372
00:19:54.524 --> 00:19:56.345
<v SPEAKER_00>I think even in the 90s,
373
00:19:56.385 --> 00:20:00.818
<v SPEAKER_00>the idea that you're going to strip off the entire silicon substrate and put lines
374
00:20:00.868 --> 00:20:06.011
<v SPEAKER_00>on the back side, that one is probably something that's a little bit out there.
375
00:20:06.851 --> 00:20:07.782
<v SPEAKER_00>Copper.
376
00:20:07.832 --> 00:20:08.192
<v SPEAKER_00>Of course,
377
00:20:08.212 --> 00:20:09.362
<v SPEAKER_00>copper wires are the best,
378
00:20:09.412 --> 00:20:14.093
<v SPEAKER_00>so I don't know how you would end up somewhere else besides copper.
379
00:20:14.233 --> 00:20:17.694
<v SPEAKER_00>I think for some of the very tightest pitches,
380
00:20:17.714 --> 00:20:20.064
<v SPEAKER_00>I think it's inevitable that you will replace copper.
381
00:20:20.114 --> 00:20:23.975
<v SPEAKER_00>And so that's a good example of where you will have another material that will come in there.
382
00:20:24.015 --> 00:20:27.306
<v SPEAKER_00>But for the larger lines, I think copper is about where it's at.
383
00:20:27.356 --> 00:20:31.197
<v SPEAKER_00>I think that once you start to do gate all-around transistors
384
00:20:31.517 --> 00:20:33.377
<v SPEAKER_00>and you do backside power,
385
00:20:33.877 --> 00:20:38.758
<v SPEAKER_00>now you start to enter a very different regime because now you see It's not,
386
00:20:39.339 --> 00:20:41.730
<v SPEAKER_00>hey, there's just some substrate and you stack everything on top.
387
00:20:41.780 --> 00:20:44.391
<v SPEAKER_00>Now you've got a transistor, which is floating in interconnect.
388
00:20:44.441 --> 00:20:45.241
<v SPEAKER_00>And you're like, okay, well,
389
00:20:45.261 --> 00:20:46.882
<v SPEAKER_00>why don't I have transistors,
390
00:20:46.922 --> 00:20:50.013
<v SPEAKER_00>interconnect, a little more transistors, more interconnect.
391
00:20:50.063 --> 00:20:55.145
<v SPEAKER_00>This whole 3D stacking that we now do with just discrete chips that we stack on top
392
00:20:55.165 --> 00:20:55.445
<v SPEAKER_00>of each other.
393
00:20:55.465 --> 00:20:59.354
<v SPEAKER_00>Now you're like, why can't I just build an entire structure like this?
394
00:20:59.407 --> 00:21:01.308
<v SPEAKER_00>You see it with memory.
395
00:21:02.100 --> 00:21:06.106
<v SPEAKER_00> NAND, DRAM, you know, they have some incredible 3D structures.
396
00:21:06.306 --> 00:21:07.178
<v SPEAKER_00>NAND already does it.
397
00:21:07.228 --> 00:21:11.464
<v SPEAKER_00>DRAM talks about it, but I think that DRAM inevitably is going to go there too.
398
00:21:11.514 --> 00:21:13.056
<v SPEAKER_00>So a lot of people say, oh no,
399
00:21:13.076 --> 00:21:16.021
<v SPEAKER_00>we're not going to do this because, hey, we can't do it in the next five years.
400
00:21:16.061 --> 00:21:18.614
<v SPEAKER_00> Well, come on, let's Let's put a larger timescale on this.
401
00:21:18.664 --> 00:21:21.288
<v SPEAKER_00>Let's put 10 years, 20 years in 2045.
402
00:21:21.348 --> 00:21:22.959
<v SPEAKER_00>Do you think you could do it?
403
00:21:23.151 --> 00:21:23.972
<v SPEAKER_00>And now you start to say,
404
00:21:24.012 --> 00:21:27.528
<v SPEAKER_00>oh yeah, I could see us having some pretty exotic structures at that point.
405
00:21:27.578 --> 00:21:31.967
<v SPEAKER_00>So we limit ourselves by what we see as possible in the next four years because
406
00:21:32.425 --> 00:21:36.601
<v SPEAKER_00>As I've always said, when people say, hey, how do you see technology scaling going?
407
00:21:36.651 --> 00:21:38.404
<v SPEAKER_00>Yeah, we have visibility about four years.
408
00:21:38.454 --> 00:21:40.146
<v SPEAKER_00>And then you get out to that four years and you go,
409
00:21:40.196 --> 00:21:43.110
<v SPEAKER_00>yeah, I think there's something we can do another four years out of that.
410
00:21:43.160 --> 00:21:45.223
<v SPEAKER_00>And then you get to that four years and you're like, yeah, I think you can do something.
411
00:21:45.264 --> 00:21:46.886
<v SPEAKER_01>But if you start to talk about 10 years,
412
00:21:46.906 --> 00:21:51.973
<v SPEAKER_01>you Chris's idea of building upwards could start with the transistors themselves.
413
00:21:52.494 --> 00:21:56.820
<v SPEAKER_01>Chips use two types of transistors called n-type and p-type,
414
00:21:57.181 --> 00:22:00.055
<v SPEAKER_01>which work the same way, but with the charges reversed.
415
00:22:00.105 --> 00:22:05.811
<v SPEAKER_01> Nearly every circuit is built by pairing Today, chip makers build them side by side.
416
00:22:06.391 --> 00:22:11.058
<v SPEAKER_01>The next step is to stack them directly on top of each other in order to save space.
417
00:22:11.115 --> 00:22:14.948
<v SPEAKER_01>In principle, that fits twice as many transistors into the same area.
418
00:22:15.118 --> 00:22:19.722
<v SPEAKER_01>This design is called a CFET, short for Complementary Field Effect Transistor.
419
00:22:19.922 --> 00:22:24.106
<v SPEAKER_01>But every extra layer adds manufacturing steps and costs and also leads
420
00:22:24.166 --> 00:22:27.438
<v SPEAKER_01>to heat building up that doesn't have a clear way to escape.
421
00:22:27.488 --> 00:22:28.488
<v SPEAKER_01>Because...
422
00:22:28.669 --> 00:22:30.836
<v SPEAKER_01> Logic consumes more power than memory.
423
00:22:30.912 --> 00:22:34.958
<v SPEAKER_01>You can't do stacks of DRAM that make HBM or,
424
00:22:34.998 --> 00:22:38.609
<v SPEAKER_01>you know, 3D NAND as easily with logic because of the heat issue.
425
00:22:38.784 --> 00:22:41.338
<v SPEAKER_01>Is that the fundamental issue then over the long run?
426
00:22:41.388 --> 00:22:42.388
<v SPEAKER_01>Is how you...
427
00:22:43.952 --> 00:22:49.039
<v SPEAKER_00> So there's three things that you have when you try to say, hey, what limits compute?
428
00:22:49.620 --> 00:22:51.620
<v SPEAKER_00>It's how fast can you do the switch?
429
00:22:52.003 --> 00:22:53.725
<v SPEAKER_00>So the frequency of the device.
430
00:22:53.786 --> 00:22:56.560
<v SPEAKER_00>How much power does it take in order to do that switch?
431
00:22:56.610 --> 00:22:58.277
<v SPEAKER_00>So the power efficiency of it.
432
00:22:58.533 --> 00:23:02.299
<v SPEAKER_00> And the second one is, how do you dissipate the heat that was generated by doing that switch?
433
00:23:02.319 --> 00:23:04.251
<v SPEAKER_00>And that's the thermals piece to it.
434
00:23:04.301 --> 00:23:07.216
<v SPEAKER_00>And I think the thermals piece is, and these are not new problems.
435
00:23:07.266 --> 00:23:10.100
<v SPEAKER_00>You can go back 20 years and you can see articles on these three things.
436
00:23:10.150 --> 00:23:10.991
<v SPEAKER_00>And so the question is, yeah,
437
00:23:11.011 --> 00:23:11.602
<v SPEAKER_00>thermals,
438
00:23:11.652 --> 00:23:12.744
<v SPEAKER_00>how do you deal with that,
439
00:23:12.794 --> 00:23:16.294
<v SPEAKER_00>particularly When we start to talk about these 3D type devices,
440
00:23:16.539 --> 00:23:21.927
<v SPEAKER_00>I think that there is a need for that sort of system level analysis
441
00:23:22.007 --> 00:23:23.169
<v SPEAKER_00>and simulation tools.
442
00:23:23.209 --> 00:23:27.295
<v SPEAKER_00>I think we're at its infancy because we've just started to look at this.
443
00:23:29.217 --> 00:23:34.999
<v SPEAKER_01>The problems respond to work,
444
00:23:35.359 --> 00:23:38.950
<v SPEAKER_01>but engineering time is finite, and so are the wafers for experiments.
445
00:23:39.000 --> 00:23:42.841
<v SPEAKER_01>Deciding where they go across thousands of problems is itself one of
446
00:23:42.861 --> 00:23:45.083
<v SPEAKER_01>the hardest parts of bringing up a node.
447
00:23:45.462 --> 00:23:49.851
<v SPEAKER_01>I sat in on one of Intel's Hot Topics meetings, where those decisions get made.
448
00:23:50.109 --> 00:23:51.230
<v SPEAKER_01>Okay, I'm here with Kevin Fisher,
449
00:23:51.270 --> 00:23:54.292
<v SPEAKER_01>who was laying down the law this morning at the Hot Topics meeting
450
00:23:54.312 --> 00:23:58.645
<v SPEAKER_01>where you guys were discussing how you're improving 18A and 18AP technologies.
451
00:23:58.715 --> 00:24:00.936
<v SPEAKER_01>And people would come to you with these different experiments they were running,
452
00:24:00.956 --> 00:24:04.629
<v SPEAKER_01>different ideas they had for improving yield and for improving performance.
453
00:24:04.679 --> 00:24:10.163
<v SPEAKER_01>And then you and your integration engineers would tell them what data you needed,
454
00:24:10.203 --> 00:24:11.373
<v SPEAKER_01>tell them how they should proceed,
455
00:24:11.423 --> 00:24:13.145
<v SPEAKER_01>tell them how you think you can move things faster.
456
00:24:13.165 --> 00:24:16.665
<v SPEAKER_01>I want people to have a sense of the culture at these meetings.
457
00:24:17.172 --> 00:24:20.165
<v SPEAKER_01>And so one thing that I found striking is just that there's,
458
00:24:20.215 --> 00:24:22.708
<v SPEAKER_01>you know, this is bottlenecking your most advanced node.
459
00:24:22.758 --> 00:24:24.450
<v SPEAKER_01>You want products to happen fast.
460
00:24:24.500 --> 00:24:26.342
<v SPEAKER_01>And so you kind of lay down the hammer.
461
00:24:26.362 --> 00:24:27.543
<v SPEAKER_01>I would say...
462
00:24:28.350 --> 00:24:34.055
<v SPEAKER_02> The average engineer doesn't understand the stakes or the urgency
463
00:24:34.315 --> 00:24:39.198
<v SPEAKER_02>of how this is going to impact Intel's bottom line,
464
00:24:39.879 --> 00:24:41.990
<v SPEAKER_02>how it's going to impact our customer.
465
00:24:42.061 --> 00:24:45.343
<v SPEAKER_02>They just have no visibility to those issues, right?
466
00:24:45.403 --> 00:24:47.525
<v SPEAKER_02>So they will typically have...
467
00:24:49.843 --> 00:24:52.446
<v SPEAKER_02> A certain set of criteria that they want to go capture.
468
00:24:52.486 --> 00:24:57.193
<v SPEAKER_02>They'll hit boundaries of, you know, I asked for something and someone said no.
469
00:24:57.894 --> 00:25:00.538
<v SPEAKER_02>And, you know, I'm done.
470
00:25:00.598 --> 00:25:03.321
<v SPEAKER_02>I guess I can't have this thing that I asked for.
471
00:25:03.922 --> 00:25:07.284
<v SPEAKER_02>One thing you learn What I learned in this industry is that you will never have
472
00:25:07.324 --> 00:25:08.435
<v SPEAKER_02>a complete data set.
473
00:25:08.505 --> 00:25:11.316
<v SPEAKER_02>If you want to wait for a complete data set, you've waited too long.
474
00:25:11.366 --> 00:25:12.476
<v SPEAKER_02>It's already too late.
475
00:25:12.526 --> 00:25:14.447
<v SPEAKER_02>So a lot of what I end up doing
476
00:25:14.887 --> 00:25:19.589
<v SPEAKER_02>in those meetings is I decide how much risk we're going to take on
477
00:25:19.889 --> 00:25:22.833
<v SPEAKER_02>a certain decision or not take on a certain decision.
478
00:25:23.090 --> 00:25:25.871
<v SPEAKER_02>And you need to say, look, do we go now?
479
00:25:26.351 --> 00:25:27.822
<v SPEAKER_02>Do we start risking production?
480
00:25:27.872 --> 00:25:30.153
<v SPEAKER_02>Because you're risking the bottom line.
481
00:25:30.173 --> 00:25:31.013
<v SPEAKER_02>You're risking revenue.
482
00:25:31.033 --> 00:25:31.483
<v SPEAKER_02>Yeah.
483
00:25:31.533 --> 00:25:35.677
<v SPEAKER_02>I'm worried you're going to put me in the light of being an ogre because I'm putting
484
00:25:35.697 --> 00:25:37.559
<v SPEAKER_02>the hammer down on you.
485
00:25:37.939 --> 00:25:39.111
<v SPEAKER_02>That's a great reputation to have.
486
00:25:39.161 --> 00:25:40.922
<v SPEAKER_01>It's really conveying urgency.
487
00:25:41.122 --> 00:25:41.653
<v SPEAKER_01>Yes.
488
00:25:41.703 --> 00:25:42.703
<v SPEAKER_01>Every day counts.
489
00:25:42.764 --> 00:25:43.194
<v SPEAKER_01>Yeah.
490
00:25:43.244 --> 00:25:46.688
<v SPEAKER_01>Can you walk me through a particular issue that might come up?
491
00:25:46.828 --> 00:25:50.912
<v SPEAKER_01>Well, one of the examples you saw this morning, which is epi nodules.
492
00:25:51.452 --> 00:25:56.257
<v SPEAKER_01>Epi is short for epitaxy, which means growing new material on top of an existing one.
493
00:25:56.897 --> 00:26:01.879
<v SPEAKER_01> Chipmakers flow gases over a heated wafer, and the gases leave atoms on its surface.
494
00:26:02.519 --> 00:26:06.151
<v SPEAKER_01>The crystal structure of the material underneath acts as a template.
495
00:26:06.201 --> 00:26:11.368
<v SPEAKER_01>Each new atom lines up with the atoms below it, and the new layer continues the same crystal.
496
00:26:11.423 --> 00:26:14.645
<v SPEAKER_01>Chipmakers use epitaxy at several stages of making a chip.
497
00:26:15.084 --> 00:26:16.235
<v SPEAKER_01>In the step Kevin describes,
498
00:26:16.285 --> 00:26:19.947
<v SPEAKER_01>they use it to grow the source and the drain as small crystals on either side of
499
00:26:19.987 --> 00:26:20.417
<v SPEAKER_01>the gate.
500
00:26:20.467 --> 00:26:22.745
<v SPEAKER_01> So during the deposition of our epitaxy,
501
00:26:23.248 --> 00:26:27.150
<v SPEAKER_02> we get abnormal growth, like a tumor, right?
502
00:26:27.250 --> 00:26:28.651
<v SPEAKER_02>It's going super fast.
503
00:26:29.051 --> 00:26:32.603
<v SPEAKER_02>And that causes problems because one epi will short to the wrong epi
504
00:26:32.653 --> 00:26:35.474
<v SPEAKER_02>and you get transistors not working.
505
00:26:35.634 --> 00:26:37.065
<v SPEAKER_02> And then you've got to narrow it down
506
00:26:37.115 --> 00:26:38.893
<v SPEAKER_01> to how are you going to fix it?
507
00:26:39.203 --> 00:26:43.476
<v SPEAKER_01> For the past decade, Intel's chips have had this feature called Processor Trace.
508
00:26:43.526 --> 00:26:44.557
<v SPEAKER_01>When you turn it on,
509
00:26:44.607 --> 00:26:47.039
<v SPEAKER_01>it starts recording all the code your program runs,
510
00:26:47.089 --> 00:26:49.620
<v SPEAKER_01>and it captures enough detail that it can go back later
511
00:26:49.670 --> 00:26:52.059
<v SPEAKER_01>and reconstruct every single function call.
512
00:26:52.252 --> 00:26:55.925
<v SPEAKER_01>Most companies don't need that level of detail, but Jane Street does.
513
00:26:55.975 --> 00:26:59.527
<v SPEAKER_01>They need to investigate specific fleeting moments in their trading systems,
514
00:26:59.577 --> 00:27:02.289
<v SPEAKER_01>things like a delayed response to a network packet.
515
00:27:02.339 --> 00:27:06.172
<v SPEAKER_01> Those events tend to be too brief for most debugging tools to catch.
516
00:27:06.385 --> 00:27:09.460
<v SPEAKER_01>So when one of Jane Street's engineers noticed Processor Trace,
517
00:27:09.510 --> 00:27:11.082
<v SPEAKER_01>he started playing around with it.
518
00:27:11.132 --> 00:27:16.440
<v SPEAKER_01>And then he and a summer intern turned that exploration into a new tool called Magic Trace.
519
00:27:17.081 --> 00:27:21.438
<v SPEAKER_01>Gadgettrace leverages the output from processor trace to give Jane Street a history
520
00:27:21.488 --> 00:27:25.163
<v SPEAKER_01>of every function call leading up to a specific moment of interest.
521
00:27:25.213 --> 00:27:26.805
<v SPEAKER_01>This project was completely bottoms up.
522
00:27:26.855 --> 00:27:29.770
<v SPEAKER_01>It started just as something that one engineer thought would be valuable.
523
00:27:29.820 --> 00:27:34.234
<v SPEAKER_01> And now, traders and developers across Jane Jane Street use Magic Trace every single day.
524
00:27:34.284 --> 00:27:36.725
<v SPEAKER_01>If you want to work somewhere where you're trusted to pursue the ideas
525
00:27:36.745 --> 00:27:40.967
<v SPEAKER_01>that you think matter most, Jane Street is hiring researchers and engineers.
526
00:27:41.266 --> 00:27:45.028
<v SPEAKER_01>Go to janestreet.com slash Dwarkesh to learn more.
527
00:27:45.628 --> 00:27:49.610
<v SPEAKER_02> One of the pieces that you observed this morning was a special clean
528
00:27:49.830 --> 00:27:53.051
<v SPEAKER_02>that we were looking at, which would eliminate the nodule, right?
529
00:27:53.071 --> 00:27:56.102
<v SPEAKER_02>So the nodule would deposit and then we'd get rid of it.
530
00:27:56.152 --> 00:27:57.632
<v SPEAKER_02>Some of the other discussion was,
531
00:27:57.672 --> 00:28:01.033
<v SPEAKER_02>well, the source of the nodule, get rid of the source of the nodule, right?
532
00:28:01.073 --> 00:28:06.129
<v SPEAKER_01> So how do you decide what, there's some issue, how do you decide what the source of it is?
533
00:28:05.675 --> 00:28:07.875
<v SPEAKER_01>For the most part, we work highly parallel, right?
534
00:28:07.915 --> 00:28:09.356
<v SPEAKER_01>So how do you decide?
535
00:28:10.036 --> 00:28:12.747
<v SPEAKER_02>It's not always evident what the easiest way to fix the problem is.
536
00:28:12.797 --> 00:28:14.964
<v SPEAKER_02>So you work on all the potential fixes.
537
00:28:16.318 --> 00:28:18.651
<v SPEAKER_02>And sometimes it's not the one you expect.
538
00:28:19.079 --> 00:28:23.481
<v SPEAKER_02>Once we've identified it as a primary problem for the technology,
539
00:28:23.901 --> 00:28:26.883
<v SPEAKER_02>that's where this Hot Topics meeting gets involved.
540
00:28:26.923 --> 00:28:32.766
<v SPEAKER_02>And that's how we align the resources into those engineering teams so
541
00:28:32.826 --> 00:28:34.607
<v SPEAKER_02>that we can accelerate the work.
542
00:28:35.047 --> 00:28:38.769
<v SPEAKER_01>You said there's some fast strike process where wafers can move through faster
543
00:28:38.809 --> 00:28:40.409
<v SPEAKER_01>if they're bottlenecking some experiment.
544
00:28:40.429 --> 00:28:44.151
<v SPEAKER_01>So we have a tiered system of what we call hotboxes in the factory.
545
00:28:44.311 --> 00:28:47.432
<v SPEAKER_02>And every grade of hotbox goes a little bit faster.
546
00:28:47.552 --> 00:28:52.434
<v SPEAKER_02>And it's just how the factory prioritizes that particular lot,
547
00:28:52.494 --> 00:28:54.775
<v SPEAKER_02>that block of silicon that's running through the factory.
548
00:28:54.795 --> 00:28:57.877
<v SPEAKER_02>So our highest grade of hotbox, hotbox one.
549
00:28:59.277 --> 00:29:00.438
<v SPEAKER_02> Races through the factory.
550
00:29:00.478 --> 00:29:04.762
<v SPEAKER_02>It gets priority at every single tool, but it's a drag on the entire factory.
551
00:29:04.782 --> 00:29:06.744
<v SPEAKER_02>If you had a factory person in here,
552
00:29:06.784 --> 00:29:08.485
<v SPEAKER_02>they don't like using,
553
00:29:08.885 --> 00:29:13.976
<v SPEAKER_02>playing that card because you're ending up Using the tools inefficiently so
554
00:29:13.996 --> 00:29:15.916
<v SPEAKER_02>that you can go super, super fast.
555
00:29:15.976 --> 00:29:20.577
<v SPEAKER_02>Think of it as a highway and you set aside that one lane for the carpool, right?
556
00:29:20.917 --> 00:29:23.238
<v SPEAKER_02>Which everyone could use, but you're saying, okay, it's just a carpool.
557
00:29:23.258 --> 00:29:25.079
<v SPEAKER_02>That's our hotbox one, right?
558
00:29:25.539 --> 00:29:28.589
<v SPEAKER_02>Everyone clear out of that lane except for that one experiment.
559
00:29:28.639 --> 00:29:30.701
<v SPEAKER_02>And that one experiment races down the highway.
560
00:29:30.751 --> 00:29:33.824
<v SPEAKER_01> Kevin's job is deciding what goes on the production line now.
561
00:29:33.874 --> 00:29:34.904
<v SPEAKER_01>But the day before,
562
00:29:34.954 --> 00:29:39.938
<v SPEAKER_01>I went to Intel's research lab with Jack Cavalieros to see ideas that aren't ready
563
00:29:40.119 --> 00:29:41.119
<v SPEAKER_01>for the node yet.
564
00:29:41.260 --> 00:29:42.538
<v SPEAKER_01>We started with wiring.
565
00:29:42.901 --> 00:29:46.123
<v SPEAKER_01>A transistor is only useful once it's connected to others.
566
00:29:46.484 --> 00:29:47.374
<v SPEAKER_01>And on a modern ship,
567
00:29:47.424 --> 00:29:51.518
<v SPEAKER_01>that takes more than a dozen layers of metal wires stacked above the transistors,
568
00:29:51.568 --> 00:29:52.679
<v SPEAKER_01>called interconnect.
569
00:29:53.129 --> 00:29:54.851
<v SPEAKER_01>These wires are made of copper.
570
00:29:55.131 --> 00:29:58.131
<v SPEAKER_01>And as they shrink, copper starts to run into trouble.
571
00:29:58.453 --> 00:30:00.286
<v SPEAKER_01>Intel is exploring a replacement.
572
00:30:00.635 --> 00:30:01.366
<v SPEAKER_01> Ruthenium.
573
00:30:01.416 --> 00:30:02.778
<v SPEAKER_01>Ruthenium has higher resistivity.
574
00:30:02.818 --> 00:30:04.912
<v SPEAKER_01>So why are you guys exploring ruthenium for the future?
575
00:30:04.962 --> 00:30:06.295
<v SPEAKER_02>So interestingly enough,
576
00:30:06.424 --> 00:30:11.231
<v SPEAKER_02>as you scale the dimensions of those copper wires, you run into challenges.
577
00:30:11.351 --> 00:30:15.477
<v SPEAKER_02>For example, copper requires typically a liner in order to deposit.
578
00:30:15.477 --> 00:30:17.421
<v SPEAKER_02> With a copper to fill those lines.
579
00:30:17.719 --> 00:30:22.886
<v SPEAKER_02>Ruthenium is very different in that regard because it's a material that we can actually etch.
580
00:30:23.426 --> 00:30:26.370
<v SPEAKER_02>And as such, by etching it, we don't need that liner.
581
00:30:26.870 --> 00:30:30.013
<v SPEAKER_02>So now you scale those very fine dimensions.
582
00:30:30.474 --> 00:30:34.738
<v SPEAKER_02> And if you can trade off that resistive liner, So what is the liner?
583
00:30:55.913 --> 00:30:56.913
<v SPEAKER_02>The liner is,
584
00:30:56.973 --> 00:30:58.574
<v SPEAKER_02>think of it almost like a glue layer,
585
00:30:58.614 --> 00:31:03.156
<v SPEAKER_02>a transition layer that we need in order to deposit the copper and have it stick
586
00:31:03.236 --> 00:31:05.807
<v SPEAKER_02>and make that connection to the copper lines below it.
587
00:31:05.857 --> 00:31:09.857
<v SPEAKER_02>These are all interlocking copper lines that interconnect to each other.
588
00:31:10.358 --> 00:31:15.120
<v SPEAKER_02>But every time you deposit copper, you've always had a liner underneath it.
589
00:31:15.540 --> 00:31:16.160
<v SPEAKER_02>And in the past,
590
00:31:16.200 --> 00:31:19.942
<v SPEAKER_02>that liner may have been a significant portion of the entirety of
591
00:31:19.982 --> 00:31:21.149
<v SPEAKER_02>that conduction path.
592
00:31:21.903 --> 00:31:22.643
<v SPEAKER_02>But over time,
593
00:31:22.663 --> 00:31:27.688
<v SPEAKER_02>we've scaled it, made it thinner, and so copper comes back into play as a contender.
594
00:31:28.008 --> 00:31:32.632
<v SPEAKER_01>One thing I'd be curious about to know is how you decide that a technology is mature
595
00:31:32.673 --> 00:31:35.515
<v SPEAKER_01>and ready for high volume manufacturing.
596
00:31:35.555 --> 00:31:37.577
<v SPEAKER_01>So with 10 nanometer,
597
00:31:37.597 --> 00:31:40.710
<v SPEAKER_01>you're mentioning you guys moved on from copper to cobalt,
598
00:31:40.760 --> 00:31:42.932
<v SPEAKER_01>and there were potential issues with that.
599
00:31:42.982 --> 00:31:46.308
<v SPEAKER_01>How do you decide that this technology is going to work at scale?
600
00:31:46.358 --> 00:31:49.980
<v SPEAKER_02>So the integration of these materials into such a complex system as
601
00:31:50.000 --> 00:31:54.602
<v SPEAKER_02>the transistor ecosystem involves many, many different components.
602
00:31:54.782 --> 00:31:58.615
<v SPEAKER_02>The scalability is one part, but its ability to integrate is another.
603
00:31:59.484 --> 00:32:02.656
<v SPEAKER_02>At the time we made a decision for cobalt, it was the forerunner.
604
00:32:02.706 --> 00:32:04.817
<v SPEAKER_02>The results were stronger at the time.
605
00:32:05.247 --> 00:32:07.428
<v SPEAKER_02>But as we work with our ecosystem externally,
606
00:32:07.448 --> 00:32:10.728
<v SPEAKER_02>the vendor ecosystem that provides these materials and the tools
607
00:32:10.768 --> 00:32:12.324
<v SPEAKER_02>that we integrate them with,
608
00:32:12.509 --> 00:32:17.750
<v SPEAKER_02>we find solutions down the road that may bring copper back in line as being
609
00:32:18.430 --> 00:32:19.790
<v SPEAKER_02>the stronger of the two.
610
00:32:20.310 --> 00:32:22.088
<v SPEAKER_02>And that's exactly what happens.
611
00:32:22.631 --> 00:32:26.575
<v SPEAKER_02>Every technology that we go through, we will evaluate multiple options.
612
00:32:27.212 --> 00:32:31.674
<v SPEAKER_02>And as we Get closer to our time horizon for delivering
613
00:32:31.714 --> 00:32:34.992
<v SPEAKER_02>a manufacturing-worthy product, we have to make a decision.
614
00:32:35.555 --> 00:32:37.726
<v SPEAKER_02>And the leading option at the time was cobalt,
615
00:32:37.776 --> 00:32:41.554
<v SPEAKER_02>now it's copper again, and perhaps in the future it'll be ruthenium.
616
00:32:42.057 --> 00:32:47.939
<v SPEAKER_01>I'd love to get your thoughts on CPET, basically stacking the transistors on top of each other.
617
00:32:48.663 --> 00:32:50.405
<v SPEAKER_01> What is progress like there?
618
00:32:50.945 --> 00:32:52.396
<v SPEAKER_01>Can you keep making more and more layers?
619
00:32:52.446 --> 00:32:53.026
<v SPEAKER_01>Is it just two?
620
00:32:53.046 --> 00:32:53.987
<v SPEAKER_01>Can we go three, four?
621
00:32:54.027 --> 00:32:54.858
<v SPEAKER_01>How high can you get?
622
00:32:54.908 --> 00:33:01.908
<v SPEAKER_02>Yeah, so that evaluation of CFED is currently underway, not just by us, by our competition.
623
00:33:03.214 --> 00:33:05.103
<v SPEAKER_02>Labs externally are looking at it.
624
00:33:05.415 --> 00:33:07.359
<v SPEAKER_02>It is the ultimate in stackability.
625
00:33:07.597 --> 00:33:10.749
<v SPEAKER_02>We're taking transistors that had to be compressed more and more,
626
00:33:10.799 --> 00:33:14.081
<v SPEAKER_02>and we're relaxing that in some ways because we're going to stack them on top
627
00:33:14.121 --> 00:33:15.121
<v SPEAKER_02>of each other.
628
00:33:15.279 --> 00:33:18.573
<v SPEAKER_02> But the act of stacking does not mean that they're not interconnected.
629
00:33:18.623 --> 00:33:21.787
<v SPEAKER_02>What used to be connections on the top or even on the bottom,
630
00:33:21.807 --> 00:33:23.899
<v SPEAKER_02>as you've seen from our press release,
631
00:33:23.949 --> 00:33:27.433
<v SPEAKER_02>now has to go vertically in between the transistors.
632
00:33:27.613 --> 00:33:32.018
<v SPEAKER_02>And that's a new challenge because the aspect ratio of creating trenches
633
00:33:32.119 --> 00:33:35.232
<v SPEAKER_02>and filling those trenches becomes more and more difficult.
634
00:33:35.282 --> 00:33:38.884
<v SPEAKER_02>So it's not as straightforward as stacking the transistors because you still have
635
00:33:38.904 --> 00:33:40.495
<v SPEAKER_02>to think about interconnecting them.
636
00:33:40.545 --> 00:33:43.136
<v SPEAKER_01>Is the issue there the etch to get that deep hole?
637
00:33:43.186 --> 00:33:45.147
<v SPEAKER_02>Aspect ratio for the etches is a big part of it.
638
00:33:45.167 --> 00:33:47.889
<v SPEAKER_02>We're working with our vendors to evolve on that.
639
00:33:48.048 --> 00:33:51.159
<v SPEAKER_02>But it's also what you fill those very tiny spaces with.
640
00:33:51.610 --> 00:33:57.313
<v SPEAKER_02>Because filling can sometimes leave air gaps or holes that never really fill.
641
00:33:57.913 --> 00:33:58.814
<v SPEAKER_02> And that's not ideal.
642
00:33:58.834 --> 00:34:01.905
<v SPEAKER_01>I assume there's a version of CFED that works inside this lab.
643
00:34:01.955 --> 00:34:06.028
<v SPEAKER_01>What is the kind of wafer or process or whatever that is working right now?
644
00:34:06.078 --> 00:34:06.818
<v SPEAKER_01>Then what's the next step?
645
00:34:06.838 --> 00:34:07.478
<v SPEAKER_01>What's the next step?
646
00:34:07.498 --> 00:34:12.121
<v SPEAKER_01>What's the next step until it's inside the full high volume process?
647
00:34:12.493 --> 00:34:15.796
<v SPEAKER_02>Part of the process of evolving these technologies,
648
00:34:15.836 --> 00:34:18.788
<v SPEAKER_02>especially something more complex like an architecture,
649
00:34:18.838 --> 00:34:21.460
<v SPEAKER_02>not just a basic chemistry or a material,
650
00:34:21.500 --> 00:34:23.481
<v SPEAKER_02>but a full architecture like CFET,
651
00:34:24.182 --> 00:34:28.571
<v SPEAKER_02>is that we have to make short loop vehicles that can give us faster turnaround.
652
00:34:28.646 --> 00:34:33.272
<v SPEAKER_02>The normal manufacturing process can take a month or longer to complete
653
00:34:33.292 --> 00:34:35.686
<v SPEAKER_02>the thousands of steps that it goes through.
654
00:34:35.736 --> 00:34:40.884
<v SPEAKER_02>Our goal here is to take unit cells of that process and qualify them.
655
00:34:43.347 --> 00:34:47.191
<v SPEAKER_02>Short-loop vehicles that can give us electrical parameters,
656
00:34:47.611 --> 00:34:52.111
<v SPEAKER_02>chemical parameters that can resolve some of those challenges, those speed bumps.
657
00:34:52.816 --> 00:34:57.821
<v SPEAKER_02>And once we've resolved them, then we combine them into a more complex test vehicle.
658
00:34:58.382 --> 00:35:01.645
<v SPEAKER_02>So what you would find in here is something very simple.
659
00:35:01.705 --> 00:35:03.046
<v SPEAKER_02>You might be making a diode.
660
00:35:03.066 --> 00:35:07.831
<v SPEAKER_02>You might be making a capacitor, which are components of the transistor.
661
00:35:08.471 --> 00:35:11.694
<v SPEAKER_02>And as those evolve and become stronger,
662
00:35:11.894 --> 00:35:12.894
<v SPEAKER_02>better performing,
663
00:35:13.015 --> 00:35:17.348
<v SPEAKER_02>you combine them to make the next stage, which might be the transistor itself.
664
00:35:17.879 --> 00:35:23.543
<v SPEAKER_02>So in the CFED example, you might not choose to do four ribbons on top of four ribbons.
665
00:35:23.563 --> 00:35:28.166
<v SPEAKER_02>You might just choose to do one-on-one because naturally the aspect ratio of dealing
666
00:35:28.207 --> 00:35:31.874
<v SPEAKER_02>with something that much taller becomes more and more challenging.
667
00:35:32.029 --> 00:35:34.862
<v SPEAKER_02>So we would We have a simplified version of a CFIT,
668
00:35:35.312 --> 00:35:39.536
<v SPEAKER_02>which has only one wire for the NMOS and one wire for the PMOS.
669
00:35:40.377 --> 00:35:41.928
<v SPEAKER_02>And that simplifies our job,
670
00:35:41.978 --> 00:35:45.961
<v SPEAKER_02>but it still helps us evaluate the stacking of devices
671
00:35:46.082 --> 00:35:47.403
<v SPEAKER_02>and how they will interconnect.
672
00:35:47.423 --> 00:35:50.936
<v SPEAKER_01>But are the feature sizes here as small as they will be eventually,
673
00:35:50.986 --> 00:35:53.208
<v SPEAKER_01>or are the feature sizes bigger as well?
674
00:35:54.229 --> 00:35:55.229
<v SPEAKER_02> At least a small.
675
00:35:55.931 --> 00:35:56.571
<v SPEAKER_02>For example,
676
00:35:56.591 --> 00:35:58.714
<v SPEAKER_02>you've heard of 2D materials,
677
00:35:59.254 --> 00:36:02.799
<v SPEAKER_02>these transition layer dicot collagenides as they're called.
678
00:36:03.800 --> 00:36:05.842
<v SPEAKER_02>They're very, very thin materials.
679
00:36:05.882 --> 00:36:09.271
<v SPEAKER_02>They're essentially one monolayer of atoms that we deal with.
680
00:36:09.773 --> 00:36:12.106
<v SPEAKER_02> Those depositions can happen in this lab.
681
00:36:12.317 --> 00:36:15.301
<v SPEAKER_02>We can evaluate those films in terms of conductivity,
682
00:36:15.401 --> 00:36:16.957
<v SPEAKER_02>our ability to contact them,
683
00:36:17.485 --> 00:36:21.811
<v SPEAKER_02>our ability to modulate that conductivity, which is what the transistor does.
684
00:36:22.412 --> 00:36:24.034
<v SPEAKER_02>So yes, we do have...
685
00:36:24.895 --> 00:36:30.236
<v SPEAKER_02>The ability to not only deposit films that are very small and thin to
686
00:36:30.276 --> 00:36:33.237
<v SPEAKER_02>the atomic scale, but also print very small features.
687
00:36:33.337 --> 00:36:35.698
<v SPEAKER_02>We have EUV technology that can,
688
00:36:36.658 --> 00:36:40.739
<v SPEAKER_02>or e-beam technology that can allow us to print very small features similar
689
00:36:40.779 --> 00:36:42.750
<v SPEAKER_02>to what we will eventually make in production.
690
00:36:42.800 --> 00:36:46.361
<v SPEAKER_01>So I guess I don't understand...
691
00:36:48.509 --> 00:36:49.509
<v SPEAKER_01>Intuitively,
692
00:36:49.671 --> 00:36:51.671
<v SPEAKER_01>lacking the context in this process,
693
00:36:51.894 --> 00:36:56.661
<v SPEAKER_01>why that you have the features that are as small for working CFET right now.
694
00:36:56.941 --> 00:36:57.552
<v SPEAKER_02>Yes.
695
00:36:57.602 --> 00:37:00.747
<v SPEAKER_01>Why will it take 10 years for it to be in my phone?
696
00:37:01.728 --> 00:37:02.890
<v SPEAKER_01>I understand it as a process.
697
00:37:02.890 --> 00:37:05.212
<v SPEAKER_01> But why is it such a long process?
698
00:37:05.672 --> 00:37:08.325
<v SPEAKER_02>The answer is slightly different when you're dealing with
699
00:37:08.375 --> 00:37:11.153
<v SPEAKER_02>an architecture like CFET versus a novel material.
700
00:37:11.978 --> 00:37:12.978
<v SPEAKER_02>Materials have,
701
00:37:13.079 --> 00:37:14.030
<v SPEAKER_02>of course,
702
00:37:14.080 --> 00:37:16.442
<v SPEAKER_02>the challenges of being deposited,
703
00:37:16.702 --> 00:37:21.306
<v SPEAKER_02>etched, removed, their compatibility with other layers above and below.
704
00:37:21.766 --> 00:37:26.440
<v SPEAKER_02>All those things have to be researched first before you put them in a production line.
705
00:37:26.490 --> 00:37:29.453
<v SPEAKER_02>An architecture may seem like a simple evolution.
706
00:37:29.573 --> 00:37:30.684
<v SPEAKER_02>Oh, you're making...
707
00:37:31.034 --> 00:37:35.346
<v SPEAKER_02> Nano ribbon transistors next to each other, what's wrong with just stacking them?
708
00:37:35.396 --> 00:37:37.177
<v SPEAKER_02>But the act of stacking them,
709
00:37:37.317 --> 00:37:37.767
<v SPEAKER_02>of course,
710
00:37:37.817 --> 00:37:39.908
<v SPEAKER_02>increases the aspect ratio for etches,
711
00:37:39.958 --> 00:37:43.940
<v SPEAKER_02>depositions, cleans, and the technology may simply not be ready yet.
712
00:37:44.261 --> 00:37:49.320
<v SPEAKER_01>But if you've already made it here, there's a version of the technology that's ready, right?
713
00:37:49.370 --> 00:37:50.020
<v SPEAKER_02> Correct.
714
00:37:50.070 --> 00:37:55.352
<v SPEAKER_02>So we've made a simplified version that may not be an advantage
715
00:37:55.492 --> 00:37:59.854
<v SPEAKER_02>over our current planar side-by-side technology of nanoribbons.
716
00:38:00.214 --> 00:38:04.815
<v SPEAKER_02>But we need to evolve it to make it maybe two nanoribbons or to add the right type
717
00:38:04.855 --> 00:38:09.337
<v SPEAKER_02>of metals and dielectrics in order to extract the maximum performance out of
718
00:38:09.377 --> 00:38:10.252
<v SPEAKER_02>that device.
719
00:38:10.302 --> 00:38:10.792
<v SPEAKER_01> Got it.
720
00:38:10.842 --> 00:38:12.413
<v SPEAKER_01>So it's like a long tail of...
721
00:38:12.463 --> 00:38:15.404
<v SPEAKER_02>There's a thousand different steps that all have to come together in
722
00:38:15.444 --> 00:38:21.047
<v SPEAKER_02>a very unique way to make the performance compatible or actually supersede
723
00:38:21.087 --> 00:38:22.238
<v SPEAKER_02>the prior technology.
724
00:38:22.288 --> 00:38:23.548
<v SPEAKER_01>Where do the ideas tend to fail?
725
00:38:23.568 --> 00:38:26.846
<v SPEAKER_01>So like, you have like 20 ideas that are like 2D materials.
726
00:38:27.750 --> 00:38:32.223
<v SPEAKER_01>What is the kind of way in which you're like, this is actually not worth pursuing further?
727
00:38:32.273 --> 00:38:37.555
<v SPEAKER_02>Sometimes the idea becomes something that we discover fundamentals about
728
00:38:37.595 --> 00:38:42.176
<v SPEAKER_02>the material that will be incompatible with the rest of the processing that we do.
729
00:38:43.157 --> 00:38:43.907
<v SPEAKER_02>At first,
730
00:38:43.957 --> 00:38:44.317
<v SPEAKER_02>you know,
731
00:38:44.337 --> 00:38:48.739
<v SPEAKER_02>the first level of experiments may simply be very simple depositions and you say,
732
00:38:48.759 --> 00:38:49.609
<v SPEAKER_02>okay,
733
00:38:49.659 --> 00:38:50.779
<v SPEAKER_02>I can deposit the film,
734
00:38:50.819 --> 00:38:51.810
<v SPEAKER_02>I can look at it,
735
00:38:51.860 --> 00:38:56.261
<v SPEAKER_02>I can measure it, but the moment I try to make a contact to it, nothing sticks.
736
00:38:56.721 --> 00:39:00.165
<v SPEAKER_02>It could be something fundamental as simple as the adhesion of
737
00:39:00.583 --> 00:39:05.596
<v SPEAKER_02>the material Next step in the process simply has no way to adhere to the material.
738
00:39:06.390 --> 00:39:10.334
<v SPEAKER_02> So you may rule out a material because of something as simple as that.
739
00:39:10.871 --> 00:39:14.112
<v SPEAKER_02>More complex challenges might be
740
00:39:15.232 --> 00:39:20.894
<v SPEAKER_02>the subsequent processing may have gaseous interactions with downstream steps.
741
00:39:20.934 --> 00:39:21.674
<v SPEAKER_02>So for example,
742
00:39:21.694 --> 00:39:22.944
<v SPEAKER_02>I've deposited the film,
743
00:39:22.994 --> 00:39:26.438
<v SPEAKER_02>I've capped it with other materials, but they're not hermetic.
744
00:39:26.615 --> 00:39:31.917
<v SPEAKER_02>And so my third or fourth or fifth step in the process may actually still interact
745
00:39:31.937 --> 00:39:33.826
<v SPEAKER_02>with it and change its properties.
746
00:39:34.037 --> 00:39:39.706
<v SPEAKER_02> That makes it unstable and now we have to find better hermetic sealing for that process.
747
00:39:40.186 --> 00:39:45.154
<v SPEAKER_02>And if we don't find a way to control it, then it's a dead end for us.
748
00:39:45.734 --> 00:39:48.512
<v SPEAKER_01>Stacking transistors is still in the research lab.
749
00:39:48.839 --> 00:39:51.693
<v SPEAKER_01>And this is why using whole chips is already in production and it tackles
750
00:39:51.743 --> 00:39:55.218
<v SPEAKER_01>a different problem, how separate chips communicate with each other.
751
00:39:55.268 --> 00:39:59.685
<v SPEAKER_01>Modern computers are divided into multiple parts, each optimized for a different task.
752
00:39:59.735 --> 00:40:03.521
<v SPEAKER_01>For example, NVIDIA's Blackwell Data Center GPU joins two
753
00:40:08.007 --> 00:40:13.034
<v SPEAKER_01>These chips have to constantly send data back and forth with each other and in AI,
754
00:40:13.355 --> 00:40:14.799
<v SPEAKER_01>the speed of that traffic,
755
00:40:15.178 --> 00:40:16.900
<v SPEAKER_01>not the raw computation itself,
756
00:40:17.040 --> 00:40:21.504
<v SPEAKER_01>is often what limits how fast the work Imagine two chips side by side,
757
00:40:21.844 --> 00:40:24.055
<v SPEAKER_01>communicating through their facing edges.
758
00:40:24.105 --> 00:40:26.276
<v SPEAKER_01>If you double each chip's width and length,
759
00:40:26.326 --> 00:40:28.516
<v SPEAKER_01>you'd have four times the area for circuitry,
760
00:40:28.566 --> 00:40:31.097
<v SPEAKER_01>but only twice the edge length for connections.
761
00:40:31.147 --> 00:40:33.480
<v SPEAKER_01>This is the area versus perimeter problem.
762
00:40:33.588 --> 00:40:35.159
<v SPEAKER_01>As transistors become denser,
763
00:40:35.209 --> 00:40:38.990
<v SPEAKER_01>a chip's ability to do computations increases faster than its ability
764
00:40:39.030 --> 00:40:40.150
<v SPEAKER_01>to move data around.
765
00:40:40.450 --> 00:40:42.761
<v SPEAKER_01>The industry has known about this problem for years,
766
00:40:42.811 --> 00:40:45.522
<v SPEAKER_01>so multiple technologies have been invented to address it.
767
00:40:45.572 --> 00:40:48.914
<v SPEAKER_01> The completed circuits must undergo two last operations,
768
00:40:49.575 --> 00:40:51.256
<v SPEAKER_03> bonding and packaging.
769
00:40:51.556 --> 00:40:52.647
<v SPEAKER_01>Once a chip is made,
770
00:40:52.697 --> 00:40:56.209
<v SPEAKER_01>it still has to be connected to other chips and to the rest of the computer.
771
00:40:56.259 --> 00:41:00.272
<v SPEAKER_01>That step is called packaging, and it has changed a lot in the last few decades.
772
00:41:00.322 --> 00:41:03.514
<v SPEAKER_01>At a high level, you can think of the evolution of packaging like this.
773
00:41:03.564 --> 00:41:06.008
<v SPEAKER_01>Initially, chips were laid out side by side.
774
00:41:06.326 --> 00:41:09.826
<v SPEAKER_01>Wires connecting them went out the side of one chip to another.
775
00:41:10.068 --> 00:41:11.961
<v SPEAKER_01>To allow for more communication density,
776
00:41:12.011 --> 00:41:14.545
<v SPEAKER_01>the industry introduced a shared piece of silicon,
777
00:41:14.595 --> 00:41:17.428
<v SPEAKER_01>called an interposer, for multiple chips to sit on.
778
00:41:17.579 --> 00:41:22.036
<v SPEAKER_01>A chip can talk to other chips through the wiring that runs directly through the interposer.
779
00:41:22.086 --> 00:41:25.972
<v SPEAKER_01>This type of packaging is often called 2.5 Another way
780
00:41:26.032 --> 00:41:30.032
<v SPEAKER_01>to increase connection density is to bond chips directly to one another.
781
00:41:30.438 --> 00:41:33.052
<v SPEAKER_01>This allows for shorter connections between chips,
782
00:41:33.102 --> 00:41:36.047
<v SPEAKER_01>but the early versions of this idea use solder bumps,
783
00:41:36.307 --> 00:41:38.529
<v SPEAKER_01>which are bulky and increase resistance.
784
00:41:38.891 --> 00:41:42.856
<v SPEAKER_01>It would be better to They skip the solder and fuse the signal wire connections of
785
00:41:42.877 --> 00:41:44.980
<v SPEAKER_01>the two chips directly to each other.
786
00:41:45.540 --> 00:41:47.207
<v SPEAKER_01>This is called hybrid bonding,
787
00:41:47.403 --> 00:41:50.548
<v SPEAKER_01>and it is one of the technologies the semiconductor industry is investing in
788
00:41:50.588 --> 00:41:51.519
<v SPEAKER_01>the most.
789
00:41:51.569 --> 00:41:54.123
<v SPEAKER_01>Hybrid bonding works by aligning the copper interconnects
790
00:41:54.173 --> 00:41:57.768
<v SPEAKER_01>of one chip This process makes the insulating surfaces around the copper bond
791
00:41:57.818 --> 00:41:58.019
<v SPEAKER_01>as well.
792
00:41:58.039 --> 00:42:02.317
<v SPEAKER_01>And so by removing the solder bumps, you end up with much denser connections.
793
00:42:09.816 --> 00:42:13.538
<v SPEAKER_01>Intel has spent over 50 years optimizing its CPUs for speed,
794
00:42:13.558 --> 00:42:14.828
<v SPEAKER_01>but lots of these optimizations,
795
00:42:14.878 --> 00:42:19.545
<v SPEAKER_01>like caching and branch prediction and speculative execution, reduce predictability.
796
00:42:35.007 --> 00:42:39.418
<v SPEAKER_01> The exact same instructions can take four cycles to execute one time and 300 the next.
797
00:42:39.468 --> 00:42:41.869
<v SPEAKER_01>When you stack billions of instructions together and execute them
798
00:42:41.909 --> 00:42:43.640
<v SPEAKER_01>across multiple threads and cores,
799
00:42:43.690 --> 00:42:47.746
<v SPEAKER_01>these non-determinisms compound into all sorts of hard-to-reproduce bugs.
800
00:42:48.211 --> 00:42:50.962
<v SPEAKER_01>If you work on serious systems, you've definitely experienced this.
801
00:42:51.012 --> 00:42:54.012
<v SPEAKER_01>Antithesis solved this by doing something a bit crazy.
802
00:42:54.253 --> 00:42:57.294
<v SPEAKER_01>They built a 100% deterministic computer.
803
00:42:57.714 --> 00:43:01.820
<v SPEAKER_01>They identified every single door in Intel's x86 architecture
804
00:43:02.101 --> 00:43:04.054
<v SPEAKER_01>where non-determinism could leak in.
805
00:43:04.104 --> 00:43:07.826
<v SPEAKER_01>Network packets, disk grids, temperature sensors, even time itself.
806
00:43:08.170 --> 00:43:12.559
<v SPEAKER_01>And they either welded each of these shut or slotted in a controlled situation.
807
00:43:12.716 --> 00:43:15.370
<v SPEAKER_01> This deterministic computer is just a foundation.
808
00:43:15.420 --> 00:43:15.911
<v SPEAKER_01>On top of it,
809
00:43:15.961 --> 00:43:19.997
<v SPEAKER_01>Antithesis built a testing platform that compresses years of production hardening
810
00:43:20.047 --> 00:43:21.019
<v SPEAKER_01>into minutes.
811
00:43:21.069 --> 00:43:23.803
<v SPEAKER_01>It runs your software through thousands of parallel worlds,
812
00:43:23.853 --> 00:43:27.178
<v SPEAKER_01>injecting faults and intelligently steering each one towards
813
00:43:27.198 --> 00:43:33.824
<v SPEAKER_01>a one This determinism is what's behind all the other insane antithesis features
814
00:43:33.864 --> 00:43:36.475
<v SPEAKER_01>that I've mentioned over the past few episodes.
815
00:43:36.586 --> 00:43:40.039
<v SPEAKER_01>It's what lets you reproduce any bug in time travel to any point in the test run.
816
00:43:40.089 --> 00:43:45.367
<v SPEAKER_01>Most importantly, it's what lets you or your agents trace every failure back to its root cause.
817
00:43:45.434 --> 00:43:49.898
<v SPEAKER_01>Go to antithesis.com slash dwarkesh to learn more.
818
00:43:53.212 --> 00:43:58.058
<v SPEAKER_01> Two different ways you could do hybrid bonding is dye to dye, then dye to wafer.
819
00:43:59.060 --> 00:44:01.293
<v SPEAKER_01>And maybe you can talk about the advantages of both and
820
00:44:01.343 --> 00:44:03.055
<v SPEAKER_01>which one actually practically works better.
821
00:44:03.105 --> 00:44:03.475
<v SPEAKER_01>Sure.
822
00:44:03.525 --> 00:44:04.727
<v SPEAKER_01>So actually around Intel,
823
00:44:04.767 --> 00:44:05.147
<v SPEAKER_01>typically,
824
00:44:05.167 --> 00:44:08.962
<v SPEAKER_02>I think as you're referring to dye to dye, we typically call it wafer to wafer.
825
00:44:09.012 --> 00:44:12.527
<v SPEAKER_02>So we actually take a full wafer and another wafer and bond them together.
826
00:44:12.577 --> 00:44:16.470
<v SPEAKER_02> That's an approach that's really popular right now in the CMOS image sensor industry.
827
00:44:16.520 --> 00:44:18.298
<v SPEAKER_02>In fact, basically dominates it.
828
00:44:18.782 --> 00:44:21.784
<v SPEAKER_02>And it's being looked at for other things like memory stacking,
829
00:44:21.824 --> 00:44:24.617
<v SPEAKER_02>all kinds of stuff people have published ideas about.
830
00:44:24.667 --> 00:44:28.880
<v SPEAKER_02>One of the challenges with that though, is that you need dyes that perfectly match each other.
831
00:44:28.930 --> 00:44:32.105
<v SPEAKER_02> And are perfectly like left-handed and right-handed, right?
832
00:44:32.155 --> 00:44:34.909
<v SPEAKER_02>So you have to be able to pull on exactly one to the other.
833
00:44:34.959 --> 00:44:37.263
<v SPEAKER_02>So one to one die size is a challenge.
834
00:44:37.383 --> 00:44:41.038
<v SPEAKER_02>So if they're not the exact same design device on top and bottom, that's a problem.
835
00:44:41.088 --> 00:44:41.970
<v SPEAKER_02>So wafer to wafer,
836
00:44:42.010 --> 00:44:44.693
<v SPEAKER_02>it's just challenging to make sure that you have wafer That match really well
837
00:44:44.733 --> 00:44:45.934
<v SPEAKER_02>in terms of the sort, right?
838
00:44:45.954 --> 00:44:48.843
<v SPEAKER_02>So sort good array here versus sort good array here.
839
00:44:49.317 --> 00:44:52.450
<v SPEAKER_02>If they match exactly good die and bad die that they all match,
840
00:44:52.500 --> 00:44:55.593
<v SPEAKER_02>I can get 100% yield of that operation of the good dies,
841
00:44:55.643 --> 00:44:57.695
<v SPEAKER_02>but the chances of that are very low.
842
00:44:57.745 --> 00:45:01.619
<v SPEAKER_02>It's gonna be some randomization of the two and whatever that randomization is,
843
00:45:01.669 --> 00:45:04.280
<v SPEAKER_02>it's just gonna be loss of good bonding to bad.
844
00:45:05.673 --> 00:45:08.785
<v SPEAKER_02> Whereas at chipped a wafer, I can dictate the terms, right?
845
00:45:08.835 --> 00:45:13.157
<v SPEAKER_02>I can singulate and have known good dyes that I've tested at the chip level and
846
00:45:13.177 --> 00:45:16.288
<v SPEAKER_02>then only bond known good to a known good base position.
847
00:45:16.619 --> 00:45:18.980
<v SPEAKER_01> Do you think then chipped a wafer is the way that you'll do hybrid bonding
848
00:45:19.020 --> 00:45:19.790
<v SPEAKER_02> in the future?
849
00:45:19.840 --> 00:45:21.211
<v SPEAKER_02>I think we're going to do both.
850
00:45:21.261 --> 00:45:22.992
<v SPEAKER_02>We definitely have the capability to do both.
851
00:45:23.042 --> 00:45:25.513
<v SPEAKER_02>It's really customer and architecture driven,
852
00:45:25.563 --> 00:45:26.974
<v SPEAKER_02> but certainly chipped a wafer in the
853
00:45:27.024 --> 00:45:28.975
<v SPEAKER_01> logic to logic space makes a lot of sense.
854
00:45:29.025 --> 00:45:33.188
<v SPEAKER_01>So you were explaining that going from advanced packaging The size of
855
00:45:33.209 --> 00:45:34.500
<v SPEAKER_01>the pitches is decreasing.
856
00:45:34.550 --> 00:45:35.752
<v SPEAKER_01>How much further could that go?
857
00:45:35.772 --> 00:45:37.074
<v SPEAKER_01>That's a wonderful question.
858
00:45:37.094 --> 00:45:37.895
<v SPEAKER_01>So, you know,
859
00:45:37.935 --> 00:45:38.687
<v SPEAKER_02>historically,
860
00:45:38.737 --> 00:45:40.570
<v SPEAKER_02>like we were saying 15 years ago,
861
00:45:40.700 --> 00:45:42.222
<v SPEAKER_02>first level interconnect was 130, 150 micrometer pitch.
862
00:45:42.242 --> 00:45:44.520
<v SPEAKER_02>Today in HVM, we're doing 25 micrometers.
863
00:45:48.230 --> 00:45:52.877
<v SPEAKER_02> Here we're doing sub 10, but there's already been literature out there.
864
00:45:52.897 --> 00:45:53.348
<v SPEAKER_02>In fact,
865
00:45:53.398 --> 00:45:57.224
<v SPEAKER_02>the biggest conference every year in packaging is the IEEE ECTC conference
866
00:45:57.244 --> 00:45:58.355
<v SPEAKER_02>that happens in May.
867
00:45:59.026 --> 00:46:02.890
<v SPEAKER_02>And there was a paper there this year showing Reliability data on
868
00:46:02.930 --> 00:46:06.411
<v SPEAKER_02>a 0.45 micron pitch hybrid bonded device.
869
00:46:07.172 --> 00:46:11.533
<v SPEAKER_02>So you can imagine that's a whole nother order of magnitude and density again from
870
00:46:11.573 --> 00:46:15.629
<v SPEAKER_02>where we are right now on HBI and scalability that's already been proven.
871
00:46:16.094 --> 00:46:18.415
<v SPEAKER_02>So I see a long runway there.
872
00:46:18.805 --> 00:46:23.182
<v SPEAKER_01> Within interconnect, within a single wafer, how far separated are they usually?
873
00:46:23.232 --> 00:46:24.994
<v SPEAKER_01> So the back end
874
00:46:25.014 --> 00:46:25.685
<v SPEAKER_02> of the fab,
875
00:46:25.735 --> 00:46:26.456
<v SPEAKER_02>you can imagine,
876
00:46:26.496 --> 00:46:31.924
<v SPEAKER_02>like the few layers below packaging are typically around one micron to a half micron
877
00:46:32.505 --> 00:46:33.505
<v SPEAKER_02>in size.
878
00:46:33.687 --> 00:46:37.468
<v SPEAKER_02>So if you can push packaging down to 0.5 microns or below,
879
00:46:37.988 --> 00:46:38.988
<v SPEAKER_02>we can start,
880
00:46:39.109 --> 00:46:43.010
<v SPEAKER_02>you can almost think about taking layers off the top of the die and connecting to
881
00:46:43.050 --> 00:46:46.641
<v SPEAKER_02>a lower layer within the silicon to another lower layer within the silicon, right?
882
00:46:46.691 --> 00:46:49.622
<v SPEAKER_02>That's really kind of where the beauty of hybrid bonding happens.
883
00:46:49.672 --> 00:46:53.573
<v SPEAKER_02>You can think someday about even having reduced interconnect layers on both sides
884
00:46:53.613 --> 00:46:57.994
<v SPEAKER_02>that we can bond together and have less total IR drop between
885
00:46:58.054 --> 00:46:59.498
<v SPEAKER_02>the two transistor layers.
886
00:47:00.595 --> 00:47:04.160
<v SPEAKER_02> Kind of cool to think about where that could go once we get into those regimes.
887
00:47:04.210 --> 00:47:04.662
<v SPEAKER_01>Actually,
888
00:47:04.712 --> 00:47:07.080
<v SPEAKER_01>I am very curious about For AI,
889
00:47:07.100 --> 00:47:08.742
<v SPEAKER_01>it makes sense why hybrid bonding is so powerful because
890
00:47:08.762 --> 00:47:10.993
<v SPEAKER_01>then you can get like higher bandwidth of the memory.
891
00:47:11.043 --> 00:47:11.484
<v SPEAKER_01>Absolutely.
892
00:47:11.504 --> 00:47:14.096
<v SPEAKER_01>But you're saying with issues with heat and everything,
893
00:47:14.146 --> 00:47:17.702
<v SPEAKER_01>what is the advantage for non-AI applications of hybrid bonding?
894
00:47:17.789 --> 00:47:18.619
<v SPEAKER_01>Excellent question.
895
00:47:18.669 --> 00:47:22.422
<v SPEAKER_02>So there are companies out there that are looking at it for non-AI applications,
896
00:47:22.472 --> 00:47:25.194
<v SPEAKER_02>even in fact in client devices, right?
897
00:47:25.895 --> 00:47:29.668
<v SPEAKER_02>And one of the big things I think that that can help with there is, well,
898
00:47:29.718 --> 00:47:30.118
<v SPEAKER_02>number one,
899
00:47:30.158 --> 00:47:30.819
<v SPEAKER_02>obviously the same,
900
00:47:30.859 --> 00:47:35.081
<v SPEAKER_02>raw interconnect density, especially between something like a CPU and a GPU.
901
00:47:35.485 --> 00:47:37.726
<v SPEAKER_02> But the other one is around power, right?
902
00:47:37.746 --> 00:47:38.996
<v SPEAKER_02>So like we talked about before,
903
00:47:39.046 --> 00:47:41.296
<v SPEAKER_02>as you get to finer and finer interconnects,
904
00:47:41.346 --> 00:47:45.757
<v SPEAKER_02>you can reduce the total power consumption in picojoules per bit for that interface.
905
00:47:45.807 --> 00:47:48.328
<v SPEAKER_02>So with hybrid bonding and those applications,
906
00:47:48.368 --> 00:47:50.369
<v SPEAKER_02>you could think about that as another way that package,
907
00:47:50.389 --> 00:47:52.639
<v SPEAKER_02>you can help reduce the total system power budget.
908
00:47:52.689 --> 00:47:53.259
<v SPEAKER_02>Interesting.
909
00:47:53.309 --> 00:47:54.960
<v SPEAKER_02>So then that gives you lots of benefits, right?
910
00:47:55.010 --> 00:47:56.330
<v SPEAKER_02>Lower power, less heat.
911
00:47:57.271 --> 00:47:59.929
<v SPEAKER_02> So far,
912
00:48:00.915 --> 00:48:02.927
<v SPEAKER_01> this has been about making better chips.
913
00:48:02.977 --> 00:48:06.866
<v SPEAKER_01>The other half of the question is how many chips the industry can make
914
00:48:06.922 --> 00:48:09.755
<v SPEAKER_01>if AI labs are willing to pay for far more of them.
915
00:48:10.278 --> 00:48:13.469
<v SPEAKER_01> I'm getting a chance to talk to Pushkar Arande, who is the CTO of Intel.
916
00:48:13.519 --> 00:48:18.279
<v SPEAKER_01>I'm very interested in understanding how the fact that the entire industry has
917
00:48:18.319 --> 00:48:21.990
<v SPEAKER_01>to rely on the same suppliers, bottlenecks your ability to ramp up production.
918
00:48:22.040 --> 00:48:25.901
<v SPEAKER_01>So for this EUV tool, ASML produces less than 100 of them a year.
919
00:48:26.181 --> 00:48:29.001
<v SPEAKER_01>And they don't plan to produce more than 100 a year,
920
00:48:29.041 --> 00:48:31.232
<v SPEAKER_01>even by the end of the decade, or significantly more than 100 a year.
921
00:48:31.282 --> 00:48:33.092
<v SPEAKER_01>And that is to be split between you,
922
00:48:33.142 --> 00:48:34.012
<v SPEAKER_01>between TSMC,
923
00:48:34.062 --> 00:48:37.053
<v SPEAKER_01>between all the memory makers who are ramping up production like SK Hinex.
924
00:48:37.103 --> 00:48:39.399
<v SPEAKER_01>How does that limit your ability to scale up to all this demand?
925
00:48:39.449 --> 00:48:40.449
<v SPEAKER_03> It is a limiter.
926
00:48:41.470 --> 00:48:45.583
<v SPEAKER_03>So we have to make the most of the capacity that we already have installed,
927
00:48:45.633 --> 00:48:49.736
<v SPEAKER_03>and we'll try to increase the output from our existing fleet of tools.
928
00:48:50.156 --> 00:48:53.658
<v SPEAKER_03>And EUV or ASML is not the only bottleneck.
929
00:48:54.238 --> 00:48:58.601
<v SPEAKER_03>It is definitely a bigger bottleneck than some of the other tools,
930
00:48:59.202 --> 00:49:06.202
<v SPEAKER_03>but to a large extent, we're seeing all equipment seeing tremendous supply shortage.
931
00:49:08.715 --> 00:49:11.826
<v SPEAKER_03>Even though there are multiple providers of other tools,
932
00:49:12.420 --> 00:49:15.984
<v SPEAKER_03>once you lock into a process flow, let's say 18A, right?
933
00:49:16.065 --> 00:49:17.847
<v SPEAKER_03>18A is a mature process now.
934
00:49:18.327 --> 00:49:20.310
<v SPEAKER_03>So we need a specific tool.
935
00:49:20.350 --> 00:49:23.314
<v SPEAKER_03>We can't just go and get a different tool for the same.
936
00:49:23.334 --> 00:49:26.398
<v SPEAKER_03>So therefore, we're locked into that one.
937
00:49:27.343 --> 00:49:28.444
<v SPEAKER_03> Two, one supplier.
938
00:49:28.985 --> 00:49:30.826
<v SPEAKER_03>And so we rely on that.
939
00:49:31.026 --> 00:49:35.781
<v SPEAKER_01>What lessons does this give for 14A in terms of by 2028, it's going to be such a crazy world.
940
00:49:35.831 --> 00:49:36.121
<v SPEAKER_01>Yes.
941
00:49:36.171 --> 00:49:39.374
<v SPEAKER_01>How do you structure things in such a way that you have flexibility in ramping?
942
00:49:39.394 --> 00:49:40.165
<v SPEAKER_03>Yes.
943
00:49:40.215 --> 00:49:40.705
<v SPEAKER_03>Actually,
944
00:49:40.755 --> 00:49:41.566
<v SPEAKER_03>the way to do it,
945
00:49:41.616 --> 00:49:42.507
<v SPEAKER_03>and we've been doing it,
946
00:49:42.557 --> 00:49:43.948
<v SPEAKER_03>and generally everybody does it,
947
00:49:43.998 --> 00:49:47.901
<v SPEAKER_03>is you try to maintain as much fungibility as possible going from one node to
948
00:49:47.941 --> 00:49:48.482
<v SPEAKER_03>the next node.
949
00:49:48.522 --> 00:49:53.887
<v SPEAKER_03> So let's say going from 18A to 14A, Maybe you would say 80% of the toolset can be reused.
950
00:49:54.188 --> 00:49:54.408
<v SPEAKER_03>And then,
951
00:49:54.428 --> 00:49:55.428
<v SPEAKER_03>of course, 14A,
952
00:49:55.569 --> 00:50:00.474
<v SPEAKER_03>for example, would require some new capabilities because it's a denser geometry.
953
00:50:01.255 --> 00:50:03.578
<v SPEAKER_03>So it would require some unique tools.
954
00:50:03.912 --> 00:50:06.323
<v SPEAKER_01>Do you have a sense of what is the ultimate bottleneck
955
00:50:06.373 --> 00:50:09.574
<v SPEAKER_01>of how many wafers you guys could produce a month,
956
00:50:09.814 --> 00:50:14.015
<v SPEAKER_01>even if you decided to invest infinity money into doing CapEx?
957
00:50:14.335 --> 00:50:16.656
<v SPEAKER_03>Given the existing constraints,
958
00:50:16.676 --> 00:50:20.897
<v SPEAKER_03>let's say we had to maximize the output from a given footprint of tools,
959
00:50:21.738 --> 00:50:24.698
<v SPEAKER_03>then I think it's Incremental because
960
00:50:25.178 --> 00:50:27.929
<v SPEAKER_03>the process today is already yielding pretty high.
961
00:50:27.979 --> 00:50:28.459
<v SPEAKER_03>And to get,
962
00:50:28.479 --> 00:50:29.170
<v SPEAKER_03>you know,
963
00:50:29.220 --> 00:50:31.050
<v SPEAKER_03>if your yield is already pretty high,
964
00:50:31.100 --> 00:50:36.121
<v SPEAKER_03>to get every 1% extra yield is extremely hard because it's already
965
00:50:36.161 --> 00:50:38.042
<v SPEAKER_03>a finely tuned process.
966
00:50:38.222 --> 00:50:39.889
<v SPEAKER_03> Are there enough tools in the
967
00:50:39.082 --> 00:50:40.382
<v SPEAKER_01> world to say you could 10x the amount
968
00:50:40.422 --> 00:50:42.493
<v SPEAKER_01>of wafers you're producing at the leading edge?
969
00:50:42.543 --> 00:50:44.963
<v SPEAKER_03>Not 10x, but probably like 2x, yes.
970
00:50:45.264 --> 00:50:50.325
<v SPEAKER_01>That's quite interesting because the AI industry for a decade has been 3x in compute.
971
00:50:50.605 --> 00:50:51.520
<v SPEAKER_01>Yes.
972
00:50:51.570 --> 00:50:52.570
<v SPEAKER_01> Yes.
973
00:50:52.871 --> 00:50:55.282
<v SPEAKER_01>And you're saying that that just can't continue.
974
00:50:55.332 --> 00:50:57.013
<v SPEAKER_03>Unless the entire supply chain,
975
00:50:57.033 --> 00:50:59.975
<v SPEAKER_03>starting from the equipment suppliers,
976
00:51:00.335 --> 00:51:01.176
<v SPEAKER_03>their suppliers,
977
00:51:01.216 --> 00:51:02.327
<v SPEAKER_03>their sub-suppliers,
978
00:51:02.557 --> 00:51:07.600
<v SPEAKER_03>unless everybody produces more, you can't increase the output collectively.
979
00:51:07.952 --> 00:51:11.341
<v SPEAKER_01>Just to give the audience a sense of how big the AI demand is
980
00:51:11.755 --> 00:51:15.617
<v SPEAKER_01>and how well it monetizes the products you guys are producing,
981
00:51:16.258 --> 00:51:17.068
<v SPEAKER_01>you can crunch the numbers,
982
00:51:17.118 --> 00:51:21.401
<v SPEAKER_01>and the numbers seem to suggest that just a couple billion dollars of CapEx
983
00:51:21.461 --> 00:51:27.206
<v SPEAKER_01>on Intel's account results in enough chips or the logic for enough chips to produce,
984
00:51:27.246 --> 00:51:29.767
<v SPEAKER_01>say, $100 billion of revenue for the AI model companies.
985
00:51:29.807 --> 00:51:32.629
<v SPEAKER_01>And, of course, there's so many other players within that stack.
986
00:51:32.649 --> 00:51:34.771
<v SPEAKER_01>There's also memory and other things.
987
00:51:35.251 --> 00:51:36.473
<v SPEAKER_01>But it's crazy that...
988
00:51:36.652 --> 00:51:40.115
<v SPEAKER_01>Within a couple billion dollars of CapEx,
989
00:51:40.155 --> 00:51:42.587
<v SPEAKER_01>which can be amortized over many different years,
990
00:51:42.637 --> 00:51:45.639
<v SPEAKER_01>produces $100 billion of revenue every single year,
991
00:51:46.000 --> 00:51:48.972
<v SPEAKER_01>which seems to suggest that at some point that should percolate down
992
00:51:49.022 --> 00:51:50.683
<v SPEAKER_01>and there should be some...
993
00:51:50.783 --> 00:51:51.184
<v SPEAKER_01>At some point,
994
00:51:51.204 --> 00:51:52.385
<v SPEAKER_01>the AI labs could just say,
995
00:51:52.405 --> 00:51:55.377
<v SPEAKER_01>we'll just buy everything, produce as much as you can, we'll just...
996
00:51:55.427 --> 00:51:57.600
<v SPEAKER_01> You know, guarantee future income streams and stuff.
997
00:51:57.650 --> 00:51:57.981
<v SPEAKER_03>Yes.
998
00:51:58.031 --> 00:52:01.465
<v SPEAKER_03>There's early signs that that could actually be happening already.
999
00:52:01.515 --> 00:52:03.778
<v SPEAKER_03>The demand signals are just so high.
1000
00:52:04.680 --> 00:52:10.522
<v SPEAKER_03>But I think you were alluding to how the value is Is accumulating at the top of
1001
00:52:10.542 --> 00:52:12.023
<v SPEAKER_03>the technology stack,
1002
00:52:12.083 --> 00:52:14.745
<v SPEAKER_03>which is essentially what is happening is,
1003
00:52:15.826 --> 00:52:16.046
<v SPEAKER_03>you know,
1004
00:52:16.086 --> 00:52:19.949
<v SPEAKER_03>we move from a fully vertically integrated industry like 30,
1005
00:52:20.009 --> 00:52:24.413
<v SPEAKER_03>40 years ago, maybe longer, to a very horizontal industry, right?
1006
00:52:24.453 --> 00:52:24.993
<v SPEAKER_03>Where, you know,
1007
00:52:25.013 --> 00:52:29.837
<v SPEAKER_03>you have foundries, you have equipment makers, you have, you know, their suppliers.
1008
00:52:30.538 --> 00:52:34.816
<v SPEAKER_03>And today you think about it, every hyperscaler is designing their own chips.
1009
00:52:35.341 --> 00:52:38.204
<v SPEAKER_03> And the scale of the hyperscalers is so large.
1010
00:52:38.404 --> 00:52:43.348
<v SPEAKER_03>And some of the model companies, for example, and their demand is so high.
1011
00:52:43.368 --> 00:52:50.206
<v SPEAKER_03>Yeah, they could easily just Consume an entire fabs worth of silicon on their own
1012
00:52:50.486 --> 00:52:53.038
<v SPEAKER_03>or multiple fabs worth of silicon on their own.
1013
00:52:53.088 --> 00:52:57.432
<v SPEAKER_03>And they definitely have the capital to fund that.
1014
00:52:58.032 --> 00:52:58.853
<v SPEAKER_03>So in some sense,
1015
00:52:58.873 --> 00:53:04.778
<v SPEAKER_03>we are moving from a sort of a horizontal world again to a pseudo vertical world
1016
00:53:04.818 --> 00:53:06.619
<v SPEAKER_03>where it's like the,
1017
00:53:06.700 --> 00:53:07.010
<v SPEAKER_03>you know,
1018
00:53:07.060 --> 00:53:08.060
<v SPEAKER_03>it's not,
1019
00:53:08.521 --> 00:53:10.753
<v SPEAKER_03>It's monolithically vertically integrated,
1020
00:53:10.803 --> 00:53:13.985
<v SPEAKER_03>but it's kind of virtually vertically integrated.
1021
00:53:14.005 --> 00:53:14.816
<v SPEAKER_01>Interesting.
1022
00:53:14.866 --> 00:53:20.490
<v SPEAKER_01>What is the nature of economies of scale in this business where you look
1023
00:53:20.510 --> 00:53:24.533
<v SPEAKER_01>at how many wafers at the leading edge TSMC versus Intel are shipping,
1024
00:53:25.033 --> 00:53:27.315
<v SPEAKER_01>upwards of 3x for TSMC?
1025
00:53:28.916 --> 00:53:32.739
<v SPEAKER_01>What kinds of advantages do you get at this point from economies of scale?
1026
00:53:32.759 --> 00:53:36.416
<v SPEAKER_01>Or is it that once you reach a certain point, the economies of scale get weaker?
1027
00:53:36.466 --> 00:53:38.077
<v SPEAKER_03> That's a very important question.
1028
00:53:38.127 --> 00:53:44.769
<v SPEAKER_03>This entire business just relies on scale and economies of scale.
1029
00:53:44.889 --> 00:53:51.050
<v SPEAKER_03>If you look at all the advanced manufacturing companies out there,
1030
00:53:51.631 --> 00:53:56.412
<v SPEAKER_03>probably semiconductor foundries, the scale economics is probably the purest.
1031
00:53:56.532 --> 00:54:00.310
<v SPEAKER_03>And the reason for that is the fixed cost is just so incredibly high
1032
00:54:01.174 --> 00:54:05.735
<v SPEAKER_03>that once you build a fab, 80% of your cost structure is fixed.
1033
00:54:06.749 --> 00:54:13.749
<v SPEAKER_03> And so what that means is every extra percentage of utilization is adding far more in revenue.
1034
00:54:16.196 --> 00:54:17.748
<v SPEAKER_03>So therefore, it's extremely important.
1035
00:54:17.798 --> 00:54:21.080
<v SPEAKER_03>And we'll fight for every extra percent of fab utilization,
1036
00:54:21.521 --> 00:54:25.023
<v SPEAKER_03>but also every extra percentage of fab output.
1037
00:54:25.063 --> 00:54:30.207
<v SPEAKER_03>As in, you know, let's say I'm making some wafers today and the yield is like 60%.
1038
00:54:30.828 --> 00:54:34.495
<v SPEAKER_03>But if I improve the process and the die yield becomes 65% or 70%,
1039
00:54:36.952 --> 00:54:38.462
<v SPEAKER_03> It's not a linear advantage.
1040
00:54:38.512 --> 00:54:42.283
<v SPEAKER_03>It's like I'm getting way more output for the given footprint, right?
1041
00:54:42.333 --> 00:54:45.674
<v SPEAKER_03>So there's always room to improve the economies of scale.
1042
00:54:45.714 --> 00:54:52.714
<v SPEAKER_03>And that's one of the reasons why you're seeing so much consolidation in this business, right?
1043
00:54:53.376 --> 00:54:57.654
<v SPEAKER_03>There's only three foundries left at the advanced node for that exact reason.
1044
00:54:58.377 --> 00:55:03.420
<v SPEAKER_03> And just along the way, Many companies just stop manufacturing.
1045
00:55:04.020 --> 00:55:04.661
<v SPEAKER_03>I don't know if you've seen,
1046
00:55:04.681 --> 00:55:10.067
<v SPEAKER_03>there's a chart where like 40 years ago, there were like 20 foundries.
1047
00:55:10.768 --> 00:55:14.373
<v SPEAKER_03>And over time, the number of foundries kept diminishing.
1048
00:55:14.413 --> 00:55:15.965
<v SPEAKER_03>Until today, there's only three.
1049
00:55:16.015 --> 00:55:19.056
<v SPEAKER_01>What is basically then the concrete master plan to catch up to TSMC?
1050
00:55:19.106 --> 00:55:20.550
<v SPEAKER_01>Even though TSMC is ahead,
1051
00:55:21.087 --> 00:55:24.870
<v SPEAKER_01>there's so much overflow demand at their leading edge,
1052
00:55:24.950 --> 00:55:27.231
<v SPEAKER_01>where N3 is now majority AI accelerators,
1053
00:55:27.491 --> 00:55:28.672
<v SPEAKER_01>maybe majority NVIDIA alone,
1054
00:55:28.692 --> 00:55:32.174
<v SPEAKER_01>that all this demand for CPUs,
1055
00:55:32.194 --> 00:55:33.084
<v SPEAKER_01>for other things,
1056
00:55:33.134 --> 00:55:33.575
<v SPEAKER_01>which are also,
1057
00:55:33.595 --> 00:55:37.787
<v SPEAKER_01>by the way, needed for AI, this humongous influx in demand for CPUs because of AI.
1058
00:55:37.837 --> 00:55:41.490
<v SPEAKER_01>How do you see this opportunity right now where Intel's a few years before,
1059
00:55:41.540 --> 00:55:43.681
<v SPEAKER_01>while TSMC is just way oversaturated?
1060
00:55:44.061 --> 00:55:47.867
<v SPEAKER_03> Catching up to TSMC maybe has multiple facets.
1061
00:55:49.189 --> 00:55:52.300
<v SPEAKER_03>I would say the catch-up that we need to do is in scale.
1062
00:55:52.494 --> 00:55:53.045
<v SPEAKER_03>Like you said,
1063
00:55:53.095 --> 00:55:58.002
<v SPEAKER_03>they're just a much larger wafer manufacturer today than we are,
1064
00:55:59.084 --> 00:56:01.946
<v SPEAKER_03>and even Bigger than what Samsung is.
1065
00:56:02.286 --> 00:56:07.687
<v SPEAKER_03>Cashing up in scale will be a slow process, a gradual process.
1066
00:56:08.908 --> 00:56:09.778
<v SPEAKER_03>If you meant,
1067
00:56:09.828 --> 00:56:10.048
<v SPEAKER_03>you know,
1068
00:56:10.068 --> 00:56:12.346
<v SPEAKER_03>catch up in terms of just the technology,
1069
00:56:12.809 --> 00:56:17.790
<v SPEAKER_03>I think that, you know, I think we're already there.
1070
00:56:17.991 --> 00:56:18.511
<v SPEAKER_03>Like, you know,
1071
00:56:18.531 --> 00:56:19.531
<v SPEAKER_03>we might maybe,
1072
00:56:19.811 --> 00:56:20.031
<v SPEAKER_03>you know,
1073
00:56:20.051 --> 00:56:27.051
<v SPEAKER_03>a few percent off on performance or power or area density, but,
1074
00:56:28.894 --> 00:56:29.894
<v SPEAKER_03>you know,
1075
00:56:30.318 --> 00:56:36.882
<v SPEAKER_03>This benchmarking of one foundry is ahead or one foundry is behind,
1076
00:56:37.883 --> 00:56:43.866
<v SPEAKER_03>it makes sense when you're a whole generation behind or two generations behind
1077
00:56:43.967 --> 00:56:44.967
<v SPEAKER_03>or ahead.
1078
00:56:45.207 --> 00:56:50.150
<v SPEAKER_03>That's when it makes a meaningful difference in your DAI output or your DAI area
1079
00:56:50.290 --> 00:56:51.846
<v SPEAKER_03>or functionality like power.
1080
00:56:52.532 --> 00:56:56.574
<v SPEAKER_03>But if you're within a few percent, it's really
1081
00:56:59.617 --> 00:57:05.519
<v SPEAKER_03>You're splitting hairs at that point in time because it's not very unidimensional
1082
00:57:05.559 --> 00:57:06.169
<v SPEAKER_03>at this point.
1083
00:57:06.219 --> 00:57:07.775
<v SPEAKER_03>It's not just about density.
1084
00:57:08.159 --> 00:57:11.280
<v SPEAKER_03>It's not just about raw performance.
1085
00:57:11.880 --> 00:57:14.391
<v SPEAKER_03>Different applications require different vectors.
1086
00:57:14.441 --> 00:57:19.196
<v SPEAKER_03> So, you know, you can be off by a few percent, but You need to be on time.
1087
00:57:19.697 --> 00:57:24.364
<v SPEAKER_03>Your execution needs to be such that your yields are very high to support very large
1088
00:57:24.639 --> 00:57:25.806
<v SPEAKER_03>and very rapid ramps.
1089
00:57:26.659 --> 00:57:33.322
<v SPEAKER_03>So that actually is more important than catching up on a few percent in performance or area.
1090
00:57:33.342 --> 00:57:36.403
<v SPEAKER_01>I was looking at some semi-analysis numbers that seem to suggest that in terms
1091
00:57:36.443 --> 00:57:37.665
<v SPEAKER_01>of transistor density,
1092
00:57:38.226 --> 00:57:42.004
<v SPEAKER_01>14A, which will come out in like 2028, would it be comparable to N2?
1093
00:57:43.266 --> 00:57:46.848
<v SPEAKER_03> Yeah, first of all, I would dispute your benchmarking.
1094
00:57:47.288 --> 00:57:48.289
<v SPEAKER_03>But like I said,
1095
00:57:48.329 --> 00:57:48.699
<v SPEAKER_03>I think,
1096
00:57:48.749 --> 00:57:55.749
<v SPEAKER_03>you know, it's important to be generally in the right ballpark, be very predictable.
1097
00:57:56.574 --> 00:57:57.574
<v SPEAKER_03>And also,
1098
00:57:57.735 --> 00:57:58.045
<v SPEAKER_03>you know,
1099
00:57:58.095 --> 00:58:00.056
<v SPEAKER_03>it's not unidimensional in terms of,
1100
00:58:00.076 --> 00:58:04.779
<v SPEAKER_03>you know, we don't build one type of transistor, let's say 14A or 18A.
1101
00:58:05.619 --> 00:58:07.911
<v SPEAKER_03>You build a few different types of transistors.
1102
00:58:07.961 --> 00:58:10.062
<v SPEAKER_03>Let's say there's a low leakage transistor,
1103
00:58:10.102 --> 00:58:13.494
<v SPEAKER_03>there's a high performance, you know, High-drive current transistor.
1104
00:58:13.544 --> 00:58:14.766
<v SPEAKER_03>You're building SRAMs.
1105
00:58:15.124 --> 00:58:16.624
<v SPEAKER_03>There's a high-density SRAM.
1106
00:58:16.644 --> 00:58:18.422
<v SPEAKER_03>There's a high-performance SRAM.
1107
00:58:18.705 --> 00:58:23.527
<v SPEAKER_03>There's many other functionalities, like some analog circuits, RF circuits.
1108
00:58:24.247 --> 00:58:29.648
<v SPEAKER_03> So it's the sum of all of those that makes a technology I
1109
00:58:29.668 --> 00:58:30.218
<v SPEAKER_01> guess that makes
1110
00:58:30.268 --> 00:58:32.520
<v SPEAKER_01>the CapEx you do right now even more important.
1111
00:58:32.570 --> 00:58:33.200
<v SPEAKER_01>So right now,
1112
00:58:33.250 --> 00:58:35.892
<v SPEAKER_01>or like TSMC is on track to do 50 billion in CapEx,
1113
00:58:35.912 --> 00:58:37.968
<v SPEAKER_01>around 50 billion in CapEx this year.
1114
00:58:38.033 --> 00:58:40.145
<v SPEAKER_01>You're on track to do around 20 billion.
1115
00:58:40.195 --> 00:58:41.926
<v SPEAKER_01>But if the tools you're buying right now will determine
1116
00:58:41.976 --> 00:58:44.968
<v SPEAKER_01>who can service all this crazy AI demand that's coming up,
1117
00:58:45.018 --> 00:58:47.920
<v SPEAKER_01>it makes the difference in CapEx even more important
1118
00:58:48.000 --> 00:58:51.663
<v SPEAKER_01>for like US versus other countries.
1119
00:58:52.103 --> 00:58:53.103
<v SPEAKER_03>Yes, very much.
1120
00:58:53.304 --> 00:58:54.304
<v SPEAKER_03>It's a little...
1121
00:58:55.516 --> 00:58:58.627
<v SPEAKER_03>A bit of an unfair comparison between us and TSMC today,
1122
00:58:58.999 --> 00:59:02.401
<v SPEAKER_03>just because today they're a foundry for basically everybody,
1123
00:59:02.921 --> 00:59:05.884
<v SPEAKER_03>and we're largely a foundry for Intel.
1124
00:59:06.084 --> 00:59:10.927
<v SPEAKER_03>We'll become a foundry for others, so in due course, our CapEx will also grow.
1125
00:59:11.227 --> 00:59:15.490
<v SPEAKER_01>Intel started as a DRAM business in the late 60s,
1126
00:59:15.971 --> 00:59:19.138
<v SPEAKER_01>and then you guys are producing DRAM, which you sold off.
1127
00:59:19.633 --> 00:59:21.965
<v SPEAKER_01>A couple years ago, you sold off your Flash business.
1128
00:59:22.015 --> 00:59:23.015
<v SPEAKER_01>Yes.
1129
00:59:25.245 --> 00:59:26.497
<v SPEAKER_01> Yeah, thoughts on that?
1130
00:59:26.547 --> 00:59:28.370
<v SPEAKER_01>For context for the audience,
1131
00:59:28.430 --> 00:59:33.978
<v SPEAKER_01>these are now multi-trillion dollar industries because they've just exploded as
1132
00:59:34.038 --> 00:59:35.941
<v SPEAKER_01>a result of AI demand for them.
1133
00:59:36.241 --> 00:59:36.592
<v SPEAKER_03>Yes.
1134
00:59:36.642 --> 00:59:40.087
<v SPEAKER_03>I mean, clearly, in hindsight, probably not the smartest time.
1135
00:59:40.167 --> 00:59:42.598
<v SPEAKER_03> We had time to sell off a flash memory business.
1136
00:59:42.648 --> 00:59:45.537
<v SPEAKER_03>There were good reasons why we did that when we did.
1137
00:59:46.431 --> 00:59:50.933
<v SPEAKER_03>Clearly, you know, nobody could see this demand, this enormous demand.
1138
00:59:52.274 --> 00:59:53.455
<v SPEAKER_03>But no, today,
1139
00:59:53.475 --> 00:59:55.836
<v SPEAKER_03>I think, I mean,
1140
00:59:56.176 --> 00:59:57.176
<v SPEAKER_03>essentially,
1141
00:59:58.118 --> 01:00:03.941
<v SPEAKER_03>the world will eat up as much compute as can possibly be made and it'll eat up
1142
01:00:04.041 --> 01:00:06.208
<v SPEAKER_03>as much memory as can possibly be made.
1143
01:00:07.645 --> 01:00:12.480
<v SPEAKER_03> The supply crunch is larger for memory today than it is for compute.
1144
01:00:12.890 --> 01:00:16.373
<v SPEAKER_01> So can I summarize what it seems to me the takeaways from your projections are?
1145
01:00:16.393 --> 01:00:17.564
<v SPEAKER_01>And you can tell me if that's correct.
1146
01:00:17.614 --> 01:00:18.204
<v SPEAKER_01>Yes.
1147
01:00:18.254 --> 01:00:22.888
<v SPEAKER_01>Marginal production can increase actually very fast, you know, on the scale of 12 months.
1148
01:00:22.938 --> 01:00:26.610
<v SPEAKER_01>But the amount of increase up till the end of the decade is extremely limited.
1149
01:00:26.660 --> 01:00:27.171
<v SPEAKER_01>Yes.
1150
01:00:27.221 --> 01:00:29.773
<v SPEAKER_01>Production could be higher next year than what people are forecasting.
1151
01:00:29.823 --> 01:00:32.975
<v SPEAKER_01>But production in 2030 is not going to be significantly higher than what people are forecasting.
1152
01:00:33.025 --> 01:00:36.057
<v SPEAKER_03>Unless the entire supply chain ramps up production very quickly.
1153
01:00:36.107 --> 01:00:37.579
<v SPEAKER_03>I mean, we're already in the middle of 26.
1154
01:00:37.629 --> 01:00:39.240
<v SPEAKER_03>So there's, you know, only...
1155
01:00:40.155 --> 01:00:42.346
<v SPEAKER_03> Not that many years until the end of the decade.
1156
01:00:42.396 --> 01:00:48.239
<v SPEAKER_03>And given the lead times, let's say you place an enormous order for tools today, right?
1157
01:00:48.719 --> 01:00:49.941
<v SPEAKER_03>And you're looking at,
1158
01:00:50.019 --> 01:00:54.130
<v SPEAKER_03>let's say, 18 months to get those tools, you're already into basically 28.
1159
01:00:54.941 --> 01:00:56.302
<v SPEAKER_03>And from that point on,
1160
01:00:56.342 --> 01:00:57.953
<v SPEAKER_03>if you have to build a new shell,
1161
01:00:58.003 --> 01:01:01.944
<v SPEAKER_03>build a new fab, I mean, you're basically looking at the end of the decade.
1162
01:01:01.964 --> 01:01:07.075
<v SPEAKER_01>I think it'll be interesting to discuss the partnership you guys have with Elon on TerraFab.
1163
01:01:07.787 --> 01:01:09.009
<v SPEAKER_01>What's going on there?
1164
01:01:10.903 --> 01:01:17.747
<v SPEAKER_03> Well, I think, so Ilan's publicly talked about his desire to build a fab.
1165
01:01:17.807 --> 01:01:20.069
<v SPEAKER_03> We either build the terafab or we
1166
01:01:20.089 --> 01:01:21.311
<v SPEAKER_01> don't have the chips.
1167
01:01:22.390 --> 01:01:24.541
<v SPEAKER_01>And we need the chips, so we're going to build the terafab.
1168
01:01:24.591 --> 01:01:25.532
<v SPEAKER_03>Sort of the same thinking,
1169
01:01:25.552 --> 01:01:25.842
<v SPEAKER_03>you know,
1170
01:01:25.892 --> 01:01:31.684
<v SPEAKER_03>I think he's seeing just a Enormous increase in demand for silicon,
1171
01:01:32.005 --> 01:01:33.866
<v SPEAKER_03>for compute and for memory.
1172
01:01:34.646 --> 01:01:38.549
<v SPEAKER_03>And I think he came to the conclusion that his own businesses are going to require
1173
01:01:38.569 --> 01:01:39.569
<v SPEAKER_03>a lot of silicon.
1174
01:01:40.371 --> 01:01:45.994
<v SPEAKER_03>And so he thought maybe he should just do it all on his own.
1175
01:01:46.455 --> 01:01:52.959
<v SPEAKER_03>Unlike building a car, for example, this is such an intricate and complicated process.
1176
01:01:53.160 --> 01:01:58.405
<v SPEAKER_03> We thought we could work together to help accelerate his Bringing up his fab.
1177
01:01:59.486 --> 01:02:02.153
<v SPEAKER_01>But because of the bottleneck at the tool level,
1178
01:02:02.587 --> 01:02:06.509
<v SPEAKER_01>it seems like the net amount of silicon in the world won't increase.
1179
01:02:06.789 --> 01:02:09.790
<v SPEAKER_01>It's just that maybe if somebody were to start a new fab,
1180
01:02:09.810 --> 01:02:13.802
<v SPEAKER_01>they would get access to guaranteed supply in a way that they wouldn't have
1181
01:02:13.852 --> 01:02:16.563
<v SPEAKER_01>if they're working with another person's foundry.
1182
01:02:16.613 --> 01:02:18.034
<v SPEAKER_03>It's actually not just tools.
1183
01:02:18.074 --> 01:02:23.236
<v SPEAKER_03>I mean, a fab does require a lot of power, a lot of water, like a lot of consumables.
1184
01:02:23.936 --> 01:02:25.325
<v SPEAKER_03>There's many other tools.
1185
01:02:25.824 --> 01:02:27.345
<v SPEAKER_03> Input variables as well.
1186
01:02:27.665 --> 01:02:28.956
<v SPEAKER_01> But those can be scaled in the way that
1187
01:02:29.006 --> 01:02:29.776
<v SPEAKER_03> tools cannot.
1188
01:02:29.826 --> 01:02:30.826
<v SPEAKER_03>Yeah.
1189
01:02:31.267 --> 01:02:32.989
<v SPEAKER_03>Some more than others, but yes.
1190
01:02:34.029 --> 01:02:37.731
<v SPEAKER_03>But yes, in one sense, yes, we need a lot more equipment.
1191
01:02:38.191 --> 01:02:39.071
<v SPEAKER_03>But it is true.
1192
01:02:39.091 --> 01:02:46.091
<v SPEAKER_03>I mean, we also need a lot more just raw fab space, raw clean room capacity.
1193
01:02:46.495 --> 01:02:48.456
<v SPEAKER_01>So if you think of a foundry like Intel,
1194
01:02:48.476 --> 01:02:52.878
<v SPEAKER_01>which has to Build these expensive facilities, buy expensive tools.
1195
01:02:52.898 --> 01:02:57.783
<v SPEAKER_01>I wonder what you think the economics of that fundamentally could look like,
1196
01:02:57.823 --> 01:03:00.936
<v SPEAKER_01>whether it could get more economical, whether it could scale faster.
1197
01:03:00.986 --> 01:03:06.412
<v SPEAKER_03>Like I described earlier, this is an extremely capital heavy business.
1198
01:03:07.530 --> 01:03:12.327
<v SPEAKER_03> And if you look at the, if you just plot the, you know, how much does it cost to build a fab?
1199
01:03:12.377 --> 01:03:13.810
<v SPEAKER_03>And if you just over the last,
1200
01:03:13.860 --> 01:03:19.087
<v SPEAKER_03>I don't know, 20, 30, 40 years, I think it's like doubling every four to five years.
1201
01:03:19.568 --> 01:03:20.730
<v SPEAKER_03>Even inside the fab,
1202
01:03:20.750 --> 01:03:22.272
<v SPEAKER_03>if you look at the cost to,
1203
01:03:22.292 --> 01:03:23.413
<v SPEAKER_03>So if you do lithography,
1204
01:03:23.433 --> 01:03:25.394
<v SPEAKER_03>which is the most expensive module,
1205
01:03:25.934 --> 01:03:26.934
<v SPEAKER_03>just patterning,
1206
01:03:27.095 --> 01:03:31.228
<v SPEAKER_03>that itself is doubling like more than that, at more than that rate, right?
1207
01:03:31.278 --> 01:03:32.278
<v SPEAKER_03>So like today,
1208
01:03:32.438 --> 01:03:34.940
<v SPEAKER_03>a high NA UV scanner costs like,
1209
01:03:35.120 --> 01:03:40.667
<v SPEAKER_03>and all its associated equipment, $400 million, right?
1210
01:03:41.107 --> 01:03:42.298
<v SPEAKER_03>And so what does that mean?
1211
01:03:42.348 --> 01:03:44.190
<v SPEAKER_03>If that rate were to continue,
1212
01:03:44.570 --> 01:03:47.313
<v SPEAKER_03>if you just draw the line and say, okay,
1213
01:03:47.673 --> 01:03:49.305
<v SPEAKER_03>does that mean like four years from now,
1214
01:03:49.355 --> 01:03:53.419
<v SPEAKER_03>like cost of patterning is going to be like $800 billion, right?
1215
01:03:53.519 --> 01:03:57.252
<v SPEAKER_03>Doesn't, you know, $800 million, it doesn't really make sense, right?
1216
01:03:57.302 --> 01:04:01.887
<v SPEAKER_03>I think that a very interesting thought exercise to do is to say,
1217
01:04:03.189 --> 01:04:09.280
<v SPEAKER_03>Are there things that could be just very radically different that we could do today
1218
01:04:09.846 --> 01:04:13.758
<v SPEAKER_03>that we perhaps couldn't do 20 years ago.
1219
01:04:14.138 --> 01:04:19.220
<v SPEAKER_03>This is a very risk-averse industry for very good reason, for exactly that reason, right?
1220
01:04:19.260 --> 01:04:24.901
<v SPEAKER_03>You put in like tens of billions of dollars and you really don't want to take any risks.
1221
01:04:25.041 --> 01:04:29.472
<v SPEAKER_03>So you want to keep doing things the way they've been done for literally decades.
1222
01:04:29.522 --> 01:04:33.522
<v SPEAKER_03>And this is not just true of semiconductors, but like everything really.
1223
01:04:33.623 --> 01:04:37.012
<v SPEAKER_03>But if you've just kept on doing that for decade upon decade,
1224
01:04:37.553 --> 01:04:41.626
<v SPEAKER_03>Many things just become like, you know, you just become indoctrinated, right?
1225
01:04:41.676 --> 01:04:42.056
<v SPEAKER_03>And I mean,
1226
01:04:42.076 --> 01:04:45.458
<v SPEAKER_03>there are engineers who probably work at Intel who are new,
1227
01:04:46.379 --> 01:04:46.929
<v SPEAKER_03>who just,
1228
01:04:46.979 --> 01:04:51.412
<v SPEAKER_03>you know, come in and they're taught, this is how the fab, this is the process flow.
1229
01:04:51.462 --> 01:04:53.693
<v SPEAKER_03>And they just take that as gospel, right?
1230
01:04:53.743 --> 01:04:55.243
<v SPEAKER_03>That's just how it is done.
1231
01:04:55.835 --> 01:04:58.891
<v SPEAKER_03> But is that really the best way to build a chip today?
1232
01:05:00.179 --> 01:05:02.100
<v SPEAKER_03>It's a really valid question.
1233
01:05:02.340 --> 01:05:03.962
<v SPEAKER_01>I'm very curious what you're hinting at,
1234
01:05:03.982 --> 01:05:05.733
<v SPEAKER_01>because it could be anything from,
1235
01:05:05.783 --> 01:05:06.253
<v SPEAKER_01>you know,
1236
01:05:06.303 --> 01:05:10.367
<v SPEAKER_01>we can figure out ways in which you use fewer lithopasses and economize
1237
01:05:10.427 --> 01:05:14.410
<v SPEAKER_01>on this expensive component to, like, maybe we need to rethink the transistor.
1238
01:05:14.430 --> 01:05:15.430
<v SPEAKER_01>Yeah.
1239
01:05:16.411 --> 01:05:18.311
<v SPEAKER_01> What is the level of?
1240
01:05:18.431 --> 01:05:20.712
<v SPEAKER_03>I think all of the above.
1241
01:05:21.073 --> 01:05:24.334
<v SPEAKER_03>Transistor architecture and evolving,
1242
01:05:25.875 --> 01:05:29.026
<v SPEAKER_03>just a silicon transistor has continued to evolve over 30,
1243
01:05:29.076 --> 01:05:33.158
<v SPEAKER_03>40 years, and that will continue.
1244
01:05:33.178 --> 01:05:36.940
<v SPEAKER_03>You've seen the evolution from the planar transistor to FinFETs
1245
01:05:36.980 --> 01:05:38.961
<v SPEAKER_03>to now gate all-around transistors.
1246
01:05:39.441 --> 01:05:40.441
<v SPEAKER_03>There'll be more.
1247
01:05:40.501 --> 01:05:41.890
<v SPEAKER_03>That roadmap is pretty...
1248
01:05:42.402 --> 01:05:45.180
<v SPEAKER_03> You know, it exists and it's pretty well defined.
1249
01:05:45.386 --> 01:05:47.053
<v SPEAKER_03>A lot of people working on it.
1250
01:05:47.929 --> 01:05:52.514
<v SPEAKER_03>But there's things like, you know, do you really need a clean room today?
1251
01:05:53.135 --> 01:05:53.506
<v SPEAKER_03>Right?
1252
01:05:53.556 --> 01:05:54.556
<v SPEAKER_03>Do you need...
1253
01:05:55.087 --> 01:06:01.773
<v SPEAKER_03> The infrastructure to be as sophisticated, as complex as it is today.
1254
01:06:02.134 --> 01:06:06.998
<v SPEAKER_01>Surely one can run an experiment where people are eating hamburgers
1255
01:06:07.018 --> 01:06:10.882
<v SPEAKER_01>and smoking cigars in the research lab and see what happens to yield.
1256
01:06:12.964 --> 01:06:19.449
<v SPEAKER_03> That would be a great experiment to run, but no incumbent like Intel or TSMC or Samsung.
1257
01:06:19.790 --> 01:06:22.679
<v SPEAKER_03>I mean, nobody would want to just willingly do that.
1258
01:06:23.233 --> 01:06:29.338
<v SPEAKER_03>So that's what I meant really by this, it's a very risk averse business for good reason.
1259
01:06:29.718 --> 01:06:34.723
<v SPEAKER_03>Every one day lost in productivity is like, I don't know how many dollars, right?
1260
01:06:34.923 --> 01:06:39.256
<v SPEAKER_01> But you save so much money and not having to build clean rooms in the future.
1261
01:06:37.865 --> 01:06:41.107
<v SPEAKER_03> But it's really the fear of the unknown, right?
1262
01:06:41.167 --> 01:06:44.048
<v SPEAKER_03>So nobody is going to willingly take that risk.
1263
01:06:44.348 --> 01:06:50.611
<v SPEAKER_03>But that's why I think sometimes it's good to sort of just start with a clean slate
1264
01:06:50.891 --> 01:06:52.251
<v SPEAKER_03>and rethink everything.
1265
01:06:52.452 --> 01:06:58.655
<v SPEAKER_03> And it's like, okay, These things, same thing applies to chip design, by the way.
1266
01:06:59.436 --> 01:07:06.260
<v SPEAKER_03>Many of the ways we do CPU design were probably locked in 30 years ago.
1267
01:07:06.700 --> 01:07:10.562
<v SPEAKER_03>Does that mean it's smart to still do it the same way?
1268
01:07:11.343 --> 01:07:12.684
<v SPEAKER_03>Probably not.
1269
01:07:13.724 --> 01:07:15.866
<v SPEAKER_03>But this is a very complex problem.
1270
01:07:16.886 --> 01:07:19.928
<v SPEAKER_03>Chip design is easy to, it's fairly low,
1271
01:07:22.830 --> 01:07:26.592
<v SPEAKER_03> I guess the capacity to take risk is maybe higher.
1272
01:07:27.533 --> 01:07:29.014
<v SPEAKER_03>This one, less so.
1273
01:07:29.695 --> 01:07:35.739
<v SPEAKER_03>But given where the economics is today, I think it's a very valid question to ask.
1274
01:07:36.799 --> 01:07:38.951
<v SPEAKER_03>Maybe there's a smarter way to do this.
1275
01:07:39.001 --> 01:07:39.551
<v SPEAKER_01>To close out,
1276
01:07:39.601 --> 01:07:43.194
<v SPEAKER_01>maybe we'll start off at the same question we began the interview with,
1277
01:07:43.244 --> 01:07:43.834
<v SPEAKER_01>which is,
1278
01:07:43.884 --> 01:07:48.707
<v SPEAKER_01>how does Intel respond to this crazy AI demand that's incoming
1279
01:07:48.887 --> 01:07:50.220
<v SPEAKER_01>and has already arrived?
1280
01:07:51.898 --> 01:07:54.180
<v SPEAKER_01>It sounds like what Intel ought to do if
1281
01:07:54.221 --> 01:07:57.724
<v SPEAKER_01>the ultimate bottleneck is you guys already have these foundries,
1282
01:07:57.744 --> 01:08:00.277
<v SPEAKER_01>you guys already have the ability to expand these foundries.
1283
01:08:00.327 --> 01:08:06.413
<v SPEAKER_01>But what you will eventually lack is the tools from upstream in the supply chain
1284
01:08:06.913 --> 01:08:09.802
<v SPEAKER_01>to just raise as much capital as possible right now.
1285
01:08:10.517 --> 01:08:14.295
<v SPEAKER_01>The same way that NVIDIA has locked down memory and other components
1286
01:08:14.521 --> 01:08:19.132
<v SPEAKER_01>for reportedly hundreds of billions of dollars worth of commitments that it's made.
1287
01:08:19.506 --> 01:08:21.158
<v SPEAKER_01>Intel should maybe do the same thing,
1288
01:08:21.208 --> 01:08:25.913
<v SPEAKER_01>make all these commitments so that as over the coming years,
1289
01:08:26.434 --> 01:08:26.874
<v SPEAKER_01>the U.S.
1290
01:08:26.914 --> 01:08:30.238
<v SPEAKER_01>is in good position to have the bulk of semiconductor manufacturing at
1291
01:08:30.258 --> 01:08:32.480
<v SPEAKER_01>the most advanced levels happening here.
1292
01:08:32.680 --> 01:08:35.431
<v SPEAKER_03> You're saying we should be buying a lot more tools, right?
1293
01:08:35.481 --> 01:08:35.731
<v SPEAKER_01>Yeah.
1294
01:08:35.781 --> 01:08:37.772
<v SPEAKER_01>Because it sounds like it's just like, well,
1295
01:08:37.822 --> 01:08:38.342
<v SPEAKER_01>in a couple of years,
1296
01:08:38.382 --> 01:08:40.272
<v SPEAKER_01>otherwise you'd just be in a position where you're like,
1297
01:08:40.322 --> 01:08:42.933
<v SPEAKER_01>oh man, we're going to be making trillions of dollars right now.
1298
01:08:42.983 --> 01:08:44.761
<v SPEAKER_01>But all the tools are in Taiwan.
1299
01:08:44.944 --> 01:08:45.394
<v SPEAKER_03>Yes.
1300
01:08:45.444 --> 01:08:47.815
<v SPEAKER_03>I mean, no, that's a very, very valid question.
1301
01:08:47.865 --> 01:08:52.587
<v SPEAKER_03>Had we known what we know today, we would have bought, invested more like a year ago.
1302
01:08:52.966 --> 01:08:56.188
<v SPEAKER_03>Knowing what we know now, I think we'll be investing more.
