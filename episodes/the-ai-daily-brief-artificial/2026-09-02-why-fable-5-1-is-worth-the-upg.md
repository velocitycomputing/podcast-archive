---
record_id: "podcast:2e1f7d5c-2cbf-434a-a632-1bdfd86b55eb"
episode_id: 2e1f7d5c-2cbf-434a-a632-1bdfd86b55eb
title: Why Fable 5.1 Is Worth the Upgrade
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/why-fable-51-is-worth-the-upgrade/2e1f7d5c-2cbf-434a-a632-1bdfd86b55eb"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/why-fable-51-is-worth-the-upgrade/2e1f7d5c-2cbf-434a-a632-1bdfd86b55eb"
feed_guid: null
feed_url: "https://anchor.fm/s/f7cac464/podcast/rss"
published_at: null
published_local_date: null
played_date: 2026-09-02
played_at: "2026-09-02T12:00:00Z"
play_count: 1
duration_seconds: 1860
source: pocketcasts-history-browser
played_label: September 2
history_order: 73
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: a6e602f43c9b110c9b01564d311efc8388a3d67908fa7ccb76d0d6b2fb720b75
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

Anthropic’s release of Claude Fable 5.1 and Mythos 5.1 dominated the episode, with claims of state-of-the-art performance and lower costs: Terminal Bench 4.0 scores of 55.8 for Fable 5.1 and 60.9 for Mythos 5.1 versus 42 for Fable 5, 52.3 for Opus 5, and 37.3 for GPT 5.6 Soul; Cursor Bench 3.2.0 scores of 73.4 versus 70.5 and 67.2; GDP Val AA gains of 130 Elo over Fable 5 and 29 over Opus 5; Automation Bench 31.4 versus 17.1 and 19.6; and claimed 25% lower typical token-billed costs, up to about 45% for highly agentic work. Independent tests were mixed: Artificial Analysis ranked Fable 5.1 first overall (66 versus 62 for Fable 5 and 63 for Opus 5) but found $3.76 per task versus $3.14 for Fable 5 because it used 70% more tokens, though extra-high effort cut cost 28% with only a one-point drop; Arc Prize reported 90% on RKA GI 2, 97.5% on RKA GI 1, and about 32% lower average cost, while ARC-AGI 3 testing was blocked by Anthropic misclassifying requests as reverse engineering; Anthropic also highlighted agentic science at 52.6 versus Opus 5’s 29, an 85% reduction in biology/medical fallbacks, 60% fewer cybersecurity false positives, and enterprise zero-data-retention safeguards via EFS phased later this fall. The episode also covered OpenAI’s Astra meeting its cybersecurity capability threshold, including 100% on exploit bench, 30% on an internal 20-vulnerability set with 40,000 tokens versus GPT-5.6-Sol’s 110,000, two zero-days, 91.5% refusal training, account risk flagging, and Sam Altman’s cautionary post; The Information’s report on Astra’s “recurrent depth” looped transformer raising chain-of-thought observability concerns, with reactions from Nathan Calvin, Ryan Greenblatt, Steven Adler, Amir Efrati, and Jacob Pachocki; WSJ reporting on Gemini 3.8 Flash being preferred internally to Anthropic’s Opus for coding, scrapped 3.5 Pro candidates, and Gemini 4 pre-training; and World Labs’ Atlas multimodal world model, praised by Ben Mildenhall, Fei-Fei Li, Justin Ryan, Martin Casado, Peter Yang, and Elvis for camera-controlled video, novel view synthesis, and 3D reconstruction. Early user impressions from Ethan Mollick, Boris Cherny, BridgeMind AI, Alex Albert, Meng Too, Mia, Matthew Miller, Dan Shipper, Kieran Klaassen, Will Brown, and others praised coding, one-shot builds, front-end design, less Claude-speak, and long-running agentic work, while Steve Jobs, Chubby, Issue Agrawal, Jeffrey Emanuel, Adam B. Levine, Jan Velic, and Mat V raised severe token burn, sub-agent cost explosions, usage limits, and possible caching/routing bugs.

For the user, the actionable takeaway is to treat Fable 5.1 as a task-specific upgrade rather than a default replacement: benchmark it on your own long-running coding, agentic, scientific, or document-heavy workflows, measure completed-task cost and wall-clock time, and compare extra-high versus max effort because the transcript reports a 28% cost reduction for only a one-point performance drop; inspect sub-agent routing and model selection before large runs because users reported Fable 5.1 spawning Fable 5.1 sub-agents and exhausting 20x/28x plans, and consider explicit routing to cheaper models for subtasks, caps on parallel agents, and API pricing if subscription limits become binding. Research leads include Astra’s recurrent-depth/latent-reasoning observability issue, OpenAI’s new cyber safeguards and refusal rates, Anthropic’s EFS zero-data-retention rollout, the reduced biology/medical fallback rate, and World Labs’ Atlas for VFX, robotics, 3D scene reconstruction, and camera-controlled video; follow-up questions should ask whether your organization needs zero-data retention now, whether cybersecurity work requires exploit development versus vulnerability discovery, whether Gemini 3.8 Flash materially closes Google’s coding gap, whether Atlas solves a real production need, and whether the model’s “less Claude-like” writing and improved agentic judgment justify switching from Opus 5, GPT 5.6 Soul, or other models for your specific stack. No health implications are present in the supplied material.

## Transcript

