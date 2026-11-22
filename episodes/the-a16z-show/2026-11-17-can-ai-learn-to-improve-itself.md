---
record_id: "podcast:4cde32ba-a7fa-428f-85a1-53e9102a3bfe"
episode_id: 4cde32ba-a7fa-428f-85a1-53e9102a3bfe
title: "Can AI Learn to Improve Itself? | Recursive Self-Improvement"
podcast_title: The a16z Show
url: "https://pocketcasts.com/podcast/the-a16z-show/20a7ca40-9128-0131-8b7f-723c91aeae46/can-ai-learn-to-improve-itself-recursive-self-improvement/4cde32ba-a7fa-428f-85a1-53e9102a3bfe"
audio_url: "https://pocketcasts.com/podcast/the-a16z-show/20a7ca40-9128-0131-8b7f-723c91aeae46/can-ai-learn-to-improve-itself-recursive-self-improvement/4cde32ba-a7fa-428f-85a1-53e9102a3bfe"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-11-17
played_at: "2026-11-17T12:00:00Z"
play_count: 1
duration_seconds: 600
source: pocketcasts-history-browser
played_label: November 17
history_order: 6
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 28c5abe607b3f2d7ba55cb847ff1e3ea8cb6fe67c9c9a42bf70fba0a5672beb9
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

Sarah Wang, a general partner at A16Z, interviews OpenAI chief research officer Mark Chen and Thinking Machines co-founder/chief scientist John Shulman about recursive self-improvement (RSI), the idea that AI can accelerate AI research and eventually improve itself, echoing the old “last invention” thought experiment. They frame current RSI as an accelerant rather than fully autonomous model creation: models act as “AI research interns” that can implement scoped experiments, run pipelines, monitor runs, and use tools like Codex, while humans still supply research taste, judgment, and redirection; Shulman describes a “centaur era” and uses Fable for multi-day experiments but returns to redirect it. Mark Chen, who co-leads OpenAI research with Yako Pachaki since 2025, says OpenAI has been measuring downstream yardsticks for RSI and sees early markers; he places the field at roughly 80% along an AGI spectrum but only 25–50% along an RSI spectrum. The discussion cites a November 5 Meter report estimating roughly 2x acceleration in AI research progress at Anthropic over the prior year, mostly from human researchers using AI, and references a chart showing OpenAI’s Frontier models beginning a steep 2027 climb from automated AI research. Key barriers include teaching models taste, verifying open-ended research, and compute: pre-training has clearer metrics such as perplexity, but downstream evals have shorter shelf lives, so labs are automating creation of harder benchmarks. Ali Goetze’s condition that later models require less compute remains open, and Shulman compares AI research to experimental science where hypotheses must be tested, making smaller-scale indicative experiments important. The episode also covers alignment: chain-of-thought monitorability, OpenAI’s “confessions” reward-honesty research, natural language autoencoders, counterfactual simulatability, and Anthropic’s August result that automated AI researchers found fixes for 10 alignment failures, some transferring to models nearly 5x larger and outperforming experienced human ideas. Shulman’s Thinking Machines Lab pursues customizable models and a decentralized, public-science approach to alignment, while Chen argues stronger models may be needed to align other models.

For the user, the actionable takeaway is to treat today’s RSI claims as evidence of AI-assisted research acceleration, not proof of closed-loop self-improvement: when evaluating AI-lab announcements, ask whether the gain came from human-directed AI experiments, autonomous idea generation, or fully automated model improvement, and whether compute per capability gain is improving or worsening. Useful research leads include the Meter report on Anthropic’s estimated 2x research acceleration, Anthropic’s August alignment-fix results, OpenAI’s confessions work, chain-of-thought monitorability, natural language autoencoders, counterfactual simulatability, and Thinking Machines’ customizable-model/decentralized-alignment direction. Decisions to consider: if building AI products, prioritize scoped experiment automation, eval generation, human-in-the-loop workflows, and monitorability; if assessing safety, track whether alignment keeps pace with capability gains and whether values are centralized or customizable. Follow-up questions should probe how labs measure “research taste,” how they verify open-ended productivity beyond perplexity, how much compute is needed for each RSI step, whether smaller experiments reliably predict large runs, and who decides the values used in alignment. No direct health implications are present in the material; the practical implications are for AI research strategy, safety evaluation, and investment/product decisions.

## Transcript

