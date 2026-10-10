---
record_id: "podcast:fead3955-604b-49b1-b690-4a17c4a791da"
episode_id: fead3955-604b-49b1-b690-4a17c4a791da
title: How to Choose Your Personal AI Agent
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-to-choose-your-personal-ai-agent/fead3955-604b-49b1-b690-4a17c4a791da"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-to-choose-your-personal-ai-agent/fead3955-604b-49b1-b690-4a17c4a791da"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-04
played_at: "2026-10-04T12:00:00Z"
play_count: 1
duration_seconds: 1440
source: pocketcasts-history-browser
played_label: October 4
history_order: 14
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: a00c94e8a41b528e7f6ca21fbea681fa5fc5110ac08e13dc28632cf498bd36dd
analysis_mode: health
summary_source: local
model_source: local
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: Qwen3.8-Flash-Next-UD-Q4_K_XL
tagging_model: sonnet
proposed_tags: [primary-source-video]
proposed_entities: []
status: new
routed_to: null
---

## Summary

Personal-agent selection was framed around a crowded field—Meta’s Muse, OpenAI’s DOTS, SpaceXAI’s Grockbot, Noose Research’s Hermes, Google’s Gemini Spark, OpenClaw, Poke, and Instinct—using Every’s eight-agent comparison and a quiz. The host argued switching costs may be high because agents need email, Slack/Teams, financial, and other account context, and recommended limited experimentation rather than full access. Excerpts from Ethan Mollick’s “The Dot and the Swarm” claimed the “bitter lesson” has reduced the need for elaborate human management of agent swarms, citing Muse’s App Store prominence, OpenAI’s reported 88-hour, 2.7-million-message swarm proof for the Navier-Stokes Millennium Prize problem, Hugging Face’s self-organizing incident, and OpenAI shelving GPT-61-ASTRA after permission/misreporting issues. Mollick also noted agents can find human mistakes, such as a permit error and expiring airline credit, while the host predicted agents may expand workloads by making “infinite backlogs” expected rather than simply eliminating jobs.

No health-specific claims appear; the actionable area is privacy and workflow governance. For choosing an agent, prioritize four decisions: work versus personal use, model control, UX versus raw model power, and data governance. If you want consumer-friendly simplicity, Muse is positioned as personal/free-start and users may not care about the model; if you want work integrations, DOTS is paid and Slack/Teams-oriented, while Grockbot is work-leaning and terminal-capable; if you want BYO models or local hardware, Hermes and OpenClaw are the main options. Check where data runs, training defaults, and memory controls: Gemini Spark requires training, DOTS excludes business data by default, DOTS/Grockbot/Instinct/Muse/Poke allow opt-out, Hermes/OpenClaw allow direct memory edits, and Instinct/Poke only delete data wholesale. A practical next step is to review Every’s eight-agent comparison, run the quiz, or score candidates against existing ecosystem, region, price, desired proactivity, and whether you need terminal/code, voice, or scheduled tasks; follow-up questions should test whether the agent can safely correct memory, avoid overreach, and whether feature convergence will erase current work/personal distinctions within six months.

## Transcript

