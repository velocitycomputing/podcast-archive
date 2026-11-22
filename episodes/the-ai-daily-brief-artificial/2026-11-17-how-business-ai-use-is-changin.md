---
record_id: "podcast:765e3530-74c0-42be-9d19-189aac343561"
episode_id: 765e3530-74c0-42be-9d19-189aac343561
title: How Business AI Use is Changing
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-business-ai-use-is-changing/765e3530-74c0-42be-9d19-189aac343561"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/how-business-ai-use-is-changing/765e3530-74c0-42be-9d19-189aac343561"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-11-17
played_at: "2026-11-17T12:00:00Z"
play_count: 1
duration_seconds: 1440
source: pocketcasts-history-browser
played_label: November 17
history_order: 9
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 97626fb7daf1a8a087b092c45d77295bc0c643078dd73207dce8b8f1107a271d
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

Three enterprise-AI studies—Databricks’ AI Index, Arcana Research’s annual enterprise-AI study, and RAMP’s AI Index—converged on the claim that token-price competition is giving businesses more leverage: RAMP reported usage up 36% while spend rose only 2%, with average OpenAI/Anthropic pricing down 21% per million tokens; Databricks’ Unity Gateway showed single-provider use falling from 64% in July to 72% using two or more providers by November; Arcana found 91% of Global 2000 leaders expect higher 2026 AI budgets, mostly 20–40%, yet two-thirds lack visibility into model/API spend. The Jensen Huang/NVIDIA saga included sources saying the board is not discussing his return while Wachtel Lipton investigates alleged national-security/company-secret risks, a 180,000-signature petition backed by Elon Musk and Tim Sweeney, shareholder letters from Brad Gertzner and Gavin Baker, and President Trump’s comments downplaying the Alice Huang spy narrative; Sam Altman said the AI industry can stand without Jensen despite OpenAI’s $100 billion NVIDIA guarantee, while interim CEO Colette Kress is reported to be tightening data-center backstops. Additional headlines included Commerce Secretary Howard Lutnick’s delayed export-control rule requiring licenses in Singapore, Malaysia, Thailand, Indonesia, and Brazil to curb remote access to NVIDIA chips, Treasury Secretary Scott Bessant’s role pushing it, Trump’s “national champion” plan naming NVIDIA, Amazon, Microsoft, OpenAI, and Anthropic, OpenAI’s embedded safety-evaluator agreements with Apollo Research, Meter, Transloose, and Goodfire criticized for limited access and a “Tattletale Clause,” and a JPMorgan Chase-originated banking outage affecting Bank of America, Wells Fargo, Capital One, and US Bank that JPMorgan blamed on an on-premises software bug, fueling skepticism after Microsoft and FAA outages. The studies also found coding dominates spend (72% on RAMP; one-third of Global 2000 piloting coding tools), Anthropic has enterprise momentum (45% of RAMP businesses vs 40.6% OpenAI; 68.8% of Unity Gateway proprietary tokens; 81% named it exciting), customer-support AI spend jumped from 0.8% to 13.3%, spend is highly concentrated (RAMP top 1% spend 625x median $16.32; Databricks 99th percentile ~$700/week vs median $2.49), frontier-model shares diverged (RAMP frontier spend 67.7% to 69.5%, Databricks Fable 5.5% to 0.6% while Opus 5.5 rose 7.2% to 37.9%), and agents remain more aspirational than deployed.