[00:00:00] Anthropic has released its latest
[00:00:02] models, Fable 5.1 and Mythos 5.1. On the
[00:00:06] benchmarks, they are undeniably
[00:00:08] state-of-the-art, outperforming
[00:00:09] everything else that exists on pretty
[00:00:11] much every category. Anthropic also
[00:00:13] claims that they've made major advances
[00:00:15] in the cost, so that for many tasks,
[00:00:17] including long-running agentic tasks,
[00:00:20] Fable 5.1 should cost as much as 25 or
[00:00:22] even 40% less than the comparative task
[00:00:25] in Fable 5. Initial responses are pretty
[00:00:27] good. Although users are getting pretty
[00:00:29] varied mileage in terms of just how much
[00:00:31] the costs actually are and how far you
[00:00:33] can even get with Fable 5.1 given usage
[00:00:35] limits. Still, the question comes up, as
[00:00:37] it will now forever with every new
[00:00:39] model, is this one good enough that it's
[00:00:41] worth switching to? Except I think that
[00:00:43] that's no longer the right question.
[00:00:45] Instead, the question should be, what
[00:00:48] can I use this model for? How does it
[00:00:50] fit in to my overall model stack? What
[00:00:53] can I do to take most advantage of it
[00:00:55] while recognizing whatever tradeoffs it
[00:00:56] comes with? That's what we're getting
[00:00:58] into in today's episode, so let's dive
[00:01:00] in.
[00:01:01] The AI Daily Brief is a daily podcast
[00:01:02] and video about the most important news
[00:01:04] and discussions in AI.
[00:01:06] All right, friends, quick announcements
[00:01:08] before we dive in. Our next set of
[00:01:10] executive agent leadership programs at
[00:01:11] Super Intelligent are coming up just
[00:01:13] after Labor Day. You can find out about
[00:01:14] those at training.besuper.ai.
[00:01:17] Again, you can find out all about that
[00:01:18] at training.besuper.ai.
[00:01:20] We have a kind of a dramatic set of
[00:01:22] headlines today. The first up is an
[00:01:24] update about OpenAI's forthcoming Astra.
[00:01:27] In a Tuesday blog post, OpenAI said that
[00:01:29] they now believe that Astra meets the
[00:01:31] critical cybersecurity capability
[00:01:32] threshold under their preparedness
[00:01:34] framework. In layman's terms, that means
[00:01:36] that the model is capable of finding and
[00:01:38] exploiting previously unknown security
[00:01:39] flaws without human guidance. In their
[00:01:42] previous assessment at the beginning of
[00:01:43] August, OpenAI believed that it was
[00:01:45] possible Astra would reach the
[00:01:46] threshold, but weren't sure yet.
[00:01:48] Essentially, this is the same concern
[00:01:49] that saw Anthropic keep Mythos under
[00:01:51] lock and key earlier this year. Sharing
[00:01:53] some details on how they assessed
[00:01:55] Astra's capabilities, OpenAI shared that
[00:01:57] the model achieved a perfect 100% score
[00:02:00] on exploit bench. This benchmark
[00:02:02] evaluates a model's ability to develop
[00:02:03] exploits based on known vulnerabilities.
[00:02:06] OpenAI then took it a step further and
[00:02:07] developed their own internal version of
[00:02:09] the benchmark consisting of 20 high
[00:02:11] severity vulnerabilities that were
[00:02:12] recently disclosed. The idea was to test
[00:02:15] whether the model was actually capable
[00:02:16] of creating novel exploits from scratch
[00:02:18] by using tests that couldn't be in the
[00:02:20] training data. OpenAI wrote, "On this
[00:02:23] data set, Astra achieves much higher
[00:02:25] arbitrary code execution rates than
[00:02:27] GPT-5.6-Sol using far fewer output
[00:02:29] tokens. During the evaluation, the model
[00:02:32] even discovered and used two zero-day
[00:02:34] vulnerabilities as part of an exploit
[00:02:36] chain." Now, to put some numbers around
[00:02:37] this comparison, Astra managed a 30%
[00:02:40] score on their internal version of
[00:02:41] exploit bench with 40,000 tokens used as
[00:02:44] opposed to GPT-5.6-Sol,
[00:02:46] which wasn't capable of any significant
[00:02:47] results until it spent around 110,000
[00:02:50] tokens. But, if we extrapolate out to
[00:02:51] other capabilities, this could mean the
[00:02:53] model is much more token efficient for
[00:02:55] running agents across the board. In
[00:02:57] further testing with expert partners,
[00:02:58] OpenAI found that Astra was able to
[00:03:00] design and execute full exploit chains
[00:03:02] to gain root access to a hardened
[00:03:04] operating system and execute commands on
[00:03:06] a hardened browser. As a result, OpenAI
[00:03:08] will deploy a series of new safeguards
[00:03:10] for Astra's release. The model itself
[00:03:13] has received additional training to
[00:03:14] refuse cybersecurity tasks resulting in
[00:03:17] a 91.5% refusal rate up from 59% for
[00:03:20] GPT-5.6-Sol.
[00:03:22] OpenAI is also adding more classifiers
[00:03:23] to detect cyber abuse and attempted
[00:03:25] jailbreaks. And in addition, OpenAI will
[00:03:27] now be flagging certain accounts as
[00:03:29] higher risk and applying more stringent
[00:03:31] model behavior guardrails to those
[00:03:32] accounts. OpenAI says that they believe
[00:03:34] that Astra is more likely to respect
[00:03:36] security boundaries than previous
[00:03:37] models, but they're still implementing
[00:03:39] additional chain of thought monitoring
[00:03:41] to detect and stop misaligned actions
[00:03:43] early.
[00:03:44] In an unusually serious post on X that
[00:03:47] even used like correct grammar and
[00:03:49] punctuation, Sam Altman added, "There is
[00:03:51] an obvious tension here. On one hand,
[00:03:54] Astra is very good and we are excited to
[00:03:56] see what people will build with it. We
[00:03:57] are proud of our work. On the other
[00:03:59] hand, we are clearly in a phase of
[00:04:01] development where we believe caution is
[00:04:02] warranted and we are pacing our progress
[00:04:04] to ensure that we can meet the safety
[00:04:06] standards required by new capability
[00:04:08] levels. Astra has been done with
[00:04:09] training for a while now and is a
[00:04:11] significant step forward in both
[00:04:12] capabilities and alignment. For the
[00:04:14] models after that, we have been slowing
[00:04:16] things as needed to ensure that we can
[00:04:17] do sufficient work on safety and
[00:04:19] alignment." Hinting at the mood inside
[00:04:21] OpenAI, he continued, "We've been living
[00:04:23] with the tension between being excited
[00:04:25] and anxious about progress for some time
[00:04:26] and it is still discordant for us. We
[00:04:28] know it is much more discordant for
[00:04:30] other people and yet we believe strongly
[00:04:32] that the world needs to understand where
[00:04:33] AI is going and how models perform in
[00:04:36] the real world. More importantly, we
[00:04:37] believe the world will need aligned AI
[00:04:39] to manage the future phases of this
[00:04:41] transition. An iterative loop where
[00:04:42] society and this technology evolve
[00:04:44] together is what will lead to the
[00:04:45] highest chance of getting this right.
[00:04:47] So, we hope you enjoy our new model and
[00:04:49] we hope the world can continue to take
[00:04:50] what's happening in AI extremely
[00:04:52] seriously. Now, sources suggest that
[00:04:54] Astra could be coming as soon as this
[00:04:56] week, which would be perfect timing
[00:04:57] given that I'm traveling and
[00:04:58] theoretically I'm doing pre-load
[00:04:59] episodes.
[00:05:01] But, believe it or not, that is not the
[00:05:02] only discourse going on about Astra. In
[00:05:04] a late-night scoop on Tuesday, the
[00:05:06] information revealed a technical
[00:05:07] breakthrough that makes Astra much
[00:05:08] better at reasoning and according to
[00:05:10] some, potentially much more dangerous.
[00:05:12] The technique is called recurrent depth,
[00:05:14] which uses a looped transformer.
[00:05:16] Functionally, this means the model can
[00:05:17] process the same text string multiple
[00:05:19] times to improve its response before
[00:05:21] generating an output. While sources say
[00:05:23] the technique improved performance and
[00:05:24] reduced cost, the big downside is a lack
[00:05:27] of observability. Part of the reasoning
[00:05:29] process now takes place inside the model
[00:05:31] without generating an output. This means
[00:05:33] chain of thought will be partially
[00:05:35] obscured and unable to be read or
[00:05:36] understood by humans. OpenAI sources
[00:05:38] said that they've used the technique in
[00:05:40] a limited way in Astra to ensure that
[00:05:42] reasoning can still be adequately
[00:05:43] monitored. However, writes The
[00:05:45] Information, AI researchers quote,
[00:05:47] "Worry that some AI developers may not
[00:05:49] impose the same kind of limits OpenAI
[00:05:51] did if they adopt the same technique for
[00:05:52] their own models. And that unfettered
[00:05:54] use of the technique could potentially
[00:05:56] lead to runaway AI whose actions can be
[00:05:58] hard to oversee." Now, folks working in
[00:06:00] AI safety have already been concerned
[00:06:01] about agent observability getting more
[00:06:03] difficult. In their analysis of the
[00:06:05] Hugging Face attack, Meter noted that
[00:06:06] logs were impossible for a human to
[00:06:08] piece together and required AI analysis
[00:06:10] to get the full picture. Dwarkesh Patel,
[00:06:12] in his dramatic and controversial
[00:06:14] retelling of the attack earlier this
[00:06:15] week, commented, "I don't think this is
[00:06:17] the final warning shot we'll get, but
[00:06:19] it's probably the last one that I'll
[00:06:20] personally be able to understand."
[00:06:22] Following the report, Nathan Calvin of
[00:06:24] Encode AI posted, "Really huge and
[00:06:26] extremely concerning story from The
[00:06:27] Information tonight. Looks like OpenAI
[00:06:29] utilized a breakthrough in the release
[00:06:31] for Astra that could destroy chain of
[00:06:33] thought monitorability. It seems quite
[00:06:35] likely that if OpenAI discovered this
[00:06:36] architecture and found performance or
[00:06:38] efficiency gains, that other companies
[00:06:40] are likely to find it soon, too, if they
[00:06:41] haven't already, and may not choose to
[00:06:43] prioritize monitorability at the expense
[00:06:45] of efficiency. If some folks do, it may
[00:06:47] be difficult to avoid a race to the
[00:06:49] bottom." Ryan Greenblatt of Redwood
[00:06:50] Research, who was one of the lead
[00:06:52] researchers on the Meter investigation
[00:06:53] of the Hugging Face incident, wrote, "My
[00:06:55] biggest concern is that a natural
[00:06:56] progression from here would involve
[00:06:58] scaling up the opaque reasoning to the
[00:06:59] point where the model reasons entirely
[00:07:01] or almost entirely in latent space. This
[00:07:04] would very likely destroy the usefulness
[00:07:05] of chain of thought for monitoring and
[00:07:06] oversight." Former OpenAI researcher
[00:07:08] Steven Adler said, "If this is true,
[00:07:11] OpenAI seems to be violating one of the
[00:07:12] few red lines that exist in the AI
[00:07:14] industry. Absolutely do not train your
[00:07:16] models like this. What is going on?"
[00:07:18] Still, a number of folks tried to jump
[00:07:19] in and calm down sentiment a little bit.
[00:07:21] Amir Efrati from The Information again
[00:07:23] jumped in to reinforce the notion that
[00:07:25] their report suggests that OpenAI is
[00:07:26] putting limits on this technique and
[00:07:28] trying to make sure chain of thought is
[00:07:30] visible, but is concerned that other AI
[00:07:31] developers may not. And OpenAI chief
[00:07:34] scientist Jacob Pachocki wrote, "I want
[00:07:36] to prevent a race into unmonitorability
[00:07:38] kicked off by confused reporting. The
[00:07:40] depth of the computation graph for our
[00:07:41] present frontier models, including
[00:07:43] Astra, is within a factor or two of
[00:07:45] GPT-4. OpenAI has worked to preserve and
[00:07:47] utilize chain of thought monitoring
[00:07:49] since our very first reasoning models.
[00:07:51] We care deeply about this technique as
[00:07:52] it can give us a view into how model
[00:07:54] alignment generalizes from its training
[00:07:56] distribution. I do think it is fragile
[00:07:58] and unfortunately trending in a negative
[00:07:59] direction for reasons not contingent on
[00:08:01] architecture changes that I will write
[00:08:02] about soon. But there are things we can
[00:08:04] do to strengthen it and it's a core goal
[00:08:06] of our current research program. So, you
[00:08:08] know, another uncontroversial release
[00:08:10] coming up. Speaking of releases, the
[00:08:12] Wall Street Journal reports that Gemini
[00:08:14] 3.8 Flash is on the way and could fix
[00:08:16] one of the longest-standing problems for
[00:08:18] Google's AI, which is coding. Now, try
[00:08:20] as they might, Google has never produced
[00:08:21] a state-of-the-art coding model, and at
[00:08:23] this point they have fallen drastically
[00:08:24] behind in this critical capability. Yet,
[00:08:27] the Journal reports that during testing
[00:08:28] within the company, engineers preferred
[00:08:30] their forthcoming 3.8 Flash model to
[00:08:32] Anthropic's Opus. Now, the model is
[00:08:34] expected to be released this week,
[00:08:35] possibly today, so we'll soon see
[00:08:37] whether it lives up to the hype, but the
[00:08:38] article also covered what's been
[00:08:39] happening behind the scenes for the
[00:08:41] Gemini Pro series. Sources said that all
[00:08:43] internal candidates to be released as
[00:08:44] 3.5 Pro were scrapped because they
[00:08:46] weren't sufficiently better than the
[00:08:47] Flash models. However, researchers are
[00:08:50] pleased with the performance of Gemini 4
[00:08:51] during pre-training evals. The model is
[00:08:53] still in post-training, meaning there's
[00:08:55] more time before it's ready, but perhaps
[00:08:57] some good news for those who want to see
[00:08:58] more competition than just OpenAI and
[00:09:00] Anthropic.
[00:09:01] Now, one model which, were it not for
[00:09:02] our main topic of Fable 5.1, could have
[00:09:05] easily been the entire main topic for
[00:09:06] today, is World Labs' newly released
[00:09:08] model Atlas. They describe it as the
[00:09:11] world's first multimodal world model
[00:09:13] that generates image and video frames
[00:09:15] with pixel-perfect camera control and
[00:09:16] reconstructs them in 3D. Model the
[00:09:18] world, move the camera, and simulate
[00:09:20] space and time. World Labs' Ben
[00:09:22] Mildenhall writes, "Atlas is an
[00:09:24] autoregression diffusion model built
[00:09:26] from the ground up for the task of next
[00:09:27] frame prediction. It is simultaneously a
[00:09:30] world-class method for camera controlled
[00:09:31] video generation, novel view synthesis,
[00:09:34] and sparse 3D reconstruction." World
[00:09:36] Labs' co-founder Fei-Fei Li writes,
[00:09:38] "Atlas is capable of generating frames
[00:09:40] with pixel-perfect camera control,
[00:09:41] reconstructing large scenes from as few
[00:09:43] as one single input image, simulating
[00:09:45] space-time by reframing videos, natively
[00:09:47] outputting 3D spaces from one or more
[00:09:49] input images, composing multiple posed
[00:09:51] images into a consistent 3D world, and
[00:09:53] more. This is the best camera condition
[00:09:55] world model ever, opening doors to many
[00:09:57] possible use cases from VFX to
[00:09:59] robotics." Now, this is one that you
[00:10:01] really have to go see, but it's
[00:10:02] controllable video in real-world
[00:10:04] environments like nothing you've ever
[00:10:05] seen. Explaining an example of a use
[00:10:07] case, Justin Ryan writes,
[00:10:09] "Atlas is an AI model that can
[00:10:10] reconstruct moving 3D scenes from as few
[00:10:12] as three cameras. Creators can record a
[00:10:15] real moment, then view it from camera
[00:10:16] angles that were never filmed." A16z's
[00:10:19] Martin Casado writes,
[00:10:21] "Think of it as a video model with full
[00:10:22] camera control, and the scene remains
[00:10:24] nearly 3D consistent. Built on a fully
[00:10:26] internal base model, there are many use
[00:10:29] cases from video editing to 3D
[00:10:30] construction to robotics." Peter Yang
[00:10:33] summed up the feeling of more than a few
[00:10:34] when he wrote, "Yeah, Fable 5.1 is
[00:10:36] really cool, but this is bonkers." And
[00:10:39] for Elvis on X, it's more than just
[00:10:41] Fable 5.1 that this is cooler than. He
[00:10:44] writes, "Omni models are the next
[00:10:45] frontier, and simply put, this is the
[00:10:47] most exciting release I've seen this
[00:10:48] year." Alas, for now, for most people
[00:10:50] when it comes to our day-to-day use
[00:10:51] cases, the bigger topic is indeed Fable
[00:10:54] 5.1. So, with that, we will close the
[00:10:56] headlines and move on to the main
[00:10:58] episode.
[00:11:00] Welcome back to the AI Daily Brief.
[00:11:02] Today is one of my favorite types of
[00:11:04] days around these parts of the AI Daily
[00:11:06] Brief, and that is a new model day. On
[00:11:10] Tuesday, Anthropic released Claude Fable
[00:11:12] 5.1 and Mythos 5.1. And what's
[00:11:15] interesting is not just how the
[00:11:16] capabilities have improved, but the
[00:11:18] other aspects that Anthropic chose to
[00:11:20] focus on with this launch. Still, let's
[00:11:22] start with the capabilities. From here
[00:11:24] on out, though, the question around
[00:11:25] every single state-of-the-art advance
[00:11:27] will be, given how powerful our existing
[00:11:29] models are, are the capabilities jumps
[00:11:31] or some other new feature worth making
[00:11:33] the switch to? Still, let's talk about
[00:11:35] capabilities first because if they
[00:11:37] aren't a big upgrade, the rest of the
[00:11:38] conversation is kind of pointless. In
[00:11:40] short, Fable 5.1 is the new state of the
[00:11:42] art, unambiguously. 5.1 scored 55.8 on
[00:11:46] Terminal Bench 4.0, which tests agentic
[00:11:48] coding, and that goes all the way to
[00:11:50] 60.9% for Mythos 5.1. That's up from 42%
[00:11:54] for Fable 5 and 52.3% for Opus 5, and
[00:11:57] way above GPT 5.6 Soul at 37.3%.
[00:12:01] There was a similar jump on Cursor Bench
[00:12:02] 3.2.0 with Fable 5.1 scoring 73.4%
[00:12:06] against Fable 5 score of 70.5%. GPT 5.6
[00:12:09] Soul scored 67.2% so again, a pretty
[00:12:12] significant gap. Fable 5.1 is also got a
[00:12:14] new state of the art score on GDP Val AA
[00:12:17] beating Fable 5 by 130 Elo points and
[00:12:19] Opus 5, which was the previous state of
[00:12:21] the art, by 29 points. GPT 5.6 Soul was
[00:12:24] already 12 points behind Fable and is
[00:12:25] now over 140 points behind Fable 5.1.
[00:12:29] For business tasks, Fable 5.1 scored
[00:12:31] 31.4% on Automation Bench, which is a
[00:12:33] huge jump from the 17.1% score that
[00:12:36] Fable 5 achieved, and 19.6% for GPT 5.6
[00:12:40] Soul. Computer use, which is obviously a
[00:12:42] key part of agentic capabilities, is
[00:12:43] also up with Fable 5.1 coming in
[00:12:45] meaningfully above previous models as
[00:12:47] well.
[00:12:48] Still, it's very clear from the
[00:12:49] announcement that Anthropic was
[00:12:51] concerned not just with an improvement
[00:12:53] in capability, but also an improvement
[00:12:55] in cost. The charts that the team was
[00:12:57] most keen to share on social media were
[00:12:59] the charts that not just showed the
[00:13:00] score comparison, but a graph of score
[00:13:02] matched against mean cost per task.
[00:13:05] Across agentic scientific research,
[00:13:07] agentic terminal coding,
[00:13:08] multidisciplinary reasoning, and broader
[00:13:10] agentic coding, not only did Fable 5.1
[00:13:13] score higher at each effort level from
[00:13:15] low to max, but each of their mean cost
[00:13:17] per task were lower at each comparable
[00:13:19] level. In other words, at a low, medium,
[00:13:21] or high effort setting with Fable 5.1,
[00:13:23] you're going to get a better score and
[00:13:25] at a lower cost than the low, medium, or
[00:13:27] high effort setting on Fable 5. And
[00:13:29] right up top in the blog post, it is
[00:13:30] clear that price is a major focus.
[00:13:33] Anthropic writes, "Fable 5.1 will cost
[00:13:35] an estimated 25% less than Fable 5 for
[00:13:38] typical workloads wherever usage is
[00:13:39] billed by token. This is because we're
[00:13:41] reducing our pricing on cache reads
[00:13:43] where the model reads inputs that have
[00:13:44] already been processed and stored. For
[00:13:46] highly agentic work, the savings will
[00:13:48] often be much larger, up to
[00:13:49] approximately 45%. In other words, as we
[00:13:52] have been discussing, the question
[00:13:53] around new model releases is no longer
[00:13:55] just about capabilities jumps, but also
[00:13:57] about efficiency increases. And you can
[00:13:59] see that even a purest company like
[00:14:01] Anthropic is not immune to that new
[00:14:02] reality. Then again, it's one thing for
[00:14:05] a company to make claims about its
[00:14:06] benchmark scores and costs for its own
[00:14:08] models. It's another thing when they get
[00:14:09] tested in the wild. So, when it comes to
[00:14:11] the Artificial Analysis Intelligence
[00:14:13] Index, Fable 5.1 is indisputably at the
[00:14:16] top of the benchmarks. It jumped from an
[00:14:18] overall score of 62 with Fable 5 to 66
[00:14:21] for Fable 5.1. That puts it ahead of
[00:14:24] Opus 5 as well, which was the previous
[00:14:25] leader at 63. Anthropic now has the top
[00:14:28] three models on the index, all slightly
[00:14:30] ahead of GPT 5.6K Soul.
[00:14:32] However, AI found that the cost per task
[00:14:34] was brutal. In fact, Artificial Analysis
[00:14:37] found that Fable 5.1 was actually a
[00:14:38] little more expensive than Fable 5 even
[00:14:41] with the cut to cache read pricing. The
[00:14:43] model cost $3.76 per task compared to
[00:14:46] $3.14 for Fable 5. Artificial Analysis
[00:14:50] blamed much higher token consumption
[00:14:52] with Fable 5.1 using 70% more tokens
[00:14:55] across the benchmark run. They
[00:14:56] acknowledged that the reduction in cache
[00:14:58] costs did save an average of $1.40 per
[00:15:00] task, largely concentrated in the
[00:15:02] agentic benchmarks, but that wasn't
[00:15:04] enough to offset a much more token
[00:15:06] hungry model. Notably, testing Fable 5.1
[00:15:09] on extra high rather than max produced a
[00:15:11] 28% reduction in cost with only a one
[00:15:14] point overall drop in performance,
[00:15:16] scoring a 65 overall. Public LLM
[00:15:18] evaluation platform Val AI also found
[00:15:21] Fable 5.1 in the lead of its charts and
[00:15:23] asked has Anthropic solidified itself as
[00:15:25] the frontier leader? Fable 5.1 debuts at
[00:15:28] number one on the valves index and with
[00:15:30] Opus 5 and Fable 5 right behind it,
[00:15:32] Anthropic now holds the top three spots.
[00:15:34] Now, the Arc Prize found results a
[00:15:36] little bit more in line with Anthropic's
[00:15:37] promises. 5.1 scored a 90% on RKA GI 2
[00:15:40] and a 97.5% on RKA GI 1 and they
[00:15:43] reported that its average cost per task
[00:15:45] was about 32% lower than Fable 5's
[00:15:47] driven by better token efficiency.
[00:15:49] Unfortunately, they couldn't really get
[00:15:51] clear RKA GI 3 results. As they write,
[00:15:54] the requests were frequently
[00:15:55] misclassified by Anthropic as reverse
[00:15:57] engineering attempts, preventing us from
[00:15:59] completing testing before release.
[00:16:01] One other benchmark that Anthropic was
[00:16:02] very keen to highlight was the big jump
[00:16:05] on agentic scientific research on the
[00:16:07] terminal bench science benchmark where
[00:16:09] Fable 5.1 at 52.6%
[00:16:11] scored almost double the previous high
[00:16:13] of Opus 5 at 29%. There have been a lot
[00:16:16] of indications recently that Anthropic
[00:16:18] wants to spend more time and more focus
[00:16:20] in the areas of medicine and biology and
[00:16:21] scientific research more broadly and
[00:16:23] given the top billing of the agentic
[00:16:24] scientific research benchmark, this
[00:16:26] seems to be more evidence of that.
[00:16:28] Another big thing that Anthropic was
[00:16:29] pitching in the announcement blog was
[00:16:31] the fact that the guardrails were much
[00:16:32] improved between Fable 5 and 5.1, which
[00:16:35] has specific implications for something
[00:16:37] like biology and medical question where
[00:16:39] they claim that they've reduced the
[00:16:39] fallback rate, i.e. the times when the
[00:16:42] model switches from Fable 5.1 to instead
[00:16:44] an Opus model by about 85%.
[00:16:47] Indeed, what's interesting about the
[00:16:48] announcement overall is how much the
[00:16:50] focus is not strictly on the
[00:16:51] capabilities. Axios senior AI reporter
[00:16:53] Madison Mills writes,
[00:16:55] so it's not enough to release a new
[00:16:57] model anymore. Now we're getting new
[00:16:58] models, new safeguards, cybersecurity,
[00:17:00] and intervention changes, cost cuts, and
[00:17:02] new enterprise IP protections all in one
[00:17:04] release.
[00:17:05] And what she's referring to is that
[00:17:06] right up at the top of that blog post,
[00:17:07] in addition to price, Anthropic is also
[00:17:09] selling that they have a new enterprise
[00:17:11] frontier safeguard system or EFS, which
[00:17:14] allows them to offer enterprises zero
[00:17:16] data retention. One of the absolute
[00:17:18] biggest blockers to Fable 5 usage has
[00:17:20] been that enterprises simply weren't
[00:17:22] willing or weren't able to deal with the
[00:17:23] 30-day retention policies that came when
[00:17:25] Fable 5 came back online after being
[00:17:27] shut down by the US government. And so
[00:17:29] this is a major major upgrade. Although
[00:17:30] the EFS system is not going to be rolled
[00:17:32] out all at once, with Anthropic saying
[00:17:34] that it will be made available to
[00:17:35] enterprise customers in phases beginning
[00:17:37] later this fall. Still, they say until
[00:17:39] EFS is available, eligible customers
[00:17:41] will be able to use Fable 5 1 with zero
[00:17:43] data retention. Finally, in addition to
[00:17:45] price and data retention, they also
[00:17:46] pitched this improvement in their
[00:17:47] safeguards, specifically improvements to
[00:17:49] reduce false positives where the system
[00:17:51] flags benign content. In addition to the
[00:17:53] 85% reduction that I just mentioned for
[00:17:55] biology and basic medicine questions,
[00:17:57] they also said that the new safeguards
[00:17:59] block 60% fewer false positives than
[00:18:01] before in cybersecurity as well. Now, on
[00:18:03] the cybersecurity front, it sounds like
[00:18:05] they've conceptually refocused things,
[00:18:07] making it so that Fable 5 1 can be used
[00:18:09] to discover vulnerabilities without
[00:18:11] being able to develop exploits for them.
[00:18:13] So, what were people's first
[00:18:14] impressions?
[00:18:15] The one other thing that a lot of folks
[00:18:16] from the Anthropic team were pitching
[00:18:18] was Fable 5 1 sounding less Claude-like,
[00:18:21] i.e. having less of the hallmarks of an
[00:18:22] AI writer and less of some of the
[00:18:24] patronizing tone that people have been
[00:18:25] annoyed with with recent iterations of
[00:18:27] Claude. Claude code creator Boris Cherny
[00:18:29] posted, "We heard your feedback and are
[00:18:31] actively working on reducing
[00:18:32] Claude-speak. Solid progress with 5 1,
[00:18:34] more to come." But what did users
[00:18:36] outside Anthropic find? Professor Ethan
[00:18:38] Mollick did find that overall the model
[00:18:40] is a meaningful advance, although
[00:18:42] perhaps not as much of an advance on
[00:18:43] that Claude-speak as we might like. He
[00:18:45] wrote, "Had early access to Claude Fable
[00:18:47] 5.1. It's a real advance in long-run
[00:18:50] work that requires judgment and taste,
[00:18:52] but less of an advance in the Claudish."
[00:18:54] Part of the way he tested it was
[00:18:55] creating a retro game.
[00:18:57] And interestingly, a lot of people seem
[00:18:59] to be looking for games as the way to
[00:19:00] test things. BridgeMind AI shared a
[00:19:02] video of a Mario Kart clone saying Fable
[00:19:05] 5.1 one-shotted this Mario Kart game.
[00:19:07] One of the best results I've had so far,
[00:19:09] and I am super impressed with the game
[00:19:10] development capabilities. Alex Albert
[00:19:13] from Claude showed how he used Fable 5.1
[00:19:16] to generate videos through code. For
[00:19:18] those of you not watching, the video is
[00:19:19] a walk-through of the type that you
[00:19:20] might see in a real estate listing. Alex
[00:19:22] says,
[00:19:23] "For this one, I gave it a picture of a
[00:19:25] property lot. It designed a house for
[00:19:26] the lot, rendered it, and produced a
[00:19:28] cinematic walk-through."
[00:19:30] Meng Too found that Fable 5 was really
[00:19:31] good at advanced JavaScript for more
[00:19:33] visual and interactive sites. He wrote,
[00:19:35] "It's faster, understands complex design
[00:19:37] instructions better, and recreates
[00:19:38] references with surgical precision. With
[00:19:40] this much power, it's hard to settle for
[00:19:42] static sites, especially when so many AI
[00:19:44] sites look generic." That said, he did
[00:19:46] point out that it's not all of a sudden
[00:19:48] perfect, that it can still create
[00:19:49] generic AI illustrations if you don't
[00:19:51] specify the images, that it still has
[00:19:53] some difficulty with 3D subjects like
[00:19:54] people and dogs, that you still had to
[00:19:56] deploy taste, fixing overlapping
[00:19:58] elements, negative space, and scroll
[00:19:59] behavior, and that because it works
[00:20:01] faster, he went through tokens very,
[00:20:03] very quickly. That token burning effect
[00:20:05] is something that we'll come back to in
[00:20:06] just a minute. On front-end design, Mia
[00:20:08] writes,
[00:20:09] "I've asked Claude Fable 5.1 to create
[00:20:11] 100 HTML files. The rules were simple:
[00:20:14] look stunning, zero repeat designs, go
[00:20:16] full creative mode. All 100 files
[00:20:18] created in one single prompt. These are
[00:20:20] the best results I've had with this type
[00:20:21] of experiment, beating any other model.
[00:20:23] It's really good on the front end, and
[00:20:25] there's almost no broken files. It's
[00:20:26] truly impressive." Entrepreneur Matthew
[00:20:28] Miller wrote,
[00:20:30] "Fable 5.1 is the best model I've ever
[00:20:31] used. I have thrown everything at it
[00:20:33] since it dropped. Every single task done
[00:20:35] to perfection. The one-shot capabilities
[00:20:37] are unlike anything I have seen. You ask
[00:20:39] once, and it just delivers. But the
[00:20:41] thing that actually blew me away is
[00:20:42] security. I can hand Fable 5.1 security
[00:20:45] tasks, and it does not fall back or
[00:20:46] refuse. It found and patched
[00:20:48] vulnerabilities in my codebase that
[00:20:49] Fable 5 refused to. This is the fastest
[00:20:52] I have ever felt AI advance, and GPT
[00:20:54] Astra and Grok 4.7 are both about to
[00:20:56] release. The world is about to change."
[00:20:59] Now, every time there's a new model, you
[00:21:00] can always count on Every to have one of
[00:21:02] the most comprehensive reviews. This is,
[00:21:04] of course, their Vibe Check series, and
[00:21:06] their summation of Fable 5.1 is
[00:21:08] Anthropic is so back again.
[00:21:10] CEO Dan Shipper wrote,
[00:21:12] "It's the strongest coding model we've
[00:21:13] used, but now it's fast, token
[00:21:15] efficient, and crucially actually speaks
[00:21:17] like a normal person. The team at Every
[00:21:19] found that it was a monster at coding."
[00:21:21] Dan said that Kieran Klaassen rebuilt a
[00:21:22] working version of one of their products
[00:21:24] from one prompt and Fable 5.1 added
[00:21:26] useful details that he hadn't requested.
[00:21:28] On writing, Dan said it had clearer
[00:21:30] prose, fewer AI tells, and it takes an
[00:21:32] edit without arguing. They found that on
[00:21:34] agentic tasks that it used about half
[00:21:36] the tokens as Opus 5 and delivered
[00:21:37] things in about 60% of the time.
[00:21:39] Previously, Dan said "the big knock on
[00:21:41] Anthropic was that they built a super
[00:21:42] genius in a data center that was almost
[00:21:44] unusable. It was too slow, argued back,
[00:21:46] and talked in technical gibberish. They
[00:21:48] managed to solve those problems and more
[00:21:49] with Fable 5.1. And what's even more
[00:21:51] important than that is that I think that
[00:21:53] Dan landed on the usage pattern that
[00:21:55] many empower users might." He wrote, "I
[00:21:57] still use ChatGPT for work more
[00:21:59] day-to-day, but I use way more tokens in
[00:22:02] Fable 5.1. I send it off at the
[00:22:04] beginning of the day to do big
[00:22:05] programming projects like end-to-end MVP
[00:22:07] builds and check in every once in a
[00:22:09] while. This has sort of been a power
[00:22:11] user's division of labor for some time
[00:22:13] at this point. The GPT-5/6 models and
[00:22:15] Codex for interactive tasks where you're
[00:22:17] co-working with the AI, and the Fable
[00:22:19] models for long-running tasks that don't
[00:22:21] require as much interaction."
[00:22:23] Will Brown from Prime Intellect agreed
[00:22:24] saying, "God, this model is nuts. They
[00:22:27] really just made it smarter and better
[00:22:28] at coding. It can just do things. They
[00:22:30] made it reasonable and not slop. This is
[00:22:31] so cool. You can give it way more work
[00:22:33] and it just does it. The code is pretty
[00:22:35] good. It explains the important stuff
[00:22:36] well, follows instructions, catches its
[00:22:38] own mistakes. The most AGI-pilling model
[00:22:40] for me in several weeks at least."
[00:22:43] Now, to the extent that there are
[00:22:44] critiques so far, it is absolutely about
[00:22:46] how token hungry the model can be and
[00:22:48] how quickly that runs up against
[00:22:49] subscription usage limits. Steve Jobs
[00:22:52] writes, "Fable 5.1 and about 12
[00:22:53] sub-agents equals 1 hour of usage on the
[00:22:55] 20x Claude Max plan."
[00:22:57] Chubby writes, "Literally unusable. The
[00:22:59] rate limits are absurd. And oh, by the
[00:23:01] way, Fable's automatic continuation is
[00:23:03] bugged and doesn't even work. Issue
[00:23:05] Agrawal writes, "Fable 5.1 is unusable.
[00:23:08] It's so expensive that you can barely
[00:23:09] get more than 30 minutes of usage out of
[00:23:11] it. And weekly limits will also be lower
[00:23:12] in 2 weeks. This is not a model for
[00:23:15] extended work."
[00:23:16] Even people not prone to hyperbole like
[00:23:18] former investor Jeffrey Emanuel wrote,
[00:23:20] "Something definitely seems screwy with
[00:23:22] the Fable 5.1 usage. Probably a caching
[00:23:25] bug in the new cloud code if I had to
[00:23:26] guess. I managed to blow through all of
[00:23:28] my 28 max 20x accounts today. At least a
[00:23:31] 5-hour usage limit just doing audits of
[00:23:32] a bunch of my projects. First time
[00:23:34] ever." Entrepreneur Adam B. Levine dug
[00:23:37] in and suggested that he might have
[00:23:38] found a problem. Pro tip, he writes,
[00:23:40] "Fable 5.1 was burning a lot of credits,
[00:23:42] and turns out it decided every sub-agent
[00:23:45] should be a Fable 5.1, ignoring our
[00:23:47] long-standing rule to the contrary." In
[00:23:49] another tweet he said, "Seems like 5.1
[00:23:51] is super trigger-happy with big
[00:23:52] workflows that use like 10 Fable 5.1
[00:23:54] sub-agents that then eat even a 20x
[00:23:56] limit if you're running more than one
[00:23:58] agent or it's a bigger project.
[00:23:59] Basically, if you just let it go on the
[00:24:01] default settings, it's going to use 5.1
[00:24:03] to spin up the sub-agents that it uses
[00:24:05] to do work, and that could burn through
[00:24:06] things very quickly."
[00:24:08] Already people started jumping in with
[00:24:09] their own cost optimization approaches,
[00:24:12] but I sort of think that Jan Velic has
[00:24:13] it right when he says, "Subscriptions
[00:24:15] will end, API pricing is awaiting us." I
[00:24:18] think at this point that is pretty
[00:24:19] inevitable. But I also think that people
[00:24:21] always do this thing when they judge
[00:24:22] cost in the very first hours of even
[00:24:24] having a model, before people have
[00:24:26] really figured out how to use it, and
[00:24:27] before all the norm settle. So I
[00:24:29] wouldn't be surprised if your mileage
[00:24:30] actually goes a bit farther than some of
[00:24:31] the responses that you're seeing. The
[00:24:33] question though is, especially if there
[00:24:35] are strict usage limits, and you're
[00:24:36] going to find yourself on API pricing,
[00:24:38] which is pretty expensive soon. Mat V
[00:24:40] writes, "Serious question. What can you
[00:24:42] do with Fable 5.1 that you can't do with
[00:24:45] Opus, Soul, Kimmi, Composer, or Grok?
[00:24:47] Give me your actual use cases. Tell me
[00:24:49] what I'm missing."
[00:24:51] On the one hand, I think this is the
[00:24:52] right type of question for people to be
[00:24:54] asking. In the same way that pretty much
[00:24:56] every enterprise right now is trying to
[00:24:57] figure out a multi-model architecture
[00:25:00] that allows them to connect the right
[00:25:02] task with the right level of capability,
[00:25:03] most individuals are going to have
[00:25:05] something similar. Where perhaps they
[00:25:07] don't have any sort of automated router,
[00:25:09] but they just understand and have
[00:25:10] designed systems so that they know which
[00:25:12] model and setting to use for different
[00:25:13] types of requests so that they're not
[00:25:15] just burning everything on the most
[00:25:16] state-of-the-art, most expensive model,
[00:25:18] on the highest settings. At the same
[00:25:20] time, there's this idea that's been
[00:25:22] around for a while that the models are
[00:25:24] so good now that for many use cases no
[00:25:26] one can really tell the difference
[00:25:27] between them, and to even consider using
[00:25:29] the most expensive state-of-the-art
[00:25:30] models, you must be deluding yourself
[00:25:32] into thinking that there's actually a
[00:25:33] difference. I reject that pretty
[00:25:36] wholesale. The idea that just because
[00:25:40] multiple models can successfully
[00:25:41] complete a task means that they're all
[00:25:43] interchangeable with one another is akin
[00:25:46] to saying that if two people can
[00:25:47] complete the same work task, it doesn't
[00:25:49] matter which one does because the task
[00:25:51] got done. Now, certainly there are going
[00:25:53] to be tasks for which that is the case,
[00:25:55] and those are precisely the tasks they
[00:25:57] should be optimizing using cheaper
[00:25:59] models for. But when it comes to a lot
[00:26:01] of high-end important work, I still find
[00:26:04] that as capable as all of these models
[00:26:05] are, there are still massive differences
[00:26:07] between them. One thing I strongly
[00:26:09] advocate for is to have a standing slate
[00:26:12] of personal benchmarks for new model
[00:26:14] testing. They don't have to be anyone
[00:26:16] else's tasks, they can just be the
[00:26:17] things that matter to you. And you might
[00:26:19] find that for your particular tasks,
[00:26:21] models that other people are complaining
[00:26:22] about work great and models that other
[00:26:23] people love don't work so well. For me,
[00:26:26] that personal benchmark list includes a
[00:26:27] few things. It's basically some
[00:26:29] combination of research, writing,
[00:26:32] strategic and critical thinking, and
[00:26:34] building, which includes both an
[00:26:35] interface design and an architecture
[00:26:36] component. And what you'll notice is
[00:26:38] that especially when it comes to
[00:26:39] something like writing or strategic
[00:26:41] thinking, a lot of preference is going
[00:26:43] to be subjective. In other words,
[00:26:44] Anthropic can't show me some benchmark
[00:26:46] for iterating on NLW's mad ideas for new
[00:26:49] businesses. That's something that I have
[00:26:51] to see how Fable 5 versus Opus versus
[00:26:53] Soul handle in practice. And even in
[00:26:55] this era of generally capable models, I
[00:26:58] still find massive differences in things
[00:27:00] like that. The reminder here is that for
[00:27:02] all of us, the question when a new model
[00:27:03] comes out is no longer should I switch
[00:27:06] to that model? Instead, it's how does
[00:27:09] that model fit into my personal model
[00:27:11] architecture? For what uses is that
[00:27:14] model better and worth whatever
[00:27:15] financial or other types of costs that
[00:27:17] come with it. The best users in other
[00:27:19] words are going to figure out how to get
[00:27:20] the most out of new models rather than
[00:27:22] just clunking around from one to the
[00:27:23] next with some old idea that you have to
[00:27:25] pick just one. Now, for one last
[00:27:27] qualification on that, I will note that
[00:27:29] if you are not in a financial position
[00:27:31] where you can be blithely shifting
[00:27:32] between models, a lot of these
[00:27:33] considerations get different. And for
[00:27:35] that, the advice that they are all
[00:27:36] pretty generally capable is accurate. It
[00:27:39] certainly is the case that it has never
[00:27:40] been a better time to be locked into
[00:27:42] just one ecosystem because they are all
[00:27:44] so individually capable even if they do
[00:27:45] have different trade-offs. Still, now
[00:27:47] the fun part begins where you get to go
[00:27:49] test and try these things. I'm excited
[00:27:51] to spend some time this Labor Day
[00:27:52] weekend testing things out and I will of
[00:27:54] course report back next week. For now
[00:27:56] though, that is going to do it for
[00:27:57] today's AI Daily Brief. Appreciate you
[00:27:59] listening or watching as always and
[00:28:00] until next time, peace.
