---
record_id: "podcast:2f567b98-aafb-4829-9338-79a3bf9b5403"
episode_id: 2f567b98-aafb-4829-9338-79a3bf9b5403
title: What Happens When AI Solves Your Life’s Work
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/what-happens-when-ai-solves-your-lifes-work/2f567b98-aafb-4829-9338-79a3bf9b5403"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/what-happens-when-ai-solves-your-lifes-work/2f567b98-aafb-4829-9338-79a3bf9b5403"
feed_guid: null
feed_url: "https://anchor.fm/s/f7cac464/podcast/rss"
published_at: null
published_local_date: null
played_date: 2026-10-09
played_at: "2026-10-09T12:00:00Z"
play_count: 1
duration_seconds: 1500
source: pocketcasts-history-browser
played_label: Yesterday
history_order: 6
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 4f92a9c8babaf20c3276bd2729304b3c3054366195b2001ba5d9d41086023a90
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

OpenAI’s annualized revenue was reported by the Financial Times as roughly $50 billion at the end of September, versus a widely circulated $68 billion figure that apparently came from an investor using Anthropic-style gross revenue before third-party revenue sharing, while OpenAI reportedly uses net revenue; OpenAI also told investors it had 77% run-rate growth in Q3 and 107% enterprise growth, yet the revenue gap pushed NVIDIA down 3%, Oracle down 5.5%, and other AI-linked stocks lower, raising questions about Anthropic’s IPO accounting. The Information’s subscriber survey found two-thirds of readers work at organizations developing AI applications, with 35% reporting multiple returns on AI spend, 17% positive but below hopes, 30% too early, 8% neutral, and 8% net negative; OpenAI regained the top vendor spot, Claude and Gemini usage fell, the top three vendors were used by 65–78%, Grok, Microsoft Copilot, and Perplexity were at 25–29%, OpenClaw hit a 12% high-water mark, Claude Code was used by 45%, Codex by 33%, Cursor by 23%, open-weight models were used regularly by 72%, Chinese open-weight models by 21%, and hiring changes were mixed: 22% hiring less, 10% more, 21% too early, and nearly half unchanged. Anthropic introduced a terms-of-service ban on “sustained and needless abusive or cruel behavior” toward Claude, which Box’s Aaron Levy framed as alignment/training-data hygiene, and launched Claude Dashboards and Claude Motion for natural-language data visualization and code-based animated presentations, with Robert Bayh and Drew Fallon highlighting practical value. The main story was OpenAI’s GitHub release of 372 novel mathematical results and 722 supporting papers from an unreleased internal frontier model, coordinated with a Mathematics Advisory Committee, with reasoning traces for 10 problems and an average compute cost of about three hours of ChatGPT Pro thinking per result; OpenAI reportedly fully solved 90 of ProofAtlas’s top 500 open math problems and made partial progress on Millennium Prize problems including the Riemann hypothesis and Hodge conjecture, following earlier AI milestones such as IMO gold-level performance, Erdos conjecture disproofs, and a Navier-Stokes proof. Reactions included Rutgers professor Alex Kontarovich saying a quasi-Riemann result would merit an instant Fields Medal if human-made, Darren Litt emphasizing verification work, Micah Warren treating it as labs spending money to solve problems, Anthropic researcher Levin Dalpogey calling it the most significant moment in mathematical history, former OpenAI researcher Acer calling it a Move37 moment, and Francesco Maggie and physicist Steve Su warning that AI-generated proofs may outpace human understanding, interpretability, and mathematical culture. Other named points included Shriram Kanan’s optimism about a “math genie,” Steven Strogatz’s note that matrix-multiplication efficiency improved to an exponent no greater than 2.25 from about 2.37, Justin Drake’s concern about missing cryptographic breakthroughs and possible government intervention, Scott Aronson’s report that AI labs may be discreetly testing whether models can break cryptographic protocols, Arpit Gupta and Ethan Mullik’s views that economics and social sciences may face similar disruption, Pedro Domingos’s Moravec’s-paradox framing, and Peyman Millenfar’s roadmap that structured domains like math and coding automate first, followed by hard sciences, finance, medicine, law, and then culture/art/strategic leadership. A KPMG/University of Texas at Austin study of more than 500 early-career professionals also claimed top “AI amplifiers” succeed by guiding, evaluating, and refining AI outputs rather than relying on knowledge alone.