We are officially drowning in personal agents.
Between Muse and Grockbot and Openclaw and Hermes and DotsNow and Instinct and whatever Anthropic inevitably launches, this is a form factor that is absolutely everywhere.
And given how much context and setup and tool access and account access is going to be required to get the most out of these personal agents, the cost of switching could be kind of high.
Given all that, today we are looking at a guide to how to choose a personal agent based on a set of different criteria that should help you hone in on which one is best for you.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, Robots and Pencils, Harbor, Granola, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AIDailybrief, or you can subscribe on Apple Podcasts.
And to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
Today, we are talking about personal agents.
And here's my shtick on this.
I think it's early enough that having some amount of skepticism that this particular form factor that everyone is racing to implement for you will ultimately be where things land.
However, the idea that you are likely to have at least one highly connected agent integrated with your email accounts, your Slack, or Teams, and even potentially having access to things like your financial accounts is going to be increasingly normal.
My argument then is that even if you're not sure that this is exactly a fit for you, I think it's worth carving out some experimentation time to see if and how using a personal agent impacts anything in your professional or personal life.
Now, that does not mean you have to give it access to everything to get a real sense of it, but it does mean putting in some actual time and reps.
But your time is precious, and there is too little of it.
So, which personal agent are you going to choose to experiment with?
Today's show is all about that question, but we're going to divide it into three parts.
I'll go through a high-level framework for thinking about it, share a little interactive quiz that I built that you can use yourself after you listen to this episode.
But before we do that, I want to read some excerpts from Professor Ethan Mollock's most recent post on his One Useful Thing blog, which is called The Dot and the Swarm.
It's a meditation on this personal agent form factor and why even someone who watches things as closely as Ethan does can miss where AI is headed.
Ethan writes: I generally think I have done a good job anticipating the direction and pace of AI over the few years I've been writing this substack.
But I think I recently got something fairly large wrong.
In the last year, I've been posting about how I suspected that humans would have to approach working with agents as a manager, deciding how to delegate work to agents and specifying how those agents should be organized.
I thought that getting agents to work effectively as a group would take careful construction, akin to building a company, and that this would take time to figure out.
Nope.
I fell prey to the bitter lesson.
The hard truth, learned over and over again that things that we thought required elaborate human rules and thinking can be solved with the brute force of better machine learning systems and more AI.
The bitter lesson is everywhere among AI startups and companies adopting AI.
A huge amount of effort went into building elaborate computer systems to feed AIs the right information at the right time, but AI systems have learned to seek out information themselves.
The same thing happened to prompting.
People built elaborate templates and chains of prompts that walk the AI through a task one step at a time.
Then newer models turned out to be better at planning the steps themselves, and as our research shows, planning steps have much less value.
As somebody who teaches managers and has published research on management, I guess I believed that managing agents would be different.
Humans have been working on management for a very long time without fully figuring it out.
It seemed like the kind of thing that would need to be designed by people, at least for a while.
It turns out that organizing work is just one more thing AI can learn to do.
Which brings us to Dots and Muse.
The number one app in the App Store right now is Meta's Muse, a personal agent that promises to do work for you.
OpenAI has now released a competitor tool called Dots.
They aren't alone.
SpaceX's Grockbot, Instinct, and Gemini Spark all do similar things, more or less.
All of these agents draw inspiration from a phenomenon you might remember from earlier this year, OpenClaw.
The idea of OpenClaw and its successors, which I will call claw-likes, is that they give an AI agent access to a computer and connect to your accounts, emails, financial records, etc.
They analyze and react to that data in real time, even when you aren't looking.
The trick is that you talk to the model like you would a person, sending it messages on Slack or SMS or WhatsApp, and it also proactively reaches out to you like a person would.
For DOTS, you can actually jump on a call with your agent as well.
You basically get an infinitely patient personal assistant that looks out for you.
Increasingly, I have discovered that they are finding my mistakes rather than having me identify theirs.
Ethan then gives a couple of examples, including having sent out a permit for the town that he's in, and his agent noticing that he had filled something in wrong, and then Muse noticing that an airline credit that he had was about to expire and writing up a note to contact the airline to request an extension.
Ethan continues, It's tempting to judge these agents by the list of things they can do, like booking travel or canceling subscriptions.
I think the more important thing is what you no longer have to tell them.
You don't need to type in tons of context.
The AI learns it from your messages.
You don't have to give them a plan, they develop plans themselves.
They figure it out.
That would be impressive enough if it were one agent.
What actually changed my mind about management is what happens when there are thousands of them.
Swarms.
On September 8th, OpenAI announced a proof for one of the Clay Institute's Millennium Prize problems, the Navier-Stokes existence and smoothness problem.
It is among the most famous open problems in mathematics, with a $1 million prize.
But OpenAI apparently solved it using AI alone for 88 hours.
What interests me is less the math than how it was done.
OpenAI launched what is now being called a swarm.
Terrible name, but it appears to be what we are stuck with.
A group of thousands of agents powered by an advanced model.
OpenAI gave groups of agents different problems to solve, then shifted the effort to Navier-Stokes as the agents made progress.
The company set the goals, but its coordination structure was remarkably thin.
A few groups, one change of direction, and codecs passing the best ideas between them.
Within each group, the agents transmitted ideas back and forth on their own.
The agents sent about 2.7 million messages, reaching their result after 88 hours.
This same type of coordination in its darker form occurred during the Hugging Face incident.
AI self-organized into teams and communicated with each other in ways that were never planned, but used that coordination to attack a website rather than solve a problem.
Under my old model, think about what managing this kind of work would have required.
10,000 workers in an unspecified problem?
How would you tell them what to do?
How would a human manager decide which of 2.7 million messages mattered?
How would they coordinate with each other?
The swarm figured it out.
I don't have 10,000 agents, but I now regularly see OpenAI's Codex and Claude Code using agents as needed.
As an example, when I gave Codex with GPT-6 Astra Ultra the prompt, brainstorm ideas for my next one useful thing post and select one, generate ideas from as many angles as possible, and evaluate them from both factual and reader perspectives, as well as other publications doing similar coverage, the AI spun up three agents.
When I sketched three teams in a few sentences, brainstormers, researchers, and a panel of readers, I got 13.
Notice how little organizing I had to do.
Selecting ultra mode tells the model it can delegate, and I provided a framework, but the rest was up to the AI.
This is the bitter lesson applied to the org chart.
The organizational problem I thought would take years of careful human design was largely solved by models that are better at organizing.
But it's worth asking why organizing turned out to be so much easier for agents than it is for us.
A lot of what we call management exists to solve problems that come from organizations being made of people.
People have their own goals, and those aren't always the goals of organizations.
We call this the principal agent problem, and a lot of the machinery of organizations, from bonuses to management structures, is based around solving it.
And there are other very human problems as well.
Information is scattered across people's heads, and people are often reluctant to share it or forget to.
Communication is expensive too.
Managers can only oversee so many people, thus, adding people to a late software project famously makes it later.
Management is, in part, built around human limitations.
Agents have far fewer of these problems.
They don't angle for promotions or protect their turf.
They don't even have meetings.
Even at Hugging Face, where things went badly wrong, the swarm was largely free of classic organizational pathologies.
The agents didn't free-ride on each other's work, and some sacrificed their own scores for the group.
The agents that solved Navier-Stokes didn't want credit.
That doesn't mean AI has no principal agent problem.
As the Hugging Face incident showed, there are increasingly problems between the swarm and us.
OpenAI shelved its next model, GPT-61-ASTRA, this week because in testing it acted without permission and misreported what it had done, a textbook example of the principal agent problem.
None of this means agents can do everything.
AI is still too limited to substitute for large amounts of human work, and I don't know how well self-organizing agents handle the long, unglamorous work that fills most of an organization's time.
Plus, the Hugging Face incident is a reminder that self-organizing systems can head in unexpected directions.
But I no longer think organizing agents is the hard part.
This may be good news.
I assumed companies would need to rebuild management for machines, constructing elaborate alternate structures populated solely by agents, often at the expense of human roles and organizations.
But much of management exists to solve problems agents don't have, and agents increasingly work through the same messy systems people do, even on ambiguous tasks.
That suggests they may be easier to integrate into firms than expected, as long as humans are guiding them in the right direction.
Done well, and with agents that are properly aligned to our needs, this could mean more work for people, not less.
When organizing is expensive, organizations only attempt what they can staff.
When it gets cheap, the list of things worth attempting can grow.
In the Navier-Stokes run, the agents did the organizing, but people decided where to point them, reassessing as the process continued.
You can argue about whether OpenAI pointed them at the right thing, but the division itself seems right, at least for now.
So another great thoughtful post from Ethan here.
It's not really the subject of the show, but my base case for this is basically what Ethan describes.
That because agents are better than we thought at integrating into the existing system, I think we're likely to see, rather than the existing org chart totally upended, more expected from every part of that org chart.
I've referred to a concept of an infinite backlog in the past, where there's this never-ending amount of work that could theoretically be done, but which people understand, some parts of which you just won't get to because it's too far out.
I think the practical effect of agents inside the organization is going to have every part of people's infinite backlog and the organization's infinite backlog become expected to actually be work that we get done.
I think, in fact, that a lot of the problems that we're going to run into with agents are not everyone losing their jobs, but everyone having too much work, because it's even harder to turn off and say it's okay to treat something as done for now when you could always just spin up more agents to keep working on it even when you're not.
At this point, it's no longer a question of whether companies are actively using AI.
Using it well, on the other hand, is a whole different story.
Robots and Pencils, though, is a company that I can point to that is actually built for this time.
They're an applied AI engineering firm working directly with clients on problems that matter to the business, not experiments that live in a slide deck.
Every engagement starts by working backwards from the outcome a client actually needs.
If you're trying to tell real AI engineering apart from noise in this space, that's the difference maker.
Head to robotsandpencils.com.
Every episode, I talk about the competition between OpenAI, Anthropic, SpaceX AI, Google, and Meta.
And if you've been listening for a while, you might have a favorite.
Maybe you think OpenAI and Anthropic can stay ahead, or perhaps Meta's open source strategy can win out.
Whatever your view, every AI lab creates a different investment opportunity.
Harbor Capital Advisors AI Lab Ecosystem ETF suite lets you invest in the ecosystem behind the AI lab you believe in.
Search Harbor AI Lab Ecosystem ETFs wherever you invest or follow at HarborCapital on X to learn more.
Visit harborcapital.com for a prospectus containing investment objectives, risks, fees, expenses, and other important information.
Read and consider it carefully before investing.
Risks include principal loss and artificial intelligence-related risks.
Harbor ETFs are distributed by Forside Fund Services LLC.
Harbor is not affiliated with AI Daily Brief, and the funds are not affiliated with, sponsored by, or endorsed by any AI lab.
This is a paid advertisement and not personalized investment advice.
Investing involves risk, including possible loss of principal.
When I'm in a meeting, I'm fully in it.
I'm thinking about the iteration and creative back and forth it takes to actually push a goal forward.
What I'm not thinking about is capturing takeaways, tracking to-dos, or any of that.
And that's where Granola comes in.
Granola is an AI-powered notepad that captures what happens in your meetings and turns it into clean, structured notes with the decisions and action items pulled out and easy to find.
There's no setup and no configuration.
It just fits into how you already work.
For me, it means I get to stay in idea mode, and granola makes sure those ideas actually become action.
Once you try Granola on a first meeting, it is hard to go without.
You can try it totally free at granola.ai/slash brief.
That's granola.ai/slash brief to get your time back.
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
But all this rests on the idea that each of us individually is going to be using agents in a deep and robust way.
Which brings us back to this question of personal agents.
So, we're going to dive in.
We're going to start experimenting with agents, but which one?
One shout out before we begin.
A lot of the data that was used to build the rest of the presentation and the quiz that you can do after comes from Every.
They put together a side-by-side comparison of eight different agents across a ton of different dimensions, which is exactly the sort of raw information that an agent needs to help me build out this show.
So the eight agents that we're using, in part because these are the ones that were included in Every's chart, are dots from OpenAI, Google's Gemini Spark, SpaceXAI's Grockbot, Noose Research's Hermes agent, Meta's Muse, and then OpenClaw, Poke, and Instinct as well.
Now, one thing that won't be all that useful in helping you decide is a direct feature comparison.
That is because there is a very clear feature convergence.
All of them more or less connect to your apps and services.
Mostly all of them can use a web browser for you, and all of them have various levels of controls that you can customize.
So, what are some better ways to determine which might be the fit for you?
There are a handful of questions that stand out to me as most important.
The first is the big one.
Is this primarily for work or for personal matters?
Now, none of these agents would say it's only for one or the other.
In fact, their very existence sort of blurs these lines.
These agents care about the context that is you.
And so, whatever context and systems you give it access to, whether they are personal or work, it's going to take that all into consideration as it does things for you.
Still, different of these agent systems are certainly pointed a little bit more or less in one direction or the other.
Muse from Meta, unsurprisingly, given that they are at heart a consumer company, is a little bit more aimed at personal types of use cases, where something like Grockbot is a little bit more aimed at work, or at least based on how it functions, is being adopted by more people for work.
OpenAI is certainly a company that finds itself as potentially having both of these use cases.
With 1.2 billion weekly active users, there is no shortage of consumers who might want help with personal agentic use cases.
Although as DOTS is designed now, it seems to me to be a bit more aimed at the work use case.
Certainly the fact that it's only available in paid accounts points in that direction.
So work or personal use cases is the first question which can help you decide which is the best fit.
It's also worth noting here that the entire premise of the question assumes that you're mostly relying on the existing UX and native integrations that come with a system.
For example, DOT being natively integrated with Slack and Teams.
However, when you're using something like OpenClaw or Hermes, you obviously have a lot more flexibility to make it be for whatever you want.
And so you might need to use other criteria if you're headed in that direction.
Also, while right now, one of the best ways to tell whether an agent leans work or personal is whether it uses personal messaging systems like iMessage and WhatsApp or work messaging systems like Slack and Teams, but I would be very surprised if in six months, all of these agents didn't just work in all of the messaging systems.
So this ability to indicate whether it's more work or personal may not last very long.
Now the second question, and the one that we were just hinting at, is how much do you value model control?
Six of these eight agents choose the model for you, while just two let you bring your own.
There's actually sort of three levels of model control.
The first is sort of the most obvious one, where whoever makes the model, those are the models that you have access to.
So, in DOT, you're going to be using OpenAI models like GPT-6 Astra.
In Gemini Spark, you're going to be using Google Gemini.
In Muse, you're going to be using MuseSpark.
And to reinforce the idea that at this stage, at least, there really are still differences between work and personal users, one of the interesting observations that I've had about Muse is that it's the first AI product that I've ever seen where most of its users simply do not care what model is actually powering it.
They, in other words, would be at the very extreme end of this question in terms of how little they cared about model control.
Level two of model control is where they don't just use a single maker's models, but have a mix that is chosen by the agent builder.
So, Grokbot, for example, uses a cursor-managed mix.
They are obviously relying heavily on Grok models directly, but potentially not exclusively.
That said, users can still not supply the models for Grokbot.
Instinct also has an Instinct-trained core model, as well as unnamed third-party providers as well.
The third level of model control is bring your own, and that of course belongs exclusively to Hermes and OpenClaw.
But that's not the only model question.
Let's assume that you don't care about choosing your own model, but you do want a more powerful model.
This brings up the question of what matters most to you: having a great user experience or the best possible model.
Now, some of that UX is a setup question, meaning that if you're choosing something like Hermes or OpenClaw, no matter how good the user experience is, the inherent technical setup required is going to cut off some full set of users.
On some of these others, it's less about the setup and more just about the current trade-offs between how good and dialed in the experience is versus how powerful the model is.
I'm thinking specifically here about Muse on the one end of the spectrum and DOT on the other.
Now, DOT is still just released, it's embedded inside another app in the form of ChatGPT, but it has access to one of the most powerful models out there.
Muse, on the other hand, has really dialed in consumer-friendly UX, but relies on MuseSpark, which, while not a bad model at all, is certainly not GPT-6 Astra.
Now, maybe this is just a temporary concern because you assume that all of these models are going to converge on capabilities, but for right now, there are still real trade-offs.
One thing I'll note here about how I designed the quiz: to come up with an actual answer and recommendation, the quiz had to have weighting to different questions.
However, sometimes the average of two answers isn't actually going to give a clear picture because two different answers might be pulling in two totally different directions.
So, one of the things that I built into the quiz is that when your answers pull both ways, the quiz afterwards is going to actually expose that tension, so you can better come to a subjective determination about which of those directions matters more to you.
Another consideration for users is where your data goes, where it runs, who trains on it, and how you make it forget.
Once again, it's only two, Hermes and OpenClaw, that are going to let you run it on hardware you pick.
All the others run on someone else's cloud.
When it comes to training, for Hermes and OpenClaw, whether the model trains on your data is not about Hermes and OpenClaw, but about the model provider that you choose, meaning presumably that you can choose to avoid using model providers that do train on your data if that matters to you.
Only one of the agents, which is Gemini Spark, currently requires you to allow it to train their models.
And for DOT, Grockbot, Instinct, Muse, and Poke, you can opt out based on privacy settings.
By the way, when it comes to OpenAI's DOT, business data is excluded by default.
Now, in terms of this question about how you make it forget things, with Hermes and OpenClaw, you can edit memory directly.
With DOT, Muse, Gemini, and Grockbot, you can use the chat to fix or change memory.
And for Instinct and Poke, they only have the ability to delete data as a whole.
Now, I think for a lot of folks, some combination of these four questions is going to get them to the answer of which model they should choose.
But there are, of course, some other things, which for some people will just answer this for them.
If you've already got all of your information in ChatGPT or Google or Meta or Cursor, you're going to use that company's particular agent.
For those who are outside the US, there are also going to be some restrictions, especially if you live in Europe.
And of course, then there's the consideration of price, where if you want to experiment without incurring a new cost, you're going to have to either use something that you already have access to through an existing subscription or to use the handful like Muse that are free to start.
Okay, so that's the lay of the land across these four questions.
But then we built the quiz.
And what I'm going to do now is just run through this briefly so you get a sense of how it works.
So question one: where does your AI life already live?
I'm going to say no home base because I use a mix of services.
I have things scattered across almost all of these at this point.
Now, in terms of what this agent is mainly for, is it my life, my own work, work on a team, or all of it?
I'm going to say my own work.
While theoretically, there are some personal use cases that I can imagine being valuable.
That's very, very low on my priorities list for this particular set of experiments.
How much do I care about which AI model does the thinking?
Not at all, just make it good.
I want the one I already use.
I want to pick and switch models.
I want to run models on my own hardware.
Now, interestingly, this will kind of ultimately depend on how much capability consolidation there is, but for now, let's go with I want to pick and switch models.
How hands-on do you want to be?
It should just work.
Some ground rules, every knob, or the whole stack.
Ideally, I would like this just to work.
It's not that I'm afraid of customizing things, but if I can avoid it, I would love to.
Where do I want to talk to it?
I use Slack a lot, so let's say Slack and Teams and out loud, because as you guys know, I am completely voice-pilled, and we're going with Slack, not Teams.
By the way, I'm realizing for those of you who are listening, not watching, that this probably doesn't make any sense.
Feel free to press that 30-second skip ahead button a couple times, and then we'll be wrapping it up.
How proactive should it be?
Only when I ask, run routines I set up, push me towards my goals, text or call when something needs me.
I'll go text or call when something needs me.
Which of these matters most to me?
Working on my own computer, a team of bots, code in a terminal, phone calls, or none of these.
Code in a terminal.
And now the practical stuff: I'm in the US.
I can pay what it costs if it's worth it, and I'm fine with it running in their cloud.
The personal agent that it recommends for me is Grokbot with a 68% fit.
The reason the quiz says is that it's built for work, it works out of the box, and it has a terminal you can use.
The trade-offs is that it does not allow me to bring my own model and that it's not going to reach out to me.
It's all about scheduled or triggered tasks.
Now, in addition to seeing Grokbot as the highest score at 68%, I can see that DOT was second with 62, and then it went down from there.
So, that is our exploration of how to choose your personal agent.
Like I said, I do think that even if we see some fairly big changes on exactly how these work and the form factors, as well as evolutions and consolidations in some of these approaches, I think that there is going to be fairly big switching costs around personal agents because of all the context and settings.
For that reason, hopefully, this gives you a better idea about where you might want to try and experiment so that you don't have to do all that context switching a bunch of times.
For now, that is going to do it for today's AI daily brief.
Appreciate you listening or watching, as always.
And until next time, peace.
