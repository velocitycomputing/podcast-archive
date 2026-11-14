---
record_id: "podcast:c09c78a8-b304-49ad-8e69-b9dc43f80ffc"
episode_id: c09c78a8-b304-49ad-8e69-b9dc43f80ffc
title: Inside Anthropic’s trillion-dollar AI gamble
podcast_title: Decoder with Nilay Patel
url: "https://pocketcasts.com/podcast/decoder-with-nilay-patel/01a33f10-fcfe-0132-18b7-059c869cc4eb/inside-anthropics-trillion-dollar-ai-gamble/c09c78a8-b304-49ad-8e69-b9dc43f80ffc"
audio_url: "https://pocketcasts.com/podcast/decoder-with-nilay-patel/01a33f10-fcfe-0132-18b7-059c869cc4eb/inside-anthropics-trillion-dollar-ai-gamble/c09c78a8-b304-49ad-8e69-b9dc43f80ffc"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-29
played_at: "2026-10-29T12:00:00Z"
play_count: 1
duration_seconds: 2940
source: pocketcasts-history-browser
played_label: October 29
history_order: 28
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 840cefcd45f143efd3a482e74a3d4068d2ae203e2752e6d8c105c617a8774c5b
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

Joey Brookhart of SemiAnalysis and Neil Patel examined Anthropic’s S1 filing for a potential NASDAQ IPO that could begin trading as soon as next month at a $1.5–$2 trillion valuation, arguing the document shows a capital-efficient frontier-AI business with more than $70 billion ARR, positive 85% inference gross margins versus negative 94% two years earlier, about $65 million revenue per inference megawatt—up from mid-teens last year and potentially $100–$120 million on Blackwell—roughly $10 million per megawatt compute COGS, only about 30% of compute serving inference, and 80% of recent revenue from models released in the prior six months. They discussed Anthropic’s dependence on coding revenue, the narrowness of the market, with the top 1% of customers spending $50,000–$100,000 per employee, and the need to expand into cyber, legal, financial services, bio, and broader white-collar labor replacement to support Dario’s trillion-dollar revenue vision. They also weighed competition from OpenAI, Google DeepMind, Meta, SpaceX, and open-weight/open-source models, which SemiAnalysis estimated grew from about $1 billion ARR in Q1 to more than $10 billion in Q3, while Anthropic captured about 90% of industry net-new ARR in the first half before OpenAI likely took the majority in Q3. Key risks and claims included enterprise data-retention concerns tied to a Fable release, the need to stay at the frontier for adversarial tasks, $80 billion non-cash charges from warrants and convertible notes tied to rising valuation, $10 billion cash burn, $120 billion-plus cash and marketable securities, possible post-IPO proceeds of another $100 billion, and large compute commitments to Amazon/AWS, Google, SpaceX, and neoclouds—headline figures of $500–$600 billion over seven to ten years, or $800 billion-plus over ten years—interpreted by Brookhart as manageable if revenue scales toward 20 gigawatts and beyond, though dilution and financing remain watchpoints. Sponsor segments also cited Comcast Business detecting 24.5 billion phishing attempts in 12 months, CrowdStrike’s AI Detection and Response, and Engine’s travel infrastructure for 40,000 businesses and 2 million travelers.

For the user, the practical takeaway is to treat Anthropic’s IPO numbers as a test of frontier-AI unit economics rather than a guarantee of durable enterprise demand: track quarterly ARR by product and vertical, inference gross margin, revenue per megawatt, compute cost per megawatt, training-versus-inference compute allocation, and the share of revenue from models less than six months old. Decisions to consider include whether to standardize on frontier models for high-stakes coding, cyber, legal, financial, or research work while using cheaper or open-weight models for low-risk tasks; demand zero-data-retention, on-prem, or private deployment options before sending sensitive data; and require vendors to disclose model deprecation, switching costs, and security controls for AI agents. Research leads include Anthropic’s S1 risk factors, compute commitments, customer concentration, enterprise adoption outside coding, OpenAI’s Q3 net-new ARR, open-source ARR growth, and cybersecurity incidents driving enterprise AI budgets; follow-up questions should ask whether frontier capability is actually needed for a given workflow, whether model improvements are translating into labor savings or only augmentation, and whether the company can fund trillions in compute without dilution or financing stress. No direct health implications appear in the supplied material.

## Transcript

