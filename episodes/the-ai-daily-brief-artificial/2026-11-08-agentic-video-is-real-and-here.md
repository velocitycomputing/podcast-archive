---
record_id: "podcast:221f5d59-1318-4b17-96ae-693b07b50822"
episode_id: 221f5d59-1318-4b17-96ae-693b07b50822
title: Agentic Video Is Real and Here’s What You Should Try
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/agentic-video-is-real-and-heres-what-you-should-try/221f5d59-1318-4b17-96ae-693b07b50822"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/agentic-video-is-real-and-heres-what-you-should-try/221f5d59-1318-4b17-96ae-693b07b50822"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-11-08
played_at: "2026-11-08T12:00:00Z"
play_count: 1
duration_seconds: 1800
source: pocketcasts-history-browser
played_label: November 8
history_order: 6
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 603999e0983ee4aab107d286124236da5a7a759da44779c12b482dbf56414452
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

After Opus 4.5, followed by GPT 5.2, triggered a step change in agentic coding, the episode argues that Opus 5.5 is producing a similar but subtler step change in video editing, letting non-coders and non-editors produce edited, graphics-rich video through natural-language workflows in Codex and Claude Code rather than only dedicated tools like Descript’s Underlord, Adobe’s Firefly AI Assistant, or Adobe’s Paper Edit for Premiere. It describes eight shifts: editing as conversation; AI “watching” or approximating footage via transcripts/timestamps, with Google’s Agentic Video Understanding launched in early September and claimed to be up to 88% more token efficient and about 7% more accurate, especially on 90-minute lectures or multi-hour recordings; connectors bringing meeting recordings, calls, demos, docs, and dashboards into agents; computer-use agents recording demos; Claude Code creating animations with React and Remotion and using external image APIs; improved generated footage from Kling 4.0 and Gemini Omni 1.1 plus normalized generated audio after VO 3.1, Runway Gen 4.5, and Kling 3.0; digital-twin avatars and synthetic voice for dubbing/translation; and integration inside Loom, Premiere, Firefly, and especially end-to-end management from Codex or Claude Code. It also notes limits—generated clips remain seconds long, timeline editing needs multiple passes, and costs can rise—then proposes six reasons video beats other formats: showing beats telling, audiences who won’t read docs, repeated explanations, multilingual needs, existing recorded raw material, and moments where conviction or emotion matters. Internal use cases include concept videos, 2–4 minute meeting highlights, customer-feedback videos for decision makers, exec pre-reads, self-updating SOP/onboarding/UI videos, narrated charts, role-based onboarding, and handoff videos; external ideas include repurposing talks, webinars, or podcasts into TikTok, Reels, or YouTube Shorts clips and experimenting with long-form thought leadership. Sponsor segments name KPMG and the University of Texas at Austin, whose study of more than 500 early-career professionals found “AI amplifiers” succeed by guiding, evaluating, and refining AI outputs, plus Robots and Pencils, C Data’s Connect AI Gateway, and Blitzy’s codebase reverse-engineering and autonomous epic delivery.

For the user, the actionable move is to treat video as a workflow decision, not just a marketing tactic, and to test one low-risk internal use case first: turn a high-stakes meeting recording into a 2–4 minute highlight, make an exec pre-read from a strategy doc, or build a self-updating onboarding/SOP video that agents refresh quarterly. The user should inventory recurring communications that meet the episode’s criteria—things they explain repeatedly, things executives won’t read, things that need translation, things with existing recordings, or things where motion clarifies a process—and then pilot with available tools: Codex or Claude Code plus connectors to meeting/call recordings, docs, and dashboards; Loom or a phone for raw talking-head capture; AI prompts to find moments, trim filler, assemble cuts, add captions, and generate or source graphics; and Google Agentic Video Understanding if large files are involved. Follow-up questions should include: which meetings or documents are valuable but unread, which processes change often enough to justify a living video, which audiences need multilingual versions, what connectors and permissions already exist, what privacy/consent rules apply to recordings and synthetic voice/avatars, and what token/video-generation budget is acceptable. The user should avoid making every meeting a video, verify AI-edited clips for accuracy, prefer animations over uncanny generated b-roll when clarity matters, and measure success by time saved, comprehension, engagement, and whether the video changes a decision or reduces repeated explanation. The material contains no health claims or health implications; the actionable area is communication, workflow automation, and content-production decisions.