For the user, the actionable implications are to treat AI adoption as a verification, governance, and workflow problem rather than a simple productivity claim: if evaluating AI vendors or financial exposure, distinguish gross versus net revenue, watch Anthropic’s audited financials and IPO narrative, and monitor whether semiconductor and AI-infrastructure stocks remain fragile to OpenAI/Anthropic growth stories; if using AI at work, track concrete ROI, hiring effects, and tool usage rather than hype, and test Claude Dashboards or Claude Motion for CRM/accounting visualization, natural-language querying, auto-updating dashboards, and editable code-based animations, while also evaluating agent tools such as Claude Code, Codex, Cursor, and OpenClaw. For open-weight models, build a governance decision around whether to use them for majority, minority, or experimental workloads, and specifically assess risk tolerance for Chinese open-weight models given the survey’s 46% work-use versus 21% Chinese-model-use gap. For mathematics, science, or research users, the follow-up questions are who verifies the proofs, whether formal verification can preserve human understanding, whether AI-generated results become “lettera morta” if not absorbed by the field, and whether matrix-multiplication advances could eventually affect AI inference efficiency. For security and crypto users, the concrete research lead is watching for AI-driven cryptanalysis, Bitcoin protocol risk, and broader digital-security exposure if internal models can break cryptographic primitives; follow-up questions include whether labs disclose such findings, whether governments suppress them, and whether post-quantum or protocol upgrades become urgent. For career and health-related decisions, there are no direct medical claims in the material, but the practical implication is that clinical diagnostics and medical decision-making are described as high-stakes, fragmented, and hard to automate, so users should not assume near-term replacement of clinicians; instead, focus on becoming an “AI amplifier” by learning to guide, evaluate, refine, and verify AI outputs, and ask which domain you work in is structured enough for fast automation versus dependent on noisy data, human judgment, regulation, or tacit knowledge.

## Transcript

