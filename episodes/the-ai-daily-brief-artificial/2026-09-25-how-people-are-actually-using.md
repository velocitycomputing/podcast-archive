---
record_id: "podcast:5b951a25-e57f-410d-bc82-4a34af8657b9"
episode_id: 5b951a25-e57f-410d-bc82-4a34af8657b9
title: How People Are Actually Using Jev
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-people-are-actually-using-jev/5b951a25-e57f-410d-bc82-4a34af8657b9"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-people-are-actually-using-jev/5b951a25-e57f-410d-bc82-4a34af8657b9"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-09-25
played_at: "2026-09-25T12:00:00Z"
play_count: 1
duration_seconds: 1500
source: pocketcasts-history-browser
played_label: September 25
history_order: 39
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: e6eeb0078a3b90604568940893c3517ef56a93bc6655dec1afe5771a378b14e6
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

Jev, built by Typesafe, is a "system one" judgment model: it doesn't write, code, or reason at length, but makes fast, cheap, parallel snap judgments in three forms: pick one of up to 255 options, score on a described 2–10 level scale, or answer yes/no with a probability. Claimed speeds are 20–200x faster and 40–400x cheaper than LLM approaches, at roughly 70–500 ms per call and about $4.20 per million input tokens (output is free). The host walks through six real-world use categories:

- **Analyzing archives:** 724 ads were broken down across 12 questions in 40 seconds for 9 cents, and about 3,300 old posts were tagged for $13.
- **Searching by meaning:** a 586-page SEO internal-link audit ran in 45 seconds, while Opus got through 21 pages.
- **Triaging inbound items:** 100 emails were rated for importance in 453 ms, a downloads-folder invoice sorter was built, and malicious-link flagging was solved in 2 hours.
- **Checking work against rules:** Jev caught 6 of 7 planted writing errors in 0.35 seconds, against Fable 5.1's 7 of 7 in 8.83 seconds, at about 580x lower cost.
- **Speeding up agents:** routing to models or skills cut costs by 50–88%.
- **Instant response:** smart paste that fills form fields from copied text.

The cautions are that Jev gives numbers with no reasoning, so hiring, money, and security uses are risky. It also does poorly at multi-step questions, math, counting, dates, and reading intent, and its consistency is a problem.

For you, the best fits are tasks where the answers can be written down in advance (categories, yes/no, or a scale), there is a pile or stream of items, a wrong answer is cheap or easy to catch, and the evidence fits as text in under 32,000 tokens. The highest-value starting points are inbox or lead triage and routing, running a few fixed questions across a large archive (emails, CRM notes, transcripts, past posts), and turning your style guide's banned phrases into yes/no questions to check every paragraph of a document. If you run lots of Claude Code skills, Jev-based skill selection (injecting only the matching skill) is reported to cut tokens by 88%. Write one judgment per question, describe each scale level in words, and hand-label about 50 examples to test accuracy before trusting it. Since a `typesafe:typesafe-ai` skill is already installed here, you can use it to prototype. The host's companion site, AI daily brief.ai, also has starter prompts and one project idea per category.

## Transcript

