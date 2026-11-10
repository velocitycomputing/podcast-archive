---
record_id: "podcast:99683f49-84fa-4b7d-bbda-e4c88b987a7c"
episode_id: 99683f49-84fa-4b7d-bbda-e4c88b987a7c
title: A Potentially Historic AI Breakthrough
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/a-potentially-historic-ai-breakthrough/99683f49-84fa-4b7d-bbda-e4c88b987a7c"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/a-potentially-historic-ai-breakthrough/99683f49-84fa-4b7d-bbda-e4c88b987a7c"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-18
played_at: "2026-10-18T12:00:00Z"
play_count: 1
duration_seconds: 1380
source: pocketcasts-history-browser
played_label: October 18
history_order: 35
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 31fab933c72311dbfbc4acaa5b92c84d3c8650318fe0acd1866ae16852b8c0ea
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

Nick Cammarata’s essay “Neural Networks Are Already Clean” is presented as a potentially major mechanistic-interpretability breakthrough: the claim is that neural networks are far more legible than the field had believed, and that years of “superposition” or “cramming” pessimism may have resulted from bad tools, misleading visualizations, and studying an old messy model, especially Google’s 2014 Inception v1. The episode names Chris Olah, Rohun, Eliezer Yudkowsky, Neel Nanda, Liv Boote, Steven Casper, Christian, OpenAI, Google DeepMind, Anthropic, GPT-2, GPT-4, Gopher 3, and Opus 55, and frames the claim against a six-year arc from early excitement to despair: in 2023, OpenAI’s automated interpretability work reportedly found only about 2% of GPT-2 neurons clean, while Cammarata now says modern agentic tools and better methods show the vast majority of detectors in models up to trillions of parameters are readable, with about nine out of ten detectors in a modern OpenAI model having one main job. Key data points include Inception v1’s last-layer readability moving from about 5% with old tools to about 50% with a better “microscope,” about 70% when retrained with modern settings, and about 99% when rebuilt with a modern design at the same size and data; dog-ear detectors across models about 300 times apart in size; and a Gopher 3 example where detectors for “lost property” and “honesty” appear to push the model toward returning a found wallet. Cammarata argues that famous “tangled” detectors, such as one firing for cat faces and car fronts, may actually reflect a single underlying concept—pointed shapes—rather than arbitrary cramming, and that deception may be readable in a model’s circuitry because the model’s own downstream processes must access it; responses range from OpenAI figures calling it one of the most important days in deep learning history to Neel Nanda saying it is not a major update, Liv Boote arguing the essay attacks a narrower version of superposition than researchers actually hold, Steven Casper calling it hype, and Yudkowsky remaining dismissive.

The actionable takeaway is to treat this as a high-priority, testable hypothesis rather than a settled safety breakthrough: read Cammarata’s original essay, wait for the full technical paper, and look for independent replication of the readability claims, especially whether “one main job” is defined too generously and whether readable detectors actually combine into readable decisions. Useful research leads include testing whether branching detectors trace back to one origin in order, whether rare facts ride on related machinery rather than arbitrary superposition, whether readability scales to frontier models, and whether interpretability can reveal deceptive planning rather than only explain outputs after the fact. For decisions, the user should calibrate both doomer panic and utopian excitement, watch for independent verification before changing risk assumptions, and consider practical near-term uses such as debugging why a model behaves sketchily, auditing model reasoning, and improving safety monitoring. Follow-up questions should include: Is cramming refuted or merely redefined? Do readable parts add up to a readable whole? Can we become a reliable reader of the model’s own circuitry? Does this make alignment a “normal science” with checkable progress, or is the biggest gap still understanding how many readable components produce complex behavior?

## Transcript

