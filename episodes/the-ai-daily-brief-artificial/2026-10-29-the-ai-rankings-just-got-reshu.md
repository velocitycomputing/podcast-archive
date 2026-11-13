---
record_id: "podcast:163de90c-dd1e-4206-9800-205748fdffbb"
episode_id: 163de90c-dd1e-4206-9800-205748fdffbb
title: The AI Rankings Just Got Reshuffled
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/the-ai-rankings-just-got-reshuffled/163de90c-dd1e-4206-9800-205748fdffbb"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/the-ai-rankings-just-got-reshuffled/163de90c-dd1e-4206-9800-205748fdffbb"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-29
played_at: "2026-10-29T12:00:00Z"
play_count: 1
duration_seconds: 1620
source: pocketcasts-history-browser
played_label: October 29
history_order: 25
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: a9f156311d5104b6ea9157db1ea2711a21f14eaaeea38ff2e1c8074ad7d81283
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

Google’s Gemini 4 Carbon, unveiled two weeks after Gemini 4 Argon, became the new Artificial Analysis Intelligence Index V5 leader at 59 points, a nine-point jump ahead of Opus 5.5; it led six of eight cited benchmarks—Terminal Bench 4.0 (+8), Frontier Suite (+6), Exploit Gym (+12), CWE Bench (+3), OS World (+7), and Agent’s Last Exam (+8)—tied Sonnet 5.5 for second on the AA Coding Index, and cost $7.76 per task, 23% below Opus 5.5 and 20% above Astra, while Google limited early access to cyber defenders and trusted partners under pre-release testing guidelines. Sundar Pichai said AI is increasing training/launch velocity and expects acceleration from RSI; Arena’s Peter Gostev said Carbon felt much better than Argon, though Arena’s render/game-design tests were criticized as less polished than Opus 5.5. Artificial Analysis’ V5 redesign moved to mostly private datasets (about 60% vs 45%), added Frontier Code 2.0 and Terminal Bench Science, upgraded HLE to HLE Diamond, removed GDP VAL AA, SciCode, and AALCR, and equally weighted four categories including knowledge work, coding, and science/general knowledge/hallucination, reshuffling rankings: GPT-6 Astra rose to second at 57, GPT-5.1 Sol to third, Sonnet 5.5 slipped to fourth, GPT-6.1 Terra to fifth, Wonder, Fable 5.1, and Kimi K3.1 Pro fell, and the open-weight gap widened from 3 to 12 points, with Kimi K3.1 Pro at 46 and DeepSeek V41 Flash/GLM 5.3 around 32. The headlines also covered Microsoft and Google earnings—Azure up 48% to $33B with OpenAI contributing $10B, Google Cloud doubling to $30.7B while search growth slowed to 12% and YouTube to 9.2%, with CapEx underspend suggesting physical constraints rather than demand collapse—and a broad DOJ antitrust inquiry into NVIDIA’s $13B Hugging Face acquisition, Grok aqua-hire, SkedgeMD/Run AI deals, venture investments, sales practices, and customer pressure; a KPMG/UT Austin study of 500+ early-career professionals identified “AI amplifiers” who guide, evaluate, and refine AI outputs.

For users, there are no direct health implications, but treat the new AA V5 ranking as a provisional map, not a purchase decision: wait for hands-on access to Gemini 4 Carbon, especially because Google is limiting rollout to cyber defenders and trusted partners and Arena’s visual/game-design tests were weaker than Opus 5.5 despite Peter Gostev’s positive coding feel. For model selection, compare category-specific scores and costs for your workload—Opus 5.5/Sonnet 5.5 around $10/task, Astra $6.24, GPT-6.1 Terra $0.96, Carbon $7.76, Fable 5.1 $13.04—and ask whether agentic coding, science/research, knowledge work, or computer use dominates your use case before trusting the headline index. Follow-up questions should probe whether private benchmarking actually reduces benchmark gaming, whether equal weighting overvalues science relative to everyday use, whether max-setting leaderboards (a critique from Sri.world) reflect real medium/high settings, and whether NVIDIA’s DOJ investigation, hyperscaler CapEx constraints, and Google’s AI-mode monetization drag change cloud/AI infrastructure assumptions. The KPMG/UT Austin finding also suggests users should train and evaluate workflows around guiding, evaluating, and refining AI outputs rather than assuming similar skills produce similar results.

