---
record_id: "podcast:7fbc3611-fa41-4187-a597-1975bf2e3636"
episode_id: 7fbc3611-fa41-4187-a597-1975bf2e3636
title: "Point-Counterpoint: Consumers Will Never Pay for AI"
podcast_title: "The AI Daily Brief: Artificial Intelligence News and Analysis"
url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/point-counterpoint-consumers-will-never-pay-for-ai/7fbc3611-fa41-4187-a597-1975bf2e3636"
audio_url: "https://pocketcasts.com/podcast/the-ai-daily-brief-artificial-intelligence-news-and-analysis/d41026a0-bb2a-013b-f3ee-0acc26574db2/point-counterpoint-consumers-will-never-pay-for-ai/7fbc3611-fa41-4187-a597-1975bf2e3636"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-06
played_at: "2026-10-06T12:00:00Z"
play_count: 1
duration_seconds: 1620
source: pocketcasts-history-browser
played_label: October 6
history_order: 9
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: d903463a68d37755cf20620835a6173abf302c6b566e6eaea5c30a83eece6584
analysis_mode: health
summary_source: local
model_source: local
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: Qwen3.8-Flash-Next-UD-Q4_K_XL
tagging_model: sonnet
proposed_tags: [primary-source-video, geopolitics]
proposed_entities: []
status: new
routed_to: null
---

## Summary

Reflection AI’s Beam launch dominated the headlines: a 501-billion-parameter U.S. open-weight model positioned against Chinese open models, with claimed scores of 44.4 on DeepSui versus GLM 5.2’s 44 and Quen38MAX’s 51, 80.1 on Terminal Bench 2.1 versus Nemotron Ultra’s 56.4 and Inkling’s 63.8, and 3–4x inference efficiency versus GLM 5.2; critics including Kyle Chan said it still trails GLM 5.3 and Kimmy K3, while Nathan Lambert and Shriram Krishnan welcomed the U.S. entry. The episode also covered a New York City Council existential-risk hearing featuring Jacob Coxon, Speaker Julie Menon, OpenAI, proposed kill-switch and whistleblower bills, and Governor Kathy Hochul’s data-center moratorium; researchers detected several thousand Tencent-infrastructure agents sending bulk requests to Alibaba’s AMAP, calling it an “agent fleet” rather than a coordinated swarm; Microsoft reportedly cut projected internal Claude spend by a third from about $1 billion, Meta cut Claude usage from about 60,000 employees to 30,000 while Metacode reached 30,000, and Anthropic’s IPO scrutiny focused on 2025 customer concentration—two customers at 25% of revenue—plus later claims of 6,000 customers above $100,000 and 100 above $10 million. A16Z’s seventh consumer AI top 100, using web, mobile, and Yippet revenue data, found only 11 debuts, revenue concentrated in build/create/work tools, ChatGPT still ahead of Gemini and Claude, Claude catching Gemini in paid U.S. subscribers but ChatGPT leading net new subscriptions in July and August, top 1% of AI spenders averaging $903 per month versus a $25 median and outspending the bottom 50% combined, and PNC data showing only 2.2% of U.S. households pay for AI; a KPMG/University of Texas at Austin study of 500+ early-career professionals also found “AI amplifiers” succeed by guiding, evaluating, and refining AI outputs.

Actionable takeaways: treat consumer AI monetization as a power-user and workflow problem, not a mass-subscription assumption—audit whether AI is being used for high-leverage tasks such as coding, automation, content creation, research, admin triage, or entertainment, because top spenders disproportionately pay for tools like Notion, Runway, Higgsfield, n8n, and agentic platforms; if usage is shallow, consider lower-cost tiers, embedded AI in existing apps, or non-subscription models such as usage-based pricing, entertainment monetization, or enterprise seats. For product, investment, or career decisions, watch Anthropic’s customer concentration, Microsoft/Meta in-house model substitution, whether Copilot growth offsets Claude cuts, and whether agent-fleet monitoring becomes part of security/resiliency infrastructure; follow-up questions include which AI tasks save enough time to justify more than $25 per month, which household use cases beat existing apps, whether NYC/state AI rules or data-center moratoriums affect vendors, and whether agent fleets are benign scraping or a real security risk. No direct health implications are stated, but if AI is used for medical, mental-health, or caregiving tasks, verify clinical validity, privacy, and human oversight before relying on it.