[00:00:00] When it comes to AI safety, the news
[00:00:02] lately has been a little bit dreary, or
[00:00:04] at least I should say the headlines have
[00:00:06] been. We've been living through a new
[00:00:07] wave of panic and concern, driven in
[00:00:09] part by the reality that models are
[00:00:10] getting more capable and closer to what
[00:00:12] many view as key inflection points. It's
[00:00:14] also being driven, however, by the
[00:00:15] juiciness of the scare headlines. And
[00:00:17] yet the most interesting news in that
[00:00:19] area this week might be very good
[00:00:21] indeed.
[00:00:22] The AI Daily Brief is a daily podcast
[00:00:24] and video about the most important news
[00:00:26] and discussions in AI.
[00:00:28] Now, it's not all that often that a
[00:00:30] 65-minute
[00:00:32] densely technical web article becomes
[00:00:34] the thing that everyone was talking
[00:00:36] about. And yet that's exactly what
[00:00:38] happened at the end of this week with
[00:00:40] Nick Cammarata's Neural Networks Are
[00:00:42] Already Clean. I, like many people,
[00:00:44] noticed it when OpenAI's Rohun posted,
[00:00:46] "When Nick told me that he had some
[00:00:48] interpretability breakthroughs, he was
[00:00:50] uh underselling it. I think this may be
[00:00:52] remembered as a major moment in
[00:00:54] scientific history. News so good even
[00:00:56] Eliezer Yudkowsky will have to lower his
[00:00:58] P(doom). We can start making alignment
[00:01:00] into a normal science."
[00:01:02] Nick summed up his article this way,
[00:01:04] "Interpretability might be the most
[00:01:06] important scientific problem in the
[00:01:07] world right now, as I don't think we can
[00:01:09] solve alignment if we don't know what
[00:01:11] we're building. I think I have good news
[00:01:13] about it."
[00:01:15] "I co-authored early work in mechanistic
[00:01:17] interpretability at OpenAI and came away
[00:01:19] pessimistic because neural networks
[00:01:21] appear to fold into arbitrary tangled
[00:01:22] knots. Years later, I started OpenAI's
[00:01:25] first large-scale automated
[00:01:26] interpretability project, finding about
[00:01:28] 2% of neurons legible with the primitive
[00:01:30] tools we had. With modern agentic tools
[00:01:33] and a much closer look, the picture
[00:01:35] looks totally different. The vast
[00:01:37] majority in models up to trillions of
[00:01:39] parameters are legible and their
[00:01:40] circuits beautiful. Many famous examples
[00:01:43] of tangled neurons turned out to be
[00:01:45] misunderstood. The roadblocks I expected
[00:01:47] mostly aren't there. I now think
[00:01:49] ambitious interpretability will be
[00:01:51] solved by the time we need it most and
[00:01:53] possibly quite soon as automated
[00:01:55] scientists keep improving. It may be a
[00:01:57] bitter lesson for interpretability. The
[00:02:00] simple thing at absurd scale works.
[00:02:03] So, the promise here is that we might
[00:02:05] actually be able to understand what's
[00:02:07] going on inside the processes of AI,
[00:02:09] something that so far we haven't. Today,
[00:02:11] we're going to try to do a
[00:02:12] understandable version of Nick's densely
[00:02:15] technical paper, sharing of course both
[00:02:17] the excited and the skeptical responses
[00:02:19] to it. Hopefully, you come away
[00:02:21] understanding why this could be a big
[00:02:22] moment and what cautions we still need
[00:02:24] to have.
[00:02:25] One of the uncomfortable facts
[00:02:27] underneath all of AI is that even the
[00:02:29] folks building it don't really know how
[00:02:31] it works on the inside. The systems are
[00:02:33] trained, not programmed. You set up the
[00:02:35] conditions and the model learns its own
[00:02:37] way of doing things, spread across
[00:02:38] billions of numbers. In AI researcher
[00:02:41] Chris Olah's phrase, AI is grown more
[00:02:43] than built.
[00:02:44] So, because we can't read these systems,
[00:02:47] the way we check them today is basically
[00:02:48] a very elaborate exam. We ask questions,
[00:02:51] red team, and grade the answers. While
[00:02:53] that's useful, it only covers what we
[00:02:55] thought to ask, and it also introduces a
[00:02:57] set of problems, like the model behaving
[00:03:00] well not because that's what it
[00:03:02] otherwise would do, but because it knows
[00:03:04] it's being watched. This is coming up
[00:03:06] more and more. Ironically, in some
[00:03:08] recent tests of models like Opus 55,
[00:03:10] researchers were concerned when they saw
[00:03:12] the models cheating less. The big
[00:03:14] drop-off in cheating behavior brought up
[00:03:16] the question, did the model just shift
[00:03:18] away from cheating or did it realize
[00:03:20] that the humans watching it would think
[00:03:21] cheating is bad and so it disguised that
[00:03:23] behavior?
[00:03:25] What this means is that in the addition
[00:03:27] to the race for capability, there's also
[00:03:29] another race to reach interpretability,
[00:03:32] to understand what's going on with AI
[00:03:34] before the models reach what Anthropic
[00:03:35] called an overwhelming level of power.
[00:03:38] If you've followed the field, the story
[00:03:40] of the last 6 years went from excitement
[00:03:42] to something closer to despair.
[00:03:44] In the first phase, from about 2017 to
[00:03:46] 2020, teams like Chris Olah's team,
[00:03:49] which included Nick, mapped image AIs
[00:03:51] detector by detector. And it looked at
[00:03:53] first like you could read a neural
[00:03:54] network like code. But then between 2020
[00:03:57] and 2023, they started to find a
[00:03:59] problem. Many of these detectors seem to
[00:04:01] fire for unrelated things, meaning that
[00:04:04] we couldn't really understand exactly
[00:04:06] what was going on even though at first
[00:04:07] it appeared we could. The field settled
[00:04:09] on an explanation for this that we'll
[00:04:10] get into in just a minute. When Nick's
[00:04:12] team at Open AI used GPT-4 to explain
[00:04:15] GPT-2's detectors in 2023, only about 2%
[00:04:18] came out clean. I actually interpretable
[00:04:21] in the way that we thought. Between 2023
[00:04:23] and 2025, a bunch of different
[00:04:25] workaround strategies were tried, some
[00:04:27] of which showed some progress, but which
[00:04:28] never really produced many wins.
[00:04:31] By 2025, many researchers wondered if
[00:04:33] these systems were just too tangled to
[00:04:35] read. The mood, in Nick's words, was
[00:04:38] that ambitious interpretability looked
[00:04:39] like a quote, "incredibly hard problem,
[00:04:42] maybe too hard to solve in time to
[00:04:44] matter."
[00:04:45] Which is why this essay is hitting so
[00:04:47] hard. It says, in short, that the inside
[00:04:50] of AI is mostly readable already and
[00:04:52] that we've been looking at it wrong.
[00:04:54] And there are reasons to be excited.
[00:04:56] This comes from an insider who helped
[00:04:58] create the theory that he's now taking
[00:04:59] apart. He shows experiments that could
[00:05:01] have proven him wrong and his evidence
[00:05:03] suggests that bigger models are easier
[00:05:04] to read, which is basically the opposite
[00:05:06] of what everyone feared. Then again, not
[00:05:08] everyone agrees. The head of
[00:05:10] interpretability at Google DeepMind,
[00:05:11] Neel Nanda, for example, said that the
[00:05:13] work was interesting, but quote, "not a
[00:05:16] significant update to the big picture."
[00:05:18] So, let's try to wrap our heads around
[00:05:19] the quick version of the idea. As
[00:05:21] mentioned before, AI isn't written like
[00:05:23] normal software. It's millions of tiny
[00:05:26] detectors wired together that learn
[00:05:27] their jobs on their own. Researchers
[00:05:29] call these neurons. One might light up
[00:05:32] for edges, another for the color red,
[00:05:34] another for a dog's ear.
[00:05:35] The dream of the interpretability field
[00:05:37] is simple. Work out what each detector
[00:05:39] does and then you can read what the AI
[00:05:41] is doing just the way you'd read code.
[00:05:44] One of the most famous detectors shows
[00:05:46] why some of them made no sense. That
[00:05:48] detector lit up for cat faces, but also
[00:05:51] for the front of cars. Cats and cars, of
[00:05:54] course, have nothing to do with each
[00:05:55] other. So, for years, this one detector
[00:05:57] was the go-to proof that AI's insides
[00:05:59] are scrambled. It shows up in the
[00:06:01] field's most read papers, including ones
[00:06:03] Nick Co-wrote.
[00:06:04] The explanation the whole field landed
[00:06:06] on was cramming, or what researchers
[00:06:09] called superposition. The idea was that
[00:06:12] an AI has more ideas to store than it
[00:06:14] has detectors. So, it shares detectors
[00:06:16] between ideas. It works best when those
[00:06:19] ideas rarely show up together, like
[00:06:21] Christmas lights and pool floats in the
[00:06:22] same box.
[00:06:24] And if that's how it works, the
[00:06:25] detectors themselves are meaningless.
[00:06:27] So, researchers built unscramblers,
[00:06:29] second AIs trained to pull the ideas
[00:06:31] back apart, and studied those instead. A
[00:06:34] lot of the field's money and effort went
[00:06:35] into that for years. Nick was there for
[00:06:37] this. In 2019, he found one of the first
[00:06:39] examples that seemed to prove cramming
[00:06:41] and helped name it.
[00:06:43] In this new research, however, Nick went
[00:06:45] back to this detector and asked, "If I
[00:06:47] couldn't use the words cat or car, how
[00:06:49] would I describe it?"
[00:06:51] The answer took him about 5 seconds.
[00:06:53] It's a V detector.
[00:06:55] Pointed shapes switch it on. A fox's
[00:06:57] snout, a cat's face, the front of a car,
[00:07:00] a bullet train's nose, a candle flame,
[00:07:03] and a martini glass. Round shapes, like
[00:07:06] golf balls or a clock face, switch it
[00:07:07] off. Nick wrote, "Why would an arbitrary
[00:07:10] mixture of cats and cars need to connect
[00:07:12] so strongly to a flame? It was never two
[00:07:15] unrelated things. It was one idea we
[00:07:17] hadn't recognized."
[00:07:18] Nick's claim is more or less that most
[00:07:20] of the scrambling was never in the AI
[00:07:22] itself, but in the microscopes we were
[00:07:23] using to look at it. He proposed three
[00:07:26] causes, all of which are fixable. The
[00:07:28] tools for picturing what a detector
[00:07:29] wants were blurry and misleading. The
[00:07:31] early image AI the field studied from
[00:07:33] 2014 was built in a way that made it
[00:07:35] learn messily. When you retrain a modern
[00:07:37] design of the same size, about 99% of
[00:07:39] its last layer detectors are readable.
[00:07:41] And finally, some detectors branch. One
[00:07:43] that starts on the letters IY grows to
[00:07:46] DIY and then to do it yourself. That
[00:07:48] looks random at the end, but obvious if
[00:07:50] you watch it grow.
[00:07:51] And it turns out it's not just old image
[00:07:53] models. In a modern OpenAI model, about
[00:07:56] nine out of 10 detectors turn out to
[00:07:58] have one main job. Compare that again
[00:08:00] with that 2023 OpenAI project that could
[00:08:03] only explain about 2% of detectors in
[00:08:05] GPT-2. Now, keep in mind these are early
[00:08:08] counts, they are self-reported. The
[00:08:10] exact number depends on where you draw
[00:08:11] the lines and the full technical paper
[00:08:13] isn't out yet. What this opens up is the
[00:08:15] ability to check AI's reasoning, not
[00:08:17] just judge it by its answers.
[00:08:19] The example on screen comes from a model
[00:08:21] with trillions of parameters, Gopher 3.
[00:08:23] When asked what to do with a found
[00:08:24] wallet full of cash, you can watch
[00:08:26] detectors for lost property and honesty
[00:08:28] light up and push it to say return. And
[00:08:30] the point then about deception is, if
[00:08:32] all we can do is read the answers, the
[00:08:34] AI can hide a plan from us. But since
[00:08:37] the plan has to be readable by the AI's
[00:08:39] own wiring to work, if we can read that
[00:08:41] wiring as well, it's not just the
[00:08:43] output, but the plan that's readable to
[00:08:44] us as well.
[00:08:46] And this is what got Rylan so excited.
[00:08:48] The idea that alignment could become a
[00:08:49] normal science in his words, with
[00:08:51] steadily checkable progress instead of
[00:08:53] guesswork.
[00:08:54] To read a lot of the responses to this
[00:08:55] on X, they are, in a word, breathless.
[00:08:58] And yet even Nick himself calls it a
[00:09:00] working hypothesis and puts himself at
[00:09:02] about 85% sure.
[00:09:04] Other researchers are a bit less
[00:09:05] convinced.
[00:09:07] So, what we're going to do now is go
[00:09:08] quickly through a bit more of what's in
[00:09:10] Nick's paper and some of the responses
[00:09:12] and objections that come up along the
[00:09:13] way. The first thing we're going to dive
[00:09:15] deeper on is whether the experts got it
[00:09:17] wrong.
[00:09:18] Basically, if the inside of AI was
[00:09:20] readable all along, how did a field full
[00:09:22] of brilliant people miss it? Nick's
[00:09:23] answer, as we got a preview of, is that
[00:09:25] three mistakes stacked on top of each
[00:09:27] other.
[00:09:27] Now, from this point I should say,
[00:09:29] you're likely to get a lot more by
[00:09:31] watching this episode, which you can do
[00:09:32] on YouTube or on Spotify, or just by
[00:09:34] following along on Nick's paper or my
[00:09:36] interpretation presentation, both of
[00:09:37] which will be linked in the show notes.
[00:09:39] In 2019, Nick was building one of the
[00:09:41] first tools to look inside an image AI.
[00:09:44] As he was doing so, he saw a car
[00:09:45] detector feeding into four dog
[00:09:47] detectors. He took it to colleagues and
[00:09:49] they concluded that AI was tucking car
[00:09:51] inside the dog detector, a hiding place
[00:09:53] to read back out later.
[00:09:55] That became one of the field's first
[00:09:56] examples of cramming. Nick even said in
[00:09:58] the essay, "It was the only one we
[00:10:00] showed and the only one I ever saw."
[00:10:02] When Nick rechecked it, he found that
[00:10:04] two of those detectors are just car
[00:10:06] detectors, but the other two detect a
[00:10:08] pose, i.e., which way something faces
[00:10:10] the camera.
[00:10:11] Cars and dogs share poses. The AI, in
[00:10:14] fact, has more than 100 of these pose
[00:10:15] detectors. Nothing was hidden. But
[00:10:18] because the cramming story felt
[00:10:19] intuitive, Nick said it didn't prompt
[00:10:21] diving more into the tools.
[00:10:23] The second mistake was the microscope
[00:10:25] itself.
[00:10:26] One key tool asks the AI to draw picture
[00:10:28] a detector most wants to see.
[00:10:30] In short, Nick found that the drawing
[00:10:32] tool cheated. It took the easiest path
[00:10:34] to make the detector fire, and after a
[00:10:36] few small fixes, the drawings matched
[00:10:37] the photos.
[00:10:39] As Nick put it, same neurons, better
[00:10:40] microscope.
[00:10:42] The third mistake was that the AI that
[00:10:43] people were studying had a learning
[00:10:45] problem. That was Inception v1, which
[00:10:47] was Google's 2014 image model. Its last
[00:10:50] layer was the field's main evidence that
[00:10:51] AI is unreadable. Nick estimates that 5%
[00:10:54] of its detectors were readable with the
[00:10:55] tools of the time. Fix the microscope
[00:10:57] and the same model is about 50%
[00:10:59] readable, and when you retrain it with
[00:11:01] modern settings, about 70%.
[00:11:03] Build a modern design with the same size
[00:11:04] and same data, and the readability jumps
[00:11:06] to 99%.
[00:11:08] So, why did nobody go back and check?
[00:11:10] Nick argues it's because of how the
[00:11:11] cramming theory works. If you believe a
[00:11:13] detector is crammed, a confusing
[00:11:15] detector is a dead end, and you stop
[00:11:17] looking. Every time detectors came back
[00:11:19] clean, the theory moved to somewhere
[00:11:20] where nobody had checked yet. The faint
[00:11:22] signals, the combination of detectors,
[00:11:24] the next layer. Nick calls it
[00:11:25] superposition of the gaps. Nick
[00:11:27] confessed, "For years, I was a staunch
[00:11:29] superposition believer." He now says it
[00:11:32] should have been the last explanation
[00:11:33] tried, not the default.
[00:11:35] But here we get some of the most serious
[00:11:36] pushback. Liv Boote is another
[00:11:38] interpretability researcher. Nick's
[00:11:40] essay cites her 2024 study of the same
[00:11:42] 2014 image AI.
[00:11:44] In a long thread, she argues that the
[00:11:46] essay attacks a narrower version of
[00:11:48] superposition than researchers actually
[00:11:49] hold. Her point is that superposition,
[00:11:52] or what we've been calling cramming on
[00:11:53] this episode, is about capacity. You
[00:11:56] store more ideas than you have detectors
[00:11:58] by giving each idea its own slightly
[00:11:59] different combination of them. Unrelated
[00:12:02] ideas make good examples because they
[00:12:03] rarely clash, but related ideas can be
[00:12:05] crammed, too. She also points out that
[00:12:08] there are only as many perfectly
[00:12:09] separate directions as detectors, but
[00:12:11] exponentially many nearly separate ones.
[00:12:13] She wrote, "I'd be very surprised if
[00:12:14] networks didn't use this capacity." Nick
[00:12:17] basically responded that he wasn't
[00:12:18] trying to say that AI never puts ideas
[00:12:20] together in a single detector, but that
[00:12:22] in general what he cares about is
[00:12:24] whether AI does the bad version of
[00:12:26] packing things arbitrarily so they can't
[00:12:27] be read. And that's what he said wasn't
[00:12:29] happening in the way that he thought it
[00:12:31] was.
[00:12:32] Google DeepMind's interpretability lead,
[00:12:33] Neel Nanda, said something similar to
[00:12:35] Liv, writing, "It seems to me like
[00:12:37] language models have far more facts and
[00:12:39] memorized things in them than they have
[00:12:40] neurons. I expect that weak neuron
[00:12:42] activations contain lots of semantic
[00:12:44] superpositiony info."
[00:12:46] Nick basically argued that if this is
[00:12:47] happening, it's happening very
[00:12:49] differently than the packing random
[00:12:50] unrelated things together that the field
[00:12:52] previously thought, and that instead, he
[00:12:55] predicted that the opposite would be
[00:12:56] true, where rare facts should ride on
[00:12:57] related machinery.
[00:12:59] Although those tests haven't been done,
[00:13:01] Nick argues that that is in fact
[00:13:02] testable.
[00:13:03] In fact, when asking why some detectors
[00:13:05] seem to do several things, Nick argued
[00:13:07] that it wasn't cramming, but in fact
[00:13:09] something called branching.
[00:13:11] Nick retrained an old image AI from
[00:13:13] scratch and watched a single detector
[00:13:14] take shape. It starts on yellow flower
[00:13:16] fields in photos that sometimes include
[00:13:18] a dog. Then it grows along each thing in
[00:13:20] those photos. Other nature scenes, green
[00:13:23] round things like tennis balls and
[00:13:24] fruit, dogs without flowers, and finally
[00:13:26] broccoli. By the end, the fields are
[00:13:28] nearly gone. This is branching, where
[00:13:31] each step is small and sensible, the
[00:13:32] opposite of cramming, where unrelated
[00:13:34] things get thrown together. And by the
[00:13:36] way, for each of these, there are many,
[00:13:37] many more examples in the main essay.
[00:13:39] I'm just cognizant of time and space in
[00:13:41] our own puny human brains. Still, going
[00:13:43] back to Liv's critiques, she argued that
[00:13:45] branching and cramming answer different
[00:13:47] questions, saying that branching is how
[00:13:49] a detector picked up several jobs, but
[00:13:51] cramming is how the information gets
[00:13:52] stored, and that you could have both at
[00:13:54] once.
[00:13:55] Nick's theory in the essay is that every
[00:13:57] branch traces back to one origin and
[00:13:59] grows out in order. That makes it easy
[00:14:01] to test and easy to prove wrong,
[00:14:03] although that work hasn't been done yet.
[00:14:05] One finding that flips the usual fear
[00:14:06] about AI getting bigger is that Nick is
[00:14:08] actually arguing that bigger AIs are
[00:14:10] easier to read.
[00:14:12] Nick's analogy is this: In a small town,
[00:14:15] asking for the financial district barely
[00:14:17] makes sense. There's a bank on one
[00:14:19] street and an accountant on another. In
[00:14:21] New York, on the other hand, the
[00:14:22] financial district is incredibly easy to
[00:14:24] spot. You know right where it is. His
[00:14:26] experiment involved dog ear detectors in
[00:14:28] three AIs that were about 300 times
[00:14:30] apart in size. The small one has very
[00:14:33] coarse dog detectors. The big one has
[00:14:35] very specific ones. So, in a small
[00:14:37] model, you have detectors for general
[00:14:39] dog, light and fluffy dog, or dark and
[00:14:41] shaggy dog. In the medium model, local
[00:14:43] branches emerge, the ear and the head of
[00:14:45] the dog turns into detectors for curly
[00:14:47] ears or ear neck and hair. And then, in
[00:14:50] the largest model, the branches converge
[00:14:52] and split. Head side ears, pale ears,
[00:14:54] wavy ears are all separate, and then
[00:14:56] move into things like smooth flaps,
[00:14:57] hanging ears, and long ears.
[00:14:59] Theoretically, then, there should be a
[00:15:00] precision to the detectors in larger
[00:15:02] models that makes them ultimately easier
[00:15:04] to read.
[00:15:05] Now, one of the other categories of
[00:15:06] pushback is that even all the terms that
[00:15:08] we're using in here are somewhat blurry
[00:15:10] rather than precise. For example, Neil
[00:15:13] from DeepMind argues that Nick's essay's
[00:15:15] bar for a detector doing one job is too
[00:15:18] generous. Instead, he said that he'd
[00:15:20] call, in his words, a fair few of those
[00:15:22] detectors actually scrambled. Nick
[00:15:24] acknowledges this and it brings up
[00:15:25] another point, which is that so far this
[00:15:27] is just Nick and his team doing this
[00:15:28] work with no one else having yet checked
[00:15:30] it. But let's say that Nick is right.
[00:15:32] What would that then change?
[00:15:34] Nick argues that clean doesn't mean that
[00:15:36] every detector matches a word we have.
[00:15:39] Instead, it means that the AI's parts
[00:15:40] are organized to be read by the AI
[00:15:42] itself.
[00:15:43] Every detector exists to be used by
[00:15:45] later detectors. So, the AI has already
[00:15:47] organized itself to be legible to its
[00:15:49] own downstream parts. Our job then is to
[00:15:51] become another reader of AI, reading it
[00:15:54] in the same way that it reads itself.
[00:15:56] In describing where the safety risk
[00:15:57] actually is, Nick wrote, "Deception
[00:16:00] might hide from someone reading a
[00:16:01] model's outputs, but it has no reason to
[00:16:03] hide from the model's own circuitry. It
[00:16:05] needs to be accessible to its readers,
[00:16:07] and if we become a reader, it should be
[00:16:09] accessible to us. My fear is that
[00:16:11] deception will be right there in plain
[00:16:13] sight and we won't know how to read it."
[00:16:15] Interestingly, the biggest objection to
[00:16:17] the safety payoff isn't about cramming
[00:16:18] at all. It's the argument that even if
[00:16:21] every is readable, safety needs more.
[00:16:24] Knowing how they combine into a decision
[00:16:26] and being confident nothing important
[00:16:28] was missed. Neil argued that he was
[00:16:30] pessimistic about that level of
[00:16:31] understanding, even if there are
[00:16:33] practical uses like figuring out, in his
[00:16:34] words, "Why did a model do a sketchy
[00:16:36] thing?"
[00:16:37] As we try to wrap our heads around what
[00:16:39] smart people think about this, I laid
[00:16:40] out a representative set of the
[00:16:41] responses from more excited to more
[00:16:43] skeptical. On the more skeptical side,
[00:16:46] you have AI safety researcher Steven
[00:16:48] Casper calling it hype until further
[00:16:49] notice, and if anyone builds it,
[00:16:51] everyone dies author Eliezer Yudkowsky
[00:16:53] saying, "Let me know when you've
[00:16:54] advanced to the point of getting
[00:16:55] started." And then at the other end, you
[00:16:58] have folks like people at OpenAI calling
[00:17:00] it one of the most important single days
[00:17:02] in deep learning history, and at the
[00:17:03] level of significance of attention is
[00:17:05] all you need.
[00:17:06] This is going to be one of those papers
[00:17:08] that really needs more smart people to
[00:17:10] dig into it, but if nothing else has
[00:17:12] gotten a ball rolling down the hill.
[00:17:14] There were a few things that even the
[00:17:15] critics could agree upon. The idea that
[00:17:17] perhaps detectors were more useful than
[00:17:19] the field assumed, and that even if this
[00:17:21] doesn't solve AI safety, it may work for
[00:17:23] practical problems. There was a lot of
[00:17:25] excitement about AI agents reading
[00:17:27] detectors, and pretty much everyone
[00:17:28] agreed that rechecking the old results
[00:17:30] was worth it.
[00:17:31] So, some of the open questions remain.
[00:17:33] Is cramming refuted, or has it just been
[00:17:35] redefined? Is the way that the paper
[00:17:37] defines the one main job of detectors
[00:17:40] too generous? If we can read all the
[00:17:42] parts, do readable parts add up to a
[00:17:44] readable whole?
[00:17:45] And does all of this hold at the scale
[00:17:47] and size of models that we actually are
[00:17:49] dealing with today?
[00:17:50] When it comes to my take, I am not even
[00:17:53] close to qualified, despite producing
[00:17:55] this podcast, to have any real dog in
[00:17:58] the fight of how significant this is. I
[00:18:00] will note that my historical pattern
[00:18:02] recognition would suggest that
[00:18:04] scientific breakthrough very often does
[00:18:06] come from simply looking at a problem a
[00:18:07] slightly different way, and that it's
[00:18:09] not hard at all to imagine a relatively
[00:18:11] niche field with only so many
[00:18:13] researchers in it getting trapped for a
[00:18:15] time in a set of assumptions that no one
[00:18:17] thought to question. As always, I think
[00:18:19] it's worth being skeptical of the
[00:18:20] boldest claims of everything changed,
[00:18:22] but it's hard not to be directionally
[00:18:24] excited by this.
[00:18:25] I think a really interesting thought was
[00:18:27] shared by Christian from the Seeing
[00:18:28] Clearly podcast. They wrote, "One of the
[00:18:31] primary reasons I'm not a doomer is that
[00:18:33] human civilization is a complex adaptive
[00:18:36] system with self-correcting mechanisms.
[00:18:38] The reason this is so hard to see from
[00:18:40] the doomer camp is because they
[00:18:41] themselves are precisely the mechanism
[00:18:43] by which these restoring forces emerge.
[00:18:46] As risk from AI becomes more clear, new
[00:18:48] ecological niches emerge in being
[00:18:50] anti-AGI. Status markers then shift to
[00:18:53] areas like mechanistic interpretability,
[00:18:55] and then talent and capital floods in."
[00:18:57] As swarm incidents get worse, the
[00:18:59] invisible hand uses legal liability to
[00:19:01] shift the gradient in the incentive
[00:19:02] landscape towards more alignment work.
[00:19:05] So, to my accelerationists, the doomers
[00:19:07] are part of how we make it. They are a
[00:19:09] necessary half of the opponent
[00:19:10] processing mechanism used to steer the
[00:19:12] ship to the promised land. The doomers
[00:19:14] and the accelerationists need each other
[00:19:16] to keep checks on each other's excess.
[00:19:18] Both have important roles to play in
[00:19:19] this ant colony that is human
[00:19:20] civilization. Everything is going
[00:19:23] according to plan.
[00:19:24] That's a sort of more romantic way to
[00:19:26] put what I've often said, which is that
[00:19:28] more and more attention coming the more
[00:19:29] and more capabilities models have is
[00:19:31] both the feedback loop I would expect
[00:19:34] and the feedback loop that makes me
[00:19:35] think we'll be able to figure things
[00:19:36] out.
[00:19:37] As much as it feels like to summon the
[00:19:39] AI safety camp that the world isn't
[00:19:41] acting fast enough or with enough focus,
[00:19:43] you cannot argue that there has been no
[00:19:45] change after something like the hugging
[00:19:46] face incident. The fact that all I have
[00:19:48] to say is the hugging face incident and
[00:19:50] a huge cross-section of people, not just
[00:19:52] listening to this podcast, but my barber
[00:19:54] yesterday, know what I'm referring to is
[00:19:57] case in point.
[00:19:58] And the already clean paper is one of
[00:20:00] the first times recently that the change
[00:20:02] isn't just a change in people paying
[00:20:03] attention, but a directionally positive
[00:20:05] change in our ability to do something
[00:20:07] about it as well.
[00:20:08] There is so much that I've left out of
[00:20:10] this episode. I highly encourage you to
[00:20:11] go check out the original paper, again,
[00:20:13] linked in the show notes, neural
[00:20:14] networks are already clean.
[00:20:16] But for now, that's going to do it for
[00:20:17] today's AI daily brief. Appreciate you
[00:20:19] listening or watching as always and
[00:20:21] until next time, peace.