## Transcript

When Opus 4.5 came in November of last year, it took about a month, honestly, till through the holiday break, for people to really realize that it represented not just another incremental change, but in fact, a step change in agentic coding capabilities.
What happened after that set up the entirety of 2026, where agentic coding became by far the most important and most dominant AI use case, and set us all racing to figure out how we could bring coding into our normal knowledge worker lives.
Opus 5.5 has been out for a similar amount of time, and people are once again discovering that it represents a more subtle but significant step change when it comes to not coding capabilities, but video editing.
In today's episode, we're exploring both what changed and what video use cases people who haven't made videos before should be considering based on the new capabilities.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, Robots and Pencils, C Data, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AI DailyBrief, or you can subscribe on Apple Podcasts.
And if you want to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
Today, we have an operator's cut that is very, very on trend.
Whenever we get a new model, people race to see based on benchmarks or their own experience how it compares at doing the tasks that are their most important, the ones that they do all the time.
Sometimes, however, usually with the benefit of a few weeks or even a month or two of experience, people start to realize that a model, or more often a set of models released around the same time, have unlocked some new capability that allows them to do either something they were doing in a totally different way, or even something that they had never been able to do before.
The quintessential example of this is the models around Opus 4.5, which was quickly followed by GPT 5.2, I believe, unlocking agentic coding in a real way and making it so that those of us who were non-coders and not developers weren't just using the simplified tools, but could actually just use the core models in their own native interfaces and in their own native harnesses to build and code things of increasingly higher complexity.
For a lot of knowledge workers, the entire story of 2026 has been in figuring out how that new set of agentic coding capabilities was going to change their work.
Over the past month, I have seen more and more people come to a determination that right now, thanks especially to Opus 5.5, we're experiencing something similar with video editing.
Now, already, in the last decade of TikTok and YouTube, more people than ever have been not just consuming video, but creating it.
But there have been, of course, fairly significant limits to what those Nouvea creators could do.
Those limits are increasingly gone.
And now, it is increasingly viable for knowledge workers who have never spent a ton of time learning how to make videos to not just create short-form vertical videos with their iPhones and CapCut, but to actually produce quality, edited, graphic-enriched video.
And my guess is that over the next six to 12 months, you're going to see more people using video for more things than ever before.
So in this episode, we're going to talk about what changed and what you should try.
First up, what changed.
To understand how the latest generation of AI models have changed video editing and creation, it's worth thinking step by step about what is actually involved in producing video and who did it before.
Despite what our phones have trained us to think, producing a video is not actually just pointing a camera at something and letting it rip.
First of all, there's the planning that can involve the script and structuring, where you're thinking about what you want that video to be about, how you want it to look and feel, what beats or narrative elements you want within it, and roughly what sequence they go in.
There's the background material and B-roll that might be involved in making the video depending on what it is.
There is, yes, of course, the recording itself, but then there's the editing, the cutting, the assembling, the tweaking, the sound perfection, all of that.
And as if all that weren't enough, there's also graphics and animations to take it to that next level.
And depending on how widely you want it distributed, the potential for translations, and even in the absence of that, the cutdowns that allow you to make shorter videos, which are optimized for the distribution channels like social media.
A lot of steps in the past tended to mean either a lot of people or a small number of people working some serious overtime.
So how did models start to shift this?
Well, the first change was that editing became a conversation.
There had already been a bunch of updates over the past couple of years around how we edit videos.
The script, for example, helped innovate timeline-based editing where you could simply highlight the words of a script and delete or modify them in some way, which already simplified the process.
But that went to the next level when the models got good enough to simply explain to them what you wanted with English language prompts.
Find the good takes, trim silences and filler, place B-roll, lay a first cut.
These are the types of things you can say to these models now and they can actually do it.
And importantly, this was not just dedicated tools like Descript's Agent Underlord or Adobe's Firefly AI Assistant or Adobe's Paper Edit for Premiere.
With the latest generation of models, these became core capabilities of Codex and Claude Code as well.
The second big change is that AI can now watch footage.
The slowest part of editing was always the watching.
And in some ways, this is the change that I think people are underestimating.
With the latest generation of models, you can realistically ask things like: find the three moments where customers complained about onboarding across 20 hours of calls.
And the models can go do that.
Now, for some of the models, they're not actually watching the video.
They're using the transcript and timestamps to approximate it.
But even that's starting to shift.
Google launched Agentic Video Understanding at the beginning of September, and they say that it's up to 88% more token efficient and around 7% more accurate and sees its biggest gains on bigger files like 90-minute lectures or multi-hour recordings.
This ability to watch or approximate watching means in short that when you're having that conversation about editing, it can actually go deliver against it.
The third big change is that the series of connectors that now surround our most important models can bring in the raw material that's required to make lots of different types of videos work.
This is especially true for internal facing video, which is going to be a major topic that we discuss in the What You Should Try section, where connectors give easy access to meeting recordings, call recordings, demos, docs, dashboards.
You don't have to reinvent the wheel to go get those things or have some complicated system for the model reaching them.
There are so many connectors that already exist from all those different apps and locations to bring that material directly into the model that's going to do the watching and editing.
On top of that, thanks to advancements in computer use, agents can even increasingly do the recording.
This is going to matter for types of videos like demos, where the agent can not only plan the demo, but actually open the page in its own browser in its virtual computer and record its own demo with an animated cursor.
Now, this might be a nascent capability, but it does exist and it's going to get nothing but better.
Another huge change is the ability for AI to animate things and bring those animations into your video.
Cloud Code, for example, can write animations as React and use remotion agent skills to render the file.
That native integration has completely transformed Claude's ability to include animations into videos.
And animations in this case aren't just useful for looking pretty or cool or keeping people's attention during videos, although that's certainly been extraordinarily valuable for a long form asset like I'm producing on how we got there.
Animations can also be an extremely valuable way to explain complex or dense information.
The old maxim of a picture being worth a thousand words has always been true, and animations can take that to the next level.
Now, further speaking to the fact that all of these systems are increasingly integrated and you can set things up however you need, even though Claude Code doesn't have native image generation, you can use APIs like OpenAI's image generation APIs or other image-dedicated APIs to give Claude Code that capacity as well, even if you want to use a model like Opus 5.5 to manage things overall.
Now, on top of animations, change number six is that generated footage has also made major improvements over the last few months.
Between Kling 4.0 and Gemini Omni 1.1, you've got better, longer, higher quality, and more controllable generated clips, which can provide b-roll to the extent that you don't have access to something from existing stock footage.
What's more, sound in generated video has become normalized.
Ever since VO 3.1, Runway Gen 4.5, and Kling 3.0, the leading video generation models have also generated audio with the picture.
Now, I will warn that not all generated footage escapes the Uncanny valley, and certainly I have found in our process with how we got here that animations work a lot better for our purposes than generated b-roll, but there are plenty of settings where I can imagine generated footage that is in animations being extremely useful.
A seventh change, which is one that actually happened pretty early but has gotten new context and life because of the other changes, is that the digital twin models for video avatars as well as synthetic voice copies have themselves brought other opportunities.
You're starting to see some prominent video creators experiment with secondary channels that are all AI versions of themselves, although I think it's fair to say that the jury is still out on whether those actually have a place in the video ecosystem or where people still reject them as being weird and synthetic in some way.
Even if in general though, people decide that they don't want social media avatars and you still have to record your own face for certain types of videos, there are plenty of settings where avatars and voice twins are extremely valuable inside of a work context.
Think AI dubbing and translation for multiple languages across an international company.
That's something where the value of the output so clearly outweighs any potential weirdness in the avatar that it's still opening up incredibly valuable use cases.
Finally, change eight is that a lot of these capabilities are already arriving inside tools that you're using.
And I think that this cuts both ways.
Not only are the existing tools like Loom or Premiere or Firefly adding these advanced video features, I think the more important one is that you can now just manage this end-to-end from your main platforms of Codex or Claude Code.
Way more than any one particular video tool, I think the democratization of video is going to come from within those harnesses that are offered by OpenAI and Anthropic.
Now to be clear, everything is not perfect and there's still lots of challenges.
Generated clips remain seconds long, not minutes.
Timeline editing is not perfect and often requires multiple passes.
The cost of advanced animation, video generation, and editing can certainly get expensive fast.
And yet, none of these things change the fact that some fundamental inflection point has been met where the average knowledge worker, I believe, should now be spending at least some time thinking about whether they can use video to aid in their work communications in some way.
Let's move on now to what those knowledge workers should actually try to use video for.
And while I am going to get into specific examples of use cases, I think it's valuable to maybe start with the principles as everyone's experience work context is different, and it may be more useful to understand the circumstances under which a video beats the format that you'd otherwise use.
I think there are six criteria when that happens.
The first is when showing beats telling.
And the principle here is basically: if a picture helps or is better than a description alone, and the thing that you're showing a picture of would benefit from any sort of movement or pacing, that's a good candidate for a video.
Sometimes it's going to be an actual visual asset like UI.
Sometimes that's going to be a multi-step process like a workflow, where showing the steps moving from one to the other is going to be more valuable than just describing it.
Another example that's maybe a little less obvious is numbers changing.
Think the difference between Q1 and Q2 in the same way that a chart helps dramatize that.
A video that shows the flow between them can take that to the next level.
The second criteria is less about the best native format for conveying the information and more realistic acknowledgement of the limitations of your audience.
You can basically ask yourself: who needs this thing that I'm making but won't actually read the doc?
Time-constrained executives, frontline teams who are handling the front lines, customers who don't want a block of text.
Anything that's for those types of audiences who have natural limits to their attention spans is another good candidate for video.
Criteria three for where a video might beat your other formats is when you give the same explanation over and over again.
So think about what do I or what does my company explain on repeat?
Onboarding is a great example, customer education could be another example.
And something that we'll get into that's a new capability is the fact that increasingly, these videos will be able to update themselves in a way that wasn't possible before.
A fourth potential criteria for where a video could work is when the asset needs to exist and operate in more than one language.
This is one of those things that used to be extremely difficult that now AI has made incidental.
A fifth category for when to consider using video is when a bunch of stuff is already sitting there recorded and just needs to be put together.
Basically where the raw material already exists.
And some of these will actually be transposing one type of video to another.
Think about it like this: Is anyone going to watch a 60-minute Zoom that they weren't on?
Absolutely not.
But would they watch a 90-second version or even a two or three-minute version with the highlights?
It's a lot more plausible.
The sixth condition that might make you want to consider video instead of a different format is areas where conviction matters, where you want something to land, where you want to convey the emotions behind a potential decision.
It's certainly not that you can't do that with words, but video gives you a more comprehensive medium that can, if done well, better convey that conviction even if you're not there to pass it on yourself.
A new study from KPMG and the University of Texas at Austin found that when people work with AI, similar skills don't guarantee similar outcomes.
Researchers studied more than 500 early career professionals and found that the best performers consistently amplify the value of AI by guiding, evaluating, and refining its outputs.
These top performers, called AI amplifiers, weren't defined by what they knew alone, but by how they worked with AI.
Learn more about what separates AI amplifiers from everyone else at kpmg.com/slash uslash AI amplifiers.
At this point, it's no longer a question of whether companies are actively using AI.
Using it well, on the other hand, is a whole different story.
Robots and Pencils, though, is a company that I can point to that is actually built for this time.
They're an applied AI engineering firm working directly with clients on problems that matter to the business, not experiments that live in a slide deck.
Every engagement starts by working backwards from the outcome a client actually needs.
If you're trying to tell real AI engineering apart from noise in this space, that's the difference maker.
Head to robotsandpencils.com.
This episode is brought to you by C Data.
Token spend is climbing, security is holding agents back, and companies rolling out AI initiatives might not know how it's truly being used.
The root cause, AI is cut off from the systems and context your business runs on.
That's why C Data built Connect AI Gateway, one control point between your AI and your systems.
Connect AI Gateway is not just another static model router.
Prompts get intelligently routed to the right model with exactly the tools and data it needs, governed down to the record.
The result?
Accurate answers at a fraction of the token cost with a context engine that learns your business with every interaction.
Built on the connectivity layer, powering Palantir, Google, Salesforce, and hundreds more.
Give it a try and start your free trial at cdata.ai.
That's c as in connect data.ai.
Every AI coding tool on the market does the same thing first.
It starts writing code.
Blitzy does the opposite.
Before writing a single line, Blitzy spends days reverse engineering your entire code base.
Thousands of agents ingest millions of lines, mapping every dependency, every undocumented constraint, every architectural decision made over the last decade.
The result is a dynamic knowledge graph that understands your software the way a principal engineer would after 30 years in the building.
Other tools guess at context with grep searches and markdown files.
Blitzy never guesses.
It builds true understanding first, then delivers over 80% of entire software epics autonomously.
Validated, end-to-end tested production-grade pull requests.
That's why Fortune 500 engineering teams trust Blitzy with the code bases that matter most.
See for yourself at blitzy.com.
That's B-L-I-T-Z-Y.com.
So, with those criteria in mind, let's actually move on now to a set of specific ideas and use cases that I think have a lot of applicability across a lot of different types of environments, work, and workplaces.
And we're actually going to start first with those workplace-related ideas.
I think a lot of people, when they hear video, they assume that we're talking about something external-facing, something for marketing.
But a huge amount of the communication that could get differentiated value from video is actually internal-facing.
Use case one is the concept video, showing the thing that doesn't exist yet.
Now, already we've gotten incredible advances in tools to show off our concepts.
One of the best uses for vibe coding is to be able to explain some new feature that you want, even if you're not a developer, for example.
But a concept video can be anything from a UI to a new event you want to hold to something else entirely.
And video is inherently so much more information-dense than text that anything from very standard product feature sort of concepts to store layouts, reorganizations, customer journeys, new processes, using a concept video for that work, I think, has major opportunity.
So, what would it look like to actually do that?
Well, if you're dealing with a product, it might still start with a vibe-coded prototype.
From there, either you could walk through it using something like Loom, or with computer use, you could simply let an agent record the walkthrough, and from there, even generate ideas of where it could go in the future.
For these more abstract concepts, like a new onboarding flow or a reorg, I think the place to start is: one, articulating the concept, which once again you can do with AI, whatever the concept is that you're trying to convey.
Two, discussing with your AI build partner what the right way to visualize that concept is, and then three, thinking about what the anchor visual content for that video is going to be.
So, the new onboarding flow, the anchor visual content will likely either be a walkthrough of the flow, if it can be done with existing parts, or again, some demonstration or prototype.
A new store layout, on the other hand, might start with a floor plan and also include mock-ups and renderings of what that store might look like.
In any case, your AI build partner is going to be able to help you flesh out the concept, pick those visuals, generate those visuals if necessary, plan and script the video, execute the recording of said video, find the relevant external assets if there are any to be included in that video, and then edit it all into one complete package.
Video use case number two.
Again, we're still internal facing.
This is one I mentioned before, but that two, three, four-minute version of the meeting is an incredible use of the new video editing capabilities of AI.
Now, some of you might rightly point out that for a lot of meetings, the written AI summary might be sufficient.
And that absolutely could be the case, especially if it's a sort of De Regor standard stand-up type meeting where there's not a lot of particularly new information and there's not a lot of debate or discussion.
But what about where you missed the meeting, where there was some meaningful and even intense conversation or debate about a particular decision?
Having AI be able to take the raw recording and hone in on that important piece and show you not just the transcript, but the actual exchanges as they happened, I think could be quite a valuable use case.
So, this is one where it's a great example of we're not trying to turn everything into a video, and frankly, it's pretty unlikely that most meetings that we hold are going to be video worthy.
But for the ones that are, this could be a game changer.
Now, I would also humbly submit that if a meeting isn't video worthy, maybe don't have that meeting and maybe just do it via text in the first place, but that's a whole separate conversation.
A third internal video use case is about giving people inside the company access to what customers outside the company are saying.
This is relevant if the company does sales calls, has records of recordings of support calls, or does any sort of recorded customer research.
And the value of video here is really two parts.
The first part is the process of aggregating and then curating the most important themes from all of that raw information.
And this is not something to be clear that needs a video output to be valuable.
In general, it is a great use case of AI to be able to take a huge amount of aggregate information, like customer feedback, and turn it into actionable themes and key insights.
But sometimes those things don't matter unless they can actually find their way to the decision makers inside the company.
And that's where video can be really valuable.
The fourth internal use case idea gets back to that idea that the people who often need the information most are the least likely to take the time to get it.
For shorthand, we're calling this the exec pre-read, but it's any time you need to get a leader or an executive team up to speed fast and frankly conversant in some important strategy document or business case, think the type of stuff that they need before going into an important meeting.
Now, maybe some of you are sitting there feeling like it's overly cynical to rank an asset built around the presumption of executives not reading things so highly.
And if your company functions well enough that that is surprising to you, well, my friends, I am very impressed with your company.
The fifth internal use case idea isn't even really a specific use case as much as a new category which I think is going to be extremely exciting and which is uniquely the domain of a Gentic video.
And that's the video that updates itself.
One of the reasons that we don't currently make videos is a rational calculation of the cost in terms of time and money to make them and their likely shelf life.
For example, if you have how-tos or standard operating procedures or UI overviews or anything like that, which changes with any sort of frequency, whether it's annually or every six months or even every quarter, justifying taking the time to make a video for those things where that video is going to be out of date in just three or six months has historically likely just not been worth it.
But now that we can build agentic video pipelines where agents can take a mission and mandate and be in charge of everything from sourcing the raw materials to writing or updating the script to creating the visuals to editing the final document, you can build those pipelines so that at some regular cadence, that video actually updates itself.
And this is not some far-off future capability.
You can set this up in clawed code right now.
This turns video from a one-time point asset to a living asset that can be updated as frequently as is necessary at only the cost of the setup and the tokens to do the updating.
A few more internal facing ideas, and we'll start to go through them a little bit more quickly now as there are lots of them.
I think showing numbers in motion can be incredibly valuable and is a type of video that AI can just crush right out of the gate right now.
If dashboards show where things stand, a narrated chart shows what changed and why, and that's exactly the type of animation and underlying data source and output that can be turned into one of those self-updating videos like we were just discussing.
Role-based onboarding is another great candidate, given how much raw information exists out there, like wiki pages, existing recordings, clips from past meetings, explainers for complicated things like comp plans, data architectures, pricing models, new policies.
And if you're skeptical here, here would be my challenge: pick something like that that you're in charge of explaining to people and just go ramble at ChatGPT or Claude about it and task it with coming up with a better way of communicating it.
This is the type of thing that AI thrives at: just taking raw inputs, restructuring them, and thinking about how to coherently output it in a simple way.
And now that simple way can be animated.
One additional internal idea before we turn external is the handoff video.
One of the biggest cost centers for companies is transitions between personnel.
And that doesn't just mean when someone leaves the company, it can also mean when someone is going out on pregnancy leave or when they're just switching roles or even when they're just going away for a vacation depending on the timing.
There is always something lost in translation, and usually that person who's doing the switching or leaving is flat out right to the last minute and doesn't have a lot of time to communicate everything that they might otherwise like to to their successor.
The reality though is that talking is much easier than writing.
It's much faster than writing.
It's much easier to be comprehensive.
It doesn't force you to have as well-structured thoughts.
And so once again, this is something where you can just let people who are going through those transitions ramble and have the AI do the heavy lifting of turning that into a handoff video that can help the next person coming in.
Now the final set of ideas is going to be external facing.
And here would be my challenge to you.
As I said before, I think a lot of folks are intimidated by the idea of external facing video, even if they recognize how valuable and powerful it can be.
Already the advent of short-form video platforms, like dedicated platforms like TikTok, or just the key features of other platforms like Instagram Reels or YouTube Shorts, have transitioned our society to consuming a lot more information in the form of short-form video.
And while the new capability of AI to edit and produce videos end-to-end is not on its own going to give you everything you need for a new external video strategy, I would encourage more of you to actually go experiment and see if the experience and output is valuable enough to invest more in.
So, a couple ideas on that front.
First of all, we've been talking about all of this internal facing material.
Well, if you have a lot of internal facing material, whether that's talks or webinars, or maybe things that relate to you personally like podcast appearances, any of that can become clips that are purpose-built for those short-form platforms.
And in this way, you're not having to produce net new video.
You're taking video assets that already exist or audio assets that already exist, because that would work as well, and getting them remade for a different medium.
The second idea, though, and again, I want to push you on this, is to invest in some experiments around long-form thought leadership.
It is almost certainly the case that by virtue of the experience that you've had, the time that you've had in your role, in your industry, doing whatever it is you do, you've built up a canon of knowledge and experiences that would be valuable for someone else.
Now, it is a skill in and of itself to know which of those things that you have learned are valuable externally and not just to you.
But if you have even an iota of an idea towards that end, I would encourage you to collaborate with an AI on some idea for a long-form thought leadership video.
The simplest version of this is to pick a topic and just ramble to camera using Loom or just your phone, and then letting AI handle the cuts, the graphics, and everything else from there.
The other approach, though, is you can be more intentional and actually architect and plan that video a little bit more.
Maybe you still do that first ramble, but you instead work with the AI to turn that into a more succinct and clear script that's still in your voice, but then you perform that script rather than just the raw ramble, and that's the material that the AI builds from.
Regardless of the approach that you take, I think that more of us out there could be doing more long-form thought leadership, and the world would be better for it if we did.
Now, the next couple ideas have to do more with sales and accounts.
One use case that has long been floating around, but which is now actually really viable, is these sort of personalized account videos where you take one base video but can then automatically, using a video agent, turn it into 20 or 30 versions, each that have the prospect's name, numbers, and use case.
Similar domain, when you send proposals that are PDFs or even websites now, if you're getting fancy, there is absolutely no reason at this point to not include the video that goes with it.
That is the succinct, clear, most visually dynamic, high-conviction version of that argument for why they should work with you.
To the extent that you invest in customer education, that customer education can now stay current if you build the pipeline the right way.
And maybe let me be clear about the terms here.
The difference between making a customer education video and making a customer education video pipeline is the way that you're interacting with the AI.
So, if I wanted to create a video, I might go into Claude Code and explain what I wanted the video to say, point it to where the assets are that it could use, give it the specs like approximate length, and then let it rip.
If instead I wanted to build a pipeline for doing that in an ongoing and self-improving kind of way, instead we're actually building an application using code that's got process logic built into it.
So, it's still gonna do all of the things that I just described for making the single video, but that's going to be housed within a process that has specific triggers.
Where, for example, at the beginning of every month, or just when I initiate that pipeline, an agent is going to be spun up or re-engaged that can go out and search for updates, refresh the script based on those updates, take the latest version of the video and the raw source material that it has to draw from, and combine that with these script updates to produce the newest version.
Basically, a video is a video, a pipeline is an application that produces videos in some recurring way.
Now, if at this point you're excited, but feeling like there's a lot there and you're not quite sure where to start, let me propose three levels for getting up and running.
The first level is to find one of those use cases where AI edits what you've already recorded.
So, the simplest example might be to take some meeting that you've recorded and actually ask the AI to go produce the highlight reel for that video.
This is the simplest layer of AI video editing sitting on top of existing assets, but will still give you a feel and flavor for what it can do.
The second level is where we move from AI editing what already exists to AI making something that you couldn't before.
Another really simple, low-hanging fruit example of this is the sort of numbers in motion charts that we've been talking about.
Take last quarter's results and this quarter's results, feed those spreadsheets into Claude, and let it build an animated chart sequence.
If you have an idea for a product feature, you could build that full concept video.
Basically, now we're moving from taking an existing recording or set of recordings and turning them into an edit to now producing something net new that just wouldn't have existed before and that you probably couldn't have done, at least not easily, just a few months ago.
The third level is where you get to AI actually running one of these video pipelines.
So, an example might be a scheduled weekly video where every Friday an agent pulls either metrics or tickets or shipped features or something like that and renders a two-minute update that is distributed through some specific process.
Once you build one pipeline like this, I guarantee you'll get a much better sense what this idea of an AI video pipeline can even be, and you'll start to come up with more ideas for how you could use it going forward.
So, that's the idea.
And I guess as we close, it's important to note that in the same way, agentic coding was never about non-coders somehow replacing developers, and was instead about non-coders being able to use code to solve their existing problems or do net new things that they couldn't do before, and generally achieve more in a way that was impossible.
It's the same idea with video.
I am as enthusiastic as I can possibly be about these new capabilities.
And yet there's no universe in which I'm claiming that me or you who are not video editors and who have not spent time building that discipline are going to, even with these tools, be able to produce something as good as actual video editors and producers and directors using these same tools.
That's not the point.
The point is that those set of people's skills would never have been applied to all these things before because the cost-benefit ratio just wasn't there.
These are new opportunities to use video to make work work better.
And that's what's exciting.
Please do share what you get out there and produce.
But for now, that's going to do it for today's AI Daily Brief.
Appreciate you listening or watching.
As always, and until next time, peace.
