---
record_id: "podcast:a5f20c6e-1ddc-4ee7-81d2-ba0df9828d91"
episode_id: a5f20c6e-1ddc-4ee7-81d2-ba0df9828d91
title: Fable 5.2 Is the Best AI Ever. So Why Am I Not Switching Yet?
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/fable-52-is-the-best-ai-ever-so-why-am-i-not-switching-yet/a5f20c6e-1ddc-4ee7-81d2-ba0df9828d91"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/fable-52-is-the-best-ai-ever-so-why-am-i-not-switching-yet/a5f20c6e-1ddc-4ee7-81d2-ba0df9828d91"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-11-10
played_at: "2026-11-10T12:00:00Z"
play_count: 1
duration_seconds: 360
source: pocketcasts-history-browser
played_label: November 10
history_order: 3
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: bf74880045b7570d2c6b4723a178cb999bdf3fc5b14178f6a936fed7522f14c6
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

Anthropic’s launch of Fable 5.2 and Mythos 5.2, framed as a pre-IPO flagship release, dominated the discussion: Fable was called the most powerful model yet, yet reviewers struggled to identify everyday use cases. Benchmarks showed Fable 5.2 leading the Artificial Analysis Intelligence Index at 65, occupying the top three effort settings, and beating GPT-6 Astra by 4 points and Opus 5.5 by 3.5 points on Frontier Code; Mythos 5.2 led cybersecurity by about 10 percentage points; Fable scored 64.9% on RoboDojo Sim, 25 points above Opus 5.5, and Mythos scored 85.1% on protein design. On agentic knowledge work, AA Briefcase improved about 5 points over Fable 5.1, Opus 5.5, and Gemini 4 Carbon, but its ELO was lower than Opus 5.5, while the Remote Labor Index jumped to 41.3% from Opus 5.5’s 21% and 2.5% a year earlier, which Garrison Lovely called alarming. Pricing fell 20% to $8 per million input and $40 per million output, but per-task costs remained high: $26.54 at max, $14.83 at extra high, and $9.08 at high, with Anthropic recommending medium as default, high for everyday coding, extra for long agentic work, and max only for ceiling tests; Matt Schumer argued low might suffice. Anthropic’s examples included 90% of code changes written by Claude under supervision, a Python-to-Rust migration, an OS built from an empty folder by 1,000 sub-agents over eight days, black-hole physics solutions, capsid modeling for 28 of 34 attempts, and a 30-hour machine-readable Fermat’s Last Theorem proof using 1,000 agents. Community reactions included Ethan Mollick’s “jagged AGI,” Dan Shipper/Every’s “paradigm shift if you know what to do with it,” Allie K. Miller’s ambitious multi-project tests, Leander Builds and Pavel Hurin’s security/bug findings, including 58 bugs versus Sonnet 5.5 Max’s 51, Riley Brown’s live video ad, Theo, Chebian X, Stefan Vascovich, Boris Cherney, and sponsor segments from KPMG on GEO, C Data on AI gateways, Granola on meeting notes, and Blitzy on code security.

Actionable takeaways: there are no direct health implications in the material, so no medical action is warranted; the practical decision is not to switch wholesale to Fable 5.2 but to reserve it for high-value, ambiguous, long-running, measurable tasks such as security audits, code migrations, custom software, game mechanics, scientific calculations, and ambitious agentic builds, while using Opus 5.5 for routine knowledge work where it may be cheaper and comparable. A user should run their own evals before adoption: plant bugs or vulnerabilities, test a real repo audit, compare Fable and Opus on a defined task, measure cost per completed task, and try effort settings from low/medium/high rather than assuming max is needed. Research leads include the Remote Labor Index as a labor-automation signal, the “jagged frontier” of strong capability paired with poor self-evaluation, Anthropic’s science/robotics demos, and enterprise controls such as C Data-style gateways, Granola-style meeting capture, and Blitzy-style code-security graphs. Follow-up questions should focus on whether Fable improves end-to-end completion enough to justify token spend, which workflows have clear success metrics, where human taste and relevance judgment remain necessary, whether autonomous business or content generation is safe to delegate, and how to catch errors that the model’s own critics, fact-checkers, or judges miss.