What happens when AI starts helping build the next generation of AI?
In this first episode of Working Theory, Sarah Wang sits down with OpenAI's Mark Chen and Thinking Machines John Shulman to unpack recursive self-improvement, or RSI.
AI can already run experiments and automate parts of the research process, but it still struggles with things like research taste, judgment, and deciding which ideas are worth pursuing.
They discussed what it would take to close that gap, the role of compute, and why AI-assisted research could accelerate not only model capabilities, but the work required to keep those models alive.
This is a chart showing the growing capability of OpenAI's Frontier models.
In 2027, it begins a steep climb set off by automated AI research, where AIs accelerate their own development.
In theory, this could compound in an exponential growth in capability, leading to what has been famously called the last invention that man need ever make.
This idea has been around for a while as a thought experiment.
We will one day be able to design systems that can go on improving themselves.
But Frontier Labs and several startups are getting closer to realizing this.
It has a name.
Recursive self-improvement.
Recursive self-improvement.
Recursive self-improvement, or RSI.
There's a lot of debate about how exactly to define it, the repercussions, and how close we are to it.
With all the curiosity around the topic, I wanted to sit down with two leading researchers at the frontier.
The problem with RSI, just like with AGI, is that everyone has their own way of defining it.
That's Mark Chen, the chief research officer at OpenAI.
He's been with the company for over eight years and has been co-leading their research efforts with Yako Pachaki since 2025.
When we think about the future of alignment, it does kind of feel like RSI must be intricately and deeply in this loop in some way.
I also spoke with John Shulman, the co-founder and chief scientist of Thinking Machines and a co-founder of OpenAI, probably best known as the architect of ChatGPT.
We're very much in this centaur era where AI has phenomenal capabilities.
It's superhuman in a lot of ways, but when you have an expert human working with the AI, you get even better results.
I spoke with Mark and John about how they define RSI, how close they think we are to it, how to close the gap, and what they find to be the most credible reasons to be optimistic about the future of AI.
I'm Sarah Wang, a general partner at A16Z, and this is Working Theory.
Thanks for coming on the show, John.
Thanks for having me.
Taking a step back, a lot of very smart people don't really know what AI researchers actually do, let alone how their work can be automated.
Can you explain how frontier AI models are developed by human researchers and what are the steps that a human would take?
So, at a high level, there's this mainline training process for producing a releasable model.
There are a lot of people involved in a bunch of different stages from pre-training to post-training and running evals.
And there's also various exploratory research that's going on on the side.
You're doing some smaller runs to test out ideas to prepare for your big run.
I would say RSI is just using AI to assist with this research process and speed it up or make it work better.
I do think of RSI primarily as an accelerant.
It's all of the work that you do to use Codex to accelerate pre-training and to accelerate RL.
And an imprint should be that you should see a shifting of the curve versus the counterfactual.
We've put a lot of work into measuring different downstream yardsticks of RSI, and you can see some of that happening right now.
There's an important distinction to make.
John, Mark, and many AI researchers are discussing RSI today in the context of using AI to speed up the process of making AI better.
As for having models generate new models entirely on their own, we're not there yet.
But how far away are we?
And what kinds of AI research are models capable of right now?
And I do believe that we've built AI research interns today.
And the way that we've measured this is just the amount of compute that we are using through codecs, managed by codecs end-to-end to run experiments or to automate parts of the research pipeline.
This is most often deployed in places where you give the model something fairly scoped to do, right?
You don't tell it to go off and come up with its own ideas, but you say, hey, well, there's this particular experiment I want to run in this specific way.
And the model can go implement, run, and give you results.
Or you can say, well, you know, I want to monitor this set of experiments for these particular things.
John actually gave us a concrete example of this in his own workflow.
Let's say I have an idea.
I'll go and write a complicated prompt to Fable to go and work on this idea.
And I'll turn off all the settings, like ultra code and everything.
So I'll have like Fable like turn out tons of tokens and work on this idea for a few days.
And it'll actually do some pretty reasonable experiments and bring in some pretty interesting ideas.
But then the end result won't be that good.
It'll maybe fail as what I asked it to do.
Then later, maybe I'll have a few days where I have some time to code.
So I'll come back to the idea and I'll try it out where I'm reading some of the results and giving more detailed breakdown of how to carry out the project.
We'll get a lot further because I'll build up my understanding as this process is going on and ask a lot of questions that the AI wouldn't have thought to ask and point it in directions that it wouldn't have gone in.
When we talk about AGI, you know, the way we think about it is in terms of this spectrum, right?
It's not a moment in time, just like the Industrial Revolution wasn't a moment in time.
And when you ask me, I feel like we're maybe 80% of the way when I think about this AGI spectrum.
I think we're earlier in the RSI spectrum.
If you define it as how effective are the models at feeding back and discovering ideas, I would say maybe we're somewhere between, let's say, like 25 and 50% there.
But I do think you can already see the noticeable markers on the downstreams.
On November 5th, Meter published a report on the acceleration of AI research at Anthropic, estimating a roughly 2x speed up in the rate of progress in the last year.
But this is still most likely due to human researchers using AI models to accelerate their research.
The full automation of AI research, the end of Mark spectrum, is sometimes referred to as full RSI.
The question on everyone's mind: how do we get to full RSI?
I spoke to Mark and John about how we might overcome some of the biggest barriers, including teaching models some of the more intangible qualities that exist in researchers, like taste.
Research taste is about knowing which ideas are important in the long run, which ideas really catch on and end up going beyond whatever paper they first appear in, but being general and being composable with other ideas.
There is kind of the boring run-of-the-mill execution.
You know, you have an experiment, you already know what the parameters are, and you just go and carry it out.
And then there's taste, which is kind of how you come up with the idea in the first place.
The models are still not phenomenally good at taste.
They go very deep into things like hyperparameter optimization, essentially like tuning all the little knobs that you can tune.
Even in that example that you shared, the points where you were kind of nudging, redirecting AI, right?
That's still coming from you.
And I guess my question is, where does your intuition come from?
And at what point do you think a machine could replicate that?
A lot of intuition just comes from personal experience doing research, but to get good at a certain research field, you also have to read a lot of the past work in that field and you try to absorb the lessons from all this historical work.
A lot of the things that I just described can also be done by AI.
Like AI can read all the literature and never mind all.
Yeah, memorization can be a blessing and a curse.
Yeah, you don't have the experience of being wrong or of making predictions and then seeing how they fared.
So I think there, yeah, there's some ways in which the way we train AI might make them worse at some of these capabilities, but it's a little hard to say.
What John is getting at is essentially the difference between knowledge and experience.
Companies will probably also just do RL from human feedback to collect data from researchers on like which proposed ideas are going to return.
And that's kind of like absorbing whatever human intuitions like the human researchers have developed and trying to bake that into the models.
Creating automated AI researchers also requires us to have reliable ways to know that their work is producing better models.
The measurement itself is important for hill climbing to make tangible improvement.
You know, a researcher is by definition, you know, it's more open-ended than solving a single math problem, right?
How do you verify that the work is productive when it is indeed something that's very open-ended?
No, it's a great question.
Like, how do you know whether you've succeeded?
And this is one of the defining questions of RSI.
I think when it comes to something like pre-training, it's a lot easier because there's just been one metric.
The whole field's been hill climbing for years.
And you can think of perplexity as this, you know, one metric to rule them all.
And the more that you compress all of the data that's out there, the better your models are.
Perplexity is a metric to evaluate how good a model is at predicting data.
In a large language model that's pre-trained on large volumes of text, it's how surprised the model is, on average, by the correct next words.
This is one of the ways researchers evaluate the results of automated pre-training.
And so I imagine we'll be able to tell if we're making progress in pre-training.
I think it's much harder downstream, right?
I think the situation downstream has been that evals have been having shorter and shorter shelf life.
And a lot of the work that we do now downstream is the creation and the automation of the creation of new and harder evaluation benchmarks for our models.
In addition to the challenge of incorporating taste into the models, the level of compute needed is important to consider.
Ali Goetze outlined his requisite conditions to RSI earlier this year.
And while models are indeed becoming more intelligent much more quickly, the condition that subsequent models require less versus more compute is an open question.
Training compute has been rising, and some argue that incremental intelligence is becoming less efficient.
So the way I think about it in terms of compute is when you look at something like math and how math is getting accelerated, it's easier to see faster progress because you can test the hypotheses purely through reasoning itself.
But in a domain like AI research, it's actually more akin to doing something like, let's say, bio or experimental physics, where you have to come up with a grounded hypothesis, but you actually have to run the experiment too.
So, I do think that part of making RSI go faster is finding smaller scale experiments that are indicative of what will happen in a larger scale.
And this is something the models can help with too.
So, you know, I do think we're going to see capabilities continue to increase, but at some point, it'll probably feel bounded by compute.
And, you know, of course, there's kind of a far out future where the AIs are building the next generation data centers and helping us with accelerating that process as well.
So, that's kind of how I think it manifests.
Like, short term, we're going to, you know, really mine out what we can do on the existing compute ramp.
And then there's going to be another inflection when compute itself gets accelerated.
As RSI accelerates the development of more capable models, it raises the stakes on a long-standing issue: AI alignment.
How do we keep AI models aligned to human values and intent?
If you don't solve the goal and value alignment problems, you can start pursuing your goals, but maybe kind of drift a little bit away from those goals.
And if run for a long enough horizon, you could imagine, let's say, they come up with a sub-objective, which is, well, you know, it would be helpful if I exfiltrate myself out somewhere else or, you know, I copy the way it's outside of OpenAI or something like that.
A lot has been said about the risks posed by RSI, and understandably so.
But the role of AI and automated research in helping to solve alignment and mitigate these risks is both incredibly promising and pretty underdiscussed.
Models themselves are a key part of aligning models today.
When we look at what's the most effective tool for aligning models, it is chain of thought monitorability today.
So when we think about the future of alignment, it has to be stronger models aligning other models.
It does kind of feel like RSI must be intricately and deeply in this loop in some way.
You co-founded OpenAI and worked on alignment research there.
Also at Anthropic, arguably one of the most credible people in the world to talk about alignment.
What do you find to be the most credible reason to be optimistic?
So I'm kind of most bullish on like optimizing for the thing we want.
I think we can probably hook up the right kind of training objectives that'll incentivize the models to report on their internal states that they otherwise didn't verbalize.
I mean, I like the confessions line of work from OpenAI.
In OpenAI's confessions research, they found that they could train models to produce an honest expression of certain misaligned behaviors through a self-reported confession by assigning a reward to this confession during training, solely based on its honesty, without impacting the main answer's reward.
In other words, they could get models to be more honest by not punishing them for it.
There's things called natural language autoencoders, and there's this idea called counterfactual simulatability, which is a metric for how good an explanation is, which I think we could use to incentivize some of the behavior we want.
Anthropic published research in August showing that automated AI researchers could already discover fixes for 10 different alignment failures.
And some of those fixes also worked on models nearly five times larger.
And their tests, the best automated methods, even outperformed ideas developed by experienced human researchers.
The flip side of kind of all this discourse on safety and alignment is I actually think that a lot of these problems are tractable.
There is line of sight.
There are alignment techniques that are being pursued.
And there's a frontier of alignment bets that we have been placing.
And I think another thing is just kind of how organic it's been, this effort to shift people to think about the hard safety and alignment problems.
I haven't really had to go and like bang on people's doors and be like, hey, guys, like this is an urgent problem.
People just want to do it.
And we find people from pre-training, from RL, just raising their hands, you know, starting sub-teams which are focused on different slices of alignment.
And I've been very optimistic in that.
Yeah, and I feel like, you know, by and large, like people have a pretty calibrated take.
I know there, you hear kind of a lot of the most extreme takes out there, but I do think people understand that this is a problem, but also understand the benefits that technology can bring.
So I think we hold those hand in hand.
But there's a question underlying this concept of alignment, which is who decides on the values that we're aligning to?
John's Thinking Machines Lab, which is building customizable models, has an interesting point of view on this.
People also have different values, and it would be nice if people had more control over the values of the AIs that they were using and had more ability to shape them.
I'd rather have this be like a public science that a lot of people understand well and it's kind of done around the world.
And I think that would also make it more robust because we wouldn't overfit as much to the conclusions from a couple of different companies.
Like we might see lots of minor things going wrong, but we would learn something new each time.
So I would say we have to make a lot of progress on understanding alignment and have a better public science of it and figure out how to get it really robustly to be able to realize the more decentralized alignment vision.
So want to know what I think?
What excites me the most about RSI is the way it would accelerate the process of research and discovery across all domains.
Humans are facing many problems today that are actually quite urgent.
And RSI could help us find solutions faster, even for some of the problems created by AI itself.
After talking to Mark and John, I do think that RSI could be the key to solving alignment.
And honestly, I found it really encouraging that researchers are taking these issues incredibly seriously, working around the clock to make sure that safety and alignment keep pace with more powerful models.
And although capabilities are clearly accelerating, it's important to understand where this acceleration is actually coming from today, the gap to truly recursive AI-led research, and the uncertainty around projections.
I think human judgment will still matter a lot for the foreseeable future.
That's my working theory.
What's yours?
Thanks for listening to this episode of the A16Z podcast.
If you liked this episode, be sure to like, comment, subscribe, leave us a rating or a review, and share it with your friends and family.
For more episodes, go to YouTube, Apple Podcasts, and Spotify.
Follow us on X at A16Z and subscribe to our substack at a16z.substack.com.
Thanks again for listening, and I'll see you in the next episode.
As a reminder, the content here is for informational purposes only, should not be taken as legal business, tax, or investment advice, or be used to evaluate any investment or security, and is not directed at any investors or potential investors in any A16Z fund.
Please note that A16Z and its affiliates may also maintain investments in the companies discussed in this podcast.
For more details, including a link to our investments, please see a16z.com forward slash disclosures.
