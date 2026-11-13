---
record_id: "podcast:2311f0e1-0516-43c0-9c78-5ae315651ee5"
episode_id: 2311f0e1-0516-43c0-9c78-5ae315651ee5
title: "Is Anthropic on the cusp of RSI? Inside the redacted METR report | Luisa Rodriguez"
podcast_title: 80,000 Hours Podcast
url: "https://pocketcasts.com/podcast/80000-hours-podcast/99d6aaa0-2e41-0135-52f9-452518e2d253/is-anthropic-on-the-cusp-of-rsi-inside-the-redacted-metr-report-luisa-rodriguez/2311f0e1-0516-43c0-9c78-5ae315651ee5"
audio_url: "https://pocketcasts.com/podcast/80000-hours-podcast/99d6aaa0-2e41-0135-52f9-452518e2d253/is-anthropic-on-the-cusp-of-rsi-inside-the-redacted-metr-report-luisa-rodriguez/2311f0e1-0516-43c0-9c78-5ae315651ee5"
feed_guid: null
feed_url: "https://feeds.transistor.fm/80000-hours-podcast"
published_at: null
published_local_date: null
played_date: 2026-11-12
played_at: "2026-11-12T12:00:00Z"
play_count: 1
duration_seconds: 900
source: pocketcasts-history-browser
played_label: Yesterday
history_order: 6
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: rss-podcast-transcript
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 16bea82d05496d2ae1fe1aef245f87ff8fd94e513e17965d4c4dc697c1e58b78
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

METR’s 11-week, Anthropic-arranged review of internal Anthropic data claims Anthropic’s measurable AI progress was about twice as fast as a year earlier, with uncertainty of 1.3–3×, and that roughly 80% of the sustained speed-up comes from Anthropic using its own models to assist research; the report cites internal test scores across all models, three unreleased models, a steepening around October 2025 when Claude could code autonomously for hours, Anthropic’s own figure that Claude was doing about a quarter of research work end-to-end by August, and examples such as Claude building a Slack-style app over 30 hours, Mythos solving an 87-year-old math problem and finding major security flaws, and Anthropic’s stated threshold of “two years of progress in one,” which Anthropic’s public August report said had not been reached but METR’s private analysis put at 1.97 and Anthropic’s latest IPO filing says has now been crossed. The discussion also covers redactions that hide most evidence, Toby Ord’s counterpoint that Mythos’s larger training run could reduce the apparent speed-up to about 1.4×, Buck Shlegeris’s view that redacted evidence matters and his ~1-in-3 chance of superintelligence within a year, economist Karthik Tadepalli’s public-data check that convinced him, Ryan Greenblatt’s revised estimate of superintelligence within one to two years, the AI 2027 scenario, and policy concerns from Alex Bores, Bernie Sanders, and Steve Bannon about banning fully automated AI research and requiring independent oversight.

The actionable takeaway is not a health decision but an AI-risk, career, and advocacy decision: if the user is considering pivoting, now is the time to choose among direct AI-safety work, a more flexible job enabling side projects, targeted donations, or public conversation, and to use the episode’s suggested free AI career advising tool if career direction is unclear. Concrete follow-ups are to read METR’s redacted report and Anthropic’s August risk report/IPO filing, track whether Anthropic implements the promised stronger security and internal monitoring after crossing its own line, ask how much of the 80% attribution rests on redacted evidence, test whether the speed-up extends beyond easily graded coding/math tasks to messy real-world work, monitor whether compute, data, or algorithmic bottlenecks appear, compare OpenAI/Google/other labs for similar acceleration, and decide whether to support proposals such as mandatory independent reporting of AI-assisted research speed-up or legislative bans on fully automated AI research.

## Transcript