## Transcript

The latest consumer AI numbers are out in terms of which apps are used most on mobile, which websites are most visited, and which AI services have the highest revenue.
For many, the most interesting story is the wild dichotomies that exist in these numbers.
First, the gap between the top-paying users and the median-paying users, where the top 1% of AI buyers spend as much as the bottom 50% combined, but then also the incredible gap in households that buy any AI versus those that don't.
Today, we're exploring whether the 98% of U.S.
households that currently don't pay for an AI subscription represent a massive revenue opportunity to come, or the reality that they will never pay for an AI subscription and might need totally different types of AI products or at least AI business models to be even a little bit relevant for the big AI companies.
The AI Daily Brief is a daily podcast and video about the most important news and discussions in AI.
All right, friends, quick announcements before we dive in.
First of all, thank you to today's sponsors, KPMG, Harbor, Granola, and Blitzy.
To get an ad-free version of the show, go to patreon.com/slash AIDailybrief, or you can subscribe on Apple Podcasts.
And to learn more about sponsoring the show, send us a note at sponsors at AIDailyBrief.ai.
After our episode yesterday about the rumored forthcoming open weight model of American origins, Reflection AI did indeed unveil their new model and positioned it as the U.S.
trained challenger to the Chinese open models that have started to compete for token share.
Beam has 501 billion parameters.
That makes it around the same size as NVIDIA's Nemotron 3 Ultra, but smaller than GLM 5.3 and tiny compared to Kimmy K3's 2.8 trillion parameters.
At this stage, the model is only available to early testers, so we can only gauge it based on the reported benchmarks.
Reflection AI claimed a score of 44.4 on coding benchmark DeepSui, beating GLM 5.2 at 44 and slightly behind Quinn38MAX at 51.
On Terminal Bench 2.1, which measures agent accoding, Beam scored 80.1.
That put it well ahead of Nemotron Ultra at 56.4, Inkling at 63.8, but slightly behind GLM 5.2 and 6 points behind Quen38MAX.
Across the core set of benchmarks Reflection chose to showcase, it only led on SuiBench Verified, which didn't include scores from any of the Chinese models.
It was also notable that Reflection didn't benchmark on Terminal Bench 4.0, which has revealed a lot of benchmark maxing since it was released last month.
Reflection also chose not to compare their model to Chinese leaders like GLM5.3, Kimmy K3, and DeepSeek 4.1 Flash.
Now, on the plus side, Beam does look like it pushes the performance of Western open models.
Reflection also claimed that it will be extremely efficient, between three and four times more efficient in terms of inference compute compared to GLM5.2.
This could make Beam a very cost-effective base model for additional post-training, which is exactly the use case that we talked about becoming increasingly interesting to enterprises, and is very clearly a big part of Reflection's goal.
Reflection noted that the model was pre-trained from scratch, then put through what they believe to be the largest publicly documented reinforcement learning run ever.
They also utilized distributed infrastructure for their reinforcement learning, which is a wildly underexplored method of training open models.
Artificial analysis hasn't completed their independent testing at this stage, but they did give some directional confirmation of some of the claims, writing, Early indicators suggest Beam will be one of the most token-efficient open models we've seen for its level of intelligence.
Now, to sum, this all fell a bit short of the hype from earlier in the week, with Kyle Chan of the Brookings Institute writing, The real game changer would be an American open source model on par with the best Chinese models.
This is an impressive model, but still behind GLM5.3 and Kimmy K3.
On the other hand, despite this not being a DeepSeek or Kimmy killer, many were simply pleased to see a competitive model out of a new U.S.
lab.
Open model researcher Nathan Lambert wrote: Congrats to the Reflection folks.
It's hard to get the first model out, and we hope you can rapidly accelerate contributions to the ecosystem from here.
Added former White House advisor Shriram Krishnan, congrats to Reflection on the launch of Beam.
It is critical for the U.S.
to have leading open models to win the AI race.
I think it's interesting to think about what the reaction would have been if there hadn't been leaks and hype for the couple of days leading up to this.
My guess is that rather than a letdown that some felt, it would have been more like when your team is down by a couple of goals and you score the first one on their way to a comeback.
It doesn't mean that the comeback is fait accompli, but you're feeling a heck of a lot better than you did just a few minutes earlier.
Moving over to the latest in AI safety, a weird one as the New York City Council held a hearing on existential risk.
It featured testimony from several prominent figures in the AI safety movement, including former anthropic employee Jacob Coxon, who of course went viral a few weeks ago.
There was nothing particularly new in what was discussed, with the hearing largely serving as a canvas for various AI regulations being proposed in New York State.
Giving a sense of the position that these regulators are coming from, City Council Speaker Julie Mennon opened the hearing by saying, The idea that artificial intelligence is going to self-regulate defies all reason.
She said that New York bills could serve as a national model, with New York already having a fairly robust set of AI regulations, with tougher consumer protection set to kick in over the coming years.
Proposals for an AI kill switch and whistleblower protections are currently before the state Congress.
In addition, Governor Kathy Hochul has imposed a one-year moratorium on data center construction.
Completely predictably, during the hearing, Speaker Menon referenced Sam Altman's recent interview comments where he said that the world should, quote, accept some bad things happening for the benefits of this technology, and even tried to get in a little gotcha moment, asking the representatives from the AI companies to attach a probability to extinction risk.
None provided an actual number.
Meanwhile, OpenAI's proposals centered on addressing the current AI safety issues rather than the hypothetical danger of recursive self-improvement.
In a letter to the New York City Council, OpenAI offered to work more broadly with cyber defenders in the city and noted they're already working with the state.
Next up, a group of self-styled agent swarm chasers, which reminds me, of course, of the 90s classic Twister, have detected a group of agents using Tencent's AI infrastructure.
In a preliminary report published on Sunday, the group said that they detected several thousand agents that seemed to be sending bulk requests to Alibaba's map service, AMAP.
The researchers went out of their way to avoid using the term agent swarm.
They found no evidence that the agents were coordinating with each other, as we saw happening with OpenAI's agents during the Hugging Face incident.
Instead, they referred to the group as an agent fleet.
This could be the first sign of large-scale agent fleets emanating from Chinese servers, but agentic swarm chasing is a relatively new trend, so we could be just seeing the first documented chase.
It's also entirely unclear about whether anything nefarious is going on.
The agents seem to be merely sending bulk requests for information about local landmarks like parks, zoos, and hospitals.
At worst, it seems like the agents are circumventing Alibaba's API rules to conduct bulk data scraping.
What's cool, in my opinion, is the fact that this is a growing area of research, and even attracted a group of like-minded people to a hackathon last weekend.
Not only do I think that these types of research will be an inevitable part of our resiliency infrastructure, I also think that by doing this work and keeping track of it, it will help demystify these agent fleets or swarms or whatever you want to call them to help people understand what they're actually doing as they crawl the internet.
Over in Enterprise Competition Land, Microsoft and Meta have slashed their clawed spending.
The information reports that Microsoft has cut their projected clawed bill by a third.
Sources said that Microsoft was on track to spend a billion dollars on internal claw use earlier this year.
Programmers have been asked to ration their use as a cost-saving measure as well as switching to Microsoft's in-house models.
The reporting notes that this figure is internal use only and doesn't include spending for Microsoft's customers.
Microsoft was forecasting $2 billion in Anthropic spend to power Copilot features earlier in the year, and that forecast hasn't changed.
Microsoft has substituted their in-house models and OpenAI's GPT-5.6 for many queries, but sources said that Copilot customer growth has offset the effects of switching away from Claude.
At Meta, meanwhile, sources said that Claude usage has been cut in half, but dramatically rained in usage during the spring.
Sources said that around 60,000 of Meta's then 78,000 employees were using Claude code at the peak, but following 10% layoffs and the in-house model releases, user numbers are down to 30,000.
That drop-off is almost completely mirrored in adoption of their new in-house tool, Metacode, which now also has 30,000 users.
Meta was reportedly on pace to spend several billion with Anthropic as of June, but they're now spending around $105 million per month.
Now, obviously, the reason the story is in the news is Anthropic's upcoming IPO.
The closer it gets, the more that Wall Street is digging in to understand what's under the hood.
We've had numerous leaks from Anthropic's financial disclosures, but mostly related to 2025 numbers, most of which have what we'll call limited relevance for where the company is today.
Still, one disclosure that people did take note of was that just two customers accounted for a quarter of Anthropic's revenue in 2025.
Speculation had suggested that the two were some combination of Meta, Microsoft, and Cursor.
Anthropic has told investors that this extreme customer concentration has expanded since then and they now have 6,000 customers with annual bills above $100,000.
Still, given that they only have 100 customers spending over 10 million annually, any belt tightening at the top could be material.
I certainly think it would be an incorrect reading of this to view Microsoft and Meta as broadly reflective of the rest of the business world, specifically because they are competing labs that have only been begrudgingly using Anthropic models because of just how much better those models were than what they had in-house.
The more that that gap closes, or at least the more that the floor level of those in-house models improves, the more those companies can justify these shifts.
That won't necessarily be the case with the average customer.
More broadly, I think that there are two very different ways to look at customer concentration for AI.
One, you can view it exclusively in risk terms, where just a handful of customers significantly cutting their spend could materially change the revenue dynamics.
The other way to look at it is, of course, that those are early adopters, and that that concentration actually shows quite a bit of growth potential across the rest of enterprise buyers.
As almost any time we're presented with a binary in life, I think it's probably a little bit of both.
But that's certainly where a lot of the debate is going to be on Wall Street in advance of this IPO.
I'm sure there will be much more to discuss on that front, but for now, that is going to do it for today's headlines.
Next up, the main episode.
A new study from KPMG and the University of Texas at Austin found that when people work with AI, similar skills don't guarantee similar outcomes.
Researchers studied more than 500 early career professionals and found that the best performers consistently amplified the value of AI by guiding, evaluating, and refining its outputs.
These top performers, called AI amplifiers, weren't defined by what they knew alone, but by how they worked with AI.
Learn more about what separates AI amplifiers from everyone else at kpmg.com/slash uslash AI amplifiers.
Every episode, I talk about the competition between OpenAI, Anthropic, SpaceX AI, Google, and Meta.
And if you've been listening for a while, you might have a favorite.
Maybe you think OpenAI and Anthropic can stay ahead, or perhaps Meta's open source strategy can win out.
Whatever your view, every AI lab creates a different investment opportunity.
Harbor Capital Advisors AI Lab Ecosystem ETF suite lets you invest in the ecosystem behind the AI lab you believe in.
Search Harbor AI Lab Ecosystem ETFs wherever you invest or follow at Harbor Capital on X to learn more.
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
Blitzy deeply understands your code base before it writes code.
Here's the first place that pays off: security in the age of AI.
Vulnerabilities don't live in isolation.
They live buried inside millions of lines of interconnected code where patching one thing quietly breaks three others.
That's why surface-level scans fail.
Blitzy starts from its knowledge graph of your entire application, identifies and surfaces CVEs across the full estate, proactively recommends patches, and can execute the PR.
Each fix is grounded in how your systems connect and validate, so nothing new breaks.
And the knowledge graph dynamically updates, keeping you ahead of an ever-accelerating threat landscape.
One Blitzy customer resolved 21 active CVEs across six core microservices in four days.
Zero compile errors, every validation scan clean, months of planned work fixed in less than a week.
Security remediation grounded in real architectural context at the speed of compute.
Harden your code base at blitzy.com.
That's B-L-I-T-Z-Y.com.
Welcome back to the AI Daily Brief.
Today we are looking at a fairly fascinating conversation about not only what the most popular consumer AI apps are and what the categories say about different types of AI usage, but we're also exploring the question of whether consumers will ever spend significant money on artificial intelligence.
And of course, if the answer is no, what does that mean for the AI market?
The inspiration and starting point for this comes from Andreessen Horowitz, who has just released the seventh edition of their top 100 consumer AI apps.
One part of this information comes from consumer traffic data.
This is the most comparable data across all seven instances of this.
The top 100 then is divided by top 50 by unique monthly visits on the web and top 50 by monthly active users on mobile.
But then for the first time this round, A16Z also used data from Yippet to publish a top 50 consumer AI apps by monthly revenue.
And in many cases, the story is quite different.
Now, before we get into the community's reaction, there were a few big takeaways that the team at A16Z had.
The first is that they found this edition had the smallest number of debuts across their seven lists so far.
In other words, the smallest number of companies that weren't on previous lists that are on the list now.
Just 11 products made their first ever appearance here.
There are a few different ways to interpret this, but one reasonable take, I think, is that we are at least inching towards some sort of consolidation phase where instead of it just being a thousand flowers blooming, we're actually starting to see some patterns and network effects take hold within certain categories.
The team at A16Z also noted a couple key trends in usage.
Perhaps unsurprisingly, they argue that consumer AI's first real market is people who pay for tools that help them build, create, and get work done.
In other words, while there might be some fun, playful, companion-style AI showing up on the mobile or the web app charts, the majority of the platforms that are on the chart organized by revenue are for people who are using those tools in their professional life in some way.
Now, focusing on the top of the charts, the study authors talk about what they see among the leading LLMs ChatGPT, Gemini, and Claude.
Overall, their positions relative to one another have stayed fairly consistent.
Again, this is among consumers.
Although over the course of 2026, Claude caught up to Gemini in terms of paid US subscribers, although both remain pretty far behind ChatGPT.
They also found that Claude does a better job of converting users to higher-cost subscriptions.
For a big chunk of this year, Claude had started to lead ChatGPT in net new subscriptions, but that's flipped once again in the past couple of months, with ChatGPT significantly outperforming Claude in net new subscriptions in the months of July and August.
And as those big leaders consolidate their position, A16Z also explored where startups still have an advantage.
They wrote, Among the startups attracting durable attention, a few themes stand out.
One is to actually own a differentiated model, with the clearest examples being the creative products like music generation platform Suno and voice generation platform 11 Labs.
Another way to stand out from the incumbents is to own a multi-model experience, with examples being Cursor, which supports models from several labs, although we'll see how that changes as they get absorbed more into SpaceX, and OpenRouter, which is of course specifically built to give developers access to multiple providers from one platform.
A third way that startups are differentiating is an extreme focus on some audience with a specific need.
The examples they give are Open Evidence, which serves physicians, and Venice, which is aimed at privacy-focused users.
Now, in terms of the community's reaction, one frequent response was to be surprised, to either not have known that something was as popular as it was, or to actually have just never heard of it as all.
Peter James sums this up when he writes: There are so many surprises here to meet.
Superhuman at number four, Suno at number seven, OpenArt above Notion and Figma.
Also, WTF is Plod.
I'm absolutely bamboozled.
I think a lot of people will have this type of response.
We all get in different bubbles where entire categories of usage might evade our notice.
Plod is a great example, where I have followed it from the standpoint of following everything for this show, but hadn't really come across it in public.
And yet, when I had an interior designer at my house this week, they pulled one out and used it because the walk around the house form factor for taking notes made more sense for the way that they work in the real world.
In terms of Suno at number seven on the monthly revenue charts, as I've discussed before with Suno, one thing that people do not realize is that while many would have assumed that the main paid users of Suno are professional or aspiring professional musicians, a huge amount of the usage is actually entertainment.
People making fun, ridiculous songs for their family and friends, and having enough fun that they're actually willing to put some money behind that.
Another thing that people noticed is that many of the big themes, such as the ones we've been talking about on this show, are showing up on these charts.
Agentic coding platforms like Replit and Lovable remain near the top of the revenue charts.
Open router being at 13 even on a consumer chart does seem to give indication of how much people are looking for cost optimization.
And seeing platforms like Noose, Genspark, and Manus all on the charts reinforces the growing competition around personal AI assistance.
Another common theme in the discourse is surprise at the stickiness of certain experiences.
Perplexity, for example, hasn't been a major topic of conversation in the super-enfranchised AI world for some time.
And yet there it sits, number 12 on the unique monthly visits chart, number 25 on the monthly active users chart, and all the way up to number nine on the monthly revenue chart.
N8N, which is in many ways a precursor to the agentic era, remains on the revenue charts as well, perhaps showing the relative slowness of behavior change once people have invested in using a particular type of platform, especially if they took the work to automate some key workflow.
And yet, if there was one major conversation, it was about the difference between power users and everyone else.
One of the things that A16Z showed was that the top 1% of AI spenders now outspend the bottom 50% combined.
The top 1% spend an average of $903 a month compared to the median customer who spends just 25%.
And remember, that's not the top 1% of all AI users.
That's just the top 1% of people who are actually spending, which itself, as we'll see, is a vanishingly small portion of AI users overall.
One of the most interesting charts to me is the chart that shows what things those 1% spend money on in higher proportion to other paid AI users.
It's basically tools that allow them to build and automate, tools that allow them to create content, and tools that you would use for work.
Their purchase rate for Notion is over nine times as much as the average.
Their purchase rate for video platforms like Runway and Higgsfield is 10 times and 15 times as much as the average, respectively.
And there again is N8N, where the top 1% are basically 23 times as likely to be paying for that service as compared to all other buyers.
Now, many people compared that chart about the concentration of the top 1% of AI buyers with this chart from another A16Z research piece, their state of markets report.
This chart is about the share of U.S.
households with paid AI subscriptions.
And TLDR, as of April of this year, according to PNC research, that number is only 2.2%.
In other words, 98% of U.S.
households aren't paying for AI currently.
The big question, of course, is whether that is 98% of U.S.
households aren't paying for AI yet, or 98% of U.S.
households aren't going to ever pay for AI.
To some, this is obviously all opportunity.
Adam at Repview writes, I think this is just a reflection on early adoption and how much TAM there actually is as mass market adoption proliferates.
Ruben Hasid pointed out that the time it took to go from 2% to 50% adoption in the US for the computer was 19 years, for cars was 15 years, for the smartphone was 6.5 years.
In other words, implying that we're just early.
Some others compared it to what other things people pay for.
Co-founders Nick points to 25% of households paying for SiriusXM, 55% paying for cloud storage, and 91% paying for at least one streaming service.
Some were ultimately optimistic, but even more assertive about how early we are.
Microsoft's Nicolas Bustamante writes, This is my thesis.
No one uses AI.
I repeat, absolutely no one.
We live in a bubble.
Even among my friends who pay for it, when I ask them to open ChatGPT and show me their queries, it's the same handful of basic things.
Most don't even know they can upload a photo and ask questions about it.
Connecting Gmail so an agent can read and send emails blows their minds.
An agent opening a browser and checking them into a flight, they've never even heard of it.
The massive challenge right now is adoption, and then getting people who already signed up to actually use what they're paying for.
Most have absolutely zero clue what's possible.
Imagine the compute shortage when everyone starts using AI like the top 1% of users do today.
Others, though, said, never gonna happen.
Lawyer Basil Musharbash reposted Nicholas and said, I'm a competent adult.
Why do I need an AI agent to check into a flight for me?
I'm literate.
Why do I need an AI agent to read and write emails for me?
The reason no one uses AI is that there's no serious utility here for the vast majority of people.
Habibi Slop also didn't like the flight booking example.
They wrote, Here's why doubling down on this flight booking thing is dumb as rocks.
One, I don't think it has ever taken me 20 minutes to check into a flight.
The steps you're describing removing are not even real steps.
They are usually open the airline's app, click the big red check-in button, click number of check bags, done.
You'd have to do the same amount of work to check if the agent actually succeeded at its task.
Two, about 55% of American adults take zero flights in a given year.
So few people care about this use case.
People underestimate AI agents is not what's happening here.
What's happening is tech people routinely mistake their own unusually high travel, high email, high admin lifestyle for a universal human workload.
The overarching problem of the tech industry the last 20 years is their inability to look outside themselves.
They become obsessed with marketing solutions to problems that nobody else has.
Some are even more pessimistic about the average US consumer, with Breaking Points hosts Cigar and Jetty writing, nobody actually needs a personal AI assistant.
The average screen time in the US is seven hours a day.
People have plenty of time.
There's no evidence that freeing up more will lead to anything but more TikTok scrolling.
If anything, daily life needs more offline friction.
I'll spend it doing what I love.
No, you won't.
You'll watch TikTok.
The data doesn't lie.
But then again, on the flip side, and this is why I called this episode a point counterpoint.
You have folks lamenting what an utter failure of imagination this represents.
Reposting lawyer Basil Musharbash, who said that they don't need an AI agent to check into flights or read or write emails for them, investor Nick Carter says, I find these takes really confusing.
You have 150 IQ plus tireless genius living in your computer.
It can use your browser and read your email and access any file you want.
It won't complain if you give it the most tedious administrative tasks.
It's willing to work 24-7 for less than minimum wage.
It can work unsupervised for hours at a time.
And you can't think of any way to put it to use?
Are you completely lacking in imagination, or do you just enjoy mundane administrative tasks?
You enjoy paying parking tickets and triaging emails and manually unsubscribing from spam and vetting credit card payments and canceling subscriptions and renegotiating insurance?
You like doing that?
For some, this split between different types of users is as close to a law of nature as we have in tech.
Personally, I bristle at the idea that everyone is too lazy and slackjawed to get off TikTok to actually take advantage of these tools, even if productivity isn't their primary motivation in life.
And at the same time, it is certainly the case that the vast majority of people that I see interacting with AI in assertive and positive ways are basically go-getter types.
They're people who want more out of life and more out of their jobs and careers and work.
They're not necessarily all entrepreneurs, but they bring entrepreneurial energy to the things that they do.
They are, in short, high aspiration.
And not everyone is.
Now, there are two reasons that even if we accept the idea that there might always be limits on how much the average consumer wants to use AI or specifically wants to pay for it, there are a couple of reasons that that doesn't necessarily undermine the financial thesis of the industry.
The first is, of course, that unlike previous categories of software, there is far less of an upper bound on how much those aspiring type individuals and the companies they work with can actually spend on AI.
This is not SaaS where the upper bound is the most premium account that costs $100 or $200 a month.
This is a domain in which power users can spend thousands and thousands or tens of thousands of dollars per month in a totally ROI positive sort of way.
But keeping it on the consumer focus, there's nothing that says that consumer AI apps have to be all about productivity or that they have to monetize strictly through subscriptions.
I'll point to Suno again, where the success in the hundreds of millions of dollars of ARR that company has now achieved is not exclusively as a productivity tool for musicians, but as an entertainment platform for a lot of normies as well.
And then, of course, there is that alternate business model, the one which we love to hate, but which funds most of the internet at this point, advertising.
Right on time, OpenAI just announced a new ad format where they'll be displaying visual ads inline in ChatGPT, not just text-based ads.
They wrote, Our new visual ad format helps people imagine how products and services could fit into their lives.
Through images showing product inspiration, product usage, or the experiences they make possible, people can discover a new brand, understand what makes an offer distinctive, and decide what to buy.
For advertisers, this creates new opportunities to tell their story through images.
Now, also in that announcement, they reiterated a number that I had heard during Dev Day as well, which is that ChatGPT now reaches 1.2 billion people each week, up 20% since they announced their billion user milestone at the end of July.
Alex Immerman points out that there is a lot of room to run here.
He wrote, ChatGPT launched ads in February, crossed 100 million run rate revenue in six weeks, and a billion by August.
Google and Meta combine for $500 billion in ad revenue.
We are so early in AI ads.
For one who is trying to understand the future of consumer AI, maybe the most interesting chart from the A16Z report is this one, where consumer AI has room to grow.
On the left, they have categories.
In the middle, the winners from Web 1.0 and Web 2.0.
And then on the right, whether that particular category has AI companies in the top 100 of consumer apps.
They are highly concentrated within productivity tools, search and answers, production and creation, photos and videos, with a little bit of education and health.
Where there are no AI platforms in the top 100 include categories like streaming and media platforms, retail marketplaces, social networks and messaging, travel, personal finance, jobs and career networks, real estate, gaming, and dating.
I do think it is sometimes too easy for early adopter types to say, we're so early when they look at underwhelming adoption numbers.
But I certainly do think that when it comes to consumer AI, it would be a mistake to assume that where we are today is where we will be a couple years down the line.
For now, that's going to do it for today's AI Daily Brief.
Appreciate you listening or watching.
As always, until next time, peace.