## Transcript

As the Anthropic IPO gets closer, we have officially gotten a new flagship model.
The company dropped Fable 5.2 and Mythos 5.2 yesterday, and a lot of the first reactions are exploring the fact that in some ways it is clearly the most powerful model we've ever had, but on the other, it's powerful in ways that don't make it abundantly clear exactly when and where most people will actually use it.
How much is this specific to Fable 5.2 versus just the reality of new models at the capability level that we're at?
That, plus everything else about Fable 5.2, is what we'll be looking at on today's episode.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, C Data, Granola, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AIDailybrief, or you can subscribe on Apple Podcasts.
And if you want to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
The website is also where you can find out about everything going on in the ecosystem.
We've got a new training program coming up with Super Intelligent focused on AI champions, i.e., the key pillars of organizational and enterprise AI, who help not only do the AI projects, but bring AI across the organization.
And you can also find a link to how we got here, my new longer form historical show that tells about the set of cultural, economic, political, social events that all went into today's most important phenomenon.
The most recent episode is about prediction markets and how gambling on everything from our phones became normal.
Check it out.
And if you like it, you can subscribe.
Again, that's how we got here with NLW on any podcast app.
But let's go see if this new model from Anthropic has any implications for how I do that show or this show or anything else that I'm working on.
Welcome back to the AI Daily Brief.
Well, friends, you knew it was coming.
No matter how much people have loved Opus 5.5, and as we'll talk about today, they continue to love Opus 5.5.
You always knew that in the run-up to the Anthropic IPO, we were going to get a new Fable model.
That model, plus its Mythos equivalent, has arrived.
And on the one hand, people are finding it unbelievably easy to describe as the best model that has ever existed.
And yet, on the other hand, people are, in certain circumstances, struggling to identify what it's actually going to be useful for.
To give you just a little preview of the nature of the discourse, even Professor Ethan Mollick decided that the best way to frame his exploration of the model was about asking whether it was officially AGI.
So, what we're going to do today is first, rip through the benchmarks pretty quickly.
Second, look at some people's first impressions and the types of things they're using it for.
Third, dig into the deep dive analyses to see where it's actually going to fit in our model stacks.
And finally, end on a few tips for how to use it best.
Now, in terms of those benchmarks, simply put, Fable 5.2 lifts the bar on what AI can do.
Across every category, Fable is head and shoulders above anything that's come before it.
In coding, Fable 5.2 was four points ahead of GPT-6 Astra in second place, and three and a half points ahead of Opus 5.5 on Frontier Code.
On Agentic Scientific Research, it was a full six points ahead of previous leader GPT-6 Astra on Terminal Bench Science 0.1.
On cybersecurity, they focused on Mythos, and in each case, Mythos 5.2 was about 10 full percentage points ahead of the previous leader.
And on top of all that, Anthropic also included a bunch of non-standard benchmarks for emerging capabilities that we're not used to seeing.
For example, on robotics, Fable 5.2 scored 64.9% on RoboDojo Sim, adding 25 points to Opus 5.5's score, which itself was a breakout result compared to other models.
In protein design, Mythos 5.2 scored 85.1%, which was six points higher than Mythos 5.1.
Now, the one place where there was some complication was agentic knowledge work.
On AA Briefcase, Fable 5.2 was about 5 points ahead of Fable 5.1, Opus 5.5, and Gemini 4.
Carbon.
However, its ELO score was actually lower than Opus 5.5's, meaning that it completed more tasks, but wasn't necessarily better than its smaller stablemate.
That said, one of the most notable results was on the remote labor index, which uses real-world contractor tasks, where Fable 5.2 scored a 41.3%, almost doubling Opus 5.5's score.
Obsolete author Garrison Lovely called this by far the most alarming score.
Garrison writes, When the remote labor index was introduced a year ago, the best AI agent could only complete 2.5% of the projects.
Opus 5.5 had the best score at 21%, and Fable 5.2 just doubled it, hitting 41.
This is still a leading indicator of labor automation, as these projects are better defined than what you'd get at a typical white-collar job.
But the fact that one model generation can do twice as many projects end-to-end is a reminder of how fast change can come during exponential growth.
Now, unsurprisingly, then, Fable 5.2 is also the new leader on the Artificial Analysis Intelligence Index.
Its score of 65 puts it five points ahead of Gemini Carbon, six points ahead of Opus 5.5, and 8 points ahead of GPT-6 Astra.
Artificial Analysis actually tested Fable 5.2 on three different settings: max extra high and high, with both extra high and high scoring 62, and Fable 5.2 now occupying the three top spots with three different effort settings.
Artificial analysis said that gains were driven by improvements in science, knowledge, and coding scores, while less progress was made in agentic knowledge work and terminal coding.
Artificial analysis wrote: Claude 5.2 improves on Fable 5.1 across capabilities, but sometimes only to Opus 5.5 levels.
They pointed out some of those same areas of knowledge work, where it wasn't all that differentiated compared to Opus 5.5.
Now on costs, Anthropic has cut the per token prices for Fable 5.2 by 20%.
Input tokens are now $8 per million compared to 10 for Fable 5.1, and output tokens are $40 per million compared to 50.
Subscribers are still limited to using half of their token allowance on Fable, but Anthropic is handing out a banked Fable reset for this week to encourage a little more experimentation.
That said, Fable is still an extremely expensive and token-hungry model.
On Mac settings, it costs $26.54 per task across the AA benchmark suite.
That's more than twice as much as Fable 5.1, 2.6 times as much as Opus 5.5, and more than four times as much as GPT-6 Astra.
With effort settings knocked down to extra high, cost per task dropped to 1483, which is still 40% more than Opus 5.5 on Mac settings.
Reducing effort down to high results in $9.08 per task, which is 10% cheaper than Opus 5.5 on Macs.
Now, Anthropic does say across their release docs that medium should be the default setting, that high is enough for everyday coding and extra should be reserved for long-running agentic work with measurable outcomes.
And Max effort, they wrote, is for finding the ceiling and not recommended for everyday use.
And at least one early tester, Matt Schumer, was absolutely convinced that not only medium, but in fact low, was enough for the vast majority of tasks, meaning that this cost-efficiency profile might look a little bit different in practice than it seems at first glance.
Now, one way to get a sense of a new model is to see which particular use cases or broader triumphs from the testing period, the company finds worth mentioning in their announcement.
Anthropic mentioned that 90% of code changes are now written by Claude under human supervision, which reflects a number that we'd heard before and isn't particularly surprising.
Where Fable 5.2 has been added to that mix to fix stubborn bugs, optimize performance, and to quote, complete high-value software projects that would otherwise have been too slow or too costly to attempt.
They gave the example of a migration of a critical production service from Python to Rust to improve its efficiency, reliability, and start time.
Essentially, and this might be good guidance for the rest of us, Anthropic is reserving Fable for ambitious tasks that other models can't handle.
They found that the model, quote, exercises strong engineering judgment and can produce high-quality results even from ambiguous requests.
The showcase demonstration of this was an experiment where Fable 5.2 was tasked with designing a prototype operating system from scratch.
Anthropic wrote, Starting with an empty folder, the model coordinated over 1,000 sub-agents, working around the clock for eight days, writing, testing, and reviewing code.
It produced a working operating system that boots on a laptop with its own core that runs the machine, drivers for the disk, keyboard, and network, permanent file storage, windows, a login screen, an installer, and built-in Claude functionality.
One of the funniest comments I saw about this came from AI entrepreneur and YouTuber Theo, who wrote, Love how Fable 5.2 literally built an operating system, and my immediate response is, yeah, and crazy how quickly we get to sensitize to things.
Now, over in science, Anthropic announced multiple breakthroughs using Fable 5.2.
They used the model to solve two open problems in theoretical physics concerning black holes.
Similar to recent math breakthroughs from OpenAI, these solutions were largely about solving calculations that were too laborious for a human scientist, even with traditional computational techniques.
In biology, Fable 5.2 used its protein-solving ability to design a new way to predict the structure of a protein shell used in gene therapy called a capsid.
Anthropic wrote, In our tests, it accurately modeled 28 of the 34 capsids it attempted.
Biologists could use it to design capsids faster and more cheaply.
In math, Fable 5.2 fully formalized Fermat's last theorem into a machine-readable proof.
This took 30 hours using a thousand agents, and by way of comparison, Opus 5.5 was only capable of getting 26% of the way through the proof, taking 18 hours before it stopped making progress.
The choice to focus on many of these scientific discoveries is, I do not believe, accidental.
Chebian X wrote, While we're all focused on Claude Fable 5.2's coding abilities, its work in science and engineering has received far less attention.
He then goes on to list some of these accomplishments and a bunch of others that Anthropic shared, and concluded, So, yeah, this is nuts.
And at the same time, that's why we need to accelerate.
AI helps us solve problems in every scientific field.
And yet, we are still in 2026, and this is still the beginning.
Fable 5.2 shows us where we are heading, and 2027 is going to be nuts.
One final demo worth mentioning: Fable's robotics demo showed the model piloting a pair of robotic arms, writing, Fable 5.2 shows substantially improved skills in controlling physical robots, even on tasks it has never explicitly been trained to do.
They noted that Fable 5.2 outperformed most models that are specifically designed to drive robotic arms, suggesting that the bitter lesson applies to advanced robotics as well.
Hello, everyone.
One big change around AI is we've shifted our thinking from how we rank our pages to how do we become the source that AI trusts enough to answer with.
At KPMG, they're seeing this firsthand.
AI-generated results now surface answers directly, often without a single click.
That's why they are increasingly focused on generative engine optimization, or GEO, structuring content so AI systems can retrieve it, understand it, and cite it as trusted authority.
This is not just an SEO evolution, but a visibility mandate.
And indeed, the GEO mandate from KPMG is simple.
If AI is shaping decisions, your expertise needs to show up inside the answer.
Read all about it at kpmg.com/slash US slash GEO.
Again, that is kpmg.com/slash US slash GEO.
This episode is brought to you by C Data.
Companies rolling out AI keep hitting the same wall.
Token spend is climbing, security is holding agents back, and no one knows how AI is truly being used.
The root cause, AI is cut off from the systems and context your business runs on.
That's why C Data built Connect AI Gateway, one control point between your AI and your systems.
Built on the connectivity layer powering Palantir, Google, Salesforce, and hundreds more, each agent gets exactly the data and tools it needs.
It governs down to the record and lets you finally see your org's complete AI usage in one place.
Accurate answers, a fraction of the token cost, and a gateway that learns your business with every interaction.
See how at cdata.ai.
You're in back-to-back meetings all day.
You're trying to stay present, but you're also worried you'll forget the decision, the action item, the important next step.
This is a scenario that we absolutely live here at the AI Daily Brief, given how fast things move and change and how quickly we're evolving everything that we do.
That's where Granola comes in.
Granola is an AI-powered notepad for meetings.
You jot down rough notes like you always do, and in the background, Granola transcribes and turns them into clear, useful notes when the meeting ends.
No bots joining your calls, no distractions, just a clean notepad that helps you focus.
During or after the call, you can chat with your notes.
Ask Granola to pull out action items, help you negotiate, write a follow-up email, or even coach you using recipes which are pre-made prompts.
Once you try it on a first meeting, it is very hard to go without.
Head to granola.ai/slash AIDAY and use code AIDALY to get 100% off for three months for new users.
That's granola.ai/slash AI daily, and code AIDALY to get 100% off for new users for three months.
Blitzy deeply understands your code base before it writes code.
Here's the first place that pays off: security in the age of AI.
Vulnerabilities don't live in isolation.
They live buried inside millions of lines of interconnected code where patching one thing quietly breaks three others.
That's why surface-level scans fail.
Blitzy starts from its knowledge graph of your entire application, identifies and surfaces CVEs across the full estate, proactively recommends patches, and can execute the PR.
Each fix is grounded in how your systems connect and validate so nothing new breaks.
And the knowledge graph dynamically updates, keeping you ahead of an ever-accelerating threat landscape.
One Blitzy customer resolved 21 active CVEs across six core microservices in four days.
Zero compile errors, every validation scan clean, months of planned work fixed in less than a week.
Security remediation grounded in real architectural context at the speed of compute.
Harden your code base at blitzy.com.
That's BLITZY.com.
So what were some of the first impressions from the community?
Perhaps not surprisingly given the origin story of Mythos, many people found even the commercially available version Fable5.2 to be extremely good with security issues.
Leander Builds wrote, Fable 5.2 in Medium just discovered more than 10 severe security vulnerabilities in my project without asking for it.
These issues were created by Opus 5.5 before.
If you haven't done it yet, highly recommend doing an audit with Fable5.2.
AI entrepreneur Pavel Hurin actually has a bug hunt bench, which tests different models for bugs in real work repos.
He planted 105 bugs across the two repos, and the previous best models mostly found between 40 and 45.
All of the big models that you probably use cluster somewhere in that area, with the only exception actually being Sonnet 5.5 Max, that recently jumped up and found 51 bugs.
Fable 5.2 found another 7 for a total of 58 bugs.
And when it comes to the cost, Pavel wrote, Fable 5.2 got there with less than half of Sonnet's turns for less money.
Now, of course, this being social media, there were a bunch of blender-based 3D rendering tests.
3D AI explorer Stefan Vascovich ran the same Castle prompt that he had run on Opus 5.5 back in September.
And while Fable 5.2 did take longer and cost a bit more than Opus 5.5, even to an external lay observer, the difference is very clear, with Fable 5.2 having radically more detail.
Maybe the most impressive video demo came from Riley Brown.
It's a 60-second ad for Fable 5.2 that uses some incredible zoomed-in visuals, artistic shots, realistic lighting and physics that change, and in a single shot, done live on stream, created this entire thing.
Even clawed code creator Boris Cherney said, whoa.
Now, if you haven't listened to it yet, you should go listen to my episode about why agentic video is real and what you should be experimenting with.
And certainly Fable 5.2 just adds more oomph to that argument.
Still, for some, the watchword for this release was ambition.
Allie K.
Miller wrote, I was an early tester of Fable 5.2, and I had it, one, build an entire water safety map of 3,100 cities in the US based on official government data with two demo videos.
Two, build a new identity and create and run an entire ADHD-themed YouTube channel that can make money for me.
Three, build psychological profiles of my stalkers to determine if any of them were the same person.
Four, build a hilarious 3D hot dog kiosk game as a command center to manage my to-do list.
Five, fill out 31 different personality tests on my behalf and provide an analysis over time.
Allie's conclusion?
I trusted it more than any other model I've tested.
Unbelievable at handling complexity.
Made some weirdly obvious errors like colors and units on the water map or overlapping text on a slide that secondary agents also didn't catch.
Importantly, there is no such thing as a needle in a haystack anymore with this model.
And I still feel like I could be more ambitious.
Now, that sense of not even knowing how to use all that power came out in Every's Vibe Check as well.
Their review was titled Fable 5.2 is a Paradigm Shift if you know what to do with it.
The piece tells the story of how one of the Every team built a working video editor that combined, they said, Adobe Premiere's editing capabilities, After Effects titles and visual effects, and Ableton's music mixing with an AI agent that can run all of it.
It's hard to overstate, they write, what a big deal this is for building software.
With Opus 5.5, you're still in the loop, checking its work as you go.
Fable 5 and 5.1 could take a big task and run with it for hours or days.
But Fable 5.2 can take the whole product.
Hand it everything you want, and it keeps building, testing, and refining until it has something you'll use every day.
This is the first model we've tested that lets professionals build production-grade tools of their own without ever reading the underlying code.
When our first round of early access ended in October, several of us put our most ambitious projects on hold until it came back, because we expected a better first pass with less steering.
Now, one of the things that I said when Fable 5 initially came out was very similar to this.
While previous models I had felt allowed me to start a bunch of different projects, Fable 5 just actually got them done in complete form.
I got the new version of the AI Delebrief website and extraction pipeline running in the 48 hours I had access to Fable 5 before it got shut down and basically didn't make any updates during the shutdown period.
Now, Dan Shipper and the Every team are actually resurfacing the narrative of people building their own professional software for the work they want to do.
This is something that people have been talking about with these agentic models for more than a year and was, of course, the narrative at the heart of the SAS Pocalypse on Wall Street earlier in Q1 and Q2.
Now, mostly the conclusion that people came to was that the difficulty in terms of time, cost, and context switching of maintaining your own software, even if you could build it, just wasn't really going to be worth it over using existing SAS solutions, especially as they evolved along with these new capabilities as well.
At least from their early testing, the team at Every is ensure that that still applies.
And yet at the same time, they also got at another big theme that came across a number of the different reviews, which is the jaggedness or spikiness, as they put it, of what the model can do.
Dan said, It's kind of nuts, but it's a spiky kind of nuts.
There's a certain kind of task where it's absolutely going to blow your mind and be unlike anything else you've ever tried before.
And for everything else, it's just sort of normal.
You should actually use Opus 5.5.
This was a major theme of Ethan Mollick as well, whose post about Fable 5.2 was called Fable 5.2 and Jagged AGI.
He writes, AI has gotten so good that it is worth asking if Anthropic's newest models, and the inevitable competing models OpenAI and Google will soon release, cross the boundary into being an artificial general intelligence.
Later on, after sharing a bunch of examples, Ethan wrote, You could start to see the limitations of the very digital tasks I picked when I felt uncomfortable letting Fable reach out to real customers.
And there were the failures.
A couple of years ago, the jagged frontier meant that failures were obviously made-up facts or failure to do basic math.
Fable's failures were different.
It made a course that was accurate and joyless.
It wrote a 182-page paper.
It kept coming back to its favorite ideas.
And it buried a creative project under rules and approvals.
Now, he did add: I teach at a business school, and I've seen talented people in good organizations do every one of these things.
If building a bureaucracy disqualified you from general intelligence, a lot of us would be in trouble.
But he continues, there are still gaps, and it's the reason that my answer is that this is almost AGI.
Most critically, the AI did not notice these problems itself.
It did not see that the course was a slog, or that it had tied itself in knots with its own rulebooks.
This was not for lack of checking.
Fable put critics, fact-checkers, or judges on nearly every project, but those checks found errors and added fixes.
None of them asked whether the work was too long, too repetitive, or no fun.
That all fell on me, and if I hadn't watched and taken action, the results would have been less impressive, though not exactly a failure either.
Knowing when your own work is not good enough is a large part of what makes someone an expert, and it's the part Fable does least reliably.
I would still not trust it to run a business on its own, even though its plan would have impressed me coming from a team of my MBA students.
Now, in my tests, I found something similar.
Basically, that while it can do impressive things, it didn't really seem to have a good sense of what would appeal to people.
I ran a version of a prompt that Ethan had used in two different places: one in the normal Claude tab and one in my Claude Code instance that has access to a bunch of different tools and systems and skills.
The gist of the prompt is basically asking it to create the most impressive thing that can share about its capabilities.
And the version that it created in the regular Claude interface was, it felt to me, pretty wildly underwhelming.
It decided that the best approach was to create things that were hard to make but easy to check, and to put it on a website where people could check them itself.
The three things were a sentence that correctly counts every one of its own letters, a piece of music that harmonized with itself played backwards, and a QR code encoded from scratch.
To the extent that these things are particularly difficult, most normal people, myself included, don't really understand why they're difficult, which makes the intellectual and emotional impact of them much, much lower.
Also, some of the capabilities don't feel that far away from things we've had before, like the QR code.
The insistence that people check it themselves kind of feels like an old lingering idea of AI from a couple of years ago.
And overall, it just didn't really have a sense of what would be impressive to humans.
Now, the version that was created in the coding harness was much more interesting.
It was a three-minute film that it pointed out had not been made from a recording.
Fable wrote: The picture is calculated frame by frame in your browser.
The score is synthesized from sine waves while you watch.
The narration is the one thing borrowed, a text-to-speech voice, and the only file this page loads.
Every letter here, this sentence included, is drawn with the film's own alphabet.
The source holds no fonts, no images, no audio samples, and no libraries.
And it basically is a really cool show-off of all the different things that you can turn code into.
Now, what was fascinating, pretty much the same prompt that Ethan had used, it was shocking how similar this output was to what Ethan got and shared on his blog.
Right down to a little twist at the end, where in the case of Ethan's site, if you take the first letter of every sentence in the script, it spells out the name of his blog, One Useful Thing.
Whereas on my test, it did the same thing, it spelled out be amazingly clever about this, which was the last line of the prompt.
Now, these are interesting results, but not particularly useful.
And so far, at least with my tests, the model's seeming inability to know what is interesting to humans and what's valuable to us is a real detriment to the type of content work that I might apply it to.
I asked it to propose an idea for the AI Daily Brief that could be built around a website and use original research and data in some interesting way.
I said this is in part a test to see what you can do compared to other AI models, so be intentional about the episode idea being impressive.
Once you have the idea, we're going to have you execute it.
The first idea that it pitched was in a phrase unfathomably boring and irrelevant.
It was called Announced is Not Available, and the pitch was time every major AI launch since ChatGPT, from the day it was announced to the day each kind of customer could use it and publish the result as a site.
The argument it says, AI coverage runs on announcement dates, but people and companies live on availability dates, and I couldn't find anyone who has measured the distance between them.
He pointed to September's GPT-6 Astra launch that Sam Altman actually apologized for because paying subscribers couldn't have it right away and a couple of others.
Now I had to explain why this was a very boring idea, which basically came down to the fact that one, no one cares about when a model from 2024 was announced and when it got access.
In fact, people pretty much only care about the models that are available to them right this second.
And what's more, with a very few exceptions, like GPT-6 Astra that he mentioned, at this point, the labs that are actually driving the conversation, which for now is pretty much just Anthropic and OpenAI, although Google might be back soon, aren't really having those sort of delays between when they're announced and when you get access to them.
Overall, what we got is an idea that while finding an actual factual gap in the coverage, had no ability to judge how utterly irrelevant the episode would be if I actually did it.
Now it did have two backup ideas, what America's 25 biggest employers told investors about AI and headcount last quarter, and every dated AI prediction that has come due graded with each forecaster's average miss.
Both of those are much better ideas for episodes.
The second about the biggest employers on earnings reports talking about AI was less interesting only because going through and aggregating and organizing public earnings statements is something that models have been able to do for a couple of years now at this point.
And so, even if Fable 5.2 had done it better in some way, it wouldn't necessarily have been an actual net new capability.
The everyday AI prediction was a bit more interesting because while it still had that same flavor of aggregating and organizing lots of data, it involved a bit more thoughtfulness and subjectivity given that it had to grade things in advance.
I had to do that third idea, rating forecasters and forecasts, and it actually was pretty interesting, but not necessarily again in a shocking new capability way.
And I'm fairly certain that if I had Opus 5.5 do that same task, it would do roughly as good a job.
So, what then are people going to use this for?
I think, continuing a pattern we've seen all year, this is a model that really asks us to push ourselves in terms of what we can do.
In other words, opportunity AI, not efficiency AI.
Not to just improve what we already do, but to do things that weren't possible before.
That was the thesis of my video episode from a couple of days ago.
And I think what Riley Brown demonstrated is proof positive that Fable 5.2 takes that to the next level.
I also think that while I am sometimes critical of people sharing 3D renderings and game demos as a way to determine whether a model is good, given how few people have that use case, the updates in game development, and particularly what people seem to be describing as the ability for Fable 5.2 not just to create the homunculus of games that look good, but don't actually play or don't play well, instead it seems like Fable 5.2 can actually do game mechanics.
Sholto Douglas from Anthropic wrote, Fable 5.2 is the first model that passes my bar for seriously fun and beautiful games.
Matt Schumer in his post about Fable 5.2 found something similar, having it create a Harry Potter-themed Fortnite-style Battle Royale game that you can play on Spawn right now, and which when I was testing it, other people actually were playing.
Now, just like advances in agentic coding weren't just about how existing coders did their work, and advances in agentic video, I believe, are not just about existing video editors doing their work differently, but all of us thinking about how we could use video in a way that we never have before, I wonder if the capability to build complete games actually changes what we use them for and the different types of people that leverage them for personal or even professional reasons.
For the first time, it seems like the capability set is at a point where it's worth asking, instead of making a deck or a website, should you make a game?
This is something that I'll want to explore a little bit more in the future, because I think even compared to video, it's going to require stretching our ideas a bit more.
Now, for completeness, as you go out and decide how much time to invest in experimenting with Fable 5.2, the single most common critique that I'm seeing is that for the vast majority of uses, it's not only not better than Opus 5.5, it's going to be kind of more annoying.
Engineering manager Gigam wrote, I've never really liked Fable models.
There's not much point to them.
They're stubborn, weighed down by guardrail filters, have poor taste, and are expensive, token-hungry, and in some areas worse than the Opus lineup.
This one is no exception.
In my view, the new Fable 5.2 makes no sense, and I think I understand why they called this release 5.2 rather than 5.5.
A revolutionary leap like the jump from Opus 5 to 5.5 just didn't happen.
Theo again echoed the sentiment, saying, It's been under an hour and I'm already struggling with should I use Opus 5.5 or Fable 5.2?
And yet even within this, I am certainly seeing people start to give their tips for the best ways to use it.
Daisy Holman responded to Theo and said, My advice, use Opus 5.5 for more specific tasks where you're already pretty sure you know what you want, and use Fable 5.2 for more creative tasks when you're not entirely sure what you want.
Now that hasn't exactly been my experience yet, but it is worth experimenting with.
The team from Every Once again emphasized that this is a model you give big end-to-end projects that you're going to leave and go away from.
And that seems to be what many of the folks from Anthropic were saying as well.
Alex Albert from Anthropic said, on big, open-ended work, it feels like a major step above Opus 5.5, and then gave some tips for getting the most out of it, like ask what's wrong with your idea before it builds anything.
It's great at brainstorming and will push back.
He also said to tell it up front where it needs your approval, such as deleting things, and be clear that the rest is its call, to start on medium or high effort and save extra high for the hardest problems, and most importantly, to give it a whole project instead of a next step and let it run for hours.
And remember, as Simon Willison points out, whenever Anthropic releases a new model, it updates their prompting guide.
One example from Fable 5.2 is that when you're using it to code, to tell it that it owns the code base.
Anthropic wrote, Claude, Fable 5.2 responds closely to what the prompt says about who owns the code it works on.
In Anthropic's testing on small coding tasks, when a prompt said nothing about ownership or presented the code base as someone else's, the model tended to add to the existing structure even when that repeated existing code.
It also tended to report nearby problems instead of fixing them.
When the prompt says the code base is the model's own, the model often merges repeated code and makes related fixes without being asked.
Ultimately, we're at the point where a new model release cannot be digested in hours or even days, or in some cases even weeks.
Even with Opus 5.5, it took three or four weeks for people to start to understand what made it different and what it could do differently, even if they had a glimpse and a sense right from the beginning that it might be one of those types of models.
It seems like there may be something like that in Fable 5.2, but it might take some time and experimentation to figure out what it is.
I will certainly be doing a lot more experimenting and we'll share along the way.
For now, though, that is going to do it for today's AI Daily Brief.
Appreciate you listening or watching, as always.
And until next time, peace.