I just got through reading what may be the scariest AI report I’ve ever seen. METR, an independent group that assesses AI risk, spent 11 weeks going through Anthropic’s internal data. They found Anthropic is now improving its AI about twice as fast as it was a year ago. And the main reason seems to be that its AI is helping build the next version of itself.
The reason that’s scary is, if Anthropic is able to hand off a big share of coding and experiments to its AI, the next, more powerful model arrives sooner. That version then does even more of the work, so the one after that arrives sooner still. And each iteration leaves less time to verify that the new model is safe before it’s helping build the next one.
AI experts have been warning about this for years, and there’s a term for it. It’s called recursive self-improvement, and if METR’s right, Anthropic might be on the cusp of it right now. Some of those experts thought this was further off. This report changed their minds.
Anthropic has drawn itself a line: the point where its AI speeds up its research enough to make two years of progress in one. By the time it reaches that point, it plans to have taken serious, specific steps to make its AI harder to steal, and to monitor everything happening inside its own AI development.
In its August risk report, Anthropic said it didn’t believe its models had reached that line. They invited METR to look into that claim, and gave them 11 weeks inside the company.
They were given access to data almost no one outside Anthropic has seen: internal test scores, data on how its AI is trained, and interviews with the people building the models. They didn’t have unrestricted access, but METR says Anthropic shared a lot more than they expected.
At the end of its investigation, METR found that, as of October, Anthropic was improving its AI about twice as fast as it was a year ago, at least on the kinds of tasks that we can easily measure. That’s METR’s best guess, though they say the true speed-up could be anywhere between 1.3 and 3 times as fast.
One of their main pieces of evidence was Anthropic’s test scores for every model it’s built, including three internal models that are better than any the public has seen. If you plot those over time, around October of last year, the line suddenly gets about twice as steep.
Personally, I find “twice as fast” hard to wrap my head around, so let me try to make it feel real. In late 2023, Claude was a chatbot. It couldn’t look at a photo. It couldn’t even look things up on the internet.
By late 2025, Anthropic said it could work on its own for more than 30 hours, building an entire Slack-style app with no human stepping in. That was two years of progress.
Then, just a year later, AI helped settle a math problem that had defeated generations of mathematicians for 87 years. That’s what METR means by making two years’ worth of progress in one.
METR’s next question was: what’s behind that speed-up? They ruled out the simplest explanation: more computing power. Anthropic is definitely using more, but that isn’t where the speed-up is coming from.
Other obvious explanations, like a hiring spree, a trove of new data, or a big research breakthrough, may have kicked it off, but they can’t explain why it’s lasted this long.
Taking everything into account, METR’s best guess is that about 80% of today’s speed-up comes from Anthropic using its own AI to help do its research. But Anthropic redacted most of the reasoning behind that number in the public report, including the majority of the evidence that METR found most convincing. METR admits this means we have to rely on their judgement much more than would be ideal.
But they were able to share some of the evidence. First, a bunch of Anthropic’s own researchers say AI has sped up their area a lot. One said, “I’ve seen us discovering very promising directions entirely because people can spam 10 ideas at Claude and just see what sticks.”
On their own, impressions like these wouldn’t be that convincing. But they line up with the timing. The speed-up seems to start in October 2025, right around when Claude got good enough to write code on its own for hours at a time.
Here’s the second piece of evidence. Claude isn’t doing major research on its own yet, but researchers say they’re seeing early signs of it in several parts of the training process.
Anthropic has its own numbers on this. Earlier this year, Claude was doing almost none of its research work end to end. By August, it was doing about a quarter, though still with humans supervising.
So METR’s read is that AI’s role in its own development has been growing, and that it’s now the main reason Anthropic is speeding up.
There’s nothing obvious that’s going to slow it down. AI building AI is different from other technologies. The better your AI gets, the faster it helps you build the next one.
That loop only stops if it hits a bottleneck, like running short on computing power, training data, or ideas for algorithmic improvements. METR looked for all three and didn’t find anything likely to get in the way in the next year.
They aren’t confident. Their picture changed several times as they got more information. But METR says they can’t rule out things getting a lot faster in the next six months. They even say the speed-up itself could be increasing.
If the speed-up does keep climbing, then two years of progress in one year could become two years of progress in six months, then three months, then six weeks.
Two years ago, AI couldn’t count the Rs in ‘strawberry.’ This year, Anthropic’s Mythos found thousands of serious security flaws that nobody knew about in every major operating system and every major web browser.
After a few more rounds of speed-up, I honestly can’t imagine what AI is going to be able to do.
This is all uncomfortably close to the way things play out in AI 2027, a well-known prediction scenario written two years ago based on AI progress and the geopolitical situation at the time. In its darker ending, by the end of 2027, AI is superintelligent and humans have lost any real chance of controlling their future. By 2030, it’s killed almost everyone on Earth with biological weapons.
In that forecast, the speed-up in AI research METR just found doesn’t happen until early 2027. If METR’s right about this, we may already be a few months ahead of schedule.
All of this rests on METR being right. So how solid is their finding that Anthropic is now making progress twice as fast?
METR redid the analysis lots of ways: with different statistical methods, changing which benchmarks they used, leaving out certain models. Almost every version still showed progress happening around twice as fast.
The strongest pushback I’ve seen comes from the philosopher Toby Ord. He points out that that line of test scores could be read another way. Mythos came from a much bigger training run, and those usually bring a one-off jump in ability. Allow for that, and the line only shows progress about 1.4 times as fast.
That’s a fair point about the test scores. But as AI safety researcher Buck Shlegeris points out, they’re not the main reason METR reached their conclusion. They’re just the only part of their analysis that wasn’t redacted. And METR says the redacted evidence made them take the twice-as-fast finding more seriously.
Another reason some people are sceptical: compared with other companies’ models, rather than its own past, Anthropic’s speed-up looks smaller. METR says that could mean Anthropic was just catching up, or that its models were less tuned to the tests than its rivals’.
But you can partly check that with public data. An economist, Karthik Tadepalli, tried, expecting to cast doubt on METR’s result. Instead, he says he came away convinced.
But the biggest caveat is that all of this is measured on tasks that are easy to grade, like a coding problem with the right answer. We don’t know if messier, real-world work has sped up as much. But that cuts both ways. METR points out that AI’s math scores haven’t sped up much, even as Millennium Prize Problems that have stumped mathematicians for decades are now being solved.
A lot of people I trust have changed their minds because of this report. Ryan Greenblatt, who studies these risks for a living, says he was seriously wrong. He’d expected much less speed-up this year, and now calls the report a big update towards superintelligence within one to two years.
Buck Shlegeris now thinks there’s about a one in three chance AI companies build superintelligence within the next year. And if that happens, he thinks AIs will take over.
Nobody knows exactly how much AI is speeding up Anthropic’s AI progress. But whether progress is 1.4 times as fast or two and a half times as fast, AI is now helping build better AI. And nothing METR found suggests that’s about to stop.
I want to come back to Anthropic’s line: two years of progress in one. If METR’s right, isn’t Anthropic already there?
Apparently Anthropic didn’t think so, at least as of August. Their last public report said progress had sped up “by less than a factor of 2.” But when METR ran Anthropic’s private numbers, they came out at 1.97.
Just as I was finishing this video, Anthropic answered this question itself. Its latest IPO filing says it has now crossed its own line, based on what it expects from its next models and based on how fast things are moving now. It hasn’t said what it’s going to do about this, only that it’s evaluating the implications.
Anthropic is either at that line or very close to it. And I want to see Anthropic do what it said it would do. That means security strong enough to stop the world’s best-resourced hackers, including governments, and tracking everything that happens in its AI development, so it would catch an employee or an AI doing something it shouldn’t.
But to be honest, even if Anthropic does all of that, it isn’t nearly enough.
Recursive self-improvement — AI building better AI building better AI — may be close. The AI companies aren’t stopping because they think that if they do, their competitors will just keep going. And those competitors might be even less careful. So if the companies won’t stop themselves, the government needs to step in.
Alex Bores, a New York state legislator, is calling on Congress to ban AI companies from fully automating their own research. And some version of that proposal has supporters from Bernie Sanders to Steve Bannon. I think that’s exactly the right place to start.
Anthropic deserves credit for agreeing to this kind of outside investigation. OpenAI, Google, and the rest could be speeding up just as fast, and we wouldn’t know.
But Anthropic set the terms here. They decided what information METR could see, what made it into the final public report, and whether METR will be invited back. They also tightened their redaction rules in the final week, forcing METR to rework their public report and push back publication.
And METR says that, while writing their report, they were worried that being too critical could make companies less willing to let them in next time. That’s the problem with outside scrutiny that only happens when the company agrees to it.
So at an absolute minimum, every frontier company should have to report how much AI is speeding up its own research, and have someone independent check what they say.
If you remember early 2020, you know how this kind of thing feels. In February, COVID seemed like a far-off problem, or even fearmongering. By April, half the world was in lockdown.
That’s what happens when something keeps speeding up. It looks manageable right up until it isn’t. And COVID spread at a fairly steady rate. With AI, the worry is that the rate itself will keep increasing.
This might just be the beginning of an almost incomprehensible speed-up in the progress of literally everything, for better and for worse.
If you’re wondering what you can do: if you’ve been considering pivoting to work on this issue, now is the time to do it. That might mean working directly on these problems. It might mean finding a more flexible job so you can take on projects on the side. Or it might mean donating more, and thinking hard about where.
And talk about it. Share this video, or your own worries, with the people in your life. Most people still have no idea this is happening.
Or learn more about recursive self-improvement and why it’s so dangerous. We’ll leave some links below. If you’re not sure where to start, we have a free AI career advising tool that can talk you through it. It can suggest options and support you along the way.
Because if things change as fast as this report suggests, there may not be long before what we do stops making much of a difference. And when that happens, I want to be able to say we gave it everything we had.
