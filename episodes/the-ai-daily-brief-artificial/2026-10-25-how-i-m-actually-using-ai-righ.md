---
record_id: "podcast:01635a1a-2d7d-4ab8-bb0b-2d7c406359c1"
episode_id: 01635a1a-2d7d-4ab8-bb0b-2d7c406359c1
title: "How I'm Actually Using AI Right Now (Including Claude Duet)"
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-im-actually-using-ai-right-now-including-claude-duet/01635a1a-2d7d-4ab8-bb0b-2d7c406359c1"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-im-actually-using-ai-right-now-including-claude-duet/01635a1a-2d7d-4ab8-bb0b-2d7c406359c1"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-25
played_at: "2026-10-25T12:00:00Z"
play_count: 1
duration_seconds: 1920
source: pocketcasts-history-browser
played_label: October 25
history_order: 30
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: ab87f12850d74cccc8907920d9e8a3baea0bf13cd210c28d0a5f06f2c352dc15
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

Claude Duet—called Claw Duet in the transcript—is presented as an experimental personal-agent form factor, and the host uses it to map his current AI stack across strategy, research, copywriting, image generation, data analysis, and building. He estimates about 60% of his AI time goes to strategy externalization, values models that push back rather than flatter, and names Opus 5.5 as his favorite for that work after Fable 5.1 and OpenAI models he found flat; for research he uses Astra and Opus about equally and cross-checks outputs for AI Daily Brief and his wife’s true-crime podcast Love Murder. His production workflow includes a daily AI/news survey, an overnight dossier by researcher Scott, unscripted talk-over visuals, AI for episode descriptions/social posts/titles (about 50% of titles remain his original), GPT image models for covers, Ideogram for four-image iteration, Midjourney for stylized exploration, Astra inside Codex for data analysis, and Claude Code with Opus 5.5 for building the AI Daily Brief site, transcript-to-shareable-assets pipeline, social cards via Typefully, and 60–90 second video clips. He also describes a new weekly show, How We Got Here, launching Oct. 26 with episodes on America’s falling out with tech, cheap stuff versus expensive essentials, and prediction markets, using Claude/Atlas for research dossiers, Opus 5.5 for 5,000–6,000-word companion essays, GPT Image for aesthetics, and video editors plus AI animation. Sponsor segments and announcements mention Super Intelligent’s AI Champions Program, KPMG, Robots and Pencils, C Data, Blitzy, and a KPMG/University of Texas at Austin study of 500+ early-career professionals identifying “AI amplifiers,” while the host also references OpenClaw, Muse’s personal-agent bias, Grokbot, Instinct, Town, Hermes, Mark Zuckerberg, Alex Wang, Google, and Microsoft.

Treat personal agents as experimental and decide whether the need is proactive net-new work—email monitoring, notifications, drafted responses—or better coordination through a single dominant thread with sub-agents; the host’s earlier chief-of-staff and research agents failed his value test because maintenance exceeded benefit, especially for someone who tightly manages calendars and email. If context switching is the problem, try a mono-thread workflow and evaluate whether compaction and sub-agents reduce cognitive load versus project-based chats. For high-stakes work, use cross-model review, demand sourced research, and choose models by use case rather than expecting a one-to-one replacement; for content pipelines, consider transcript-to-web-card, social, and short-video automation while preserving human judgment and net-native engagement. The KPMG/UT Austin finding suggests training should teach people to guide, evaluate, and refine AI outputs, not just use tools; follow-up questions include which recurring tasks justify an agent, whether third-party agents can connect to existing ChatGPT/Claude context without migration, and whether video/essay pipelines improve distribution enough to offset editing effort. No direct health implications are present.

## Transcript