## Transcript

So frequently on this show, you will hear me ramble off a bunch of numbers that are supposed to tell you something significant about a new model that has just come out.
And more often than not, those benchmark numbers are in some ways related to Artificial Analysis, the company that has become the leading provider of the overarching benchmark that people use to judge AI models.
And as AI models become more significant, the benchmarks that tell us how they perform relative to one another consequently get more important.
Today, we are looking at a major update to Artificial Analysis' Intelligence Index, as well as a new leader for the benchmark, which comes, believe it or not, from Google.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, C Data, Granola, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AI DailyBrief, or you can subscribe to Novel Podcasts.
And if you want to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
On AIDailyBrief.ai, you can also find links to everything else going on in the ecosystem, free trainings, paid trainings like our new champions program at Super Intelligent, or of course the new How We Got Here podcast, and the first episode out this week called How Tech Lost America.
Again, you can find all of those links from AIDailyBrief.ai.
Welcome back to the AI Daily Brief Headlines Edition, all the daily AI news you need in around five minutes.
We kick off today with a story that could have easily been the main and honestly probably would have been if more people had had their chance to get their hands on this model.
Google has unveiled their next frontier model, Gemini 4 Carbon, just two weeks after the release of Gemini 4 Argon.
As I've mentioned on this show a number of times since Argonne arrived, having a new base model means Google can iterate quickly with reinforcement learning rather than needing to complete a lengthy pre-training run to put out a new model.
And this is definitely a quick pace, one of the shortest gaps we've seen between versions of ultra-large models.
CEO Sundar Pichai even suggested the pace would increase from here, commenting on Wednesday night's earnings call: This rapid progress underscores our incredible model momentum.
We are at the point where AI is helping us increase our training and launch velocity.
I would expect the next 12 months to see continued acceleration because of RSI.
So, Google is iterating at a record pace, but I'm sure you are sitting there asking yourself the same question that everyone is: which is, is the model any good?
In particular, is it a significant improvement on the underwhelming release of Argonne?
Certainly, when it comes to the benchmarks, the answer is a definitive yes.
In coding, Carbon gained eight points on Terminal Bench 4.0 and 6 points on Frontier Suite.
Cybersecurity saw a 12-point increase on Exploit Gym and a 3-point increase on CWE Bench.
For computer use, Carbon picked up 7 points on OS World and 8 points on Agent's Last Exam.
On 6 of those 8 key benchmarks, Gemini 4 Carbon is now the top of the leaderboard, ahead of Astra and Opus 5.5.
Gemini 4.
Carbon is now the frontrunner on the new Artificial Analysis Index V5, which we will be discussing in the main part of the episode.
It scored 59 points, representing a nine-point jump on the new scale and placing it ahead of Opus 5.5 in first place.
On the AA Coding Index, Carbon landed in second place, tied with Sonnet 5.5 and 3 points behind Opus 5.5.
Now, these are huge jumps for Google.
When Argon was released two weeks ago, some felt that Google had missed their window.
The model might have been impressive a month or two earlier, with benchmark scores topping Fable, but the release of Opus 5.5 and GPT-6.1 Soul had pushed the frontier sufficiently that it left Google in the second tier alongside Meta.
This release, if people's experience with it matches the benchmarks, puts Google genuinely back in the race for the frontier.
Cost is basically unchanged compared to Argon, with artificial analysis measuring costs per task at $7.76.
For reference, that's 23% cheaper than Opus 5.5 and 20% more expensive than Astra, so right in the middle of the road for Frontier models.
Now, here we come to the less great part.
We don't have many first-hand testimonials, as Google unveiled the model before it's ready for general release.
They're following the administration's pre-release model testing guidelines and said they're taking what they call a deliberate approach to the rollout.
The model will be made available to a subset of cyber defenders beginning this week, with access extended to trusted partners in their cyber defense program.
As for the rest of us, Google wrote, We're continuing to gather feedback and iterate on guardrails before making carbon available to developers, businesses, and consumers via our product services as soon as possible.
One of the few groups talking about their experience with the new model was Arena, who had access for testing purposes.
They put out a video review full of render and game design tests that were generally slammed for not being as pretty as Opus 5.5.
Now, as I have said before, I am not particularly convinced that 3D design is the right yardstick for LLMs, no matter how much social media users like to focus on that, but certainly at least when it comes to that particular use case, Carbon is not at the same level as its rivals.
Arena's Peter Gostev did give a few more details, however, posting, I've used Carbon a bit before the release, and I can tell you it feels a lot better than Argon.
This is a real deal from Google this time.
I hope they keep up with the rapid pace of releases from now on.
And that does seem to be the plan.
Responding to Tior Tax's commenting that Fable 5.5 isn't here yet, though, DeepMind researcher Zachary Natto wrote, Gemini redacted, isn't here yet though.
Chubby on X commented, okay, now things get crazy.
They have another unreleased Gemini model that's even better than Carbon, and Carbon has already reached number one in the AA Intelligence Index today.
Gemini post-training researcher Xiao Zhang added that Google AI is out of their funk and operating like a well-oiled machine.
Less than a year ago, he wrote, Launching Gemini 3 Pro was a big bang event where the whole team celebrated number one benchmark numbers.
Today, Gemini 4 Carbon hits number one on the AA index, yet the feeling inside is distinctly different.
We've been dog fooding continuously for weeks, and we've almost adapted to the new intelligence, taking ambitious code rewrites for granted, leaving loops overnight that launch dozens of experiments to repo, root cause, and fix mysterious bugs, and using swarms to inspect and fix RL data.
Launches just feel like periodic checkpoints now.
And despite taking 10 months off the early adopter AI conversation, you can see that Google still has lots of people's benefit of the doubt.
Crusader Benges Hesim writes, Why is Google suddenly dropping models like they invented Transformers, own half the internet's data, and sit on an ocean of TPUs?
Oh, wait.
Latent Space's Swix writes, Gemini number one on AA V5?
This is making me open up anti-gravity for the first time in a long time.
If Google actually pulls this off, it is officially comeback season, with Meta, Grok, and now GDM being cool again.
For my part, I think we will suspend judgment until we get our hands on the actual model, but it looks promising, and that in and of itself is exciting.
Now, speaking of Google, the other story was in their and Microsoft's earnings reports.
Both companies delivered another incredibly strong quarter in cloud growth, which is where, of course, they contain their AI revenue.
Microsoft said their Azure division grew at 48% over the past year to reach 33 billion.
This is the first time Microsoft has broken out Azure revenue as a separate line item, which seems like a very good decision with growth this strong.
Azure drove overall revenue growth of 19% to reach $92.3 billion for the quarter.
Each of those figures was a slight beat over analyst estimates.
Microsoft also disclosed that OpenAI contributed $10 billion to Azure revenue, around a third of the total business.
Microsoft's stock was up as much as 4.8% to reach a new all-time high in after-hours markets.
Google's cloud division, meanwhile, doubled revenue compared to year-ago figures, reaching $30.7 billion for the quarter, and meaning they've almost entirely closed the gap with Microsoft.
This was well above Wall Street's high expectations.
However, as David Wagner of Aptus Capital Advisors put it, the problem is everything else.
Search revenue growth came in at 12%, a massive slowdown from 17% in the previous quarter and 19% the quarter before that.
YouTube revenue also added a third continuous growth slowdown to reach 9.2%.
Even TPU sales was a bit of a question mark, with executives dodging a question about profit margins for the chips during the earnings call.
Overall revenue growth still came in at 25%, roughly in line with expectations, but to some analysts, it looks like Google might have reached the moment where they're forced to cannibalize their own search business because it's no longer a reliable growth driver.
In fact, CEO Sundar Pichai acknowledged this dynamic during the earnings call, commenting: It's worth noting that the strong growth in AI mode queries had an impact because of the lower monetization we're seeing in AI mode.
In addition, Google missed on bottom-line earnings largely due to a markdown on their SpaceX stock.
Tech analyst Dan Ives, ever the optimist, tried to strike a positive tone, writing, This is the cloud print we have been waiting for, and in our view, it matters more than a lighter search number the bears will lean on tonight.
And lean on it, they did, sending the stock plummeting as much as 10% in after-hours markets.
Much of the coverage focused on the cloud race between the two companies, which are now neck and neck, but the pace of the data center buildout might be even more consequential.
Both companies held CapEx forecasts steady for this year and next, but actual CapEx spend for the quarter came in under expectations.
Google, by way of example, is guiding a 50% increase in CapEx next year to $300 billion, but they're currently undershooting this year's numbers.
Oracle and Meta are in a similar position.
So it looks like the AI buildout may have reached peak velocity.
That's not at all surprising given physical constraints around components, power, and labor, let alone community support running on empty.
Now, we are quite early in this trend, and Google said that they would have more in-depth discussions on CapEx during the next quarterly earnings.
But what makes this interesting is that many AI bearers suggested that a CapEx slowdown would be the catalyst that pricks the AI bubble.
What we're seeing, however, doesn't exactly line up with that theory.
The logic was that demand would falter and force the hyperscalers to slow down.
Instead, it looks like the hyperscalers, if they had their drothers, would like to continue accelerating their data center buildout, but are running into more fundamental and physical constraints.
Tech analyst Luke Longo thought the slowdown was more about finance, but are running into more fundamental and physical constraints.
Lastly, today, more antitrust scrutiny for NVIDIA as the DOJ queries their acquisition of Hugging Face.
Reuters reports that the Department of Justice has made inquiries about how the acquisition would impact competition in the AI industry.
In particular, the DOJ has asked whether ownership of HuggingFace would allow NVIDIA to control a key distribution point for AI models.
When they made the $13 billion acquisition in September, NVIDIA maintained that Huggingface would remain free to offer a platform and partner with a wide range of model developers, chip manufacturers, and cloud providers.
They said the deal was expected to close in the first half of 2027 pending regulatory approval.
These inquiries form part of what is now revealed to be a multi-year antitrust investigation into NVIDIA.
In September, the New York Times reported that the DOJ had opened an investigation in NVIDIA's licensing and talent acquisition deal with chip-making startup Grok.
That deal was structured as an AquaHire deal, which has been a common practice in the AI industry dating back to Google's 2024 deal with Character AI.
Because these deals are not technically acquisitions, they don't trigger automatic antitrust reviews and can therefore theoretically close much faster.
The assumption had been that the DOJ was using an investigation into NVIDIA as a way to crack down on this practice more broadly.
However, sources told Reuters this week that the investigation is much broader and seems to predate the Grok deal.
Acquisitions of data center optimization companies SkedgeMD and Run AI are also within scope for their impact on the competitive landscape in AI infrastructure.
And both of those deals were traditional acquisitions, not AquaHire deals.
Furthermore, sources said that recent questioning from the DOJ covered NVIDIA's venture investments, sales practices, and whether the chip designer has exerted pressure on its customers.
In other words, rather than just a narrow investigation about circumventing antitrust rules, it now seems the DOJ is embarking on a full top-to-bottom antitrust investigation of NVIDIA.
Obviously, no charges have been filed at this stage, and the investigation could conclude with no action, so there's no implication that NVIDIA has done anything improper.
Still, compared to what most people thought this was, it appears to be a much more concerning investigation for the dominant chipmaker.
Something to keep an eye on as we go forward for sure, but for now, that is going to do it for today's AI daily brief.
Next up, the main episode.
A new study from KPMG and the University of Texas at Austin found that when people work with AI, similar skills don't guarantee similar outcomes.
Researchers studied more than 500 early career professionals and found that the best performers consistently amplify the value of AI by guiding, evaluating, and refining its outputs.
These top performers, called AI amplifiers, weren't defined by what they knew alone, but by how they worked with AI.
Learn more about what separates AI amplifiers from everyone else at kpmg.com/slash uslash AI amplifiers.
This episode is brought to you by C Data.
Token spend is climbing, security is holding agents back, and companies rolling out AI initiatives might not know how it's truly being used.
The root cause, AI is cut off from the systems and context your business runs on.
That's why C Data built Connect AI Gateway, one control point between your AI and your systems.
Connect AI Gateway is not just another static model router.
Prompts get intelligently routed to the right model with exactly the tools and data it needs, governed down to the record.
The result?
Accurate answers at a fraction of the token cost with a context engine that learns your business with every interaction.
Built on the connectivity layer powering Palantir, Google, Salesforce, and hundreds more.
Give it a try and start your free trial at cdata.ai.
That's c as in connect data.ai.
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
Head to granola.ai/slash aidaly and use code AIDAI Daily to get 100% off for three months for new users.
That's granola.ai/slash AI Daily, and code AIDALY to get 100% off for new users for three months.
Blitzy's deep code-based understanding unlocks the thing every roadmap owner cares about: shipping new features.
Here's the truth about building inside a massive enterprise codebase.
Writing code was never the bottleneck.
Context is.
Which system does this touch?
Which contracts can't break?
Which standards apply?
Blitzy already knows because it reverse-engineered your entire codebase into a dynamic knowledge graph before feature work began.
With that complete picture, Blitzy builds features end-to-end.
Architecture, APIs, UI, and tests all validated against your existing systems.
One Blitzy customer built an AI-native application from scratch with 100% autonomous completion, saving over 2,700 engineering hours.
Features that respect your codebase instead of fighting it.
Stop letting your backlog grow faster than your team.
Accelerate your roadmap at blitzy.com.
That's B-L-I-T-Z-Y.com.
Welcome back to the AI Daily Brief.
Today we are talking about benchmarks, specifically a new set of benchmarks and how they're shaking up our sense of the AI field.
Now, the eagle-eared among you may wonder exactly what I think about benchmarks, given that on the one hand, with every new model release, I implore you to only give them so much attention and yet at the same time still rattle off a whole bunch of them as though they matter.
In short, I think that benchmarks are inherently limited, but also important.
Without them, we don't have good tools other than strictly vibes to understand the difference between different models.
And yet, in almost no circumstances, do I think we should take the performance of one model on any one benchmark or even in the aggregate as the gospel.
Done well, they are a useful guide to helping us understand where different models fit into our overall stack.
But as we will see today, there is more and more effort to addressing some of the inherent limitations of benchmarks and trying to make them better.
Whenever there is a new model, you'll hear me talk about the scores that it gets on the independent tests administered by Artificial Analysis.
Well, that company has just overhauled the way that they test model, giving us a brand new yardstick for Frontier AI with version 5 of their intelligence index.
The index takes around a dozen key benchmarks and distills them into a single score.
And while the index is now entrenched in how we understand the AI race, leaning so hard on that single score is a relatively new phenomenon.
Prior to the era of agentic coding, when LLMs were in many cases still glorified Google or writing assistants, vibes reigned supreme.
Ranking on the chatbot arena leaderboard was the pinnacle test of a new model because it told developers what users wanted.
But as research and coding became more important use cases, we got more objective benchmarks giving a clearer indication of how each model would perform on real work.
These evaluations have evolved over time.
First, by adding harder questions as benchmarks became saturated.
In other words, as all the models crowded the very top score of a benchmark, the creators of said benchmark would go add in a bunch of new or harder questions, creating an iterative version that would hopefully provide more granularity on the difference between different models until that model got saturated as well.
As agentic computer use became a fundamental part of model performance, the evaluations got an even more complete rethink.
Through each of these changes, artificial analysis also evolved, switching out benchmarks and rebalancing their weightings as different model abilities became comparatively more important.
This hasn't always been a smooth process.
There have been moments where the intelligence index looked extremely saturated and stopped giving us a good indication of which models were best.
There were moments when benchmark maxing allowed developers to game the system and rank much higher than real-world testing would support.
In fact, this has been a fairly consistent story when it comes to Chinese open weight models.
In early September, Artificial Analysis pushed an early update with version 4.2, pulling forward many of the changes they had planned for V5.
That decision was triggered by the release of GPT-6 Astra, which focused heavily on improving computer use.
The problem was that V4.1 of the Intelligence Index still had relatively light weightings for agentic benchmarks, leading GPT-6-Astra to have a slightly disappointing score.
And more than just disappointing, one that didn't really comport with people's lived experience of the model.
After the update, Astra was still ranked slightly behind Fable 5.1, but the index had become a closer reflection on how people were actually using the new crop of models.
And this has been the story of the Intelligence Index, a constant cat and mouse game of updating the mix of benchmarks to match the rapidly evolving real-world use cases for AI.
Introducing version 5 of the index, Artificial Analysis highlighted that for the first time, the majority of the benchmarks are built on private data sets.
The idea is to make benchmark maxing more difficult, as model developers theoretically can't train their models to the test.
And that, by the way, is what we mean by benchmark maxing, when developers include those sort of evaluation tests and their answers in the training data set, leading to an artificially inflated score, as the benchmark cease to measure what the model can do and instead reflect simply a memory of the correct answers.
For version 5, AA added two new benchmarks: Frontier Code 2.0, which is the brand new version of Cognition's private benchmark of real-world coding tasks.
This test features scoring based on whether a repository maintainer would merge the code.
They also added Terminal Bench Science, which is an agentic scientific research benchmark.
Humanity's last exam, once pitched as a near-impossible knowledge search task, has been upgraded to HLE Diamond, the even more difficult version.
Similar saturation updates have been made to AA Omniscience, which measures knowledge and hallucinations, as well as CRITPT, a physics test.
GDP VAL AA, the measure of agentic work in real-world settings, is out, with the index now relying on AA Briefcase, Automation Bench AA, and GDP.PDF to measure white-collar work along more granular lines.
Also removed are SciCode, a scientific research test, and AALCR, which tests long context reasoning.
Now, rather than just a list of names and acronyms, these adjustments say a lot about how AI models have changed since V4 of the index was released in January.
At that time, long context reasoning was one of the most critical features, used for working on large code bases.
Many coding models still had limited token context windows and suffered from fatal issues with context rot.
Since then, improvements to compaction and memory have allowed us to take a lot of that long context performance for granted.
Agentic work is the other huge change that's evident from the redesign of the index.
The coding benchmarks included in the index now only measure agentic performance, as that has been cemented as the way developers use modern AI, and the science benchmarks are now testing real-world agentic research work rather than pre-existing scientific knowledge.
For the time, artificial analysis has chosen to equally weight the index across four categories: knowledge work, coding, science in general, which encompasses both general knowledge as well as hallucination rate.
In some ways, it feels like that 25% waiting for science is a forward-looking bet based on how Anthropic and OpenAI have been trading science and math headlines over recent weeks.
So, what did this change in the scores?
In version 5, Opus 5.5 was still in the lead with a score of 58, at least until Google dropped Gemini 4 Carbon on Wednesday.
GPT-6 Astra jumped into then second place with a score of 57, and Astra had previously been in 6th place, showing there's a pretty big jump based on the index giving more weight to computer use and scientific tasks.
GPT-5-1 Sol takes third place up from 9th, followed by Sonnet 5.5, which slipped from 2nd to 4th.
GPT-6.1 Terra was in 5th up from 10th, suggesting the model is a little better than many assumed earlier in the week.
In just a moment, we'll get into what I think that reflects.
Gemini 4 Argon gained a rank to Tymeta Wonderful in 6th place, which is a pretty notable drop for Wonder, which was previously in 3rd, although many felt that that ranking didn't line up with real-world experience.
Fable 5.1 is looking a little long in the tooth in 8th place, sliding from 5th, and in 9th place, we have one of the most notable drops in the new index, with Kimi K3.1 Pro falling all the way from 4th.
In fact, artificial analysis noted that the gap between open weight models and US proprietary models had opened up massively after the index rebalancing.
They wrote: The open weights gap widens from 3 points to 12.
Kimi K3.1 Pro is the top open weights model at 46.
Among models with released weights, DeepSeek V41 Flash and GLM 5.3 lead at 32, 26 points behind the leader and below Claude Haiku55 with 36 points.
Now, in addition to the new gulf between US and Chinese models, there was also a clear drop-off between the handful of leading labs and everyone else.
Anthropic, OpenAI, Google, and Meta all have models with scores of 50 and above.
Fable 5.1 and Kimi K3.1 Pro are just outside that cutoff.
However, there's then a 10-point gap between Kimi K3.1 and Claude Haiku55, which leads the rest of the pack.
Basically, by adding more agentic tasks to the index, there's now a clear separation between Frontier models and the rest.
Artificial analysis noted that costs vary wildly among the top 10 models that arguably make up the Frontier.
That's largely because the top 10 is a mix of large models, token-intensive models, and a few smaller, more efficient models.
At each end of the spectrum, we have GPT-61 Terra as the cheapest at 96 cents per task, and Fable 5.1 is the most expensive at $13.04 per task.
For a more apples-to-apples comparison based on model size, Opus and Sonnet both cost around $10 per task, compared to $6.24 for GPT-6 Astra, and only $1.27 for GPT-6.1.
Muse, Wonder, Grok 4.7, and Gemini 4 Carbon are all slightly more expensive than GPT-6 Astra in the high $7 range.
Now, most people found this to be a welcome update.
OpenAI head of strategic futures Dean Ball wrote, This is the first time an artificial analysis ranking has even roughly approximated my own subjective ranking of models.
Haseeb Qureshi wrote, Artificial analysis re-ranking their intelligence score seems to match the vibes a lot better and clear out a lot of benchmaxing.
Shows a deeper gap between Anthropic OpenAI and everyone else.
Also shows a bigger gap between closed and open weights.
Ethan Malik wrote that the analysis, quote, matches the general vibes that we haven't seen a Fable class open model.
And AI content creator Theo drove that point home, writing, terrible day to be an open weights models are just as good as Opus 5.5 guy.
Now, there were a few people who spoke up for the open weights models.
Brookings Institute fellow Kyle Chan pointed out that even before this, artificial analysis had some private benchmarks, it's just that the share went from 45% to 60%.
Using Kimmy 3.1 Pro score as an example, he suggested that while the headline news is the gap with the top US model widening from three points to 12, that it's more important to look at the specifics.
Science, he points out, is a major weakness, with Kimmy scoring just 34% on Terminal Bench Science versus 63% for GPT-6 Astra.
But he writes, Kimmy is still extremely strong at coding agents, pointing out that it actually leads all models on Terminal Bench 4.0, scoring 67%.
Kyle's conclusion, is this evidence of benchmark gaming?
Not necessarily.
Some of Kimmy's biggest deficits are on non-private benchmarks, while it actually beats Claude on the private automation bench AA evaluation.
The bigger story, he says, Chinese models can match or beat U.S.
Frontier models on certain agentic tasks, but a significant gap remains in advanced scientific reasoning and research workflows.
And ultimately, even if in general people think that this is a positive update, no one is going to agree on everything.
In particular, I think one of the biggest debates will become what the relevant weighting should actually be.
Yes, OpenAI and Anthropic are clearly emphasizing scientific discovery, but relative to the average individual use case, does that matter as much as agentic coding as it does in the weighting of the new V5 index?
Now, that might be an argument for a different weighting, or it might be an argument that instead of paying attention to the headliner number, we'd be better suited to focus on the individual benchmarks for the categories of use cases that we care about.
One critique that I do think is worthy of consideration is the fact that the leaderboards are run based on Max settings.
Sri.world writes: No one runs Macs in real life.
Where's the medium/slash high slash extra high leaderboard?
And to be clear, it's not like artificial analysis ignores that, especially in their analysis that involves cost, the effort setting does become part of the calculus.
But I do think that on a practical level, people might be better served by the ability to organize the index not just by model, but also by effort.
Now, one last note: alongside the new intelligence index, artificial analysis introduced a new progress index.
The index places all models released since November 2022 on a capability scale to see how each lab's leading model improves over time.
It's designed less to be about the current batch of models and more to give a long-term view of model progression.
Still, the new measure gave people easy access to a bunch of data to play with.
Lasan Al Gui, for example, looked at how the switch to reasoning models impacted the major labs, commenting: OpenAI really does have the best reinforcement learning, or their models just suck without reasoning.
And by charting the data in a different way, they estimated that the gap between the US and China is now 3.3 months and closing.
Summing up, like I said at the beginning, I think benchmarks are important and inherently limited, but I love that more effort is going into improving them, and I think even the debates that follow are also extremely value-accretive when it comes to how we understand how different models compare to one another.
For now, however, that is going to do it for today's AI daily brief.
Appreciate you listening or watching, as always.
And until next time, peace.
