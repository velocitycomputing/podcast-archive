---
episode_id: f7bbdc0c-23b4-40fe-aec5-5e3d9875c933
title: 9 Codex Tips From the Codex Team
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/9-codex-tips-from-the-codex-team/f7bbdc0c-23b4-40fe-aec5-5e3d9875c933"
played_date: 2026-05-19
played_at: "2026-05-19T12:00:00Z"
play_count: 1
duration_seconds: 1740
source: pocketcasts-history-browser
played_label: May 19
history_order: 77
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: cache
summary_model: claude-haiku-4-5
tagging_model: claude-haiku-4-5
proposed_tags: []
proposed_entities: []
status: new
routed_to: null
---

## Summary

The episode covered three major AI stories: Cursor's release of Composer 2.5, a competitive in-house coding model priced at 10x cheaper than Opus or GPT-5.5 while maintaining comparable benchmark performance; Cloudflare's analysis of Anthropic's Mythos Preview, highlighting its unique ability to build multi-step exploit chains and generate functional proofs rather than just identifying bugs; and Elon Musk's lawsuit against OpenAI being dismissed on statute-of-limitations grounds. The main segment featured Jason Liu's "Codex Maxing" guide with nine practical tips for getting the most from Codex: maintaining persistent long-running threads for each workstream (leveraging improved context compaction), using voice input to provide richer, messier context that models can refine, employing the Steer feature to update prompts mid-generation, building a structured memory vault (like Obsidian) to serialize learnings into reusable artifacts, granting Codex tool access (computer use, browser, connectors), utilizing remote control features for mobile steering, and implementing heartbeat check-ins to revive threads.

For actionable application: adopt the durable thread pattern by creating separate persistent threads for your major work areas rather than one-off chats, enable voice input to capture unpolished thinking that the model can shape into clarity, set up your environment with computer/browser/connector access so Codex has full context, and implement a memory system that turns long conversations into structured, editable files you can reference across projects. The core shift is moving from treating Codex as a chat interface to using it as a complete work system where memory persists, context compounds over time, and you can steer work in progress rather than waiting passively for full responses.

## Transcript