For the user, the practical move is to treat enterprise AI as a procurement, governance, and operational-risk problem rather than a health issue: there are no health implications in the supplied material. Actionable decisions include renegotiating model contracts using evidence that usage can rise without proportional spend, building or testing model-routing/switching infrastructure so the organization can move between OpenAI, Anthropic, and other providers, replacing raw token-price dashboards with cost-per-successful-task metrics, and creating visibility into API/model spend because two-thirds of surveyed Global 2000 leaders lack it. Research leads and follow-up questions should focus on whether the organization is overpaying for frontier models when cheaper or newer models dominate usage, whether coding and customer-service pilots have measurable ROI, whether autonomous-agent plans are realistic given adoption lags, and whether safety/vendor agreements provide employee-like access, unredacted evidence, independent reporting channels, and external standards rather than company-controlled disclosure. For infrastructure and compliance, ask whether critical systems depend on single points such as JPMorgan backend services, whether on-prem software bugs and maintenance failures have redundancy and postmortems, and whether operations in Singapore, Malaysia, Thailand, Indonesia, Brazil, or remote-access arrangements trigger new export-license obligations; monitor NVIDIA leadership, data-center financing, national-champion designations, and OpenAI/Anthropic pricing as leading indicators for budget and vendor strategy.

## Transcript