So far, the idea that AI would upend and undermine entire industries hasn't really come to fruition.
Certainly, we're seeing how people do pretty much everything change.
Coding is perhaps the most changed, and yet demand for coders seems to be going up.
With a new set of mathematics results from OpenAI, however, some are asking: is this the first field-level AI disruption actually happening in practice?
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, Harbor, Robots and Pencils, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AIDailybrief, or you can subscribe on Apple Podcasts.
And if you want to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
Uh-oh.
Financial figures for the AI industry are being called into question as OpenAI's revenue numbers are revealed to be significantly lower than previously reported.
The Financial Times reports that OpenAI has told investors that they hit roughly $50 billion in annualized revenue at the end of September.
That's a fairly big gap from the $68 billion that was widely reported last month.
So, is this just misreporting or something else going on?
Well, sources said that the $68 billion whisper number came not from OpenAI itself, but from an OpenAI investor.
Apparently, what was going on is that that investor was trying to get an apples to apples comparison with Anthropic.
Anthropic numbers are always quoted as gross revenue before revenue sharing.
In other words, when Anthropic tokens are sold through a third party like Amazon or Microsoft, Anthropic is including that in the total revenue, even though by the terms of their deal, some big chunk of that revenue is going straight to the pockets of those third parties.
The logic, I imagine, is to try to provide an overall number of the total expressed demand in the form of Anthropic tokens sold.
And that is a useful number to know.
However, now that these companies are going public, that's not really a convention that's likely to fly in public markets.
Meanwhile, OpenAI has, for their part, always used net revenue after those revenue splits.
To make matters worse, the FT noted that the OpenAI investor calculated gross revenue based on a short timeframe.
It's unclear whether they extrapolated annualized revenue from a month, a week, or even a day.
The news was not all bad here.
OpenAI also told investors that they achieved 77% run rate growth in the third quarter and 107% growth in their enterprise business, but even that incredible growth was completely overshadowed by the $20 billion gap in revenue.
In many ways, Wall Street reacted as if OpenAI had missed on revenue during an earnings report.
Semiconductor stocks were down significantly after the FT published their report, with NVIDIA down 3%, Oracle down 5.5%, and the long tail of NeoCloud stocks seeing even larger drops.
And yet, even if we recognize that OpenAI is not yet a public company, had not shared the misreported number, and did not, in fact, miss projections on an earnings report, the reaction still brings up some big questions around the Anthropic IPO.
Once Anthropic's audited financials are available, they are presumably going to be much lower than the numbers Anthropic has been sharing with private market investors by the nature of using non-standard accounting.
Ultimately, the narrative battle is growing more intense as Anthropic heads towards IPO.
Ahmed is investing wrote: I don't know all the facts about this OpenAI revenue story, but what's becoming apparent once again is that this entire semi-trade is levered against OpenAI and Anthropic and its fragile AF.
Any narrative on slowing growth in the street loses their mind.
Next up, some interesting results from the information's latest subscriber survey.
In terms of audience, the information has a very tech-forward tech industry type of reader base.
They found that two-thirds of their subscribers work at an organization that develops AI applications.
Perceived return on investment seems to be rising rapidly, with 35% saying their organization is returning multiples on their AI spend.
Another 17% said the returns are positive but less than hoped.
30% said it was too early to tell, and 8% said returns were neutral, leaving just 8% who said AI spend had been a net negative.
The split between AI services is shaken up again, with OpenAI back on top.
During the last survey conducted during the summer, Claude had overtaken ChatGPT and Google Gemini was also gaining.
In this edition, usage of Claude and Gemini both fell as the information's readers signed back up with OpenAI.
These three vendors are still in the clear lead, with between 65 and 78% of readers using their services.
The next grouping includes Grok, Microsoft Copilot, and Perplexity, each between 25 and 29%.
The survey didn't include a specific section on recently released personal agent use, but the information did find that OpenClaw use is still at 12%.
Fascinatingly, this is the high watermark for OpenClaw among subscribers of the information so far this year, which means despite that hype train having died down quite a long time ago, the product itself continues to resonate.
Among other agent decoding tools, 45% use Claude Code, 33% use Codex, and cursor usage has doubled in recent months to reach 23%.
The information noted huge changes from a year ago.
This time last year, 59% of readers said that they had never used an agent.
The use of open weight models is also climbing, with 72% of survey respondents now using OpenWait models with some regularity.
20% said that OpenWait models now drive the majority of their organization's workload, 10% said usage was about even with closed models, and 42% said OpenWait models are deployed to a minority of workloads.
Interestingly, although 46% of respondents said that they were using open weight models for their work, only 21% said that they were using Chinese open weight models.
suggesting that most organizations, even these very forward startup type organizations, are still a little hesitant to rely on foreign models.
Finally, the information found little evidence that AI adoption has shifted hiring patterns.
Only 22% said that they were hiring less, 10% said that they were hiring more, and 21% said that this was too early to tell.
This left almost half saying that AI hasn't altered their hiring practices at all.
Of course, this is all just a small snapshot of a highly enfranchised set of AI users, but still provides some really interesting patterns nonetheless.
One update that is getting a lot of chatter on social media: in a change to their terms of service, Anthropic will now ban users for being too mean to Claude.
According to the new policy, users are prohibited from, quote, sustained and needless abusive or cruel behavior.
Anthropic said that the policy is only meant to apply in extreme cases and should not interfere with quote common versions of user frustration and pushback.
Thank goodness because the number of times I find myself asking Claude or GPT what the heck is wrong with it in much more colorful language would most certainly get me banned.
Now the discussion from there mostly went into AI model welfare and AI model consciousness, which is way beyond the scope of the headlines.
But for a takeaway from the AI Realist perspective, Box's Aaron Levy writes, This sounds weird, but it is actually probably a good policy.
Even if you don't believe AI is conscious, I don't, it stands to reason that you don't want future models trained on endless content of humans being rude to models.
The models only understand the data they've been trained on, or what they run into in their interactions.
So, if you want safe and aligned models, we probably want AI to have lots of good interactions in their training data.
For those just here for the features, a more interesting update for Claude was the introduction of Claude Dashboards and Claude Motion.
Dashboards allow users to connect Claude to a data set such as a CRM or accounting software and generate a custom dashboard for visualization of the data.
Users can also query the data in natural language to gather further insights.
The dashboards are also configured to automatically update as new data comes in.
Now, this kind of functionality has been technically possible for a while, but Anthropic is packaging it as a simplified feature accessible through simple prompts.
Motion, meanwhile, allows users to transform the data into short animations suitable for presentations.
The animations are written in code rather than video frames, so you can easily modify words and numbers without needing to start over with each edit.
This seems to be the practical use case for the flashy animations highlighted in the release of Opus 5.5.
Along with OpenAI's introduction of intelligent UI earlier this week, we're seeing a massive expansion in how AI can be used to communicate and interact with data.
The folks at Anthropic, meanwhile, suggest pushing this feature as hard as you can, with Robert Bayh posting: Try giving it bigger briefs than you think it can handle.
It will seriously impress you.
And indeed, early users are certainly impressed by what they see.
Drew Fallon of Iris Finance made an animated product demo commenting: A year ago, this would cost tens of thousands of dollars.
Insane.
If you haven't yet decided what you're going to spend your hacking time on this weekend, Claude Motions seems like a pretty good place to play.
For now, though, that is going to do it for today's headlines.
Next up, the main episode.
A new study from KPMG in the University of Texas at Austin found that when people work with AI, similar skills don't guarantee similar outcomes.
Researchers studied more than 500 early career professionals and found that the best performers consistently amplify the value of AI by guiding, evaluating, and refining its outputs.
These top performers, called AI amplifiers, weren't defined by what they knew alone, but by how they worked with AI.
Learn more about what separates AI amplifiers from everyone else at kpmg.com/slash uslash AI amplifiers.
Every episode, I talk about the competition between OpenAI, Anthropic, SpaceX AI, Google, and Meta.
And if you've been listening for a while, you might have a favorite.
Maybe you think OpenAI and Anthropic can stay ahead, or perhaps Meta's open source strategy can win out.
Whatever your view, every AI lab creates a different investment opportunity.
Harbor Capital Advisors AI Lab Ecosystem ETF suite lets you invest in the ecosystem behind the AI lab you believe in.
Search Harbor AI Lab Ecosystem ETFs wherever you invest or follow at HarborCapital on X to learn more.
Visit HarborCapital.com for a prospectus containing investment objectives, risks, fees, expenses, and other important information.
Read and consider it carefully before investing.
Risks include principal loss and artificial intelligence-related risks.
Harbor ETFs are distributed by Forside Fund Services LLC.
Harbor is not affiliated with AI Daily Brief, and the funds are not affiliated with, sponsored by, or endorsed by any AI lab.
This is a paid advertisement and not personalized investment advice.
Investing involves risk, including possible loss of principal.
The best teams don't have a single star carrying everyone else.
They know their own strengths and each other's weaknesses and play to both.
That's the team Robots and Pencils has built on purpose.
Nobody there is grinding through busy work to pad a headcount number.
People come for the hard problems and they stay because everyone around them is leveling up at the same time.
In a market full of companies that are just trying to hire fast, that's worth a look.
Check out robotsandpencils.com/slash careers.
Blitzy's understanding of massive code bases unlocks autonomous security fixes, modernization, and new features.
So, what happens when there's no legacy code at all?
Greenfield is supposed to be the easy part: clean slate, no technical debt.
But even Greenfield moves at human speed one sprint at a time.
Blitzy changes the unit of work from the developer to the project, autonomously planning, building, testing, and validating entire applications from scratch.
Hundreds of thousands of lines of production-ready code.
One Blitzy customer stood up a brand new application, 534,000 lines of code, compressing a 65-week roadmap into two weeks.
Another shipped an entire application with no front-end engineer.
Legacy or Greenfield, the answer is the same: software at the speed of compute.
Build what's next at blitzy.com.
That's B-L-I-T-Z-Y.com.
Welcome back to the AI Daily Brief.
Earlier this week, OpenAI released a tome of pioneering mathematical proofs that completely upended the academic field.
The results were published on a GitHub repo and included 372 novel results and 722 supporting papers.
OpenAI said that the results were generated by an internal frontier model that hasn't been released to the public, likely the same model that produced the Navier-Stokes solution last month, which kicked off a massive round of discussion.
This time around, OpenAI coordinated the release with their newly appointed Mathematics Advisory Committee.
Some of their suggestions included releasing reasoning traces alongside the proofs, which OpenAI has done for a sample of 10 problems.
The committee also suggested it would be useful to know the resources committed to each problem.
In that regard, OpenAI disclosed that the average results used compute equivalent to roughly three hours of ChatGPT Pro thinking.
But the real story here is how this release changes the field of mathematics.
In one fell swoop, OpenAI has solved a significant chunk of the most difficult outstanding problems in the field.
We did have a few progressive warning shots over the past year.
Last summer, models from Google and OpenAI achieved gold-level performance in the International Math Olympiad, the top contest for high school mathematicians.
Then, earlier this year, models from OpenAI and Anthropic disproved several Erdos conjectures, which are famous and long-standing problems in geometry.
Then last month, OpenAI released a proof for the Navier-Stokes equation, an almost 200-year-old problem in fluid dynamics.
Navier-Stokes is one of seven Millennium Prize problems which have a million-dollar prize attached.
Only one has been solved by a human, and merely making significant progress on one is enough to guarantee a Fields medal often compared to a Nobel Prize.
If you are currently in your head hearing Robin Williams and Stellan Skarsgård argue about a Fields medal, in Goodwill Hunting, you are not alone.
In any case, the Navier-Stokes problem was one of the most significant scientific results produced by an AI model.
And yet, it was just a tiny precursor for what OpenAI released this week.
The best way to understand the scope of OpenAI's proofs is to refer to a list of the top 500 open problems in mathematics produced by ProofAtlas.
This is an AI-generated list, but it's a decent representation of the most well-known problems in the field.
OpenAI fully solved 90 of the top 500 problems.
There's also dozens of partial proofs that would qualify as significant contributions to the field.
Among them were partial solutions to two additional Millennium Prize problems: the Riemann hypothesis and the Hodge conjecture.
For the purposes of this episode today, I'm not going to get deep into what these problems actually are, as they all involve postgraduate-level theoretical mathematics that is basically impenetrable to a layman.
Just to make that point, the Riemann hypothesis is arguably the most important problem in number theory.
It states that the Riemann zeta function, which concerns the distribution of prime numbers, has zeros only at even integers and complex numbers with a real component of one-half.
Instead, it's easier to gauge how big a moment this is by observing how professional mathematicians reacted.
Alex Kontarovich, a Rutgers professor, wrote, Quasi-Riemann hypothesis?
Are you kidding me?
If a human did this, it would be an instant Fields Medal, no questions asked.
Indeed, most of the initial takes came from mathematicians that have been relatively positive about AI's contribution to the field.
Darren Litt from the University of Toronto framed this moment as being about mathematicians shifting from working on problems for decades to verifying proofs produced by AI.
He commented, Fun.
Looks like mathematicians have a lot of exciting work to do.
If I understand correctly, one of the results is a very special case of a conjecture of mine, which is also a consequence of stronger work in progress by a student of mine.
Mathematician Micah Warren wrote, I didn't see anything particularly unexpected.
Labs can solve math problems now, so they just spent a bunch of money and solved a bunch of problems.
Historically speaking, in baseball terms, today would be the day that Barry Bonds blasted his 756th home run.
If you would have told Bonds this in 1987, it would have been unbelievable.
But in 2007?
Still, there was a sense of awe from those who had worked at the intersection of AI and mathematics over recent years.
Anthropic researcher Levin Dalpogey, who had been working on Navier-Stokes before OpenAI released their result, called this obviously the most significant moment in mathematical history.
Former OpenAI researcher Acer said the quasi-Riemann result was his personal Move37 moment for mathematics.
Move37 refers to AlphaGo's unintuitive move that helped it defeat Go world champion Lee Seidel in 2016.
Even for those without mathematical training, the results were fairly mind-blowing.
Responding to his first read-through the results, Chubby on X wrote, The list is absurd.
A zero-free half-plane for the zeta function, which is the first result of its kind in over a century.
Hilbert's 10th problem over the rationals, the Hodge conjecture for CM Abelian varieties, irrationality at Catalan's consent, and dozens more.
Any one of these would normally be a career.
But the number that many aren't seeing is the following: it's three.
That's the average hours of ChatGPT Pro compute per result.
A month ago, Navier-Stokes took them around 10,000 agents in 88 hours.
That efficiency gain is within just a few weeks.
Math Twitter obviously is shocked.
Again, this is literally the intelligence explosion happening right now.
2027 will be the year of superintelligence.
I'm now convinced of that.
Still, one big wrinkle in the release is the difficulty in understanding exactly what's been published.
The Navier-Stokes result published last month is still in the process of being verified by mathematicians, and this is hundreds of new results to pour over.
Mathematician Francesco Maggie pointed out the obvious issue with high-volume AI mathematics, writing: Mathematics does not simply grow by accumulating correct statements.
Results have to be understood, connected, explained, challenged, reused.
Until that happens, they risk remaining lettera morta.
Now imagine adding 400 more AI-generated proofs.
For each of them, until some human mathematician picks it up, studies it, and connects it to the existing mathematical culture.
Isn't it in essentially the same position?
So, my question is genuinely: what is the intended mathematical value of releasing hundreds of proofs at once?
What happens if there simply aren't enough people willing or able to read them?
To be clear, I think mathematicians should discover mathematics by any means necessary, including scavenging through artificial alien-looking mathematical material, since there may be extraordinary things to find there.
But humans are not machines, as attention, understanding, taste, and mathematical culture are scarce resources.
What happens if the rate at which mathematics is generated becomes much greater than the rate at which mathematicians can absorb it?
Physicist Steve Su took it a step further, asking, What happens when a single day of AI research produces more mathematics than humanity can absorb in a century?
Imagine millions of superhuman research agents at work.
Formal systems may verify the proofs, but humans won't have enough context to understand the underlying web of machine-invented concepts.
In his view, we could quickly reach a period where fields like mathematics and physics lose interpretability.
At that point, he continued: AI is no longer a scientific tool.
Humans are receiving selected explanations from a much larger intellectual civilization they cannot independently grasp.
Another big strand of the conversation was speculation on what this could mean for mathematics as a field of academic study.
Dan McCaddier wrote, Open AI is downplaying this for PR reasons.
If you're a mathematician, you must feel like a nuclear bomb hit and you're at ground zero.
Reasoning models are two years old.
In that time, they went from incapable of basic arithmetic to solving problems humans couldn't solve for decades.
Math is only the beginning.
AI will revolutionize the entirety of the human scientific endeavor.
Most of us don't appreciate what that means.
And you can feel a bit of that shell shock that Dan is talking about, especially among mathematics students still trying to find their place in the world.
Mostly harmless grad students asked, What can I pivot to now that AI has taken away math?
They later explained that this release, quote, kind of nukes basically all the problems and projects I'd want to contribute to or work on in my program.
And yet, if there were many lamenting over the apparent end of a field, some mathematicians were incredibly optimistic.
Shriram Kanan, a former math professor at the University of Washington, wrote, It's a great day for humanity and math.
If you asked a mathematician anywhere from 5000 BC to January 2026 whether they would like a math genie to exist, 100% of mathematicians would have said yes.
Mathematicians give up significant opportunity costs to help advance human knowledge.
It's a no-brainer that they will eventually adjust to this new world and be glad this happened.
It's just an extreme but temporary shock to I am world class at math as an identity.
Another very different topic of conversation was how results in any of these theoretical mathematics problems apply to the real world.
The Erdos problems are mostly just intellectual exercises with no clear application.
Even the Navier-Stokes proof, while very impressive, doesn't really have an obvious impact in the real world.
Engineers working on fluid dynamics problems like aircraft design get by just fine using a simplified version of Navier-Stokes.
Most of the problems that OpenAI solved in this batch are similar, very impressive, long-standing, but ultimately not all that practical.
Still, there were a few examples that could make an impact in the real world.
One was a dramatic improvement to the theoretical efficiency of matrix multiplication, the math that underpins AI inference.
Cornell math professor Steven Strogatz commented, many staggering results here, but this is a particularly amazing one.
The exponent for matrix multiplication is no more than 2.25.
The previous world record had been something like 2.37.
This leap in progress is like Bob Beeman's long jump.
For some, what was most interesting was not what was there, but what was missing.
Bitcoin security researcher Justin Drake noted a quote, striking underrepresentation of cryptographic breakthroughs among the 722 mathematical results OpenAI published.
I've witnessed firsthand the US government censoring academic quantum cryptanalysis results.
Backroom interventionism is my base case.
University of Texas computer science professor Scott Aronson added on his blog, My sources tell me that AI companies have now started, gingerly and discreetly, investigating whether their latest internal models can break important cryptographic protocols and primitives.
If they can, then it would certainly be nice to get ahead of things before the rest of the world figures out the same.
In other words, if OpenAI's internal model can break major cryptographic schemes, that's not just a problem for Bitcoin, it's a problem for the cryptography that underpins pretty much all of the digital world.
Still, with all of this, maybe the most resonant conversation was whether we can expect the same thing to happen to other fields.
Arpit Gupta, an associate professor of finance at NYU Stern, wrote, You're deluding yourself if you think AI advances like in math aren't coming to economics and other social sciences.
Warden economics professor Ethan Mullik is already starting to see it, commenting, After a brief but institution-eroding slop science era, it increasingly looks like we are going to have two revolutions from AI.
One, everything ever published will be reread and rejudged in ways that human scientists never anticipated.
Two, novel discoveries will start to come fast.
I am seeing rapid increases in the ability of AI to do novel work in my field of economic sociology, with nearly autonomous research getting to top journal level.
Still, a big question is whether all other fields are able to be approached in the same way as mathematics.
By and large, these math proofs were not generated by reasoning into novel ideas.
They were largely within the domain of problems that could be solved with big data approaches coupled to pattern recognition.
It would be reductive to call them brute force, but these are all verifiable problems that fit neatly into the reinforcement learning paradigm.
Pedro Domingos, a computer science professor at the University of Washington, summed it up by commenting: Mathematics is a classic example of Moravec's paradox.
Hard for humans, easy for machines.
Unpacking his roadmap for where this is all going, Google distinguished scientist Peyman Millenfar wrote: Speed of automation is in inverse proportion to the entropy of the subject domain.
Math and coding are structured and orderly, which is why AI is able to do them so well.
In order of difficulty, the hard sciences are next.
They may be governed by strict physical laws, but are complicated by dependence on noisy measurements and laboratory experimentation.
Financial markets are more difficult still.
They are complex, adaptive systems subject to human psychology.
While past data is abundant, the underlying statistics are non-stationary and highly variable.
Clinical diagnostics and decision-making in medicine are far more difficult than most people realize.
It's very high stakes, it requires synthesizing very fragmented signals, and dealing with idiosyncratic human behavior in biology.
It's a nightmare of incomplete information.
The law, jurisprudence, and legal interpretation operate on structured text and precedent most of the time, but rely heavily on ambiguous language, evolving societal norms, persuasive rhetoric, and human judgment.
They won't be automatic anytime soon.
Culture, art, and strategic leadership are an odd mix, but I think all of them are quite safe from automation.
They are the pinnacle of disorder and human creativity.
They rely on tacit knowledge, intuitive perceptions of the world, emotional intelligence, understanding of cultural consensus, and navigating complex moral trade-offs.
So rejoice!
We'll have artists, lawyers, doctors, and CEOs for a long time yet.
In fact, I think from here, there are two incredibly fascinating paths to watch.
One is what Payman was speculating on, which fields this sort of disruption comes to in what ways, or alternatively, it shows us that there are human or systemic inertia road bumps that make this disruption not as inevitable in other areas.
But the second thing that I think will be interesting to watch is what mathematicians do with all of this.
To use the words of the previous commenter, what happens when every mathematician has a mathematical genie?
Does it negate all of their hard work and learning, or does it allow them to do things that are undreamed of as of yet?
Over the coming months, that is what we will begin to see.
For now, that is going to do it for today's AI Daily Brief.
Appreciate you listening or watching, as always.
And until next time, peace.