Today on the AI Daily Brief, nine Codex tips from the Codex team.
Before that in the headlines, yeah, we got a verdict in the Elon OpenAI trial, but that's
much less interesting than Composer 2.5.
The AI Daily Brief is a daily podcast and video about the most important news and discussions
in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, Robots and Pencils, Bolt, and Zencoder.
To get an ad-free version of the show, go to patreon.com slash AI Daily Brief, or you can
subscribe on Apple Podcasts.
To learn more about sponsoring the show, head on over to aidailybrief.ai or send us a note
at sponsors at aidailybrief.ai.
While you are at aidailybrief.ai, you can apply for our new growth engineer role.
I'm going to be closing that soon, so if you are interested, get your application in.
And you can also find a link to register for the third cohort of Enterprise Claw, which
is coming right up soon.
Basically, if you get all excited about the Codex talk today and want to get that spirit
of agent building across your company, that's what Enterprise Claw is going to be good for.
But with that out of the way, let's talk Composer 2.5 and what it says about Cursor in the AI
race.
One of the questions coming into this year was whether what SWIX calls the agent labs, but
which we now might call the harness-first labs.
These are companies like Cursor, Cognition, etc.
would be able to compete on the model front.
The concern for these companies, of course, was that if they were totally beholden to the
models from the big labs, if those labs started to move in the direction of building their
own harnesses as well, it could squeeze out the space for the Cursors and Cognitions
of the world.
And at the same time, the Cursors and Cognitions of the world had something valuable in the
form of the data exhaust from the usage of their platforms, which theoretically gave them
insight into how people were actually interacting with these models, which could turn into a
valuable asset for training their own models.
Whether it could or couldn't, it was clear that this was the direction that they were
going to start to head, and that the space between these so-called agent labs and the
model labs was destined to close.
The model labs were going to move into the harness space, the agent or harness labs were
going to move into the model space.
In January, CEO Michael Truel told staff that it was, quote, wartime, recognizing that Cursor's
business model was being eroded from both sides.
Claude Code was coming after them on the harness side, but they also couldn't keep eating the cost
of serving Anthropic models at a discount.
With that in mind, he said that the company's number one priority was to build the best coding
model this year.
The release of Composer 2 in March was a decent first step, but it was still mostly about
bringing down costs.
Where users adopted the cheap in-house model, it was mostly for simple tasks.
However, it failed to drive new users to the platform.
The just-launched Composer 2.5 could be a different story.
The model appears competitive on the key benchmarks.
It scored 69.3% on Terminal Bench 2.0, which is just behind Opus 4.7, 69.4%.
On Sweebench Multilingual, it scored 79.8%, comparable to both Opus 4.7 at 80.5% and GPT
5.5 at 77.8%.
On Cursor's in-house benchmark, which tests more difficult coding tasks, Composer 2.5 scored
63.2%, just about a point behind both 4.7 and 5.5.
Now, the coding performance gets Composer 2.5 into the ballpark of usability for serious
coders, but the bigger part of the story is the cost.
Cursor is serving this model at just $0.50 per million input tokens and $2.50 per million
output tokens, making it half the cost of Opus 4.7 or GPT 5.5.
They also seem to have delivered some big token efficiency gains.
Their benchmark run on Sweebench came in under $1 per task, compared to around $5 per task
for GPT 5.5 on extra-high settings, or $11 per task for Opus 4.7 on max settings.
That has led Cursor to claim that their model is 10x more efficient, compared to similarly
capable models.
Now, Composer 2.5 is still built on top of the same base model as Composer 2, which is
Moonshot's Kimi 2.5.
That implies that the entire performance boost came from better reinforcement learning techniques,
and suggests that even if people don't switch en masse from Opus and GPT to Composer,
that there is a ton of room to post-train leading open-source models to compete at the
frontier, especially around these discrete tasks.
Cursor also announced that they're in the middle of training a new model from scratch
using XAI's Colossus 2 training cluster.
They wrote,
With Colossus 2's million H100 equivalents and our combined data and training techniques,
we expect this to be a major leap in model capability.
Leon Lin summed up the model release posting,
So basically we got an Opus 4.7 model that costs 10x less.
I have to test this.
Later in the day, he checked back in with the results, writing,
Pretty fast and efficient model.
Does a great job.
I'd say it's almost as strong as Opus 4.7, or in some cases just at the same level.
Cheap model.
Good at front-end.
Still a bit generic design when used without skills.
Analyst Max Weinbach agreed, writing,
Composer 2.5 is very good.
It's good at doing more than just quick iterations of front-end now.
I will probably use it over Claude and Cursor.
Addressing what had changed from Composer 2, he added,
Composer 2 was good at some quick tweaks, but I didn't trust it enough to do more.
I trust 2.5 a lot more.
Ellie from Prime Intellect noted that following the XAI deal, which you might remember is where
XAI has the option to buy them for $60 billion, Ellie said that Cursor is now competitive with
the Frontier Labs on both model performance and training compute.
Certainly Elon seems excited, spamming retweets to all of the excited posts about the model.
And to give you a sense of the type of opening that Cursor might have,
especially if you're sitting there thinking to yourself,
aren't companies all just signing up with either OpenAI or Anthropic at this point?
Jamat Palahapatiya wrote,
If you're running a consulting business and you're deploying Anthropic or OpenAI directly
into your organization, I'm looking at you, PwC and Accenture,
you're letting the fox into the henhouse.
OpenAI and Anthropic are openly funding and starting competitors to you
while also using your usage to drive more success for them.
This is not a failure on their part, but a failure on your part.
Consulting businesses that understand this are adopting a control plan
that allows them to arbitrate where tokens go and who generates tokens for them.
Controlling the tokens is controlling the spice.
Basically, there is a lot more conversation around just how locked you want to be as an enterprise
into these models, which creates an interesting open lane for the harness-first companies
that may, yes, have their own models, but are also ultimately model agnostic.
Next up, Cloudflare has published their findings after working with Mythos over the past couple of months
in what could be one of the most useful reviews of Anthropic's secretive new model.
Cutting directly to the chase, they write,
Mythos Preview is a real step forward, and it's worth saying that plainly before getting into anything else.
We've been running models against our code for a while now,
and the jump from what was possible with previous general-purpose frontier models
to what Mythos Preview does today is not just a refinement of what came before.
It's a different kind of tool doing a different kind of work,
and that makes a clean apples-to-apples comparison to early models difficult.
Cloudflare goes on to explain two big differences in kind.
Unlike previous models, Mythos is capable of creating an exploit chain rather than just detecting single bugs.
That means it can synthesize multiple attack primitives into a functional exploit.
Cloudflare wrote that the use of reasoning to build complex exploits
makes the model work more like a senior researcher rather than an automated bug scanner.
The other big change is the ability to generate proofs.
Previous models were quite good at detecting potential vulnerabilities,
but they would rarely demonstrate an exploit.
Mythos can generate functional exploits,
making it far more useful as a debugging tool that doesn't simply generate a list of false positives.
What's more, Mythos is able to test and refine its exploits if they don't work the first time,
providing additional evidence to fix the vulnerability.
Cloudflare said that some other models have been able to find the same underlying bugs,
but would rarely go much further.
All of this adds a huge amount of context on why Mythos matters.
In the weeks after the preview release,
many pointed out that other models could find many of the same bugs that Mythos identified.
But, as Cloudflare points out,
there's a big difference between pointing out potential bugs
and providing full code for a functional exploit,
demonstrating exactly what needs to be patched.
Author Daniel Jeffries argues that this is the type of analysis we need around these tools,
saying,
Lastly today,
One little bit of AI drama comes to a close,
at least in this version.
Elon Musk has lost his case against OpenAI and Sam Altman.
After three weeks of testimony,
it took the jury just two hours to return a unanimous verdict,
one which will be wildly unsatisfying to many,
and leave many issues unresolved emotionally,
even if they are resolved legally.
The jury found that the claim of breach of charitable trust
was barred by the statute of limitations,
meaning that Elon took too long to commence his lawsuit.
With it,
the claim that Microsoft aided and abetted this breach also fell away.
Musk's claim for restitution was also found to be barred by the statute of limitations,
and with that,
this big,
massive headline-grabbing tech trial fizzled into nothing.
Now,
honestly,
the trial was already weird,
even before we got to the verdict.
In the weeks before the trial commenced,
Elon abandoned his more ambitious claims of fraud
to focus solely on the breach of charitable trust.
He went to trial seeking two outcomes,
the removal of Sam Altman and Greg Brockman as executives,
and a casual $134 billion in damages.
But even with the reduced scope,
the jury didn't need to consider the merits of the case,
simply making their decision based purely on technical defects with the complaint itself.
This fatal issue was itself an interesting microcosm of how the case played out.
Musk had claimed that Altman and Greg Brockman conspired to,
quote,
steal a charity,
linking these claims to Microsoft's $10 billion investment in 2023.
However,
OpenAI convinced the jury that Musk was aware of plans to form a for-profit company as early as 2018,
after being sent a term sheet describing the proposed structure.
The trial also surfaced Elon's own thoughts on the matter,
namely a 2017 proposal to fold OpenAI into Tesla to allow for commercial fundraising.
The jury determined that these events began the three-year limit for Elon to bring this lawsuit.
Last week, The Verge did a pretty good job summing up the case,
arguing that it, in their words, accomplished nothing but airing dirty laundry.
We certainly got a lot of new information on what went on behind closed doors over the past decade at OpenAI.
That includes the power struggle between Elon and other co-founders,
the fateful week where Sam Altman was ousted and then returned as CEO,
apparently internally referred to as the blip.
But beyond that, there were no real answers.
All we got was a three-week interrogation into the characters of Elon, Sam Altman, and other leaders,
which, to borrow a phrase from a Muramirati text message disclosed during the trial,
was directionally very bad.
Now, the good news for the AI industry is that as blustery as this whole thing was over here,
I don't think that most people in the world outside of AI were paying any attention at all to this.
Unfortunately for us,
broad popular opinion already has it that AI is just another tool for the rich to become richer,
and not something that's actually going to help their lives in any meaningful way,
at least not at a cost that they're willing to bear,
and so more evidence of the billionaires flinging their golden s*** at each other
really doesn't change that perspective.
Do I think it would be better for AI if all of these leaders had a moratorium
on speaking to the public about the industry?
Yes, yes I do.
But am I also glad that at least this particular bun fight is done?
Yes, yes I am.
With that, I am so glad to close the coverage of that particular saga,
and move on over into the main episode.
All right folks, quick pause.
Here's the uncomfortable truth.
If your enterprise AI strategy is we bought some tools,
you don't actually have a strategy.
KPMG took the harder route and became their own client zero.
They embedded AI and agents across the enterprise,
how work gets done, how teams collaborate, how decisions move,
not as a tech initiative but as a total operating model shift.
And here's the real unlock.
That shift raised the ceiling on what people could do.
Humans stayed firmly at the center while AI reduced friction,
surfaced insight, and accelerated momentum.
The outcome was a more capable, more empowered workforce.
If you want to understand what that actually looks like in the real world,
go to www.kpmg.us slash AI.
That's www.kpmg.us slash AI.
Today's episode is brought to you by Robots & Pencils,
a company that is growing fast.
Their work as a high-growth AWS and Databricks partner
means that they're looking for elite talent ready to create real impact at velocity.
Their teams are made up of AI-native engineers,
strategists, and designers who love solving hard problems
and pushing how AI shows up in real products.
They move quickly using RoboWorks, their agentic acceleration platform,
so teams can deliver meaningful outcomes in weeks, not months.
They don't build big teams.
They build high-impact, nimble ones.
The people there are wicked smart with patents,
published research, and work that's helped shape entire categories.
They work in velocity pods and studios that stay focused and move with intent.
If you're ready for career-defining work with peers who challenge you and have your back,
Robots & Pencils is the place.
Explore open roles at robotsandpencils.com slash careers.
That's robotsandpencils.com slash careers.
One personal recommendation, hit plan mode before you build.
I had a project I'd half described in three different prompts,
and plan mode made me actually think through it with Bolt.new before a single line got written.
It saved me from rebuilding the same screen probably about four times.
Build better apps, faster.
Start with the link in the description.
So coding agents are basically solved at this point.
They're incredible at writing code.
But here's the thing nobody talks about.
Coding is maybe a quarter of an engineer's actual day.
The rest is stand-ups, stakeholder updates, meeting prep, chasing context across six different tools.
And it's not just engineers.
Sales spends more time assembling proposals than selling.
Finance is manually chasing subscription requests.
Marketing finds out what shipped two weeks after it merged.
Zencoder just launched Zenflow Work.
It takes their orchestration engine, the same one already powering coding agents,
and connects it to your daily tools.
Jira, Gmail, Google Docs, Linear, Calendar, Notion.
It runs goal-driven workflows that actually finish.
Your stand-up brief is written before you sit down.
Review cycle coming up?
It pulls six months of tickets and writes the prep doc.
Now you might be thinking, didn't OpenClaw try to do this?
It did, but it has come with a whole host of security and functional issues,
which can take a huge amount of time to resolve.
Zencoder took a different approach.
SOC 2, Type 2 certified.
Curated integrations.
Tighter security perimeter.
Enterprise grade from day one.
Model agnostic and works from Slack or Telegram.
Try it at zenflow.free.
Welcome back to the AI Daily Brief.
We have had two pretty big think type of episodes in a row.
And right now, as I record, we are eagerly awaiting all the new goodies we're going to get at Google I.O.
And so given that, I thought it would be a good day to have a bit more of a practical hands-on kind of mane.
Now this, of course, is the year of the harness,
where people realize that unlocking the true power of agents involves getting good at using the software
through which you spin up and manage those agents,
whether that's something open source like OpenClaw,
or something from one of the big labs like ClawedCode or Codex.
Codex specifically has been on an absolute tear this year,
going from almost no users at the beginning of the year to mid-single digits right now.
And as Anthropic has been forced to make some difficult decisions around their pricing model
and move to cut off certain categories of usage that were previously being subsidized,
particularly outside their own harnesses,
OpenAI has taken advantage to pull more of these advanced coding type users
into the GPT and Codex ecosystem.
What this leaves us with is a lot of folks who are digging into Codex seriously for the first time
and figuring out all the ways to make it work for them.
Now, I had been planning a Codex Primer episode,
but over the weekend I saw this post from Jason Liu from the Codex team
talking about the tips that have made his use of Codex really perform even better.
The post was called Codex Maxing, it was published on Jason's GitHub,
and so what we're going to do today is extract the biggest insights from that post
as a bit of a 101 to see the best practices in using Codex from some of the folks who built Codex.
My presentation version of Jason's post was, of course, built with Codex.
Now, by way of background,
Jason said that for a while he'd been using Codex for coding-related tasks,
but over the last few months it's really become an entire workspace for him.
And part of what makes it valuable is that it replaces the single instance,
give a prompt, get an answer of a chat GPT-style interface
with a broader complete experience that can hold context over time
and do much more extensive types of work.
The core of Jason's tips are nine practices that add up to one larger shift.
The first is using long-running, durable threads.
Now, you might remember a few weeks ago when one of the recent Codex updates
had a new system for compacting context.
This is basically the way that on the back end,
the harness collapses and compresses the context from a long-running conversation
into just the key elements that it needs to know,
clearing out space in the context window to keep the chat moving.
Part of what OpenAI insiders noted around that update
was that the compaction system had gotten so much better
that they could basically keep a set of persistent threads going
that never lost the larger context of the thread
and were able to continuously add it on.
Jason's experience building a chief-of-staff thread
was actually one of the examples that I pointed to
as I talked about how you might use this new version differently.
And to try to put a little meat on the bone here
of why this sort of durable thread could be valuable,
A lot of the features inside apps like ChatGPT
are basically just proxies for memory and context.
When you use a project and you add a bunch of files to that project,
it's effectively about giving each new conversation in that project
the ability to go draw from all of that context.
But it still has to go draw from that context,
it's not necessarily up to date unless you specifically maintain it,
and the process of retrieving context from those files isn't always perfect.
That's not to mention UI UX issues
of having a whole bunch of different threads and chats going
that you have to sort through and figure out
which one you are actually having the relevant conversation within.
The idea of the monothread pattern
is to put key conversations about a particular topic
all in one log thread,
relying on Codex's compaction
to allow that thread to be durable and persist over time.
Jason's tip is not only to use this monothread pattern,
but to have a different thread for each of his key work streams.
Which is not to say that every single thing that you work on
is deserving of this type of monothread,
but that for key persistent work streams,
they often are.
Tip number two is about voice.
Now this is one that if you are a regular listener,
you will have heard me squawk on about endlessly.
I actually strongly advocate that anyone who's interacting with agents,
or basically doing any work on computers at this point,
download something like Whisperflow
as an improved version of their computer's native voice recognition.
But with Codex, you don't even actually have to do that
because its internal speech-to-text system is basically the gold standard.
For Jason, voice is not just about getting the message out faster.
It actually opens up a totally different type of relationship with Codex itself.
The art of the ramble gives you the ability to provide much more backstory.
It allows you to provide richer information about areas of uncertainty versus certainty.
It allows you to explain what you do know, what you don't know,
what you think you know, what you don't think you know,
to name trade-offs, and to allow the AI itself to help you turn messy thoughts into something clear,
rather than having to do that all yourself.
As Jason puts it,
a lot of plans get better when the model has access to the messy version of what I think,
not just the polished one.
This is 100% my experience as well, could not co-sign harder on this particular tip.
Tip three is an interesting one that takes advantage of a key feature in Codex
to break the pattern a little bit of how we interact with AI.
If you are a prolific AI user, you're probably used to an interaction pattern that goes something like,
ask for a particular output, i.e. prompt the thing, wait for it to do its work,
and then once it does its work and delivers things,
you figure out what corrections and changes you want it to make,
and then that whole system repeats.
But Codex's Steer feature allows you to do things a little bit differently,
especially once you've got the first artifact that you're reviewing.
You can actually be starting to build that feedback even as the tool is working.
Steer is the feature in Codex that allows you to add or update the prompt without stopping the flow overall.
Among other implications, this means that you don't necessarily have to get the entire prompt perfect up front.
Instead of this sort of brittle upfront planning,
you can start a little bit more broadly with the overall goals and constraints,
and then as progress comes in, actually steer the conversation
so effectively you and the agent are working in parallel,
and you're not just stuck having to sit around,
wasting time on Twitter as you wait for the AI to do its work.
By the way, voice is the perfect medium for this type of steering,
because once again, as you observe things, as the agent is building,
you can just ramble into them, you don't have to have a perfect constructed sentence typed out every time.
Tip number four from Jason is about memory.
And one of the things that's interesting about it
is that even though Codex has started to introduce native memory features,
you can go to settings, then personalization, then memories,
Jason's argument is that while those things are, quote,
useful for stable preferences, recurring workflows, project conventions, and known pitfalls,
they are not, as he puts it, a replacement for checked-in instructions or an explicit fault.
Jason's core argument is that work should leave behind structured memory,
not just a longer chat.
And so he's built a whole file system in Obsidian,
which if you haven't used, is a simple file-based note system
that interacts with your local environment,
to, in a structured way,
turn his threads into a structured set of context that can be called upon later.
Talking about his durable threads, Jason writes,
A long thread can remember a lot,
but that memory is trapped inside the thread
unless the useful parts get serialized somewhere durable.
The point of the memory system is to turn what the thread learns
into an artifact I can inspect, edit, and reuse.
Jason also shares the specific structure of the vault he puts together
with a top-level agents.md markdown file
that has instructions that say things like,
As you learn more about people,
make progress on projects,
or close an open loop,
update the relevant pages in the vault.
The vault, he says,
holds rolling context around my work.
People, decisions, open loops, daily notes, project state,
and the bits of understanding that would otherwise get lost between threads.
So for any of you who use the personal context portfolio builder
that I shared about a month and a half ago at this point,
while that personal context portfolio builder
was about putting together the broad context
that you would take to any new agent experience,
Jason's basically bringing that back down
to the project-based level
in a way where there is a direct flow
from the big threads where he's working on things
into this vault that gets updated automatically.
He also notes that he keeps the vault as a GitHub repo,
which allows him to also work in the cloud.
This memory section is one of the most overloaded with insights,
which is why I'm sticking a little bit more closely
to what Jason wrote.
For example, he talks about why the review step
of seeing what the agent decided to put in the vault,
i.e. what it thought was important enough to remember,
is a valuable step.
He continues,
I do not want evergreen threads
to quietly accumulate vibes in conversation history.
I want them to write down what changed.
This person prefers this,
this project is waiting on that,
this decision was made,
this loop is closed.
This is also, he says,
why I like memory as files.
Files force the agent to compress experience
into a form that can survive the thread.
If the thread dies,
compacts badly,
or becomes too expensive to keep leaning on,
the useful knowledge is still there.
At that point,
pinned threads start to feel less like chats
and more like different workers
reading from the same notebook.
So some of the other ideas
for things that you could put into that memory
include rules,
taste, i.e. what good means
for tasks that include design, writing, or analysis,
lists of relevant sources,
anti-patterns or what not to do,
links to key artifacts, and more.
Tip number five is about computer and browser use.
Although I think the way
that my codex interpretation summed it up
as tools is a pretty good shorthand.
Tools allow codex to turn into an evidence gatherer.
When you give codex the ability
to use your computer and use the browser,
it can do things like read files,
open pages, run tests, edit artifacts,
check visuals, and more.
And understanding which tool
or which environment matters
for each different type of work
is a key skill.
So if the truth and evidence that matters
lives in code, documents, logs, CSVs,
slide files, PDFs,
or other types of artifacts on your computer,
that's where you're going to need computer use.
When the artifact needs visual inspection,
or it needs to go check live documents
or sources that live elsewhere,
that's where browser use matters.
And then of course,
when the relevant information lives in other systems
like Slack or Gmail or GitHub or Notion or Vercel,
that's when you're going to use connectors.
On the one hand,
this sort of tool use is pretty obviously valuable,
but it still does require a bit of setup
that can feel like you're delaying yourself
when you're just trying to get a thing done.
However,
if and as you move from thinking about codex
as just a different interface
for the same thing that you would have used
ChatGPT for previously,
and instead think of it as the guts
to an entire new work system,
tool-based access to whatever environments codex needs
to have the full context,
and do all the work it needs to do become essential.
And speaking of codex as a new work system,
one of the biggest changes
that is only just starting to emerge
is the idea of being able to disentangle your work
from physically sitting in front of a laptop or desktop.
Codex is pushing hard into this area.
First, it had remote control,
and now of course,
codex is actually available
as a full-fledged feature
in the ChatGPT app.
And for most people,
the implication isn't going to be
that they're going to do everything from their phone now,
but simply that you can work more nimbly.
Thanks to these remote control type features,
you can capture intent while ideas are fresh,
you can help redirect,
or you can steer a thread
without reopening the whole project.
In the same way that Jason's tip
was that steering can be used
to compress the time where you're waiting,
remote control effectively does the same,
but for much longer running work.
If increasingly we have projects
that take on the scale of hours,
not just minutes,
being able to steer them while on the go
is a massive productivity enhancement,
and so it's really worth taking the time
to figure out the relationship
between the full-fledged desktop type experience
and the remote controls
that you can use to interact from mobile.
Tip seven is about heartbeats,
and anyone who built an open claw
will be well familiar with this pattern.
Heartbeats are a recurring or scheduled check-in
that let the thread that you're working on
wake back up.
Heartbeats can be scheduled
on a particular time basis,
like every half hour, every hour,
or they can be tied to specific triggers.
A couple examples that Jason gives,
include his chief of staff thread.
He has a heartbeat that every 30 minutes,
that thread checks Slack and Gmail
for unanswered messages
to help him prioritize what matters most.
This is exactly the sort of feature
that was very common
for the first early build-in experiments
in open claw.
Jason also gives an example
that shows how setting up the ecosystem
that Codex can interact with
can make this sort of heartbeat
even more powerful.
Talking about an animation project,
Jason writes,
I had posted a video in Slack
and asked Codex to check the thread
every 15 minutes for feedback,
re-render a new version
when comments came in,
and reply back into the thread
tagging the reviewer.
The Slack MCP server
could not upload files,
so the agent used Add Computer
to press the Add File button
and post the revised render anyway.
In other words,
what Jason is saying
is that these Slack-specific tools
didn't have an upload feature,
so he just used computer use
to take care of that manually.
The interesting part,
writes Jason,
is not just that it checked
Slack every 15 minutes.
The loop crossed tool boundaries.
Slack for feedback,
re-motion for the render,
Add Computer for the upload.
That is when HeartBeats connectors
in computer use
stop feeling like separate features.
Together, they become a feedback loop
that keeps running
without me sitting there.
Jason's eighth tip
in behavior pattern
is around goals,
although he fully admits
that he's still working
to figure them out right now.
The TLDR of the Slash Goal feature,
which by the way,
is now not only in Codex
but also in Cloud Code,
is that when you have a project
that has a very specific,
knowable,
and verifiable success criteria,
you can use the goals feature
to keep the agent
pushing against that objective
in a way that a normal prompt
might just give up on.
Now, I'm actually going to
skip over goals here
because later in the week,
either as a main episode
or as an operator bonus episode,
I've actually got a full goals guide
also built off of recent tips
from the Codex team themselves,
but suffice it to say
that goals is big enough
for an entire episode on its own
as people really figure out
how it changes the behavior pattern
of interacting with agents.
Jason's last tip
is about the side panel,
and this is one area
where I think Jason is thinking
about things differently
than many others.
He writes,
The part of Codex
I am most excited about
is the side panel.
It's easy to think of this
as a place where previews happen,
but that undersells it.
The side panel is where Codex
stops being only a chat app
and starts becoming the place
where work happens.
For him,
he says it does three jobs,
inspecting artifacts,
operating web services,
and reviewing changes.
And the reason that this
is so important
is that this is the space
that allows him
to parallel process and work
even as the other agent
is working.
The important thing,
he writes,
is not merely that Codex
can generate artifacts,
it's that I can inspect
and annotate them
without breaking the loop.
And I think here
it's worth taking a step back
to recognize that the TLDR
of this entire set of tips
is about exactly that,
not breaking the loop.
How, in other words,
do you allow
the agents inside Codex
to keep working
in parallel
with their human partner
rather than it being
an endless series of turns
between the two?
I think part of the value
of Jason's tips
is even just thinking about that
as the desirable behavior shift.
Which is of course
not to say that
A, you're never going to have
that turn-based interaction
with AI
where you give it a prompt,
you let it do a thing,
and then you review it
when it's done.
Nor is it to say,
I don't believe,
that if you don't have
your agent running 24-7,
you're somehow not maximizing
the value of the system.
But for anyone
who has found themselves
distracted
by the context switching
as you wait
for these ever more powerful tools
to do ever bigger jobs,
this sort of shift in thinking
has a lot of potential
to reintegrate
those work experiences.
So that's going to do it
for our nine tips
from the Codex team
about how to maximize Codex.
There will of course
be a link to Jason's
original post
in the show notes.
Hopefully this helps you
get more out of
one of the most powerful
harnesses you can be using.
For now though,
that's going to do it
for today's AI Daily Brief.
I appreciate you listening
or watching as always,
and until next time,
peace.
Bye.
Bye.
Bye.
Bye.
Bye.
Bye.
Bye.
Bye.