[00:00:00] Jev is one of the buzziest models we've
[00:00:02] had in a long time. And that's because
[00:00:04] it's not just another LLM like a GPT6 or
[00:00:08] an Opus or Fable model. It is something
[00:00:10] fundamentally different. But because
[00:00:12] it's different, it's not necessarily
[00:00:13] clear at the beginning exactly what it's
[00:00:15] going to be best used for. With the
[00:00:17] benefit of a week and a half under our
[00:00:19] belts now though, people are discovering
[00:00:20] and sharing a slew of different use
[00:00:22] cases that take advantage of what makes
[00:00:24] Jev unique. And today, we're going to
[00:00:25] get into the best of them and where they
[00:00:27] might be relevant for you. The AI Daily
[00:00:30] Brief is a daily podcast and video about
[00:00:32] the most important news and discussions
[00:00:33] in AI.
[00:00:35] Welcome back to the AI Daily Brief. Over
[00:00:37] the last couple of weeks, one of the
[00:00:39] buzziest new things to come up in the AI
[00:00:41] world has been a new model called Jev.
[00:00:45] Now, what makes Jev interesting is that
[00:00:46] it is not just another LLM that you
[00:00:49] would use for the same thing as GPT6 or
[00:00:51] Opus 55, but actually works in a
[00:00:54] slightly differently and as we will see
[00:00:55] complimentary way. In the 10 days or so
[00:00:58] since launch, not only has there been a
[00:01:00] ton of buzz, I'm talking hundreds of
[00:01:02] different posts on X, which each
[00:01:04] themselves have hundreds or even
[00:01:06] thousands of likes and shares, but that
[00:01:08] attention has also translated into
[00:01:10] significant financial opportunity with
[00:01:11] the information reporting that the
[00:01:13] company is in talks to raise as much as
[00:01:14] $1 billion at a $10 billion or higher
[00:01:17] valuation. That is a decent jump from
[00:01:20] its $40 million seed that was completed
[00:01:21] at a $200 million valuation. But now
[00:01:24] that we've had a chance for people to
[00:01:26] actually get their hands on Jev itself,
[00:01:29] I wanted to go back through and talk
[00:01:30] about how people are actually using this
[00:01:32] thing outside of the buzzy visual and
[00:01:34] game demos that have been all over
[00:01:35] social media. Basically, is Jev
[00:01:38] something that the average person who's
[00:01:39] not a game designer or not a developer
[00:01:42] should be paying attention to and even
[00:01:43] thinking about as part of their larger
[00:01:45] AI stack? Now, to recap what Jev is.
[00:01:48] Previously, I called it a judgment
[00:01:50] model. What Jeb can't do is write in the
[00:01:53] traditional way that you think about
[00:01:55] chatbots writing. Instead, the team at
[00:01:57] Typesafe who built Jev calls it a system
[00:02:00] one model after a concept from Daniel
[00:02:02] Conaman's thinking fast and slow. System
[00:02:04] one thinking is fast instinctive pattern
[00:02:06] matching, i.e. snap judgments and that's
[00:02:09] what Jev is built for. A good way to
[00:02:11] think about a test for whether something
[00:02:12] is a good job for Jev is where you
[00:02:15] repeatedly read something, make a small
[00:02:16] judgment, then take a predictable next
[00:02:18] step. So take for example a file landing
[00:02:20] in your downloads folder. An ordinary
[00:02:22] rule that existing software might have
[00:02:24] would be to classify it as a PDF. But
[00:02:26] what Jev can do is go a step further
[00:02:29] identifying is it an invoice? Which
[00:02:31] projects is it for? And does someone
[00:02:32] need to see it? Once the judgment is
[00:02:34] made, it can be predictably moved on to
[00:02:36] the next step in a system. There are
[00:02:38] three core types of questions that you
[00:02:40] can ask Jev. The first is pick one or
[00:02:43] what Jev calls choice. It answers which
[00:02:45] of these fits. You list up to 255
[00:02:48] options and Jev can find the best fit.
[00:02:51] So an example of this might be which
[00:02:53] team should handle this ticket. Is it
[00:02:54] billing, tech support, sales or other?
[00:02:56] The Jev model is going to give you back
[00:02:58] the pick plus a probability for every
[00:03:00] other option. The second type of
[00:03:02] question that you can ask Jev is what
[00:03:04] they call a score, which is basically
[00:03:05] rating on a scale. You describe each
[00:03:08] level in words from 2 to 10 levels, and
[00:03:10] Jev can answer where something falls. So
[00:03:12] for example, on the scale from calm to
[00:03:15] very angry, how frustrated is this
[00:03:16] customer, you're going to get back from
[00:03:18] Jev a position on that scale as well as
[00:03:20] an indication of how sure the model is.
[00:03:22] The last type of question is a yes or no
[00:03:24] question, what Jeb calls a new, which is
[00:03:26] short for Berni, and it simply answers,
[00:03:28] is this true? So to stay on this
[00:03:30] customer service example, is this person
[00:03:32] explicitly asking for a refund? What
[00:03:35] you're going to get back is a
[00:03:36] probability from 0 to one that the
[00:03:37] statement is true. Hey Stephan and next
[00:03:40] did a really cool very simple
[00:03:42] visualization where he put a pile of
[00:03:44] emojis at the bottom of a screen and
[00:03:46] then into a text box he wrote you can
[00:03:48] type in classifiers like things you can
[00:03:50] wear or things you can wear in winter.
[00:03:52] The emojis that match race to the top or
[00:03:54] fall off if the classification has
[00:03:56] changed. And so what's happening in the
[00:03:58] background is that every emoji is
[00:03:59] getting the same yes or no question.
[00:04:01] Does this match what you typed? And
[00:04:03] importantly nobody labeled or tagged the
[00:04:05] emoji as would happen in traditional
[00:04:07] machine learning. There's no rule, in
[00:04:09] other words, for winter. Every emoji
[00:04:11] gets the same question at the same
[00:04:12] moment. Does this match? And part of
[00:04:14] what you might be recognizing if you're
[00:04:16] watching this demo is that because what
[00:04:17] Jev does is limited and specific, it can
[00:04:20] do it incredibly fast. When Typesafe
[00:04:22] launched the model, they said it can
[00:04:23] work 20 to 200 times faster and 40 to
[00:04:25] 400 times cheaper than comparable
[00:04:27] processes with LLMs. Now, instead of
[00:04:29] this pile of emojis, imagine that the
[00:04:31] pile is your leads, your tickets, your
[00:04:33] documents, or some other big
[00:04:35] undifferiated mass of information.
[00:04:37] Importantly, you can ask many questions
[00:04:40] about the same item all at once. Because
[00:04:42] questions run in parallel, asking the
[00:04:44] 9th or 10th question doesn't cost more
[00:04:46] time. It just costs more tokens. Say,
[00:04:48] for example, you have a single customer
[00:04:50] email. You might want to ask three yes
[00:04:52] or no questions at once. Is the customer
[00:04:54] angry? Did they get a delayed response?
[00:04:56] Are they dealing with an incorrect item?
[00:04:58] These are three separate questions that
[00:05:00] are each going to have their own
[00:05:01] probability. In their testing, Typesafe
[00:05:04] found that 13 questions handled in a
[00:05:06] single call was 12.2 times cheaper and
[00:05:08] 10 times faster than one at a time and
[00:05:10] got to the identical answers. Matthew
[00:05:12] Burman did an analysis of 724 live ads
[00:05:15] with each ad being asked 12 questions.
[00:05:18] One about the hook archetype, one about
[00:05:20] the format, one about the offer, one
[00:05:21] about the CTA intent, one about the
[00:05:23] awareness, etc., etc. He found that that
[00:05:25] single request for the 12 questions for
[00:05:27] that ad took just 173 milliseconds to
[00:05:30] complete. And this is really where the
[00:05:32] power of the model comes in. It's not
[00:05:34] just that it's good at judgment. It's
[00:05:35] that it's fast enough and cheap enough
[00:05:37] to ask and make judgments about
[00:05:39] everything. A million input tokens cost
[00:05:42] just 4.2. And output tokens are free.
[00:05:45] And each call is going to take between
[00:05:47] 70 and 500 milliseconds and as we've
[00:05:49] seen can combine a bunch of different
[00:05:50] questions in a single call. Now,
[00:05:52] importantly, Jev makes trade-offs that
[00:05:55] allow it to be good at the things that
[00:05:56] it does. But that also means that it
[00:05:58] doesn't do certain things. It's not
[00:06:00] going to write code. It's not going to
[00:06:01] draft contracts. And it's not going to
[00:06:03] make nuance decisions that involve a
[00:06:04] variety of factors that aren't
[00:06:06] quantifiable and clear. It's going to be
[00:06:08] used for small judgments at volume.
[00:06:10] Which bucket? How urgent? Is it
[00:06:12] relevant? Is it safe? So, now let's talk
[00:06:14] about six different ways that people are
[00:06:16] actually putting Jeb to work outside of
[00:06:18] just cool demos. A first category is
[00:06:21] analyzing what you already have. A
[00:06:23] second category is searching by meaning.
[00:06:25] A third category is triaging what comes
[00:06:27] in. A fourth category is checking work
[00:06:29] against your rules. A fifth category is
[00:06:32] speeding up AI agents. And a sixth
[00:06:34] category is responding instantly. So
[00:06:36] let's move to category one, analyzing
[00:06:38] what you already have, aka what's in
[00:06:40] this pile. This is basically where
[00:06:42] you're going to take a collection you
[00:06:44] already have, ask Jeb the same questions
[00:06:46] about every item, and then count the
[00:06:48] answers. This is analysis that
[00:06:49] previously could not be justified doing
[00:06:51] by hand, but is now going to take
[00:06:53] seconds and cost sense. One example was
[00:06:55] that from Matthew Burman that we just
[00:06:57] talked about where he analyzed and broke
[00:06:59] down 724 live ads from 37 brands to
[00:07:02] identify every hook, every format, every
[00:07:04] offer, every CTA. The idea is to be able
[00:07:06] to then take this data and compare it to
[00:07:08] what actually performed, giving you
[00:07:10] incredibly deep and complex fine grain
[00:07:12] information about advertising
[00:07:13] performance that would have been
[00:07:15] extremely difficult before. It took 40
[00:07:17] seconds and 9 cents worth of tokens for
[00:07:20] Burman to get the full breakdown of
[00:07:22] those 724 live ads. 2 days later, Burman
[00:07:25] went further and instead of just asking
[00:07:27] those questions in general, this time he
[00:07:29] had Jev Scroll 723 ads as 30 different
[00:07:32] buyer personalities. The personalities
[00:07:35] were archetypes like gym owner, dental
[00:07:37] office manager, toddler mom, or AI
[00:07:39] curious engineer. Jeff's job was to ask
[00:07:41] for every buyer in every ad, would this
[00:07:43] person stop scrolling or keep going? It
[00:07:45] cost 22 cents to get 21,690
[00:07:49] stop or scroll decisions. Now, of
[00:07:51] course, this is not data. This wasn't 30
[00:07:53] actual buyers. It was just buyer
[00:07:55] archetypes as considered by an AI. In
[00:07:58] other words, it's better to view this as
[00:07:59] a hypothesis generator. But it's hard
[00:08:01] not to think that marketing will shift
[00:08:03] to using this as a key part of its
[00:08:04] process to pressure test ad or landing
[00:08:06] page angles before paying for real
[00:08:08] tests. Lots of other folks are running
[00:08:10] Jeb over whole archives, whether that's
[00:08:13] email archives, past exposts, folders of
[00:08:16] documents, or databases of research
[00:08:18] projects. And in each case, what Jeb is
[00:08:20] doing is asking the same few questions,
[00:08:22] but about every single item in the
[00:08:24] archive. Ian Nuttall, for example, had
[00:08:26] Jev ask eight questions each topic,
[00:08:29] hook, and tone about nearly 3,300 of
[00:08:31] their previous exposts to be able to
[00:08:33] then compare that data with engagement
[00:08:35] metrics to get a better sense of what
[00:08:37] actually worked. And by the way, those
[00:08:39] eight questions each across 3,300 posts
[00:08:41] cost about 13. So how might we try
[00:08:44] something like this? Basically any big
[00:08:47] pile of data you have. A year of
[00:08:49] customer emails, CRM notes, a folder of
[00:08:52] meeting transcripts, anything where you
[00:08:54] can write a few simple questions and run
[00:08:56] them against all of those queries.
[00:08:57] That's a potentially useful place for a
[00:08:59] dev job. Category 2 is searching by
[00:09:02] meaning. In other words, which of these
[00:09:04] match what I mean? The idea is to be
[00:09:06] able to describe what you're looking for
[00:09:08] in plain words and let Jeb check every
[00:09:10] candidate. The power is that it can find
[00:09:12] what you mean even when the words don't
[00:09:14] match. There were a bunch of examples of
[00:09:16] this with people basically using it as a
[00:09:18] new approach to natural language search
[00:09:19] on websites. Justine Moore from A16Z
[00:09:22] gave the example of scanning thousands
[00:09:24] of Zillow listings and classifying
[00:09:26] properties by things you can't normally
[00:09:27] filter for, such as architectural style,
[00:09:30] renovation status, or proximity to
[00:09:31] freeways. In one example that piqued my
[00:09:34] interest, Burhan took a 90-minute video
[00:09:36] and was able to clip it based on themes
[00:09:38] that they described in natural language.
[00:09:40] So, for example, across that 90-minute
[00:09:42] video, they were able to look for and
[00:09:44] clip quote their predictions for when AI
[00:09:46] will automate AI research, and they were
[00:09:48] able to find a bunch of examples of that
[00:09:50] in under 2 seconds for under two cents.
[00:09:53] Another example of this is an SEO audit
[00:09:55] where Boura deployed Jev to read all 586
[00:09:58] pages of their website to rebuild the
[00:10:00] site's internal link map which it was
[00:10:02] able to do in 45.1 seconds for 21.
[00:10:05] Claude Opus 5 only got through 21 of
[00:10:07] those pages and spent a buck 43. Boura
[00:10:10] explains internal linking is the perfect
[00:10:12] Jev job. It's not writing. It is 8,790
[00:10:16] yes or no calls. Does this page have a
[00:10:18] real reason to link to that one? and is
[00:10:20] there anchor text already sitting in the
[00:10:22] copy? That is a classification problem
[00:10:24] and we've been paying frontier prices to
[00:10:26] do it one page at a time. A final
[00:10:28] subcategory of the searching by meaning
[00:10:30] is filtering what you read by what you
[00:10:32] care about. So for example, Robin
[00:10:34] Billgill built a realtime AI slop
[00:10:36] detector. As they scroll X, the slop
[00:10:39] detector gives a confidence score on
[00:10:41] that 0 to1 scale about how much it
[00:10:43] thinks a post is AI slop or not,
[00:10:44] blocking out the ones that reach a
[00:10:46] certain confidence threshold. This sort
[00:10:48] of filtering though can be applied in a
[00:10:49] bunch of different ways. Elvis Sonx gave
[00:10:51] an example of letting Jev browse 384
[00:10:54] morning news stories and identifying
[00:10:55] which of them 15 different brands should
[00:10:57] be paying attention to. That was
[00:10:58] completed in 24.9 seconds for 19. And by
[00:11:01] way of comparison, in that same time
[00:11:03] period, Opus 5 got through four of those
[00:11:05] articles, leaving 380 unread. Jev use
[00:11:08] case category 3 is triaging what comes
[00:11:11] in. In other words, what is this and
[00:11:13] where does it go? The kinds of questions
[00:11:15] that people are experimenting with are
[00:11:17] things like, "How important is this
[00:11:19] email? Is this downloaded file an
[00:11:21] invoice? Is this link malicious? Should
[00:11:23] this lead go to sales self-s serve or
[00:11:25] nurture?" One really interesting
[00:11:27] experiment came from Jonathan Unicowski.
[00:11:29] He wrote, "Every email app shows your
[00:11:31] inbox in reverse chronological order.
[00:11:33] What if it was live prioritized by
[00:11:35] importance instead?" Jeb's job in this
[00:11:37] case was to rate every email's
[00:11:39] importance. And in the test, it was able
[00:11:41] to rate a 100 emails in 453 milliseconds
[00:11:44] for about a tenth of a cent with
[00:11:46] Jonathan reporting that Jeb's rating
[00:11:47] matched his own on every single one.
[00:11:50] This is a use case that I want right
[00:11:52] now, not tomorrow. In fact, I want it
[00:11:54] yesterday. And so do all of the people
[00:11:56] who are sitting there beating their
[00:11:57] heads against the wall because I haven't
[00:11:58] responded to them yet. Some other folks
[00:12:00] are experimenting with a pattern of
[00:12:02] asking one quick question per item.
[00:12:04] Marcel Pio, the CTO of Beyond Code,
[00:12:06] writes, "I built a Mac OS app that
[00:12:08] monitors my downloads folder along with
[00:12:09] a customizable set of rules. Is the
[00:12:11] downloaded file an invoice? Move it to a
[00:12:13] special folder with the correct file
[00:12:14] name. No other LLM calls involved, just
[00:12:17] Jev." Dev Ed use Jev for live chat
[00:12:20] moderation, removing swearing and
[00:12:21] negative comments as they arrive. Steven
[00:12:23] Tay of the Dub link shortener fed Jev
[00:12:26] 10,000 malicious domains they'd caught
[00:12:27] before to flag bad links on their free
[00:12:29] shortener service. He wrote, "This has
[00:12:32] been something that we've been wrestling
[00:12:33] with since day one. With Jev, we solved
[00:12:35] it in 2 hours." In fact, this sort of
[00:12:37] triage is so integral to so much of
[00:12:40] business. In a post about 10 Jev use
[00:12:42] cases for a marketer, Yumanx identified
[00:12:44] workflow decisions as one, saying, "Most
[00:12:46] workflows eventually hit the same
[00:12:48] question. What should happen next?"
[00:12:50] That's probably the best place to use
[00:12:52] Jev. Box gave an example having already
[00:12:54] experimented with incident triage where
[00:12:56] Jev is used to judge customer impact and
[00:12:58] severity as well as things like which
[00:12:59] routes it can be escalated to. Udu CRM
[00:13:02] has a proposed module that asks three
[00:13:04] things about every new lead. Their
[00:13:06] priority, their buying readiness, and
[00:13:07] whether it's spam or not. If you had to
[00:13:09] look at just one area to explore,
[00:13:11] especially if you were in a company with
[00:13:13] multiple people touching the same leads
[00:13:14] or customers or contacts, this sort of
[00:13:17] triage and routing is I think where Jev
[00:13:18] is going to become absolutely integral
[00:13:20] basically from the moment that it gets
[00:13:22] integrated into the systems. A fourth
[00:13:24] category of Jev use cases is checking
[00:13:27] work against rules, i.e. does this meet
[00:13:30] the bar. Instead of the standard LLM
[00:13:32] question of please review this, you turn
[00:13:34] please review this into specific
[00:13:36] questions and then ask those questions
[00:13:38] about every draft. One example of this
[00:13:40] came from Langchain, which was grading
[00:13:42] an AI agent's work the same way every
[00:13:44] time. Harrison Chase from Langchain
[00:13:46] pointed out that Jev is quote great for
[00:13:48] evals, especially online evals where you
[00:13:50] want to grade lots of traces. Now, this
[00:13:52] might feel initially like something that
[00:13:53] is more for devs than for other types of
[00:13:55] knowledge workers and companies. But
[00:13:57] given how much all of us are going to
[00:13:58] start putting agents into production or
[00:14:00] managing agents that already exist,
[00:14:01] things support bots, research agents,
[00:14:03] etc., having a better tool to build
[00:14:05] evaluation systems into how we judge
[00:14:07] those agents work seems like it could
[00:14:09] very easily become core infrastructure.
[00:14:12] And the team at every showed how you
[00:14:13] could use this sort of ability to check
[00:14:15] work against rules at mass scale and at
[00:14:17] incredible speed as a way to improve AI
[00:14:19] writing. They planted mistakes on 12
[00:14:22] passages of writing with Jeb catching
[00:14:24] six of seven as compared to Claude Fable
[00:14:26] 5.1s catching all seven. Jeb, however,
[00:14:29] caught at 6 in 0.35 seconds as compared
[00:14:31] to 8.83 seconds for Fable 5.1. And it
[00:14:34] did so at about 580 times cheaper,
[00:14:37] meaning that you could rerun that same
[00:14:38] check a huge number of times and still
[00:14:40] have it be both cheaper and faster than
[00:14:42] using a Frontier model for the same sort
[00:14:44] of review. So, how might you actually
[00:14:46] turn this into something that you would
[00:14:47] use? You'd basically need to go through
[00:14:49] a translation process for your rules for
[00:14:51] writing. So, let's imagine that you had
[00:14:53] a style guide or a list of phrases you
[00:14:55] never want to see. You could turn each
[00:14:57] of those into a yes or no question and
[00:14:59] then run those yes or no questions on
[00:15:01] every paragraph of your next long
[00:15:02] document as a way to ensure no AISMs or
[00:15:05] other writing third rails in your key
[00:15:07] communications. And this gets, I think,
[00:15:09] at one of the biggest rewirings that
[00:15:11] we're going to need to do with Jev. A
[00:15:13] lot of the unique value of Jev is not
[00:15:15] just being able to do a thing. It's
[00:15:18] being able to do a thing at such scale
[00:15:20] that it actually becomes a difference in
[00:15:21] kind rather than a difference in scale.
[00:15:24] Being able to realistically check every
[00:15:26] single sentence in minute detail for
[00:15:28] AISMs, in other words, becomes
[00:15:30] categorically different from just
[00:15:31] running a generic LLM check across the
[00:15:33] document as a whole. The fifth category
[00:15:36] of use cases that lots of people were
[00:15:38] experimenting with admittedly does get a
[00:15:40] little bit closer to the developer
[00:15:41] realm, but I think at least for the sake
[00:15:43] of completeness, it's still worth
[00:15:44] discussing. These use cases you might
[00:15:46] sum up as speeding up your AI agents.
[00:15:48] And a lot of this is around the sort of
[00:15:50] model routing that we've been talking
[00:15:51] about for the past several months. The
[00:15:53] kinds of questions people were asking
[00:15:54] were things like which model can handle
[00:15:56] this task? How much reasoning does this
[00:15:58] step need? Which skill fits this
[00:16:01] request, if any? Is this old tool output
[00:16:03] still relevant? You can see how in each
[00:16:05] of these cases, the common thread is
[00:16:07] people using these small automated micro
[00:16:10] judgments to route an agent to the right
[00:16:11] level of intelligence, the right
[00:16:13] context, the right skills, the right
[00:16:14] tools to do whatever its job is in the
[00:16:17] most efficient way possible. Vchen
[00:16:19] wrote, "People use Jev to pick a model
[00:16:21] before a task. I made it change GPT6
[00:16:23] reasonings effort inside codeex during
[00:16:25] the task. More thinking when stuck, less
[00:16:27] for routine steps. And in their test,
[00:16:29] they found 50% lower Astra costs while
[00:16:32] also getting faster runs. People are
[00:16:34] also using Jev to manage the context
[00:16:36] window. Daniel Son built something
[00:16:38] called Jev skill suggestion for Claude
[00:16:40] code where quote, "For every request,
[00:16:42] Jev classifies which skill best matches
[00:16:44] the task, then injects only that skill
[00:16:46] into Claude's context." This led to an
[00:16:49] 88% decrease in tokens and cost. I know
[00:16:52] a lot of even you formerly
[00:16:53] non-developers have started to be
[00:16:55] sufficiently proficient with things like
[00:16:56] codecs and cloud code that you've built
[00:16:58] up big skills libraries and these sorts
[00:17:00] of dev based tools are potentially a way
[00:17:02] to stop sending all of those libraries
[00:17:04] to the model with every single request.
[00:17:07] And one thing to note here is that while
[00:17:08] a lot of these use cases that we're
[00:17:10] discussing are at this stage individual
[00:17:12] experiments, you're also going to see
[00:17:13] Jev and judgment models like it built
[00:17:15] natively into the tools and harnesses we
[00:17:17] use. AJ Aspher, for example, wrote, "We
[00:17:20] built a new harness using Jev that cuts
[00:17:22] the cost of repetitive work by 90%." The
[00:17:25] harness learns the job as it runs,
[00:17:27] moving steps from LLM calls to code. The
[00:17:30] example they gave was compliance alerts,
[00:17:31] and they measured the cost per alert,
[00:17:33] batch by batch, with each batch
[00:17:35] representing 50 of those compliance
[00:17:36] alerts. At the beginning, the cost per
[00:17:38] alert was about $2.95, but by alert
[00:17:41] 10,000, it was down to just 25.
[00:17:44] A sixth category of Jev use cases are
[00:17:48] about instant response. What does this
[00:17:50] person want right now? A lot of people
[00:17:53] were experimenting with some version of
[00:17:54] this. Marcus Low wrote, "What if copy
[00:17:57] paste was smart? Copy a resume, paste
[00:17:59] into an application, and the fields fill
[00:18:01] themselves." Norman on X also did a
[00:18:03] version of this. Splitting the pasted
[00:18:05] text into pieces, working out what each
[00:18:06] field is, matching them, checking
[00:18:08] against the original, and pasting only
[00:18:09] the confident matches. Given how much
[00:18:12] work at work is moving details from one
[00:18:15] format i.e. emails, PDFs, meeting notes,
[00:18:17] etc. into other places where that
[00:18:19] information is supposed to live like
[00:18:21] CRM, intake forms or templates. This is
[00:18:23] a category of use cases that feels very
[00:18:25] very relevant. Now, just as important as
[00:18:28] knowing where Jev is useful is knowing
[00:18:30] where you got to be careful with it as
[00:18:32] well. A couple places that I think
[00:18:33] warrant greater caution are areas like
[00:18:35] hiring, money, and security. on hiring.
[00:18:38] You can see how if Del used by a set of
[00:18:40] applications, you might be tempted to
[00:18:41] use something like Jev to rank them. But
[00:18:43] the problem is that even if you've given
[00:18:44] it good criteria, Jev is going to return
[00:18:46] with a number that doesn't have any
[00:18:48] reasoning attached. This, by the way, is
[00:18:50] a great example of where you might want
[00:18:52] to build a more complex system that uses
[00:18:54] multiple types of AI. Imagine you do
[00:18:56] that same sort of ranking with Jev, but
[00:18:58] then automatically have other types of
[00:18:59] LLM review, for example, for bubble
[00:19:01] candidates that might be deserving of a
[00:19:03] second look. Types safe, the makers of
[00:19:05] Jev, actually even try to be clear about
[00:19:07] what they think Jev is bad at. Some of
[00:19:10] the things they put include multi-step
[00:19:12] questions where they see accuracy drop
[00:19:13] with each hop. They point out that Jev
[00:19:15] isn't really good at counting math or
[00:19:17] dates, that it can extract the facts,
[00:19:19] but that you're going to want to do the
[00:19:20] actual math elsewhere. And they also
[00:19:22] point out some other issues like
[00:19:23] problems with consistency and problems
[00:19:25] with reading intent. So, if you're
[00:19:27] trying to figure out if a task is a good
[00:19:28] fit for Jev, four criteria might help.
[00:19:31] The first is that you can write down the
[00:19:33] answers in advance. Think categories, a
[00:19:36] yes or no binary, a scale. If the answer
[00:19:38] is a sentence or a calculation, that's
[00:19:41] probably not a good fit for Jev's sort
[00:19:42] of judgment model. Criteria number two
[00:19:45] is about volume. There's a pile or a
[00:19:47] stream, such as hundreds of tickets,
[00:19:49] hundreds of emails, things like that. A
[00:19:51] third criteria is about stakes, where a
[00:19:54] wrong answer is cheap or it's easy to
[00:19:56] catch. Basically, although I'm calling
[00:19:58] it a judgment model, you don't want to
[00:19:59] leave things up to its judgment alone if
[00:20:01] getting it wrong has big consequences. A
[00:20:04] final criteria is whether you can give
[00:20:05] it the evidence that it needs as text in
[00:20:08] under 32,000 tokens. Once you've figured
[00:20:10] out a good task, the next step is going
[00:20:12] to be to write good questions. Some of
[00:20:14] the tips there from across all of these
[00:20:16] different examples are things like one
[00:20:18] judgment per question. In other words, a
[00:20:20] not so good question is, is this a good
[00:20:21] lead? Cuz that's actually not one
[00:20:23] judgment. That's a whole bunch of
[00:20:25] different judgments embedded in one good
[00:20:27] lead might refer to how good a fit the
[00:20:29] industry is for your service, whether
[00:20:31] the company size matches who you like to
[00:20:33] serve, how strong their buying intent
[00:20:35] is, etc., etc., etc. Basically, you're
[00:20:37] going to want to break questions into
[00:20:38] their constituent parts. If your
[00:20:40] question involves a scale, you need to
[00:20:42] describe each level of that scale in
[00:20:43] words. And you also might even want to
[00:20:45] take advantage of Jeff scale
[00:20:46] opportunities to ask more questions than
[00:20:48] you think that you need. Lastly, like
[00:20:50] everything with AI, you're going to want
[00:20:52] to do some tests before you actually
[00:20:53] trust it in production. It might be a
[00:20:56] pain, but if you are using that email
[00:20:57] classifier, for example, to try to
[00:20:59] organize things based on priority, maybe
[00:21:01] you want to label 50 emails yourself as
[00:21:03] a test and see how it compares to make
[00:21:05] sure it's actually going to do for you
[00:21:06] what you want it to do. Now, as we wrap
[00:21:09] up, I will be posting this presentation
[00:21:10] that I've been working through on this
[00:21:12] episode's companion site on AI daily
[00:21:13] brief.ai. And the last couple of pages
[00:21:15] get a little bit more practical with one
[00:21:17] idea for each project in the six use
[00:21:19] case areas. Things like a content
[00:21:21] archive analyzer, a research raider, an
[00:21:23] inbox triager, a rewrite checker, etc.
[00:21:26] And there'll even be a starter prompt in
[00:21:28] there as well. In the first 10 days
[00:21:29] since Jev was released, we've gone from
[00:21:32] buzzy exciting concept to actually
[00:21:34] valuable production use cases extremely
[00:21:36] quickly. And yet, because this is at
[00:21:39] core a new primitive in its ability to
[00:21:41] apply simple judgment at scale, at
[00:21:43] speed, and for effectively no money, I
[00:21:46] think it's going to take some time for
[00:21:47] us to really figure out just how deeply
[00:21:49] we can weave this into all sorts of
[00:21:51] different use cases. As more and more
[00:21:53] come online, I will come back and share
[00:21:54] the best of them. For now though, that
[00:21:56] is going to do it for today's AI daily
[00:21:57] brief. I appreciate you listening or
[00:21:59] watching as always and until next time,
[00:22:01] peace.