Three different studies of enterprise AI behavior have just come out, and today we're exploring how they're telling a kind of similar story about where enterprise and business AI is.
In short, the leading companies are taking advantage of increased token price competition to get good deals, move towards efficiencies, and increase their AI usage without increasing the cost proportionally.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors: KPMG, Robots and Pencils, Granola, and Blitzy.
For an ad-free version of the show, go to patreon.com/slash AIDailybrief, or you can subscribe on Apple Podcasts.
And if you want to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
Finally, a quick reminder that this week's How We Got Here is all about GTA 6, but not really the game, and instead, it's about how the game reflects the changing economic and social expectations of America.
People seem to be really liking this one, so check it out in the show notes.
We kick off today with the latest updates in the Jensen Huang saga, where the NVIDIA board seems to think that his return is off the table.
As we have been following, influential tech leaders have been rallying around the embattled CEO since his resignation last Thursday.
A petition gathered 180,000 signatures and counting, including Elon Musk and Epic Games CEO Tim Sweeney.
Investors Brad Gertzner and Gavin Baker wrote to the board in their capacity as shareholders, demanding a replacement process that included full consideration of allowing Jensen to return.
When asked about Jensen returning, President Trump even said, I would not mind that.
A lot of people are asking Jensen, they think Jensen should go back.
That certainly isn't a bad idea.
In a follow-up question about Jensen's conduct putting national security at risk, Trump responded, It was not put at risk, and our country is now stronger than ever before.
And you know, China plays games with us, and we play games with China.
Trump appears even skeptical of the narrative that Alice Huang is a Chinese spy, commenting, Nobody's proven that she's a spy.
She may not be a spy.
As of last weekend, Jensen was reportedly on board, and the idea seemed to be gaining momentum.
However, on Monday, sources went to the media to throw cold water on the idea.
Speaking with CNBC, a source with knowledge of internal matters said that the NVIDIA board is focused on the investigation into Jensen and is not in discussions to bring him back.
The reporting noted that law firm Wachtel Lipton was retained last week to conduct the independent investigation, which is still ongoing.
The scope was described as covering Jensen's conduct and whether it compromised national security or company secrets, i.e., it seems clear for the board that Jensen's infidelity is the least of their concerns.
One thing that's important to keep in mind is that the stakes are not low for the board either.
When asked on CNN if there was any chance that Jensen would be reinstated, Scott Galway said, I think the odds are almost zero.
But if you're on the board, you've got to assume at some point you might not only be testifying in front of Congress, but you might be testifying in a court of law.
This is an issue of national security.
This certainly could change, but at the moment, it does feel a bit like the story is dying down.
And barring some major moves from Jensen himself, I think it feels as though we're soon to be moving on.
In that context, Sam Altman has said that the AI industry will be fine without him.
During the fallout from the resignation, one of the biggest industry concerns has been the loss of NVIDIA as a financing channel for infrastructure development.
The company has been acting as something of a central bank for AI, and by all accounts, Jensen was personally directing the flow of funds.
During an interview at Semaphore's event on Monday, Altman made clear that he believes the industry can now stand on its own two feet.
The revenues and demand are growing so strongly that I think the industry will be fine, he said.
He did add, I think Jensen has played this extremely special and valuable role as someone to really drive things forward with great vision.
Notably, OpenAI secured a $100 billion guarantee from NVIDIA to build their Ohio facility, so even they were dependent on NVIDIA as a financing vehicle.
Altman believes this won't change all that much under new leadership, commenting, NVIDIA is a behemoth of a company.
I think people still trust their guarantees very much.
Altman is, of course, in a unique position to understand what Jensen is going through.
At that same event, he referenced his own ouster as OpenAI CEO in 2023, saying that he has, quote, personal strong empathy to a situation like this.
Outside of Silicon Valley, there's much less conviction that data center funding will continue in the same way.
John Todorom, a senior analyst at Needham <unk> Co., said, chip manufacturer support was becoming more needed than before.
Any disruption at NVIDIA raises questions and leads to a more uncertain environment for credit support for NeoClouds.
The Wall Street Journal reports that interim CEO Colette Kress is expected to rein in data center backstops and venture investments, but interestingly, they claim that Jensen was already in the middle of pulling back on commitments over recent months.
During a Berlin meeting last month, Jensen reportedly demanded upfront payments for chips, telling the NeoCloud bosses, you're not charging what you should be charging.
I don't even need you guys.
I could just give all this capacity to Elon.
Elon wants it.
The message was clear, writes the Wall Street Journal.
NVIDIA's days as an open checkbook were over.
Moving on, one of the big questions we had in yesterday's show was whether we'd start to see actual actions around some of these China and export control issues.
Well, the Commerce Department apparently has been spurred into action on export controls after facing tough scrutiny over the past week.
Commerce Secretary Howard Luttnick has been heavily criticized for dragging his feet on export controls and was called out multiple times on the Sunday shows.
On Monday, the Commerce Department announced a long-awaited rule designed to shut down remote access to NVIDIA chips.
Basically, for years, Chinese labs have been gaining access to chips installed in third-party countries.
The new rule requires data center operators in Singapore, Malaysia, Thailand, Indonesia, and Brazil to apply for an export license to purchase advanced AI chips.
The rule states that these countries, quote, present a higher-than-normal risk of diversion.
Existing data centers are required to get licenses within 90 days, allowing the Commerce Department to investigate prior shipments of chips.
The announcement also sheds some light on the interdepartmental fight over chip policy within the Trump administration.
Treasury Secretary Scott Bessant was understated in his criticism of the Commerce Department during an appearance on Fox News on Sunday.
He said many other departments were pushing for this and Commerce had the pen.
Strangely, the new rule states it was, quote, written by and at the direction of the Department of Treasury and the National Security Council.
Sources told Politico that Bessant pushed the new rule through with support from Secretary of State Marco Rubio.
An earlier version of the report said that this was done despite objections from commerce, but that reference was removed.
It has been clear for some time that there are two warring factions within the administration when it comes to chip policy, but the fight is now bursting out into the public.
During press availability on Monday, President Trump said that the conflict between Besson and Luttnick came down to their different viewpoints.
One wants to be friendly with China, he said, and one wants to have a blow-up with China.
We're having a very good relationship with China right now, and I understand both sides of it.
When asked if he would fire Luttnik, Trump responded, No, he's done a very good job.
For the China hawks, the division on policy seems like a recipe for disaster.
Chris McGuire from the Council on Foreign Relations said, What this says to me is on a macro level, they're not on the same page, and commerce doesn't want to do this at all.
He added that it's dangerous to trust commerce to enforce the rules, saying, We're just going to see these loopholes continue to be exploited.
Christopher Padilla, a former commerce official from the W.
Bush administration, said he couldn't recall another instance of an agency distancing themselves from a rule they issued.
He said, By exposing this level of interagency disagreement, what it does is open an opportunity for China or others to find ways around the rule if they think they can devise some workaround that they can convince the Commerce Department to go along with.
Both Lutnick and Besson have joined the president on his trip to China this week, so, you know, maybe they'll settle their differences on the long flight to Shenzhen.
In some good news for NVIDIA, the Trump administration plans to name them as a national champion under a new program.
Sources told the Wall Street Journal that the administration plans to identify several AI companies as national champions next week.
The designation would allow these companies to receive expedited approvals for export licenses, government support for international business development, and access to federal financing.
The program will be run through the Commerce Department and was announced around a year ago.
However, this will be the first time that Commerce names champions.
Sources said the list includes NVIDIA, Amazon, Microsoft, OpenAI, and Anthropic.
A core goal is said to be packaging chips, models, and other AI products together to streamline international sales.
Moving over to some safety discourse, OpenAI has signed agreements to embed independent safety evaluators in their organization.
On Monday, OpenAI announced agreements with Apollo Research, Meter, Transloose, and Goodfire, where evaluators will be granted, quote, deep access to OpenAI's internal models and systems for the purpose of assessing model alignment and gauging the effectiveness of safeguards.
Each of the major frontier labs committed to giving external evaluators access as a response to the Hugging Face incident and the outrage that followed.
This pledge later formed part of the White House Accord on Superintelligence.
Anthropic granted access to Meter and SecureBio last month and said evaluators would be given quote employee-like access.
We've already seen the first report from Meter, and while they noted that Anthropic censored the report, most in the safety community seems satisfied.
The same cannot be said for OpenAI's efforts.
Apollo Research published their own press release describing the scope and limitations of their engagement.
A team of six evaluators will be embedded at OpenAI for four months.
The goal is to test whether OpenAI's internal models subvert alignment and control mechanisms.
They wrote that they will have enough access to assess these concerns, including reasoning traces, reinforcement learning rewards, and the ability to query immediate model checkpoints.
However, Apollo noted that the agreement allows OpenAI to withhold information as they deem necessary in relation to technical limitations, security risks, and IP protection.
In addition, OpenAI will only make certain staff members available for discussion, and Apollo will not be granted access to the company's Slack channel.
They also retain the right to censor reports in relation to confidential information, including when it's used as supporting evidence.
But conclusions from the report are to be published without change, even if they're unfavorable.
Apollos seem to have a few complaints about the arrangement, posting on X: Embedded evaluations must be credibly independent of trust in the developer.
This requires strong guarantees for access, disclosure, and meta-transparency.
This pilot is an ambitious first step towards the goal of obtaining these strong guarantees, but its access and disclosure rights don't yet meet our bar for full embedded evaluations.
The safety community was up in arms over the limitations.
Neil Nanda, the interpretability lead at DeepMind, complained that the agreement fell short of the employee-like access that Sam Altman had promised in September.
Stephen Adler, a former OpenAI safety researcher, was frustrated at what he called the Tattletale Clause, writing, If an OpenAI employee raises concerns to Apollo, even with info clearly relevant to the investigation, Apollo must stop them and go through OpenAI's lead unless they were pre-authorized.
The debate about this probably deserves an entire show, given how many dimensions of this there are.
But at the end of the day, even if people like Anthropic's version of this better, these are still the companies in question handpicking groups and giving them the access that they deem fit, which, while completely reasonable from their standpoint as trying to run a business, has a completely different set of incentives than the broader societal need that these independent auditors are supposed to be addressing.
If we want to be serious about this, there need to be agreed-upon standards, not necessarily just written by the industry, and third parties with actual clear independence dictated by some external force.
Now, if you're surprised at my tone here, I think that this sort of independent embedded auditors is one of the very few things around safety policy where we can build actual broad consensus, and so it behooves us to try to get it right.
Lastly, today, one that we're keeping an eye on, a major banking outage has added to fears that critical systems are failing across the world.
First, we had the Microsoft outage, then the nationwide FAA grounding, and now the banking system has suffered a major issue.
On Monday, JPMorgan Chase and Bank of America ran into problems when web and app logins, ATMs, and transfers stopped working.
The problem spread across the banking system, with Wells Fargo, Zell, Capital One, and US Bank all reporting issues.
The source of the problem was ultimately traced to JPMorgan Chase.
In addition to servicing customers, the mega bank also manages several critical backend systems that allow the financial system to function.
Like the other issues, many were quick to assume AI, but after bringing their systems back online, JPMorgan Chase blamed a quote technical issue.
They said the disruption was caused by a software bug in on-premises hardware and claimed the issue wasn't related to cybersecurity.
Without commenting, I would say that the sentiment surrounding these issues is getting more and more incredulous.
Semi-paid Vibecoder wrote: Outlook being down for 24 hours wasn't a cyber attack.
FAA ground stop of all planes for 12 hours wasn't a cyber attack.
US banking system being down, including ATMs, not a cyber attack.
Okay, but why are we having all these catastrophic maintenance and upgrade issues all over the place?
Academic and entrepreneur Vivek Wadra writes: I'm not a conspiracy theorist, but all these coincidences and denials are turning me into one.
Microsoft, the FAA, Workday, JPMorgan, and other major banks all suffer outages within days of one another.
Could China be probing and testing vulnerabilities in America's critical infrastructure?
I'm not convinced by the denials.
Something doesn't add up.
As I said in yesterday's episode, the narrative around this and AI's role is something that I am continuing to watch.
For now, however, that is going to do it for the headlines.
Next up, the main episode.
Hello, everyone.
One big change around AI is we've shifted our thinking from how we rank our pages to how do we become the source that AI trusts enough to answer with.
At KPMG, they're seeing this firsthand.
AI-generated results now surface answers directly, often without a single click.
That's why they are increasingly focused on generative engine optimization, or GEO, structuring content so AI systems can retrieve it, understand it, and cite it as trusted authority.
This is not just an SEO evolution, but a visibility mandate.
And indeed, the GEO mandate from KPMG is simple.
If AI is shaping decisions, your expertise needs to show up inside the answer.
Read all about it at kpmg.com/slash us slash GEO.
Again, that is kpmg.com/slash us slash GEO.
The best teams don't have a single star carrying everyone else.
They know their own strengths and each other's weaknesses and play to both.
That's the team Robots and Pencils has built on purpose.
Nobody there is grinding through busy work to pad a headcount number.
People come for the hard problems and they stay because everyone around them is leveling up at the same time.
In a market full of companies that are just trying to hire fast, that's worth a look.
Check out robotsandpencils.com/slash careers.
You're in back-to-back meetings all day.
You're trying to stay present, but you're also worried you'll forget the decision, the action item, the important next step.
This is a scenario that we absolutely live here at the AI Daily Brief.
Given how fast things move and change and how quickly we're evolving everything that we do.
That's where Granola comes in.
Granola is an AI-powered notepad for meetings.
You jot down rough notes like you always do, and in the background, Granola transcribes and turns them into clear, useful notes when the meeting ends.
No bots joining your calls, no distractions, just a clean notepad that helps you focus.
During or after the call, you can chat with your notes, ask Granola to pull out action items, help you negotiate, write a follow-up email, or even coach you using recipes which are pre-made prompts.
Once you try it on a first meeting, it is very hard to go without.
Head to granola.ai/slash AI Daily and use code AI Daily to get 100% off for three months for new users.
That's granola.ai/slash AI Daily, and code AI Daily to get 100% off for new users for three months.
Blitzy deeply understands your code base before it writes code.
Here's the first place that pays off: security in the age of AI.
Vulnerabilities don't live in isolation, they live buried inside millions of lines of interconnected code where patching one thing quietly breaks three others.
That's why surface-level scans fail.
Blitzy starts from its knowledge graph of your entire application, identifies and surfaces CVEs across the full estate, proactively recommends patches, and can execute the PR.
Each fix is grounded in how your systems connect and validate so nothing new breaks.
And the knowledge graph dynamically updates, keeping you ahead of an ever-accelerating threat landscape.
One Blitzy customer resolved 21 active CVEs across six core microservices in four days.
Zero compile errors, every validation scan clean, months of planned work fixed in less than a week.
Security remediation grounded in real architectural context at the speed of compute.
Harden your code base at blitzy.com.
That's B-L-I-T-Z-Y.com.
Welcome back to the AI Daily Brief.
Today we are looking at some changes and shifts and trends in how business and enterprise AI is being rolled out.
We'll look at spending, behavior, usage, and trying to see what it all means.
Now, there are four sources for this, and the episode was inspired by running into all of them telling fairly similar stories in just a couple of short days.
The sources are Databricks' new AI index that was just introduced and published on Monday, Arcana Research's first annual study on the state of enterprise AI, and the RAMP AI Index, both for November, which came out about a week ago and for October.
Together, they tell the story of a business AI environment where the businesses themselves have a lot more options and they're getting much more comfortable moving around to find the best deals.
So let's talk about some of the big overall themes.
The first is that growth in usage is outpacing growth in spend.
RAMP found that over the past month, while usage was up 36%, i.e.
the total number of tokens that were consumed across RAMP businesses was up over a third, they only spent 2% more to access those increased tokens.
Unsurprisingly, the reason for this is that tokens in aggregate are getting cheaper.
Across OpenAI and Anthropic, the average price per million tokens in October was down 21%.
And what's important to note here is that this means not only, or not even necessarily, that companies are shifting to cheaper Chinese models, but that the very presence of those cheaper models is forcing price decreases among the big providers.
Now, one could also argue that it has been a prerogative for both OpenAI and Anthropic to drive more efficient models that bring their prices down, anyways.
And whatever the combination is, it's starting to show up in the numbers.
And part of the motivation seems to be that enterprises are getting much more comfortable switching models than they were in the past.
Databricks offers a product called Unity Gateway, which is basically a model router style efficiency solution to help enterprises find the right model for the job and save costs along the way.
Back in July, 64% of the companies on Unity Gateway used only a single model provider.
The ratio had completely flipped as of the beginning of November, with 72% now using two or more model providers.
Databricks argues something that we've been talking about a lot here: that this means that token price in the raw is actually the wrong number to watch, and that instead, enterprises are going to increasingly be focused on cost per successful task.
Across the leaders at Global 2000 companies that Arcana surveyed, they found not only was AI now an eight-figure budget line, but that 91% expected to spend more in 2026, with most expecting their spend to go up between 20 and 40%.
And yet there is clearly still a gap between those Vanguard organizations like the ones in the Ramp Index, who are operating more nimbly with regard to AI, and a lot of the more middle-of-the-range Global 2000s, who seem to still be operating with some old methodology.
A full two-thirds of the leaders Arcana surveyed said that they didn't have visibility into what they spend on model and API usage.
You gotta think that that's something that's going to change very quickly.
So, where all of these reports agree?
The first is that this is increasingly a buyer's market where buyers have the leverage.
Part of this is because switching is getting increasingly normal and adding more heft to the Databricks finding.
In our CANA survey, a full third of OpenAI customers said they'd be open to switching, frequently considering a move to Anthropic, and 43% of GitHub co-pilot customers were open to switching, generally naming Claude Code.
Another area where the reports agree is a phenomenon that we are tracking closely, which is spend concentration.
As of November, RAMP found that the top 1% of firms are spending about 625 times what the median firm is spending per employee per month.
The median firm sits at $16.32, while the top firms are spending over $10,000 per employee per month.
As I always mention when we're talking about RAMP, it is important to point out that they are a very specific sample of generally technology-based and tech-forward companies.
So their top 1% are really going to be a very differentiated group.
Still, Databricks also found a huge gap, whereas their median user spends $2.49, the 99th percentile user spends almost $700 a week, a 281x difference.
Across all these studies, coding remains king.
72% of spend on RAMP comes from the engineering teams.
And of Arcana's Global 2000 respondents, a full third are piloting AI coding tools, which is the biggest pilot group of any category.
Now, in terms of the competitive set, Anthropic pretty clearly has the enterprise momentum.
Just under 45% of U.S.
businesses on RAMP pay Anthropic against 40.6% for OpenAI.
68.8% of proprietary model tokens on Unity Gateway go to Anthropic's models.
And when asked to name an exciting AI vendor, 81% of those surveyed by Arcana named Anthropic.
One growing use case appears to be customer service.
The percentage of spend on RAMP from customer support teams grew from 0.8% in June to 13.3% in November.
And 38% of the Global 2000 respondents for Arcana already use AI customer service.
But the reports don't agree on everything.
While Arcana's survey found that 91% expect to spend more on AI in 2026, token spend on RAMP has been fairly reduced.
Token spend growth in August was 1.05%, went down to just 0.22% in September, and grew 1.65% in October.
Now, if that 1.65% number held, it would compound to about 22% a year.
While that is a significant slowdown in what we've seen in the past, that would fall within the expected 20 to 40% range reported by the Arcana survey.
Another place where there's divergent signals in the data is around how enterprises are interacting with the most state-of-the-art models.
In October, AI spend on RAMP on Frontier models went from 67.7% up to 69.5%.
Over on Databricks, however, Fable's token share fell from 5.5% to 0.6%.
Now, what's interesting is that this may be less about Frontier models in general and more about Fable specifically, because also on Databricks over a six-week period, Opus 5.5 went from 7.2% to 37.9% of tokens.
In other words, it may be that Opus 5.5 is just so dominant that Fable 5.2 hasn't really found its place yet.
And as we settle into our year-end assessments, which spoiler alert, I think pretty much everyone is going to declare 2026 having been the year that agents got real.
When it comes to many of these more average enterprises, agents in many cases still remain aspirational.
Arcana, for example, found that while autonomous agents are number four on their heat index of pilots and plans, i.e., the things that people are most excited about, they are dead last on the adoption index of what is actually deployed.
Now, to reiterate, each of these surveys has its challenges.
Databricks is focused on the customers that are actually running through their gateway.
RAMP is dealing with a very small set of buyers that reflect a very particular type of group.
And the Arcana sample size of Global 2000s is quite low overall.
And yet, across all of this, I think that the convergent stories are much stronger than the divergent ones.
And it's the stories we've been telling for months now.
Model competition is putting pressure on everyone to reduce prices.
Enterprises are thinking in terms of not just capability, but efficiency, and are increasingly willing to switch models.
And when it comes to market opportunity, the big question remains: whether these 1% of companies who are spending 625 times as much in RAMP's estimation and 281 times as much in Databricks estimation are complete outliers or closer to a vision of the future where the median buyer of everyone else will increasingly nudge in that direction.
Inevitably, it's going to be somewhere in between, but how close the industry gets to that 1% actually reflecting the median is going to say a lot about the size of the overall market and its ability to turn all this CapEx spend into ROI.
Now, if you are an enterprise yourself, I think the main takeaway for you from all of this is that you probably have a lot more leverage than you're exerting when it comes to negotiating deals.
Competition is vicious, and the model providers are trying desperately to not just have their product turn into a generic commodity.
In that competition, there are deals to be had if you've built the infrastructure to be able to actually switch and take advantage of all these changes.
Big thanks to Ramp, Databricks, and Arcana for sharing these results.
For now, that's going to do it for today's AI Daily Brief.
Appreciate you listening or watching, as always, and until next time, peace.