Claw Duet is out this week, the latest in the personal agent space, and today I am going to walk you through how I'm actually using it, which, when I dug in, kind of required me to give you an overview of how I'm using AI overall.
So, let's dive in.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, Robots and Pencils, C Data, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AI DailyBrief, or you can subscribe to Apple Podcasts.
To learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
Also, one more announcement: we recently launched at Super Intelligent the new AI Champions Program.
It's a way to learn not just how to use AI well, but also how to bring that AI to the rest of your organization.
There's a link to that you can find at the top of the AI Daily Brief website, or you can just go directly to besuper.ai.
So, for this episode, I wanted to go a little bit deeper on the just announced Claw Duet.
And more broadly, I realized as I was preparing for this, I haven't done an episode for a while around how I'm actually using AI, what my current stack is, which tools I'm using for what purposes, what use cases are getting the most value.
And it turns out that in sharing how I'm using this new generation of personal agents, or at least experimenting with them, some amount of that background is necessary.
What's interesting to me is that I believe pretty firmly that we have to treat the form factor of these personal agents as still experimental.
Yes, we are absolutely seeing early traction and uptake, especially with Muse.
And certainly the fact that we've been playing around with this form factor since OpenClaw exploded earlier this year suggests that there is some here here.
What I found, though, to give a bit of a preview, is that I'm still trying to figure out how much these personal agents are supposed to be my chief of staff organizing everything I do versus a very specific proactive proxy me type of employee that goes out and figures out how to be helpful without me asking.
But I'm getting ahead of myself, and to understand the background of how I'm using these tools, let me situate you more broadly in my major AI use cases.
I'll try to make this as valuable to a wide cross-section of people as I can.
My main job, cutting across both the AI daily brief and super intelligent, is thinking about what to do or what to create next.
On the AIDB side, this is primarily in the content domain, whereas on the super intelligent side, it's more about business strategy, about trying to understand what learning gaps there are for AI users.
And because a big part of my job is strategy, that involves a lot of externalization.
I'm not a person who just quietly thinks to myself, I like talking it out.
In fact, I have reams and reams of notes and notion that I call walk notes that are the times when I'm either walking or driving or sitting and thinking through ideas and what I'm going to do next.
This particular use case has always been my number one, at least in terms of sheer volume of time spent.
If you look across every thread and conversation and session I've ever had with AI, probably 60% maybe are in this strategy realm.
Not necessarily in terms of volumes of token consumed, that of course goes to building, but just in terms of the sheer amount of time I've spent, it's absolutely tops.
This is one area where model differences have huge impacts.
I always say when there's a new model that at this point, it's not about asking if they're going to be a one-to-one replacement for what you're using, but understanding where they fit into your stack.
But I am always, with every single new major model, testing it against this sort of strategic externalization to see if it will, in fact, be a one-to-one replacement for what I'm using now.
When it comes to what makes for a good model for me when it comes to strategy, there's a whole bunch of factors.
The most important and hardest in a lot of ways is its approach to pushback and sycophancy.
For a long time, these models were frankly not all that much better than just writing things down on paper because they would never push you.
Everything was the best idea ever, and that's actually not that helpful if you're trying to make ideas really good and only pursue the ones that are really good.
In that circumstance, you don't want a yes person who's saying that every idea you have shines like gold.
You want someone who can critically engage and who importantly is doing so based on something, not just because it's been trained that pushback is good.
This is a really, really hard line.
Models have to be dynamic enough, creative enough, but also adaptable enough, but also confident enough.
And yes, I'm using all these anthropological terms, even though I don't ascribe to the anthropomorphic view of AI because they're the only real way to describe what I'm looking for when it comes to this use case.
Anyway, Opus 5.5 is my favorite model that I've used in a very long time for this.
I was using Fable 5.1 before that, which was okay.
And before that, for a while, had been using OpenAI models.
Although for most of this year, I found the GPT models to be a little bit flat and not dynamic for this sort of work, which, as we'll see, follows into dots.
My next use case is research.
As you might imagine with the AI Daily Brief and with this new upcoming project that I'm about to tell you about how we got here, research also represents a big chunk of what I do.
We also often have research for my wife's true crime podcast, Love Murder, that I produce.
And because all of this research is resulting in either me or my wife saying things publicly, we really need the models to be good, to be well sourced, to not hallucinate stuff, to be able to understand the sourcing, to be able to put proper emphasis on different types of sources versus others.
And for this use case, I actually use Astra and Opus about equally.
And it's also the type of use case that can, especially in really important circumstances, benefit from them interacting with one another.
If I'm researching a topic, I will very frequently have both Astra and Opus go at it and then share the results across so that Astra is reviewing Opus and Opus is reviewing Astra to add that additional layer of confidence before it then turns into content, however it is that I happen to go turn it into content.
The next use case that is a daily one for me is copywriting.
I don't use AI to write any of my podcasts because they're not scripted podcasts.
For a little behind the scenes, the way that we produce the AI Daily Brief is that every evening, I do a big survey of everything that has happened in AI that day.
A lot of times I've been tracking it all day, but if I haven't been, I'm going to take an hour or two to go deep on both the news, but also the discourse.
Meanwhile, my researcher in Australia, which is a hack that allows us to be working 24 hours a day, by the way, does the same during his morning.
And at about 8 or 9 p.m.
Eastern time, we lay out exactly what the show the next day is going to cover.
My researcher Scott then overnight prepares a dossier that includes key sources that I'm going to talk over, and especially a lot of the key commentary, things like posts from social media, that form a lot of the meta narrative of the show.
When I wake up, I use that dossier to lay out the screens that I want to talk over in the rough sequence that's in my head, and then I just let it rip.
I always think it's funny actually when I get comments that I'm AI talking about AI because there's actually shockingly little AI used in this process.
And honestly, probably some ways that we could be more efficient, but that's how we do it.
On the flip side, though, when the episode is done, copywriting is something I use AI for every day.
Episode descriptions are an obvious place for that, as well as social posts, although that's a process that I'll get into in just a moment.
And titles are a bit of a back and forth.
I always have a title that I'm coming in with.
I always give the AI a chance to try to convince me of something different.
And I would say about 50% of the time I stick with exactly what I had, with the other 50% of the time some back and forth between me and the AI producing a different title.
For that, I actually use Astra.
I think this one is a little bit about memory and context.
I've been using GPT models for so long for this that there is a very long track record of what I do and don't like.
And so even if Opus or Fable were just as good or even better at copywriting, the amount of time to tune it just doesn't strike me as worth it.
I also think that the concision of copywriting is something that I've heard lots of people like OpenAI's models better for right now.
And that certainly plays into the value for copywriting as well.
Closely related to the copywriting is the way I use image generation.
Image generation actually comes into my work a lot on a daily basis.
I will very frequently use it for inside shows as I'm doing right now.
You can see these images that I'm talking over.
And no matter what, every day I'm creating the cover image at least for the show using AI as well.
At this point, image generation has pretty much just become the GPT image models.
That's not necessarily because I am convinced they're better.
I still maintain subscriptions with Ideogram and Midjourney.
Ideogram I really like as a way to iterate, because as opposed to creating a single image at a time like you do with ChatGPT, Ideogram is creating four at a time and gives you toggles for how widely varied you want them to be.
And Midjourney is just its own weird beast with a lot of strange taste and artistry that, depending on the particular use case, can sometimes just be way better.
Especially if you're not exactly sure what you want out of an image, you just want it to be cool or interesting or visually arresting, and you want to give the model some latitude, that's where Midjourney is really valuable.
For my purposes, the main image generation is going to be those covers, and I'm producing them right after I've finished locking in the headline, so it makes sense all to just keep in that single thread.
Another big use case, which is one that actually extends and expands outside of my role as a content creator, is data analysis.
My brothers and sisters in arms, who filed their taxes on an extension this year, probably just went through this experience of dumping a whole bunch of financial data in and having it organize it, extract your expenses, et cetera.
And for almost every sort of data analysis project, I'm using Astra inside of Codex.
For me, it provides the best results and has that sort of concision of thought that I think is really valuable for this type of use case.
And then we come to building.
And this, of course, is a huge category.
I, like many of you, have used lots and lots of different tools and harnesses and models and stacks for building this year.
We did OpenClaud for a while, and of course, Codex and Claude Code in both their application as well as the CLI versions, third-party tools like Cursor.
But for me, where things have landed pretty consistently is Claude Code, with Opus 5.5 being the default model, and the effort settings usually on high or extra.
Now, I will frequently build inside Codex using Astra as well, specifically to get native access to the image generation models.
So a lot of times the companion experiences that go with the show, if they're particularly visual, will be built in Astra.
But ultimately, I do most of my organizing, narrative architecture, and orchestrating all the building in Claude Code.
I also, I should note, give Claude Code access to GPT image models via the API, although I have found a difference using the image models inside Codecs as opposed to via the API through Claude Code.
In terms of specific assets that you guys see, all of the AI Daily Brief site was built and is maintained by Claude.
In fact, part of the reason for this actually, I think, tells the story of one of the key model updates of this year.
When I first got access to Fable, what made it feel different from other models was that while it had been easy for a while to start building things, Fable, it felt like brought that ease to just getting them done.
As opposed to having projects hang at 80 or 90% complete, with the activation energy sufficiently low, but the completion energy still too high, Fable just brought that completion energy way down and matched the activation energy.
Now, specifically with the AI Daily Brief website, I had known for a couple of months that I needed to switch off the old cutesy 1990s aesthetic website that I had that was fun and retro and evocative for me, but totally non-functional.
And I had a specific mandate that I knew I wanted to achieve.
The AI Daily Brief is a very information-dense show, which I think, and it seems, is a big part of the value proposition that you get as much information per minute as you do, but that also, speaking of activation energy, creates a pretty high barrier to entry.
I had heard from lots and lots of folks that a really important thing that they wanted was an easier way to share specific parts of their show with their peers and colleagues.
So I knew that the website needed to not just be a website, but actually needed to be a production pipeline that could take the raw content or transcript of the episode and turn it into a very different type of web content.
That's what I designed and built with Fable.
And I actually did it on the first afternoon I got access, completing the entire first draft in that afternoon, which was a good thing because the next day was when Fable got taken offline because of the export control dust up with the White House.
The first stage of building that pipeline was to build a system by which I can upload a transcript and it can extract the relevant information from that transcript and organize it into these shareable assets that then go up on the web.
Using Fable and Claude Design, we were able to build an aesthetic for this that doesn't use any image generation, which of course has limits, but it works for what we're trying to do here.
It's visually consistent, it's clear, it's readable, and it uses text and color-based elements for a lot of the brand identity.
The next step, which was also with Claude, was expanding that pipeline to social.
Truth be told, I have never given social the time it deserves, and to be clear, the way to be successful on social is to actually sit there and engage with people and spend time on it, but I at least wanted some amount of content going up.
Using Fable again, because this was pre-Opus 5.5, I added a secondary pipeline, where once the episode is finished extracting, those cards then go through a secondary process, generating a set of tweets and a LinkedIn post.
Those are then scheduled with a third-party service, Typefully.
I did explore messing around with the APIs to connect directly to the services, but a third party like Typefully has already done all that work, and it was way easier to just plug in there.
The most recent step has been video, and here it's got the same principle as social.
It's better to create net native video for the channels, but in the absence of that, I wanted at least one clip per episode to go with Spotify.
Recently, and especially with Opus 5.5, the models in Claude have gotten enormously good at video editing.
So much so that I actually think that even if you don't think you have a reason to be using video right now, you may still want to go and experiment.
But in any case, I asked Claude Code to build me a video production pipeline that matches the aesthetic of the website.
And so what it does each day is I feed it the transcript, it reviews and makes a judgment call around the best, most compelling, most self-contained 60 to 90 seconds.
It then extracts that clip, builds other visual assets around it, and packages the whole thing up for download that I can then upload wherever it goes.
Now, spoiler alert, for something that the rest of the audience will hear about tomorrow, this process was all in place when I started working on a new show called How We Got Here.
The idea of how we got here is kind of right there in the name.
It's a show that looks at the specific social, cultural, technological, and economic factors that led to today's biggest stories, phenomenon, and events.
The idea is that everything that we experience now comes from some specific set of decisions that were made in the past, and in order to remake or reimagine those phenomenon, we need to understand how we got here.
It came out of a lot of times recognizing on this show that I just didn't have the space to go as deep as I wanted to into a particular issue, and so it's 45 minutes to an hour, it'll be once a week.
And to give you a little bit of a flavor, the first episode is about how America fell out of love with the tech industry.
The second is about how it was that stuff got cheap while all the important things in life got more expensive.
And the third is about prediction markets and how we started betting on everything.
The first episode comes out on Monday, October 26th, but I've been working on this for a while now, and luckily I had all these processes in place.
Claude is where I iterate on the ideas, both from a strategic and distribution standpoint as well as the content ideas.
From there, I'm going to use both Claude and Atlas to create rich research dossiers.
I then do a round of feedback, have Claude lay out the key beats based on the arguments I'm trying to make.
I go source visuals, lay them out just like I do for the AI Daily Brief, and then talk over them.
This time for a long time, resulting in a 40-minute to hour-long show.
But here's where we really started to expand and even push on the process from AI Daily Brief.
After I record, I rip out the raw transcript of myself and hand that plus the original research back to Opus55 to have it do the first draft of a companion essay.
The goal of the companion essay is to be a place that makes the same argument I'm making on the show, but with a lot more visual richness, and that is presented in a format for people who like to read, with the easy ability to get more links and the sources behind the show.
But we're talking about an hour of material, 5,000, 6,000 words of essay.
So from there, I take the essay, drop it into Codex with Atlas, and leverage GPT Image to create a whole aesthetic and look and feel.
For those wondering, by the way, I then do an exhaustive, an exhausting edit of that essay, where based on the first three, I rewrite about half of it.
But we're still not done with Claude Code at that point, because, like I said, this latest round of models have made a major jump in video editing.
Now, I have a team of video editors, but we're doing things a little bit differently, where they do the first pass, taking advantage of a lot of the processes that we've built over the years with AIDB, and then we integrate AI to add animations and to plug it directly into the clip pipeline.
A new study from KPMG and the University of Texas at Austin found that when people work with AI, similar skills don't guarantee similar outcomes.
Researchers studied more than 500 early career professionals and found that the best performers consistently amplify the value of AI by guiding, evaluating, and refining its outputs.
These top performers, called AI amplifiers, weren't defined by what they knew alone, but by how they worked with AI.
Learn more about what separates AI amplifiers from everyone else at kpmg.com/slash uslash AI amplifiers.
The best teams don't have a single star carrying everyone else.
They know their own strengths and each other's weaknesses and play to both.
That's the team Robots and Pencils has built on purpose.
Nobody there is grinding through busy work to pad a headcount number.
People come for the hard problems and they stay because everyone around them is leveling up at the same time.
In a market full of companies that are just trying to hire fast, that's worth a look.
Check out robotsandpencils.com/slash careers.
This episode is brought to you by C Data.
Companies rolling out AI keep hitting the same wall.
Token spend is climbing, security is holding agents back, and no one knows how AI is truly being used.
The root cause: AI is cut off from the systems and context your business runs on.
That's why C Data built Connect AI Gateway, one control point between your AI and your systems.
Built on the connectivity layer powering Palantir, Google, Salesforce, and hundreds more, each agent gets exactly the data and tools it needs.
It governs down to the record and lets you finally see your org's complete AI usage in one place.
Accurate answers, a fraction of the token cost, and a gateway that learns your business with every interaction.
See how at cdata.ai.
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
That's why Fortune 500 engineering teams trust Blitzy with the codebases that matter most.
See for yourself at blitzy.com.
That's B-L-I-T-Z-Y.com.
Okay, so this is all the relevant background on how I use AI on a daily basis.
It's obviously super closely focused on content creation and building the infrastructure around content.
And you'll probably notice that a lot of the things that other people get lots of value out of AI with are not here.
For example, I didn't mention inbox monitoring, automated responses to certain types of emails, Slack monitoring, general updates, all that sort of proactive stuff.
And I haven't taken the time to really organize that sort of AI work because up until now, for me personally, the juice wasn't worth the squeeze.
I did experiment with this with OpenClaw.
I had individual claws managing specific pieces of what I did, using the heartbeats and cron job setup to monitor and do specific things at specific time intervals.
I also had a chief of staff agent that was meant to coordinate across all of those.
And at the time, there was a persistent research job that I was doing as part of AIDB and Super Intelligent that was monitoring studies and surveys and AI adoption.
So those were my two experiments with proactivity: the proactive always-on research agent and the chief of staff-style monitoring agent.
Now, eventually, I stopped having need for the research agent because that just wasn't a project that I was working on in the same way.
And when it came to the chief of staff, it candidly just wasn't adding enough value to deal with the maintenance and upkeep.
Now, to be clear, that might have a lot to do with me.
I am incredibly assertive about limiting and managing my calendar.
90% of the calls I do are not scheduled, and it is extremely hard to get me to actually schedule a call, as anyone who's ever tried to discuss an ad buy for AIDB on the phone will have found out.
And I don't know if it's just being an internet boomer, but when it comes to email, I just star important things as they come in and clear out the inbox every couple of days, and that's worked for me for forever.
Which is not to say that proactive agents are not useful.
It's that in the version that we had access to, they did not add a sufficient amount of value to me personally to be worth the setup cost.
It's why, for example, you haven't heard me talk about the Hermes agent, even though I think it's an excellent product, because it just hasn't fit specifically with how I work and what I work on.
Which brings us to this new phase of personal agents.
The interesting question for me has been: will they lower the cost of setup and maintenance sufficiently that the type of proactivity that they can offer actually feels worth it?
Now, I personally am in the category of people who, at least for now, believe, and of course I could be eating my words in the future, that I was very unlikely to use these sort of agents for personal uses.
You might have even heard me denigrate all of the use cases that these companies pitch, like flight booking and agentic shopping and booking restaurants and things like that.
Again, it's not that I don't see how they could be valuable for some people, it's just that they're not for me.
To take just one example, when I'm booking a flight, I'm pretty much always booking the airline where I have my miles, unless I absolutely can't for some reason.
And in that case, it's usually one other airline that does those other routes where I also have miles, meaning that I'm working within the ecosystem of a single airline's booking system, and it would take absolutely as much time to explain to an agent the variables and contingencies as it does to just look at their specific web interface.
So, coming back to personal agents, I was always going to be on the professional use case side of those personal agents.
So, then the question becomes: is the value of a personal agent for me net new things like this proactive work of the type that I haven't set up yet?
Or is it some type of coordination that replaces my normal interactions with AI?
So, let's look at these two possibilities a little more directly.
By net new, I mean that proactive stuff like watching my email, sending me notifications about something that needs to be done, and drafting responses that I can approve.
Again, that's not a thing that I have agents doing right now.
By better coordination, I mean a bit like this chief of staff role, but I think in some ways it's actually closer to the mono-thread paradigm that we've discussed here over the past couple of months.
The mono thread paradigm is the idea that instead of a slew of different chats spread across a ton of different projects that each only have the context of that particular chat or that particular project, you instead have a single thread that has all of your context and pulls up what it needs to do when it needs to do it and can shift around and behave and work on different things and spin up sub-agents to do different things as they are required.
Organizing things into individual chats and individual projects can be really useful for organizing one's own brain in the same way you use folders on a computer.
The benefit of the mono thread paradigm is that for the user, you don't have the cognitive load of doing that organization.
You just get to go stream of consciousness.
This has only been possible as a paradigm with advances in compaction and context window management going on behind the scenes.
In other words, it used to be that at some point your AI would get very tired because its context window was full and you just had to move to a new chat.
In fact, a bunch of the lessons in the early education programs we did in 2026 were about the best ways to do handoff documents, but the labs have all gotten much better on the back end about compressing the context and carrying it forward so that you don't actually have to leave the single chat that you're in.
This mono thread paradigm frankly fits my way of working in my brain zone organization a lot better than structured hierarchical organization.
I've already been pushing Claude Code and Codex in this direction, having things much less divided and working off a single dominant thread.
So my question for these personal agents would will it be more of that?
So then we come to the different tools.
One category that was a lower priority for me were third-party new tools like Instinct and Town.
Even though people rave about these tools, they were always in that lower priority for me because of the mismatch in terms of what they were good at and what I wanted to do, and fundamentally, my unwillingness to move all of my professional and work context over from the places I do that work already, which, as you've heard, is ChatGPT and Claude.
Then we have Grokbot and Muse.
Muse again, a little bit less interesting to me because of its bias towards personal stuff, although it's very clear that that is not where Mark Zuckerberg and Alex Wang's ambition end.
And with Grokbot, I do have all of the ultra subscriptions, but I would really prefer not to have to move out of the OpenAI and Anthropic ecosystems because it's already enough to maintain those two.
Grokbot, I find valuable because of its integration with X, which is really valuable from a content production standpoint.
And basically, my approach right now with Grokbot is to stay just enough engaged so that at any point there were compelling reasons to switch, I wouldn't be starting from zero.
I should mention Google and Microsoft at this point.
Google, I still, at the moment, I'm sorry to say, I don't think it makes sense to invest a lot in.
That could absolutely change.
In fact, I am optimistic that it will change as they get back up on the horse.
But for now, the fact that they are behind in this area is one less load for me to invest in.
With Microsoft, I keep close professional track of what they're doing because of both the podcast and super intelligence users, which are largely in the enterprise.
But being totally solo, I'm always going to bias towards the much more nimble, fast-moving versions that aren't heavily enterprise-focused.
All of which is to say that when it comes to Microsoft, I'm specifically not making any value judgments about their tool set right now.
It's just not an ecosystem that I'm playing in.
So that leaves us with dots and now duet.
So far, how I use my dot and my feelings about it are pretty reflective of the way that I use ChatGPT more broadly.
It's basically right now for me, a new version of the mono thread organization for any of what I would consider important professional work that I do in ChatGPT.
In other words, if I'm doing important research or doing data analysis on my podcast statistics, that I am now managing through Quasar, who is both the nullian lawyer of Dungeon Crawler Carl, as well as my dot.
On the other hand, for simple fast things, like random queries that I would have googled before, or even that copywriting for the daily podcast episodes, that's happening in the same space away from Quasar that it always has.
I will say that even with that professionally relevant work, like doing a bunch of data analysis on past podcast performance, I'm not 100% sure that it wouldn't have been better served being done in Codex.
And when it comes to other things like that strategy work, I'm certainly not finding any more compulsion to do it with my DOT.
In fact, I have found, and I've seen a number of other people reflect this as well, that the DOT's personality at this point is so flat that it almost stonewalls that sort of strategic engagement.
I will sometimes dump a load of context to Quasar, and it almost feels like pulling teeth to get it to engage.
I had a telling experience the other day where I spent all day while walking and hiking, strategizing and planning with Claude with Opus 5.5, and then shared the whole conversation after with Quasar so that it had the up-to-date information without me having to share it again.
Instead of picking up on any of the threads from that conversation, which are again, probably six hours of talking, I think its response was literally: great, this information has been saved for the future.
My dot I have found not to be particularly proactive, and frankly, it took very little time before I basically just stopped really seeing a reason to engage with it.
So far, if I'm in OpenAI, I'm either doing that basic, fast stuff, or I'm deep in codecs.
So, summing up, my initial experience with DOTS, and of course, this is completely subject to change and does not make me pessimistic for the future, but my initial experience is that as a feature, it doesn't really add anything when it comes to ChatGPT being the place for me to go reactively do things.
It's very weak on proactive work, but it does seem like it could be valuable as a master holder of context.
In other words, I can just dump all the relevant context to Quasar and have that sync and do things rather than having a bunch of chats where I have to repeat that context later.
Then we come to Duet.
Duet is, of the major personal agents, the one that's least concerned with a personality and character.
It doesn't have a cute fuzzy logo like Muse, and it doesn't have you name it like Dot.
It is very clearly, following the larger pattern of Anthropic, focused on work, which seems like it could be a good fit for me.
When I got Duet up and running, the first thing it asked me to do was to connect Slack, Gmail, Drive, et cetera, right away.
And before I had done anything else, it gave me a stack of options for proactive projects.
In fact, Duet is so biased towards proactivity that I found that it maybe overestimates how valuable that set of work is because it can be proactive about it.
I'll give you an example.
One of the proactive projects that it wanted to help with, based on being in my inbox, was managing podcast sponsor inventory, specifically making sure that we didn't commit the same ad slot to multiple sponsors.
This it picked up on as a problem because in two separate emails I had given two separate sponsors the same date as available, and the duet did not yet know that I actually have a set of slots for those days, so that wasn't necessarily a problem.
It basically had a spasm about this thing, reminding me like four times before I had to tell it that that didn't matter, and in fact, that that entire work stream was not one that I cared about.
And yet there are other proactive things that I found it much more valuable for.
A couple of times now, there's been an email of exactly the type that I would star and go back to a couple days later.
And in each of those cases, Duet has proposed a response that I could either edit or authorize it to send directly from my chat.
A couple of times I've just let it send, and one time on the most substantive and creative proposal, I didn't send it right away, but it got me about 90% of the way there without me having to go back and think about it.
This makes me more optimistic for the value of Duet for this proactivity.
I would also note that while Duet is pushed as an iOS app, I actually quite like its web interface.
In addition to your main everything stream, you can also create separate channels for Duet so that to the extent that you want some amount of that continued hierarchical organization, you can do it.
And Duet takes advantage of Claude's artifact infrastructure so that it can actually create things that you can interact with and edit without having to go into some separate interface.
It can automatically organize things that you're doing into tasks that it groups as active, up next, scheduled, or resolved, which you can modify either through the main chat or by directly adding a task.
Now, of course, I am only a few days in, but I'm already much more optimistic about this approach.
I will say that I don't think you're going to want to do everything in Claude with Duet.
I had a UI and brand visual design task, and doing it inside Duet was much worse than doing it in Claude's native design experience, which I believe is being folded into artifacts later this year, but still is its own designed UX.
So for me, it really is going to be about that proactivity.
My goal with all of this is not to provide a particular ranking of these tools or to make any definitive statements about how you might want to use them or where I see them going.
I think, frankly, you kind of don't have to worry about which ecosystem of these that you're investing in because the moment that some feature works in one, within weeks, if not days, it's going to become part of all of them.
If my experience, for example, of dots not being proactive enough is something that is more commonly experienced, you better believe OpenAI is going to tweak that.
If there are some UI elements that people like about Duet or about one of the others better, at some point the other labs are going to copy those UI features as well.
The broader question remains, where these personal agents fit?
For me so far, it is much less a big shift towards it being the main way I interact with AI, and much more an easy-to-set up little baby version of myself that does a bunch of stuff that I don't want to do.
That's valuable, but is it future of the industry valuable?
Remains to be seen.
Hopefully this was a useful peek behind the curtain.
For now, that's going to do it for today's AI Daily Brief.
Appreciate you listening or watching.
As always, until next time, peace.