Support for the show comes from Comcast Business.
With advances in AI, cybersecurity is getting more powerful, but so are attacks.
In the past 12 months, Comcast Business detected 24.5 billion phishing attempts designed to exploit user behavior, steal credentials, and compromise devices.
AI is forcing a shift in how organizations defend themselves, demanding not only faster responses, but continuous intelligence.
To survive in the current climate, leaders must build a security-first culture to equip their team with the tools they need to stay protected.
With Comcast Business, connectivity, intelligence, and response work as one orchestrated system.
Get better equipped to handle today's cyber threat landscape with the 2026 Comcast Business Cybersecurity Threat Report.
Read it today at ComcastBusiness.com/slash cybersecurity.
Cyber confidence starts with Comcast Business.
Support for the show comes from Engine.
Travel tech from the 80s got us this far, but it's about time someone rebuilt it for the modern era.
That's what Engine has done over the past eight years: building strong hotel partnerships, proprietary supply, real-time rate shopping, and payment rails.
That kind of infrastructure work simply can't be bought.
Today, that foundation runs travel for nearly 40,000 businesses and 2 million travelers, and it's growing 60% a year.
Intelligent travel.
The future of business travel runs on Engine.
Learn more at engine.com/slash decoder.
Support for the show comes from CrowdStrike.
It's not a huge stretch to say that AI is the next major computing platform.
Every platform shift changes the way we build software, and it changes security too.
CrowdStrike is defining cybersecurity in the AI era with AI Detection and Response, or AIDR, a solution for seeing, monitoring, and securing AI across the enterprise.
Learn more about how leading companies are turning to CrowdStrike to secure AI and secure their business at crowdstrike.com slash decoder.
Hello, and welcome to Decoder.
I'm Neil Patel, editor-in-chief of The Verge, and Decoder is my show about big ideas and other problems.
Today I'm joined by Joey Brookhart, an analyst at the chip and AI research firm Semi-Analysis.
To help me dig into the story inside the numbers of the Anthropic IPO filing, a document known as an S1.
Anthropic just filed its S1 to go public on the NASDAQ Stock Exchange, and it could start trading as soon as next month at a valuation of anywhere between $1.5 to $2 trillion, immediately making it one of the most valuable companies on the planet.
But the price tag really isn't the whole story here.
The S1 published earlier this week is hundreds upon hundreds of pages filled with details that finally paint a picture of the economics of a frontier AI lab.
And as you might imagine, that picture is both really complicated and built on a series of very, very ambitious assumptions about the future and what AI will do to it.
So I wanted to Joey on the show to help break down what this document really tells us, both about Anthropic's finances and the broader AI economy.
Joey and his colleagues at Semi Analysis actually built a model of Anthropic's finances from the outside back in July.
So he's been waiting for the S1 about as eagerly as anyone.
And I was excited to hear his take on what we've learned and importantly, what we still don't know.
Before we get going, do me a favor and subscribe to Decoder on YouTube, where we put out new episodes every Monday and Thursday.
Okay, SemiAnalysis, Joey Brickhart on the Anthropic S1 and the costs and risks of building Frontier AI.
Here we go.
Joey Brookhart, you're an analyst at SemiAnalysis.
You're also co-lead the tokenomics model, which is going to come up a lot in this episode.
Welcome to Decoder.
Yeah, thanks so much, Neil.
I am very excited to talk to you.
We're talking just a couple of days after the big Anthropic S1 was filed.
It's our first look inside of the finances of one of the leading Frontier models.
What's your take?
What's your reading to it?
It was an awesome S1.
I think, you know, it's been a rough three weeks since the Investor Day.
I think, you know, some people were somewhat disappointed in the September ARR numbers.
But what we saw here was a company that has capitally efficiently scaled to an amazing level, trillion plus valuation, you know, 70 billion plus of ARR in a very short amount of time.
And gross margins, compute margins, free cash flow, everything is what you'd want to see.
So I don't think there was much to nitpick in this filing.
And it's the reason you've seen the last two days.
I think a lot of the semiconductor complex and NeoClouds and compute stocks really rally again.
I'm actually, it's funny.
I don't think I can nitpick the S1 itself.
I want to get into some of the details because there's a lot of numbers in there that are worth thinking about.
I actually just want to start a really big picture.
I look at Anthropic and where it could go.
I look at Dario saying that he can see his way to a trillion dollars in revenue.
Where does that money come from?
Because so much of these businesses are about eating every other business.
And it feels like somewhere, someone else has to make some money to pay Anthropic to generate these revenues.
And I haven't actually seen that laid out very clearly.
It's so interesting, I think, today, because even though the scale are at, you know, 120 billion of ARR between the two leading labs, it's still an extremely narrow market.
The top 1% of customers are the one that are spending $100,000, $50,000 per employee.
Your broader Fortune 500, Global 2000, who typically has a lot of IT spend, isn't spending much.
And then two, a lot of the spending, especially at Anthropic, is coding specific.
So we're kind of in, you know, it's almost a single vertical company.
And then we look in the future into 27, you know, you think of just this broader adoption and white-collar work, this, you know, typical enterprise Q4 budgeting season.
We actually haven't gone through with, you know, one of these labs yet in any meaningful way because ARR did really start to accelerate till the beginning of the year.
We think of other cases like cyber, where that can be similar to coding, where these are eight-figure plus contracts with leading enterprises that can scale very quickly due to all the cybersecurity incidents we're seeing.
And then I think you get to other verticals like Bio, and then to get to a trillion, I think we do have to move some of that white-collar work and where it's more of AI's augmentation to labor-saving or replacement in some areas.
And I think you look at things like Microsoft's offerings to employees as maybe down the line at some point.
But there's no wealth of other verticals that they can get into and really start to move the needle.
This to me is the single biggest question I have, not just about the S1, but the entire industry.
I would understand that if there are one or two leading labs, right?
There's two big companies.
They've got a technology that can automate a whole bunch of things.
We will see how well that automation goes sector by sector.
But there's not just two leading labs.
There's quite a few of them.
There's open weight models.
I've heard from a lot of CEOs who are very nervous about giving all their data to an open AI or Anthropic, and they would like to run some things on-prem.
There's like law firms running on-prem AI now, which is just the funniest turn in maybe all of history.
How do you see that playing out?
Because so much of the pressure on this S1 was the numbers inside themselves, which I want to talk about.
But then there's the external pressure of, well, you've got to grow.
And growth is not assured.
So how do you see all of that playing out?
When we look at like coding today, for example, and I think we saw this in Q3 with OpenAI kind of catching up, there's areas of coding where there's very low switching costs.
And, you know, I can just move between that.
I think what we hear from enterprises and maybe too on the open weight side, like obviously, I think they somewhat botched the Fable release and why we saw some of the slowdown because of the zero data retention or lack of zero data retention.
And is that something they can fix with Fable 5.5 and maybe drive more enterprise adoption there?
I think that's a huge thing for enterprises when we talk with them.
We definitely see enterprises now, and more so to a lot of the AI natives, custom training, post-training on open weight models and then running either their inference off of that or even their products for internal or external use cases.
So there's that.
And then obviously, DeepMind at Google and MSL, with Meta, are very well-funded labs that have pretty similar training compute capacity.
And they're bringing on a ton of, and not even to mention SpaceX as well, with what Elon said on how much 10 net new gigawatts next year and half of that kind of as the long-term internal use case.
I think in the first half of the year, Anthropic ran away with it.
They were 90% of the industry's net new ARR.
And then we saw in Q3, OpenAI was probably actually the majority of industry net new ARR.
And then open source has grown from probably a billion-dollar ARR in Q1 to 10 billion plus here in Q3.
So yes, the industry's gotten much more competitive, but I think all these new use cases too, and some of these verticalized use cases are really where we're going to see the growth going forward because it's obvious coding isn't going to power us to even triple from here.
It's interesting.
The concept is called Tokenomics.
You run that practice alongside a co-lead at Sevi Analysis.
Explain what it is, because to me, it's such a smart way of thinking about, okay, we're going to put some money in, and maybe we'll get some money out.
I think of it as like the unit economics, or even just the broader everything from a macro to microeconomics of running an AI business or even looking at AI demand.
So, we cover the hyperscalers, you know, now some of the neo-clouds as well, and kind of a separate product, but then two, just the AI labs.
And I think for investors or just people that are interested in the business, it's you know, Anthropic had negative 94% gross margins on inference two years ago.
Now they have positive 85%, and people didn't understand kind of you know, how do they allocate compute?
What are actually, you know, how do we think about the inference business model?
I think, you know, part of that gross margin conversation is the revenue per megawatt in inference.
And why are all companies that are running inference seeing massive gains inference and compute efficiency?
So we try to model out these businesses.
And obviously, when Anthropic was private, we're dealing with information we can get from the press and things like that.
But now that we have numbers or concrete audited numbers, it's easy to explain the unit economics of this and to how the businesses differ.
OpenAI is a much different business than Anthropic, just in both their consumption versus subscription and then historical weight versus consumer versus enterprise.
So trying to understand across the demand level the economics of these businesses.
Several years ago, when I talked to Sundarbashai about the cost of inference, I said, How are you ever going to make money?
He was just very clear.
He's like, if there's one thing Google's good at, it's bringing this stuff down the cost curve.
And it was a very blunt answer.
And I understand how Google can do it.
They make their own chips.
Anthropic is running on everyone else's clouds, right?
I mean, this is like the core part of the S1 is how much they've committed to spend on other people's clouds, SpaceX, Google, Amazon.
Where does their efficiency come from?
Really, token throughput, and I think they have a very diverse chip fleet.
So, between training's TPUs, and GPUs, across all of those, we hear a ton of token efficiencies.
So, I think like token throughput, for example, on training chips are up five to 10x year over year right now.
So, dealing with both the hardware-level efficiencies and the software, how the model interacts with the hardware, there's a lot of token throughput gains where if you're doing X tokens per second, now you're doing 5x, 10x just a year later.
And I think what they'll tell you is they see continued compute efficiencies as well going forward.
So, we've even published some research.
So, Max, who co-leads Tokenomics model, right now, if Anthropic's at 65 million of revenue per inference megawatt, this was mid-teens last year at this time.
And I think what we've said on maybe Opus 5.5 on a Blackwell, you can get to 100 to 120 million of revenue per megawatt.
But the big thing here is they're paying on average now just a little over 10 per megawatt in COGS or just in compute costs.
So, what you can do with those sort of margins and then reinvest in training, people don't realize this, but only about 30% of the compute is actually in inference, serving revenue.
The rest is being for experimentation and research, training models.
So, there's a lot of compute that is building the next model.
And that's more of like the RD side and where you actually get your returns and defensibility in this business.
Actually, what I was expecting to see in the S1 was that dynamic play out much more strongly.
That Anthropic makes a bunch of money selling the models they have now, and there are more customers in the future for the models they have now.
That's going to throw off a whole bunch of margin.
And then, because they're Anthropic and they think they're building digital God, they're going to train the next models as much as they can.
And that is like a very particular Anthropic story.
They are chasing AGI.
They will happily tell you that in the S1, that Claude might be conscious, and this could all go to hell.
Like, Anthropic is a very unique company in its conception of itself, but you don't really see that dynamic playing out in the S1, right?
They are managing their training costs against their inference margin pretty well.
Do you see that going up or changing in any way?
I agree.
I think long-term, and we've even said this internally, they want to increase actually the percentage of training if you believe you're building digital God or going towards HEI.
And as long as you have the margins, gross margins, 85% plus on inference to do so, you can.
I think they've grown faster, you know, obviously a lot faster than they thought.
And they didn't expect to be at 11% non-GAP EBIT margins.
I think they'd love to be closer to zero or even below that if they could get that compute and allocate it towards training and continue to see these compute efficiencies.
And I think they've messaged that too to investors in the roadshow that, hey, you can look at this S1 and just the curve of profitability over the last few years and how little cash they burned to get to this point.
And you can say, you know, hey, this is a good business model, but we're going towards HEI.
Don't expect these margin, you know, the margin leverage we're seeing to continue to this level, even though we can, you know, long-term margins can be, you know, quite a bit higher.
There's some real shades of Amazon in there.
Jeff Bezos famously telling investors he wasn't going to make money until he could make a lot of money.
Obviously, Amazon and Anthropic have a lot of back and forth.
Maybe there's some family resemblance there.
But I'm curious, there's a point of model capability that would allow you to go into more verticals than just coding, right?
We might be at it now, right?
The idea of capability overhang exists.
The idea that the models we have today could go and take over bio research.
They're taking over mathematics today.
Like, there's a point at which the smartest business decision is to stop training and to just sell your profitable model into more and more companies.
Anthropic as a public company will face that pressure.
Do you think they're organized or structured to fend it off?
Yeah, I think they're structured.
Well, I think with some of the voting stock and areas like that, they definitely are.
We've seen this in tech before and even like, you know, publicly, you know, when Zuckerberg has made these decisions before to invest heavily.
I just want to point out, didn't always pay off.
Yeah, did not always pay off.
But you and I technically are in the metaverse right now.
Yeah.
And that's some definition.
Right.
But I think that's something.
And there's an interesting number in the S1 that 80% of revenue in the last six or last three months comes from models released in the last six months.
So then you say, okay, 20% of the models are like Opus 4.5 in earlier versions.
I think one thing going forward is you always need to be, if you're a frontier model company, you always need to be at the frontier.
Wait, can I ask a really dumb question about that?
Yeah.
Why?
Like, this is, I think, the heart of my sort of curiosity about the industry right now is if you enabled some bleeding-edge technology that could revolutionize the entire world, at some point, the most profitable thing to do is to just go play it out in all the different verticals, right?
And it's not to go make the next one.
And it's to actually run an efficient model in legal services and medicine and wherever else that there hasn't been diffusion of AI yet.
And so this idea that you always have to be at the frontier, that Anthropic always has to be competing with Google and OpenAI and whoever else, I get it right from their self-conception.
But from a business point of view, an AI-enabled business is going to throw off more money and spend more money with me, the AI provider.
And that isn't necessarily related to being at the frontier.
Yeah, I think there's a few portions of that.
You know, four new verticals, and this is like very cyber-specific.
If an adversary is using a frontier model, you need to be defending with a frontier model.
You know, things like, you know, when we talk to like some enterprises, you know, it's not like email summary where I can run that on open source or Sonnet.
Like there are just certain verticals where having, you know, I mean, if you were in a legal case as a defendant, would you want your lawyer using a non-Frontier model if the prosecution was.
I don't know if you're getting news for you about what's going on in the legal market right now.
Yeah.
So, you know, that's there are certain areas, yes, that are more, you know, the competitive dynamics do dictate that.
And I, you know, I think from a go-forward perspective, we've seen this with like open source too catching up.
The demand will be there.
I think Dylan says this a lot, like the demand will always be there for frontier intelligence, especially in competitive industries.
And there are certain tasks, I think, as you go towards more labor replacement versus labor augmentation where that also is the case.
You know, at the same time, they are getting more vertical.
If you go look at like job postings or what they're hiring for, you know, putting out more of these SKUs and areas.
And there's a lot of beta testing going on, like Cloud for Financial Services, Cloud for Legal.
Their cyber program, they're giving away 250 or sorry, 25K of credits per month for people in their cyber program.
So that'll be a huge skew for them in 27.
Those verticalized areas and then ones that are specifically where you need to be, you know, it's more adversarial, I should say, or competitive, are kind of the main reasons why.
But I think we can both agree there's areas like email summary and work that definitely doesn't need to happen.
Support for the show comes from Engine.
When $1.6 trillion moves through travel every year, it's a shock to remember that most of it still runs on tech from the 80s.
I mean, work travel works fine, but it certainly isn't all that intelligent.
That's why businesses and travelers book directly through Engine.
Engine closes the gap between wanting to be somewhere and actually being there.
Developers, expense tools, and AI agents all plug into Engine's API.
And as AI spreads, Engine only becomes more valuable.
Every AI agent that wants to book travel needs real supply, real pricing, and real payments.
That's why Engine was built to go far.
With 40,000 businesses relying on Engine and growing fast, they're powering travel for the masses with partnerships like Navan and Tampa Bay Buccaneers.
Strong hotel partnerships, proprietary supply, real-time rate shopping, and payment rails.
That's the kind of foundation that takes years to build.
Eight years in Engine's case, and it can't be bought.
The future of business travel runs on Engine.
Visit engine.com/slash decoder.
Support for the show comes from CrowdStrike.
AI is already fundamentally changing how companies build products and run their businesses.
If you listen to the show, you probably already know this.
But while AI drives innovation, every new model and agent also creates new cybersecurity vulnerabilities.
That's why CrowdStrike built AI Detection and Response, or AIDR.
AIDR helps organizations discover where AI is being used, monitors AI activity at runtime, and helps teams detect, investigate, and respond to threats involving AI systems.
As companies adopt AI, security has to be built in from the start.
More than 70% of the Fortune 100 trust CrowdStrike to protect their businesses.
Now, CrowdStrike is helping secure the AI era.
You can learn more about AI detection and response at CrowdStrike.com/slash decoder.
Company spending is complex.
Managing it should be simple.
This is Amex Corporate, a single platform connecting cards, expenses, and payments to streamline the way you work.
Flexible controls for when priorities shift, support around the clock, all backed by American Express, so you can stay focused on what matters most.
Built to simplify, designed to scale.
This is Amex Corporate.
Get started at go.amex slash Amecorporate.
Terms apply.
I'll just bring a dumb comparison to the iPhone.
It's iPhone season.
I just reviewed the iPhone Duo.
Apple keeps the iPhone looking the same for several years now, right?
They build all of the tooling for the new iPhone, and then they just reuse it for two or three or four models to get all the value out of that investment back before they move on to the next thing.
Apple puts out a new iPhone, they keep selling the old iPhone for a while to get more value out of that investment and that development program.
The AI industry does not seem to be doing that, right?
All of their emphasis is on developing the next new thing, deprecating the old thing pretty fast, and moving you on to the new expensive product, which at the same time they're building the next new expensive product.
At some point, it feels like that will rationalize, right?
That there will be something that is worth just collecting margin from while they go invest in the new thing.
And I just can't figure out where Anthropic sits in that cycle.
I mean, we do see this.
Open source token volumes are picking up, and there's a lot of areas, yes, where the open source models have become good enough.
And I think on a go-forward basis, you're like, okay, was that because of distillation?
And the Frontier labs have some defensibility actually going forward.
Or, you know, I think when we talk to clients too, it's, you know, how do we actually think about Frontier versus open source on this debate, or even non-Frontier.
So something like a Sonnet type model, if you want to do the iPhone 18 versus, you know, the SE type, you know, analogy.
We do see that dynamic.
And obviously, open source is it's a question of how much can that take?
And then, two, because we're so early in these verticals, we don't know what's going to be like fully agenic.
There's no human in the loop for actually human in the loop where, yes, you can do, you know, where the harness actually has, I should say, some value and defensibility to it.
The kind of you know, big area I'd look at here, especially when we talk to enterprises today, is yeah, only the coders are allowed to use the frontier models at a lot of these enterprises.
If you're a non-coder, you are, some of these companies just limit you to Sonnet if you're a you know, cloud, an Anthropic company.
And I think that's reflective of how you know management views and wants to budget for this, like what Frontier intelligence is actually worth to them in certain areas.
Like in my financial analyst brain, you know, cloud could not build a good financial model, you know, six months ago.
It's getting better if you connect it to the right areas.
But we've gone from something where, okay, I needed a junior analyst six months ago.
Maybe I don't as much anymore.
And then, will I have a full junior analyst at my disposal anytime or multiple pretty quickly if I have unlimited budget or token budget?
And I think we just look at that across every vertical and major job category.
And the time horizon in each of those categories is going to be different.
And I think that's just one of the bigger questions I have is how quickly do they get to where they think they can go?
I want to dig in on some of the numbers here.
The one that jumped out in all of the comment sections on all of the forums and all of our articles yesterday was $80 billion.
Anthropic lost $80 billion.
That is related to a technical charge.
Can you just explain the $80 billion?
Because it doesn't seem particularly relevant to the revenue and profits they're talking about.
Yeah, it's a non-cash charge because their valuation has gone up so much and they've issued warrants or convertible notes.
You have to account for that in your balance sheet.
So it's just a non-cash charge because their valuation has gone up so much since they issued these warrants and notes.
So yeah, that's something you would always back out.
You can argue on stuff like stock-based compensation.
Should we really be thinking about that on a non-GAP versus a cash versus because it's a non-cash, if I just hand employees shares, I have to account for that on my income statement, but I'm not actually handing them pure cash out of my bank balance.
So it's not an area like that.
It gets the accounting, the high level, if you don't know accounting, it looks bad, but it's because they've grown so much and their valuation has gone up so much.
Some of the argument here about that charge is obviously that's Amazon was the other party there.
Obviously, Amazon's very happy because Anthropic is buying a ton of AWS.
I'm sure they're happy their valuation has gone up.
But over time, Amazon's going to get diluted this way, right?
That's part of the dynamic there.
They're going to obviously IPO, they're going to put a bunch of shares in the market.
It's very clear that over time, they will issue more shares to raise more money.
It doesn't seem like they're going to stop wanting to raise money anytime soon.
How are you thinking about that in terms of just investment into a company like Anthropic that your valuation might be going up, but your actual ownership stake might be getting diluted over time?
Yeah, I mean, I think the deals have always been very creatively structured.
And I think the numbers, they've actually only burned 10 billion of cash.
You know, they have 120 billion plus of cash and marketable securities on the balance sheet today.
You know, post-IPO, probably another 100 billion.
You know, it's a great deal for both parties.
They only really rent compute.
That's not like they have these massive capital outlays or even rent to own.
So, yeah, and you can make some arguments about like certain accounting and okay, there are these massive commute commitment obligations.
That's technically, you know, future debt.
From a dilution perspective, all tech companies dilute.
You know, do they are they going to need to raise another 100 million of debt or equity at some point?
You know, possibly.
Can they continue to creatively structure and finance future compute build outs?
You know, probably as well.
I know there's been a lot of in the last few weeks, a lot of angst about the future of compute financing and data center financing.
But if you're Anthropic, you know, if you're a major lab, a hyperscaler, or Broadcom NVIDIA that are backstopping a lot of these deals, you know, that's probably not going to change anytime soon.
As an equity investor, would I be worried about getting super diluted?
I don't think so.
If you believe in this long-term AGI bull case and that Anthropic is going to be a leader in this, you're probably looking at a 10 multi-10 trillion plus dollar business.
I think they can outrun dilution at that point.
Let's talk about the compute commitments.
I saw at least one analysis saying over the next 10 years, it's 800 billion plus in commitments to the various hyperscalers and NeoClouds.
That's a lot.
You're saying that they don't have that much money.
They haven't even spent that much money yet.
Do you see them generating the revenues to pay off those commitments?
Yeah, I think when people look at the headline commitments, the 500, 600 billion number over seven to 10 years, let's call it, it actually at what they're paying for compute today actually isn't that many gigawatts.
If you think about them spending right now, I think on average, they're close to 11 million per megawatt in spend or 11 billion per gigawatt.
If you kind of take that back to the annual level and say, okay, the 520 numbers over seven years, for example, that's really not that many gigawatts.
And they're going to be well beyond, when they get to something like 20 gigawatts, that future compute commitments that they're running, essentially, is going to be well over, well into the trillions.
So yes, they are going to have the revenue to do so.
I think it's more of how much revenue are they going to have relative to how much compute?
And then two, the compute efficiency equation.
If they keep getting a lot more revenue out of every inference megawatt, how much do you really want to invest in training and take margins to zero from like a rental perspective?
Because you can get to something where they get to even 80, 85% of their fleet is just on training and research.
The revenue, yes, it's going to scale pretty well.
They're not in any direction, unless we realize all this revenue disappears or people churn.
We're really not in a huge, it's like they have to hit a trillion dollars of revenue extremely, extremely quickly, you know, to achieve all this and pay for this.
Unless you're trying to build digital god and unless it doesn't diffuse across the economy as fast as everyone wants it to.
Those are bets, right?
They're huge bets.
And I think like the numbers you look at, if you're really bullish on this ramp of like into the digital economy, is, you know, they say within their Fortune 500 customers, they have 50% of the Fortune 500.
They are 0.1% of their total customers' operating expenses.
I think when you look at that on like a per user basis, it's like $8 a month.
If you believe OpEx is, you know, doesn't include cost of goods sold.
And if you believe they included cost of goods sold, it's sub $50 per month.
And they said the same thing of their top 5% of cloud code users, they're spending $18,000 a year on average, the top 5% of users.
Their non-cloud code users spend under $75 a month, well under 75%.
So there's this huge, especially when we talk to enterprises and these traditional buyers of software of IT, penetration is extremely low in like traditional white-collar work.
And I think that's the big point is too, there is a large ramp period here of both seats adoption and usage.
You know, you can make arguments of who's going to win in this, but it's obvious the Frontier Labs are going to get some portion of this.
It's going to be pretty material to a net new ARR next year in 2027.
One of the things that's really interesting about that is we talk about the Frontier Labs, we talk about the hyperscalers.
Anthropic has a lot of wild risk factors in this S1, including that cloud might be conscious and kill us all.
But one of the most direct and maybe easiest to understand is that AWS, Azure, and Google Cloud are both suppliers and competitors in some real way, particularly Google.
They say, well, these relationships could turn, right?
They have a big relationship with SpaceX AI.
Elon is going to train Grok.
They're going to compete with SpaceXAI at some point.
That relationship might become precarious.
As you say, they're only renting their compute.
At some point, the market might force them to own more of their compute because their own competitors don't want to lease their capacity to the leading company.
How do you see that playing out?
We definitely see both OpenAI and Anthropic going more directly and owning, not owning the compute, but more rent to own, or going through an SPV that some financial sponsor does, and kind of doing the compute more directly versus renting.
So there's two points of this too.
Google, from one perspective, is also selling their external chips to customers and saying, hey, we don't care to monetize this within Google Cloud or even allocate the share of, if you think we're very chip constrained, we don't even care that these are going to deepmind our internal GCP compute for us to monetize.
We're just willing to become a chip seller.
And Anthropic loves TPUs and they have, you know, there's, you know, three and a half, four gigawatts plus and probably more in the pipeline in terms of orders there of Anthropic buying these chips directly to then rent.
So that's the market.
They're buying them directly to rent.
So they're buying them into a NeoCloud?
Yeah, they buy them through like an SPV or the SPV buys them and then they rent it from the SPV.
Got it.
Even within Google Cloud or AWS or Foundry, Anthropic is massive.
48% of their business comes through like the Bedrock Foundry and Vertex, where people are paying, you know, through their existing cloud relationship to access these models.
They're not even talking to, you know, they are, but you don't have to interact with the Anthropic Salesforce.
You mentioned this earlier.
This is the marketing channel where Anthropic gets a rev share.
Right.
And if you're AWS and you're saying, oh, I'm running Anthropic compute for, let's say, 10 million per megawatt, but now I'm getting 16% of 65 a megawatt plus the compute cost as well.
We're seeing margins at all the clouds go up right now.
Part of it is CPU utilization is going up because of all the coding and then some of the RL side, but these token as a service businesses, as we call them, so AWS, Bedrock, Microsoft Foundry, Google, Gemini, Agent Enterprise Platform, formerly Vertex, are actually massively increasing kind of the margins on AI at these clouds.
So they're benefiting as well, and shareholders are giving them credit for this recently.
I think in Q2, both Azure and AWS had extremely, extremely strong quarters on the back, AWS specifically on the back of Anthropic's growth on Bedrock.
Do you think that will keep Amazon from ever wanting to train its own Frontier models?
They're doing a good job of letting AWS be the infrastructure for everybody else, but they're one of the only big tech companies that hasn't felt the insecurity of not having their own models.
It's interesting.
I think they're very happy to serve a wide variety of customers.
And they have very little.
When we look at our estimates of training compute, they have the least of any hyperscaler.
If you don't, X Oracle, maybe.
It doesn't seem like there's much strategy there.
I know both Microsoft in the last two quarters has been talking about it a little more.
AWS on the call has been talking about it a little more, but it's not a huge, huge, they're not doing it to the same extent that Meta is or trying to be competitive here or even Google with Gemini.
And I think, especially someone like Dylan will tell you, if you're not trying to compete at the frontier, there's really not a place for you, especially if you're only dedicating a few hundred megawatts to internal, you know, one internal use cases like serving Amazon retail, but then two training.
There's a lot of commitments to make to be good at this.
It's a conversation for a different day, but I look at these Microsoft job cuts and I see it as the glimmer of evidence that they're going to try to compete in the future.
They got burned.
They obviously got burned pretty bad by OpenAI.
Yeah, I mean, they have, in the new agreement that they signed, they have the right to monetize OpenAI models for essentially not paying OpenAI anything.
They're going to have, you know, some interesting things ahead where they monetize, you know, OpenAI models or even through like Microsoft 365 cowork and co-pilot applications where they're not paying OpenAI anything for a Frontier model.
Support for the show comes from OutShift, Cisco's incubation engine for frontier technology.
You can find multi-agent AI in every enterprise roadmap right now.
But here's the problem everyone's facing.
Agents can pass messages, but can't think together.
These systems silently underperform through cognitive failures, misreadings, unverified claims, false consensus, and conventional monitoring can't detect them.
Outshift by Cisco is building the fix with their new comprehensive resource, the Internet of Cognition.
It's an open source guide that's a foundation for building multi-agent systems from design to production.
The goal is to give agents shared context, shared memory, and guardrails, all to drive the results we actually expect from AI.
You can lean on this resource to understand Agentic AI's evolution and how it's shifted from isolated agents to orchestrated superintelligence.
You can gain insights for how to future-proof your business by tackling complex challenges with multi-agent systems.
You can read the paper, experience a demo, grab the code from outshift.com.
That's O-U-T-S-H-I-F-T.com.
Today's social engineering attacks look trustworthy by design.
Disguised as a routine request, an internal email, a familiar face on a call.
They succeed because they blend in, but not with DopPle.
Doppel sees through the disguise.
Their AI-native platform delivers a complete three-layer defense stack designed to disrupt campaigns at every stage.
Digital risk protection detects and shuts down fake profiles, look-alike domains, and impersonations across every channel.
Human risk management trains your team to recognize deep fakes and bad links.
And email security provides agentic protection, inspecting every message, tying it to the attacker's external infrastructure, and taking it down so it can't strike again.
Doppel outpacing what's next in social engineering.
Learn more at doppel.com.
That's D-O-P-P-E-L.com.
Why can't we get AI to production?
Our competitors are already.
How do we keep data secure?
When do we actually see ROI?
All this talk about AI, but talk doesn't transform businesses.
AWS AI cuts through the noise, making AI easier to securely deploy and scale.
With ready-to-use agents and the broadest set of AI tools and services, you can build, buy, or partner your way.
Stop overthinking.
Start building.
AWS AI is how.
The other dynamic here, and you brought it up earlier, is over the last few weeks, there's just been a lot of stress about Neo-Clouds, whether they will succeed, whether they will fail.
I think Elon Musk said there will be a guppy-like extinction event, which is just a brutal metaphor to use to describe a bunch of data centers.
But this is a bunch of circular financing, and NVIDIA stood a bunch of them up.
And maybe the hyperscalers are just going to run away with it.
Or maybe Anthropics demand, maybe they will want to own more of their own compute because renting it is precarious in all these ways.
What do you make of the NeoClouds?
And do you think they're going to survive the market actually shaking itself out as these companies go public?
Yeah, look, Elon obviously has some incentive to say NeoClouds are going to be extinct.
You know, there's a lot of, and ClusterMax had someone else's does amazing ratings of the NeoClouds.
There's a lot of NeoClouds that are like ex-crypto miners that are not good businesses and are not good at operating.
Core Weave is an ex-crypto mining company, right?
And I don't mean Coreweave, but there's others further down the list.
I think Coreweave Nebbius, anyone that has backing or backstops from one of the major labs, hyperscalers or NVIDIA or Broadcom, is going to be okay.
It's that longer till I think hyperscalers have been 65% of CapEx and net new compute brought online.
So then there's 35% of the market that's non-doesn't have the balance sheets that the hyperscalers have.
Both Google and Meta have recently raised or announced they're going to raise.
When we look at the big four hyperscalers, they don't actually need to raise that money over the next two years, even though CapEx is growing from 1.2 to 2 trillion pretty quickly.
But a lot of these other neo-clouds, if you don't have that sort of backing, I think it gets, you know, it is very hard, even right now, and becoming extremely difficult if you don't have the backing or backstops from those players to keep building compute.
It's a very, very tough financing market.
One of the things that I think is really interesting about Elon in particular talking about Neo-clouds dying and obviously hyping up his own data center business is he's trying to put them in space and to get away from the backlash in the United States around data centers in particular.
We have a lot of coverage about a data center backlash in the United States.
It is slowing down a lot of projects.
But at the rate we're going, if you think the neo clouds are shaky, you might actually end up abandoning a bunch of GPUs and half-built data centers or have them tied up in financing agreements where they can't be lit up.
What do you make of that?
Do you think we actually just need to go to space?
Or do you think the market is going to rationalize and actually take advantage of all the compute that is currently allocated but not being used?
The market's very good at finding places to put chips here, you know, on the ground, I should say.
There will be, you know, politically, you know, we'll see what happens next week with midterms and kind of the fallout from that.
And obviously there's some very large sites, you know, still that have massive permitting problems.
And then there's the entire power equation as we look towards next year.
The data centers will be built.
There will be a method to get these built.
I think the biggest thing, and like the hyperscale CFOs have said this, from like an overbuilt perspective, you know, it's on a relative basis, it's pretty cheap to build the data center shell.
What they can do if they overbuild is they're going to say, okay, we're just not going to take delivery of the chip.
We're not going to buy chips.
We're not going to fill them up.
And these, you know, they'll just sit empty and chipless.
But that's where a lot of the, you know, that's the majority of the spend is on the chip side.
So if we do end up in a place where we're actually oversupply from a data center perspective, I know that's a little bit different.
That's the exact opposite of what the question was.
They kind of had said that from like an ROI perspective.
I think this comes back to that larger question.
Are we still going to be super, you know, supply constrained?
A lot of people now, especially in the last three weeks, are talking about, are we in this massive glut of compute as we look towards 2028, actually?
Actually, because the same thing we talked about from Anthropic going from negative 94% margins to positive 85% and kind of compute efficiencies, you know, means as you bring on more inference megawatts that are making a lot more revenue per megawatt, you know, all else SQL, you need less compute.
So it's a question of, you know, are we going to have enough revenue in 2028 to justify the ROI, you know, on 2 trillion plus of CapEx?
This is why I spent so much time asking about capability overhang and how good the models are today.
Because you can see some competitor that is less idealistic about AGI saying, actually, we're going to do a bunch of forward-deployed engineers in all of these verticals where they haven't taken advantage of AI and sell them high-margin inference because we'll automate big chunks of their business and they'll see the return.
And right now, a bunch of the Fortune 500 has not seen return on AI spending.
So if you're actually just better at customer service and deployment and productizing the model, you might get way ahead of where Anthropic needs to be because they're still thinking about AGI every single minute of every single day.
And I don't know, man, I look at Dario standing next to Mark Benioff at Dream Forest.
I'm like, that dude does not want to be there right now.
He wants to be thinking about like the machine god.
There's something there where you can just see that competitor coming up with an open source model and be like, we're actually going to productize this and we will actually take the revenue that everyone else is depending on.
And too, like in the interim, that's why it is getting more verticalized because you need something to bridge at AGI where it just fully does the job.
You need something to bridge the actual model today.
We just take that for granted.
The Agent AI will show.
Yeah, to get there, you need some bridges of where it actually sits in with the actual end user at some point.
And so I think everything is going to come down to this: is there going to be some timing or adoption mismatch where we just don't get the revenue at a certain point in time to justify that chase of training compute towards AGI?
And I think that's a risk.
The other risk I think we look at is: do we get more models at the frontier or even at the open source that are as competitive in coding where token pricing across the frontier needs to be taken down because, like I mentioned earlier, like you know, lower switching costs.
Even at semi-analysis, we went from 95%, 90% plus of our usage at the end of Q2 was on Anthropic models after the release of 5.6 and Astra.
That went down to 70%.
And then with Opus 5.5, it's gone back to 90% plus, roughly.
So it does come back, even like the base of revenue today.
And they've said, you know, that we have net revenue retention of 900%, seeing this massive, massive growth.
This isn't a traditional software business like ServiceNow or Workday, where you have just incredible logo or gross retention of 95, 98%.
And customers sign these nice three-year contracts, they never churn.
They add some seats, maybe they adopt another product that is being upsold.
This is purely consumption.
I think the other portion was the 20% drop in the two weeks, last two weeks of the year versus the prior two weeks last year in token or in token spend because the holiday season.
People aren't, you're not going to do work code stuff.
You're not going to be coding for work during the holidays.
So this consumption business, I mean, this is extremely, extremely pure consumption business, even different than how we think about like Snowflake or Datadog today in public markets.
Obviously, Anthropic is not the only company that's going to do IPO.
OpenAI is right next to them.
They've delayed theirs.
You mentioned earlier, Anthropic is much more enterprise-focused.
I think OpenAI for a long time thought that Google wouldn't react to them and they would just take the search business away and everything would be fine.
Google obviously reacted for better or worse.
Searches now, AI overviews.
Looking at the Anthropic S1, what are you looking ahead to in OpenAIs?
Because they are a more consumer-facing company.
Yeah, so OpenAI was 60-40 consumer, you know, 60% consumer, 40% enterprise.
At the end of Q1, that didn't flip for the first time until January or August to be enterprise-focused.
And what they'll tell you is, you know, enterprise business, the consumption business, because it was so consumer and subscription-focused, consumption, you know, this consumption business that's 80% of Anthropic's revenue, just the token business, that didn't take off till the release of 5.6.
Oh, you know, and then with Astra.
And those are really great models.
OpenAI took the majority of actual net new ARR in Q3.
But it's going to take some time because I think what's been public, you know, what's been in the Wall Street Journal, like negative 100% EBIT margins versus we're seeing positive 11 here.
You know, there's some differences, some pretty big differences in the business model where they just haven't, they just don't monetize at the same rate that Anthropic does.
And that's a little bit because the business makeup, you know, the verticals, you know, like that consumer versus enterprise split, you know, that's changing.
And I think what they'll tell you is, you know, they see a really good Q4.
They have a much stronger enterprise sales function than Anthropic has.
So I'd expect them to come up, but I don't think the financials are going to look as good as this even when they S1 maybe in early 27.
Do you think that's why they delayed it to get their financials looking better?
Yeah, I think they're, you know, they had a really strong Q3.
Enterprise grew 100% quarter to quarter versus the total business was 77%.
So I think you get another strong quarter of enterprise here.
If Opus 5.5 didn't take a ton of share, that, yeah, it'll put them in a much better position to kind of tell the story.
There are some other turns here between now and when Anthropic actually goes public.
They're going to do a roadshow.
There'll be some pricing events.
What are you looking for from Anthropic?
They did an investor day two or three weeks ago where they did give some more color.
I think they'll kind of walk through why Q3 was so weak.
And Meta was a very, very large customer, probably over 10%.
I think what's been publicly reported is they went from 60,000 cloud code seats down to 30,000.
These token volumes didn't disappear.
They just shifted to Meta's internal models.
They started cracking down on anti-distillation, Anthropic did.
And that was 5% of revenue prior.
And I think they said 5% to 7% was of revenue in the S1 and stuff against their terms of service.
What's here on the road shows a lot of this October acceleration after Opus 5.5.
I think we believe they're back on track.
If they were doing 10 billion of net new ARR per month in Q2, and that fell down to 4 billion in Q3, they're getting back on that 8 to 10 pace here in Q4.
And then too, I think people want to hear about these new verticals about specifically Cyber.
I think they're doing some patching until they have that full cyber skew rolled out, but they're definitely monetizing cyber today for vulnerability code scanning.
They're not small contracts, I should say, with existing customers.
So I think they'll start to message that and what kind of the 2027 ARR growth path kind of looks like.
The other thing, too, is expectations management.
Keeping numbers, you know, low enough, you know, not talking about AGIs as much.
It's hard to do expectation management when your risk factors are like we could pose an existential risk to all of humanity.
Right.
And so, saying you do that, you know, you're going to achieve AGI at some point.
We're going to replace everyone's jobs.
But then, too, trying to keep numbers low enough for Q4 and to beat, you know, have this massive beat the first quarter you become public and have a very nice, you know, a decent guy for 27.
It'll be a nice mix of a seesawing between, you know, that long-term vision and short-term, you know, expectations management.
There's a lot going on, Joey.
This has been great.
We're going to have to have you back as these companies barrel towards actually being public and their economics become much more visible.
Thank you so much for being on Dakota.
Yeah, thank you so much.
Hello, thank you Joey Brookhart for joining me and thank you for checking out this episode of Dakota.
To get new episodes every Monday and Thursday, subscribe to our YouTube channel at DecoderPod and find us on TikTok and Instagram under at DecoderPod for more fun stuff we put out almost every day.
If you enjoyed this episode, please send a link to it to someone you think you might like it.
It really helps us grow the show.
You can also subscribe wherever you get your podcast.
Decoder is Proxima, part of the Rock Smooth Podcast Network.
The show's producers are Greg Ott, Kate Cox, and Nick Stat.
This episode was edited by Ursa Wright.
Our editorial director is Kevin McShane.
The Dakota music is by Breakmaster Cylinder.
We'll see you next time.
When you shop pickup at Smith's, you can expect the savings you love and fresh groceries selected just for you.
Our associates are committed to getting every detail right, carefully handpicking your items, checking for quality and freshness, and packing your order with care.
Because bringing you fresh, quality groceries is what we do best.
And right now, enjoy $20 off your first online order of $75 or more.
Restrictions apply, see site for details.
Smith's, fresh for everyone.
