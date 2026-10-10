---
record_id: "podcast:d5423e55-194d-4729-bbb4-7e2254848a55"
episode_id: d5423e55-194d-4729-bbb4-7e2254848a55
title: "What America and China Fear Most About AI: A Conversation with Kyle Chan and Helen Toner"
podcast_title: The Foreign Affairs Interview
url: "https://pocketcasts.com/podcast/the-foreign-affairs-interview/e2f31bf0-b915-013a-d903-0acc26574db2/what-america-and-china-fear-most-about-ai-a-conversation-with-kyle-chan-and-helen-toner/d5423e55-194d-4729-bbb4-7e2254848a55"
audio_url: "https://pocketcasts.com/podcast/the-foreign-affairs-interview/e2f31bf0-b915-013a-d903-0acc26574db2/what-america-and-china-fear-most-about-ai-a-conversation-with-kyle-chan-and-helen-toner/d5423e55-194d-4729-bbb4-7e2254848a55"
feed_guid: null
feed_url: "https://feed.podbean.com/foreignaffairsmagazine/feed.xml"
published_at: null
published_local_date: null
played_date: 2026-10-01
played_at: "2026-10-01T12:00:00Z"
play_count: 1
duration_seconds: 3300
source: pocketcasts-history-browser
played_label: October 1
history_order: 30
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: acbfbe22faf98f67bfa13e8b98fcd5002992a3d596902b2a06aeff62b418fc09
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

AI has become a central U.S.-China issue after Xi Jinping’s first Washington visit in more than a decade, with the Trump-Xi summit yielding only minimal progress—agreement to talk and establish a hotline—while policymakers debate whether a decisive strategic advantage in AI could yield superintelligent military and cyber capabilities. Kyle Chan and Helen Toner describe Chinese concerns as led by regime stability, cybersecurity, and critical infrastructure, citing Chen Yi Xin’s rare public piece, and note China elevated AI alongside Taiwan and trade. They contrast U.S. existential-risk discourse—Dario Amodei’s “Pacing the Frontier” letter, Anthropic researcher Jacob Coxon’s warning about humanity being killed within a decade, P-doom, and calls for slowdown—with Chinese skepticism that such fears are overblown or a U.S. ploy tied to export controls, with parallels to climate negotiations. The discussion covers OpenAI, Anthropic, Google DeepMind, Demis Hassabis, Sam Altman, Alibaba, DeepSeek, MiniMax, and Japu; claims that U.S. frontier researchers are shaped by a futurist community; and data points including distillation possibly accounting for 10–50% of China’s catch-up, open-weight models, lower Chinese data-center, energy, and talent costs, state compute vouchers, and risks of hacking or stealing model weights.

Actionable follow-up is to watch whether the new dialogue and hotline narrow to concrete shared risks: preventing non-state actors from obtaining powerful open-weight models or advanced cyber capabilities in the next six to eighteen months, and sharing information about incidents involving increasingly autonomous systems escaping developer control at OpenAI, Anthropic, Alibaba, DeepSeek, MiniMax, or Japu. Decisions to consider include whether U.S. domestic regulation can proceed without assuming China will simply sprint past, whether export-control leverage framing undermines cooperation, and whether speed is creating hackable targets rather than durable advantage. Research leads include CSET’s distillation analysis, Chen Yi Xin’s security priorities, the U.S. compute-scaling and data-center backlash constraints, and whether Chinese labs have comparable incidents. Follow-up questions: Does China identify any issue it believes requires coordination with the U.S.? Are open-weight releases a shared liability? Is distillation or model-weight theft more important than raw frontier speed? No direct health implications are present; the actionable domain is AI governance, national-security risk, and bilateral confidence-building.

## Transcript

I'm Dan Kurtz Phalan and this is the Foreign Affairs Interview.
The concept of a decisive strategic advantage of whoever gets to a certain threshold of AI capabilities, whichever country gets there first, will have super intelligent systems that could potentially have super smart military weapons systems, could have dominant cyber capabilities, could basically come to rule the world.
I mean, I like put it so bluntly because I think that does kind of reflect the stakes that many in Washington feel when it comes to why the U.S.
needs to lead in AI.
And I don't think that's how it's seen, at least among Chinese policymakers.
The fact that China is, you know, relatively close behind the U.S.
should not be a reason for us to not regulate our own industry.
We should not treat the speed at which the two industries are developing as totally independent.
That is to say, it's not like 100-meter sprint where if one runner just stops running, the other runners are going to continue at exactly the same speed.
I think it's much more like a Peloton in a bike race where you have a group of cyclists and the front rider is taking on more work to kind of lead the pack.
Over the course of just a few months, artificial intelligence has become one of the most central issues and one of the most fraught issues in the relationship between America and China.
Policymakers in Washington and in Beijing simultaneously worry about which country's tech sector has the advantage and whether the search for advantage will itself lead a catastrophe for both countries and for everyone else.
Recent bilateral meetings, including last week's between Donald Trump and Xi Jinping, have yielded only minimal progress toward cooperation.
Agreement, as one of my guests this week put it, to start talking about talking about AI.
Kyle Chan is a fellow at the Brookings Institution.
Helen Toner is Executive director of Georgetown University's Center for Security and Emerging Technology.
Both fairly uniquely combine deep knowledge of AI and deep knowledge of China, which they bring to their work in foreign affairs and beyond.
We discussed how the two countries think and approach AI with real differences as well as some new convergences, what it means to compete, and what it will take for America and China to find some way to reduce the biggest risks.
Helen, Kyle, thanks to you both for doing this.
You've no doubt been in high demand over the stretch.
Great to be here.
Great to be here.
The reason for the most recent wave of demand for your expertise was, of course, the centrality of AI in the U.S.-China dynamic at a time when Xi Jinping was coming to Washington for his first aid visit in more than a decade.
It did not, as far as I could tell, get a ton of attention between Xi and Donald Trump, but it did get a fair amount of attention in the meetings running up to it, especially between Treasury Secretary Scott Besson and his counterpart.
As you watched those discussions and what emerged from them, what did it reveal to you about Chinese views, about the Chinese approach to both AI safety risks and to the competition, and also about the prospects for real cooperation and addressing some of those risks?
Helen, why don't we start with you and then Kyle, we'll go to you for anything you'd add or disagree with.
It was really interesting to me as someone who's been kind of both following AI safety and security conversations for about 10 years and also U.S.-China relations and tech competition for about 10 years.
Really interesting to me to see those worlds finally intersect with AI really high up on the agenda.
I think what we saw, you know, what did it reveal about Chinese perspectives?
I think the most informative thing, there was a fair amount of news coverage in the lead up on kind of different things that were coming out in Chinese media, you know, reacting to Dario Mode's Pacing the Frontier letter or kind of other things.
I think that a lot of that coverage missed what to me was the most important messaging out of the Chinese government, which was Chen Yi Xin, who's the head of the Ministry for State Security, really powerful, really security-focused ministry in China.
I've heard that Chen himself is quite influential, you know, with Xi Jinping.
And he doesn't normally write anything publicly.
And so for him to write a whole piece about AI was really informative.
And he kind of had at the top of the list the effects on the political security environment was the top concern, basically meaning regime stability.
Below that, cybersecurity and critical infrastructure.
So to me, that was the most meaningful signal of China is really ready to take this seriously.
But I think both in that piece and then also in what came out in the summit, in and around the summit last week, it feels to me like China doesn't necessarily clearly see where they need to be talking to the U.S.
There's sort of an interest in talking.
There's a high level of concern.
But I don't think they've yet identified in their minds the issue where they feel like we really have to be talking to or coordinating with the US on this.
So maybe that's something that is still to come in the future.
Kyle, I'm interested in your perspective, anything you'd add or any disagreements.
But also when you look at the, I think, two more specific agreements that came out of it, relatively specific by the standards of U.S.-China diplomacy in this era, at least, one was to have some kind of dialogue continue or start in the next few months and then agreement establish some kind of hotline between the two countries to address risk.
So both on the general perspective, and then on the utility or significance of either one of those announcements.
Curious how you saw it.
Yeah, I mean, one of the most striking things to me about all of this is how important AI has become as an issue to the Chinese side in the U.S.-China relationship.
So it's almost ironic given that originally AI was kind of emerging as a new flashpoint between the two countries, right?
They already have so much to disagree about.
There are so many ongoing tensions and issues.
And then AI threatened to become kind of the ultimate front line in many ways, at least on the tech front.
And then what happened is, I think, a shift in perceptions of AI on the US side, a shift of perceptions of AI on the Chinese side, as Helen pointed out.
And then, especially on the Chinese side, this elevation of AI to literally alongside Taiwan and trade, one of the few points brought up in the Chinese readout from the summit.
And so that is already quite notable, how significant it has become as an issue, as a bilateral relationship issue for the Chinese side.
And then specifically on those two proposals, they're either hugely disappointing or actually quite productive, depending on your expectations going into this.
So if your expectations were that the US and China would get together and form some kind of arms control treaty for AI, some new nuclear security pact or agreement, then it was obviously very, very disappointing.
They agreed to talk about AI.
They agreed to tell each other about issues that come up.
I mean, a lot of details are scarce, but that's roughly speaking what came out of this.
But on the other hand, if you had very low expectations or no expectations, especially given the very, very deep distrust between the two countries and the extremely fierce competition on AI between the two countries, and then also, if you are someone who was privy to the previous AI talks between the U.S.
and China during the Biden administration, like Cess Center's really excellent op-ed in the New York Times about China not taking AI safety very seriously and wanting to focus on other issues like export controls.
Seth Center, who have led AI diplomacy for the Biden State Department, if I remember correctly.
Yes, I believe that's right.
Then your expectations going to this would have been very, very low.
You would have thought there's not really much the two sides can agree on or even talk about.
And so from that point of view, and honestly, I share more of that skeptical, low expectations viewpoint coming into this.
From that point of view, there was actually more here than meets the eye.
And I think Helen's point is exactly right.
I think part of this is that China's taking some of these risks more seriously.
And I think there's actually more possibility for progress to be made, especially compared to the last official dialogue on AI between the US and China during Biden.
Helen, if you take that glass half full view, what might happen?
What would we like to see in the next six months or year that would make good on that sliver of promise that Kyle is highlighting?
I do think that is the right read.
And relative to the rock bottom expectations that we saw around any results of the summit more generally, I think this was at least somewhat productive.
I think the thing that I will be watching is: do they narrow in on specific issues of concern that both countries are interested in talking to each other about because you know a huge problem with AI in general is it's sort of an everything technology, so it affects every industry in all kinds of different ways.
Even talking about kind of AI security or AI and national security, there's still so many different things you might be talking about.
Are you talking about AI adoption into military systems on the battlefield?
Are you talking about AI and non-state actors potential for terrorists to use AI?
Are you talking about risks from autonomous AI systems themselves?
You know, there are lots of other things you might mean, even if you narrow it down to AI and national security.
I see, in my mind, there are at least two quite concrete things that the US and China could have an interest in talking to each other about and working collectively on.
One has gotten a little more attention.
This is essentially thinking about sort of open release of models, bad actors using powerful models, thinking about sort of who has access to mythos-level cyber capabilities in the next six, 12, 18 months.
I think that's one area they could potentially talk to each other about.
That'll be a tricky thing because China will tend to think that the US is trying to rein on their parade, where China's having such success with open models.
And so the US coming in and saying you shouldn't do that, it's a bad idea, you know, will not land super well.
But I think the underlying interest of they don't want non-state actors, terrorist groups to have too powerful AI systems is a genuine shared interest.
The other area, which I think I wouldn't have thought was really possible if we hadn't seen some of the incidents this past summer, is looking at essentially risks from increasingly capable and increasingly autonomous AI systems escaping from the companies that are developing them.
So this is not about bad actors.
This is about the frenetic pace at which companies like OpenAI, Anthropic, but also, you know, I've heard rumors of incidents within Alibaba.
China has other, you know, DeepSeek, Minimax, Japu, other AI developers that are also trying to move at this breakneck speed.
Are they also going to start having some of these kinds of incidents as their models get more advanced?
And if so, you know, I would argue there is something that the US and China could benefit from in talking more directly about what is going on there.
So, you know, one of those two options would be two concrete topics to talk about.
There's other more concrete sort of AI-specific topics they could agree to talk about.
But if we're just continuing to sort of talk for the sake of talking and stay at this very high level about sort of security, risks, you know, ensuring wide benefits, then I don't think that we'll necessarily get anything out of it.
Of course, you know, this kind of thing takes time.
So, you know, I think if we're settling on more concrete topics over the course of multiple months, that's decent progress.
Though also has to be said at the speed the technology is moving, the diplomatic speed may not be sufficient to actually make a difference here.
Yeah, in the diplomatic world, you do have to talk about talking before you talk.
So that's not necessarily a sign of failure, but I take your point about the difference in speeds.
I'm curious in how Chinese thinking on some of those specific threats has developed and evolved.
Let's focus on the kinds of existential concerns that came to at least wider appreciation in the wake of some recent incidents, and especially the resignation of anthropic researcher Jacob Coxon, who warned of relatively high likelihood of all of humanity being killed by AI in the next decade or so.
Kyle, when Chinese policymakers and leading Chinese thinkers here read that kind of warning and see the debate that it precipitates in the United States, what do they think of it?
Does it resonate with them?
Do they see similar concerns?
Does it seem hysterical and overblown?
Does it validate their model?
I mean, there's any probably a range of views, but how would you break down the Chinese version of this debate and their reaction to what's happening here?
I think the Chinese reaction is they're sort of scratching their heads about the existential risk issue.
I think that is just not a very big part of the discussion in China.
It is not really talked about in Chinese official circles very much.
You don't hear so many statements gesturing to this concern that AI could wipe out all of humanity.
And then within the industry, it's also not as big a theme.
There's not discussions of P-Doom or the probability that AI could kill us all, as is much more common in Silicon Valley and sort of the US AI scene.
So calls for a slowdown, for example, depend on your views of this sort of imminent broader threat, I think, in part.
And so, at least on that front, I think the Chinese side is a little bit not only skeptical, but even wondering if this is sort of a broader ploy to slow China down, specifically, not to have a mutual slowdown for the benefit of humanity, but building on previous U.S.
export controls on semiconductors in particular, I think.
And then also more recently, a number of statements from Anthropic and especially from Dario Amade framing the AI race as an as almost sort of this existential struggle between democratic AI and authoritarian AI and his sort of doubling down on wanting to use export controls almost kind of like as a form of leverage or at least to tighten them to generate leverage for the US side.
I think all of that has been interpreted by a lot of folks in Beijing and elsewhere in China.
That, you know, is this for real or is this sort of a trick to get China to slow down?
And the funny thing is, I see some parallels with the climate change story, where in sort of the early years of climate negotiation, there were efforts to try to get China to come to the table to figure out a way of committing to carbon reduction and maybe co-investing or building up a mutual financing mechanism.
And the refraint from the Chinese side was often that they did not want Chinese development to be slowed down in order to deal with this problem that they saw as mainly created by the West.
And the analogy is not perfect here, but there were even fears in China back then that that also was a ploy to nearly slow China down rather than, again, to address this broader global issue.
So I think that's some of how this is being interpreted by the Chinese side.
Why do they not share our fears, the fears that are prevalent in most U.S.
debates about that existential risk?
Is it some difference in how they view technology?
Is it that they're right and we're simply wrong, that their reaction here is simply incorrect?
Is their suspicion of the U.S.
overriding every other consideration?
How do you understand that?
And if you have to associate yourself with one view or one level of anxiety, where would you put yourself?
So I can throw out two factors, and then I'm sure Helen has some interesting takes on this.
But I do think one of the major differences is just the speed of development in AI in the two countries.
I do think that Chinese AI researchers see things moving at a slower pace and don't feel that imminent sort of escape velocity about to reach them.
Whereas I think maybe for some of the American AI researchers, they feel like, especially given greater compute, faster development, more powerful models, maybe they feel that it's closer.
But at the same time, and this comes to the second factor, at the same time, I think U.S.
AI researchers were worried about this a lot earlier, even back before really, really powerful models that we see today.
And I think maybe some of that stems from a different kind of culture around technology and around AI in particular.
I mean, this is going out on a limb, but even the kind of sci-fi literature that the two countries tended to dig into, right, in the U.S., pretty much every, you know, many books, many films end with some form of machines killing us all or trying to kill us all.
And that is like a key Hollywood plot driver.
And also, you know, big in the sci-fi literature as well as the nonfiction literature versus in China, I don't think those narratives were as dominant.
And if anything, you have, you know, stories like the three-body problem, where the question is not, you know, how do we control this technology that's getting out of hand, but how do we continue to make progress on technology despite maybe other people, other entities trying to slow us down, right?
So it's about catching up and making progress and not wanting to fall behind.
So if there's a close to existential dread in China, it's more that than the Terminator vision of the world.
The extent to which sci-fi has shaped this entire debate is fascinating and a bit terrifying if our future is in the is in the it depends on which um which crop of sci-fi writers is correct helen i i'm i'm curious in your answer to that why question but i also want to go back to a piece you wrote three and a half years ago and as you know a lot changes here where you poured a little bit of cold water on on u.s fears of chinese ai progress at the time you said that it was uh those fears about chinese capabilities were overblown.
So I'm curious if you see changes there as well as how that's affected this basic view of ai risk, as Kyle was laying up.
Yeah, it's really hard to overstate how much of the US AI world, especially the kind of frontier AI world, the leading edge, most advanced AI developers, stem from quite a specific intellectual community that developed well before, you know, well before ChatGPT, well before even deep learning and deep neural networks were starting to work well in the early 2010s.
This is more kind of in the 90s and 2000s, kind of futurist type of thinking about what artificial intelligence might look like, what it might mean for the world, how it might work.
And I would argue that this kind of sort of big picture, technical, societal, philosophical, political thinking, which is certainly allowed, maybe also to some extent fostered in the US system, is really not what the Chinese system wants its engineers and scientists to be doing.
So I think it's not a coincidence that we had that community arise in the US and less so in China.
And I think that community, there's sort of different pieces of this.
On the one hand, it's quite insular and makes a bunch of assumptions that may or may not hold.
On the other hand, I think a lot of the sort of assumptions and predictions and expectations that have come out of that community have been fairly prescient.
So I think kind of trying to build AI systems that are extremely capable across the board, expecting that AI will get more agentic, meaning sort of more inclined to, or able to take actions, able to carry out complex plans, not just something that is kind of passive and tool-like, thinking of AI as something that could far surpass human capabilities, but I think we're starting to see glimmers of in certain areas.
I don't want to say that this sort of this little community that grew into Demos Sassabas of Google DeepMind, Sam Altman of OpenAI, Dario Modi of Anthropic, you know, these people were all shaped by it.
I don't want to say this community is always correct, but I think they've been pressing it in important ways.
And I just think that has been much less true in China.
So I think sort of in addition to the sci-fi factor, which I think is maybe more affecting, I would say more affecting sort of public perceptions, I think in terms of the people building this technology, my experience when I talk to Chinese AI engineers, researchers, and others is they are just much more straightforward engineers or straightforward scientists, as opposed to these sort of big thinkers who are, you know, doing more.
So pros and cons on both sides, but I think that is another kind of distinction worth naming.
What about the pace of Chinese progress on AI, which you were a little skeptical of a few years ago?
Yeah, the core of that piece was not so much about saying, don't worry about Chinese AI, they're not going to do well.
The core of the piece was really about saying the fact that China is relatively close behind the US should not be a reason for us to not regulate our own industry.
And I think the core argumentation there still holds, which is we should not treat the speed at which the two industries are developing as totally independent.
That is to say, it's not like a hundred meter sprint where if one runner just stops running, the other runners are going to continue at exactly the same speed.
I think it's much more like a Peloton in a bike race where you have a group of cyclists and the front rider is taking on more work to kind of lead the pack.
And what that means is if that front rider, in this case the US, slows down, two things might happen.
One, the whole pack behind them might slow down because they're not able to kind of come out and overtake.
Or two, if the second rider, China in this case, comes out into the front, then they're going to suddenly be facing the headwinds that the US had been facing, if that makes sense.
So there's sort of a joke version of this meme version that I sometimes see get play on Twitter, which shows the US as a speedboat and then China as a water skier.
And then the speedboat says, they're catching up, we have to go faster.
I think that's kind of overstating the case.
It's not that the US is just fully pulling China along, and without the US, they would lose all momentum.
But my point in that piece a few years ago, which I stand by, is we should not treat it as though us doing anything to regulate or govern our industry domestically is purely going to let China just blitz past us, continuing at the speed that they have been developing.
The strongest version of that speed road analogy or Peloton analogy, if you want to use that one, comes from some of the leaders of the US industry who accuse Chinese companies of achieving most of their progress through distillation, which is using American models to train their own.
Has that been an important part of Chinese success so far?
Or do you think that's overstated by the American executives?
I think it is really, really difficult to tell based on publicly available information.
And that is something, so our team at CSET, Center for Security and Emerging Technology that I lead at Georgetown, our team at CSET has concluded that it's very hard to know how useful distillation is.
It's also something I've seen from multiple other independent commentators who are trying to assess: is this 90% of the story of how China's catching up?
Is it 10%?
I think we can say it's surely meaningful enough for them to invest kind of the time and effort to do it, because we are seeing very large-scale Chinese distillation attacks or distillation efforts, I should maybe say.
My best guess would be that it's not 90% of how they're keeping up, but maybe it's somewhere in the 10 to 50% range, but it's really very difficult to know.
I do think there's an inherent contradiction that we often kind of skim past of, for someone like Dario saying, on the one hand, Anthropic has been so vocal about distillation and really emphasizing how much of a threat it is.
And then on the other hand, Dario is saying, well, we can't slow down unilaterally because then China won't slow down.
You can't actually believe both things.
So maybe Dario disagrees with other people in the company about how important distillation is.
I'm not sure.
The other thing that is worth naming as well is the possibility of China just straight up stealing US IP if they wanted to, up to and including stealing the model weights and for leading US models and then just having copies of the AI systems.
the best AI systems.
In my mind, this really undercuts.
There's a narrative of, well, we have to win the US, the AI race, and so we have to go as fast as possible.
But if you're going so fast that your leading companies are hackable, which OpenAI and Anthropic and even Google certainly are by state-based actors, then all you're doing is just sort of creating a juicy target for China to come in and take.
And then you haven't won any race you're not leading.
You've just kind of handed them something valuable.
So I think we, yeah, I think there's lots of ways in which the assumption that China would just blaze past us if we slowed down and therefore we have to go as fast as possible.
I don't think that's a good model of the situation.
Kyle, do you see other advantages that Chinese labs and the Chinese state more generally has over the United States?
Yeah, I think overall, this very efficient cost structure is something that is sort of born out of necessity, but has turned out to be useful at least for keeping up and doing so at a much lower cost.
So yeah, I mean, to take Helen's analogy, I like this sort of Peloton view, where also I think if we add the data center part, it kind of like really makes this very stark.
Where in the US, right, we are investing extremely heavily in building out compute.
And that gives us a lot of advantages, especially on training the frontier for multi-trillion parameter or maybe a 10 plus trillion parameter models.
So these are very, very sizable models that would be difficult to develop without the kind of compute that we see in the U.S.
And compute, just to be precise about this, because I think those of us who are not expert in this throw it around, but often have a kind of a hazy view of it.
It just means the amount of computing power, the amount of semiconductors and power going into training and processing as possible.
Exactly.
Yeah, that's right.
Yeah.
And so I think what's happened is it's become increasingly challenging to continue to scale compute at sort of like on an exponential curve.
Like that is an open question as we see some of the physical constraints coming to bear on the data center build out, much less some of the political and social constraints, including like the local community backlash and political opposition to data centers.
There will have to be sort of like real world limits to that to that growth and expansion.
But in the meantime, the US hyperscalers and the US AI companies are pushing very hard on that.
And for the Chinese side, I think what's interesting is they are trying to do something similar, but are able, as Helen mentioned, to kind of draft behind the US on some of these ideas, but then also to innovate on the model efficiency side and come up with these interesting tricks for model architecture to reduce, say, memory usage or to reduce just overall computing costs for not quite the same level of capabilities, but almost as good.
And so what you then see here is, I mean, there's got to be some other good analogy where it's like on the US side, you're kind of like working out as hard as you can in order to be like 10 feet ahead.
And then the Chinese side, you're not having to run or work out as hard, but you can kind of still keep pace, roughly speaking.
And yeah, and then what that means concretely on the Chinese side in terms of why they have that efficiency, it's not just sort of the model architecture, but also, you know, their cost for building out equivalent, at least in terms of energy scale data centers, is much lower, even if their chips are low performance.
Their cost for running models is lower, and their cost for employing the talent, these are all lower.
And then on top of that, on the application layer side, in terms of building out AI applications, you also have some state support, like local governments will offer compute vouchers to allow local startups to get access to chip clusters that they otherwise wouldn't have.
So these are all sort of reasons why, like to Helen's point, I don't see these as helping China get ahead of the US, but I do see them helping China sort of keep pace and do it at a much lower cost level and a much more sort of economically sustainable way.
Although, of course, you know, the last caveat there is the Chinese AI companies themselves are under huge pressure to make money.
And they're not making the billions of dollars that the US AI companies are making.
So, you know, they may be spending less, but they're also making far, far, far less.
Yeah.
And that's in part because if they're releasing their models as open weight models, people can just use them much more cheaply.
They don't get the automatic revenue of every time someone wants to use one of their models, they have to come to the company that developed it.
And I was going to ask you about the emphasis on open weight that you see in China.
I think the discussion, again, among non-experts, is that this reflects a difference in kind of understanding of artificial general intelligence or superintelligence and whether it's worth being kind of obsessed with reaching some kind of threshold where a step change happens.
Is that the right way of thinking about it?
And what kind of accounts for the Jemerson approach between the U.S.
and Chinese AI ecosystems?
I'm not sure I would put it that way.
I think in many ways it's just the logical strategy for the follower.
It doesn't make sense for the leader to open source their models or open weight their models because it's all sort of downside.
But if you're a follower and you're trying to make a name for yourself, you're trying to show, hey, here's what we got, releasing your models weights is one of the best ways to make people actually pay attention.
So I think that is a huge part of the strategy.
At this point, I think there is also some identity stuff tied up in it.
It's going to be really interesting to see if the Chinese state changes posture towards that at all over time.
I read, so Xi Jinping gave a big speech at the World AI Conference in Shanghai in July, which included some discussion of kind of open development, but also I think left him and the party space to kind of change and adapt whether the very most advanced models are released openly or not in the future.
So that'll be something that's interesting to watch.
Kyle, how much do we know about what Xi Jinping thinks about AI?
We have the speech Helen mentioned earlier that he's quite influenced, or we think he's quite influenced by the Minister of State Security in a highly personalistic centralized system.
Ultimately, his views of a 70-something man are maybe determinative.
What's our sense of how he understands the issue and thinks about the issue?
So it seems like, in general, Xi Jinping's approach and Chinese policymakers' approach to AI is really, really reminiscent of how they try to approach the internet and other general purpose technologies like digitization and IT systems.
Going back through earlier five-year plans from China, you can see sort of the mania around the dot-com boom in China about trying to have intelligence systems everywhere and trying to digitize, especially traditional industries, outdated government systems to try to bring them to the 21st century.
And now I see a lot of that language and a lot of that playbook being deployed for AI.
One thing that is different, though, is it does seem that AI is not merely one of a number of different important technologies for China, but it has become sort of more foundational to China's sort of tech and industrial strategy going forward.
And I think in that way, yeah, the way I would put it, and I've sort of phrased this before, is while I don't think Xi Jinping is AGI-pilled, that is, I don't think Xi Jinping believes that superintelligence is around the corner.
I do think he is very AI-pilled.
That is, he does believe that AI can be fundamentally transformative for China's performance in a whole bunch of related industries from healthcare, education, and then especially military.
We'll return to my conversation with Kyle Chen and Helen Toner after a short break.
What if you could explore places in the news like a reporter does?
I'm Nicholas Wood, a former journalist with the New York Times and BBC.
And 16 years ago, I created the travel company Political Tours.
Our small groups are led by top correspondents around the world.
In the next few months, we're off to Mexico, followed by South Africa, Japan, and the French presidential elections.
Come and join us.
Go to politicaltours.com.
That's politicaltours.com.
Foreign Affairs Group subscriptions give your organization access to all of our trusted content in more ways than ever.
With a wide range of critical views, Foreign Affairs prepares your community to consider and discuss the most pressing challenges of today.
Students and employees can read or listen to the latest articles on campus or in the office, anytime, anywhere.
Join top universities and institutions around the world with a custom plan tailored to your organization's needs.
Learn more at foreignaffairs.com/slash group.
Helen, you wrote in Foreign Affairs a few years ago, I think in that same piece, about the Chinese political anxieties around AI and the ways in which AI could threaten the security of the Communist Party and the control of the Communist Party.
What is the state of those fears now?
I mean, I think that's another difference between the way U.S.
and Chinese governments at least think about the threats from this issue.
What is the state of those fears now, and how is China trying to manage it?
That is one area in the piece from 2023 that I have changed my mind on.
I wrote in the piece at the time that I expected this to be a significant barrier to Chinese development and adoption of AI.
Basically, you know, the fact that language models produce text and it can be quite difficult to constrain them.
But what we've seen since then, as Kyle said, China has taken the regulatory apparatus it built up for the internet and for censoring the internet, has turned it onto AI with pretty good effect, I think, from the Chinese state's perspective.
They have focused on publicly available private.
So it's actually quite interesting to look at if you compare, for instance, DeepSeek, if you interact via the DeepSeek website or the DeT app versus DeepSeek model that you download, an open source version of or an open weight version of, they often behave somewhat differently because there's so many more constraints on products that are publicly available in China.
But yeah, I think this is, I think it's turned out to be more feasible than I would have expected.
Maybe part of this is just they are not that worried about people who really go out of their way to jailbreak a model and try to get it to say things that it shouldn't say.
Maybe that's not so different from their perspective from someone who figures out a way to get a VPN and then is reading the New York Times and CNN and reading bad things about Xi Jinping.
Then the next sort of their next layer of defenses kicks in, which is like, okay, if that person starts trying to post about it on Chinese social media, then you have the existing repertoire of controls.
I do think one thing that you've seen in some commentary over the past few weeks, Chinese commentary about U.S.
fears in the space as well, is China does have this pretty robust regulatory apparatus.
And I think they're somewhere between perplexed and suspicious that the US is making such a fuss about these risks and has what China sees as almost no regulation in place.
There are some state laws that are starting to take effect.
It's not absolutely blank slate, but that is also something that I think they are looking at with somewhere between confusion and suspicion.
Mistaking incompetence for malice or dysfunction for malice in this case.
Yeah, maybe it's all a psyop because Congress can't get its act together to pass regulation, and so therefore the concern must be fake.
Kyle, what's your sense of the extent of these fears on the part of Xi Jinping and Chinese leadership when it comes to those political risks?
So I think that AI kind of reveals this pendulum swing that is constantly happening in China and among Chinese policymakers between their two top priorities, control and development.
And I think for AI specifically, you see this pendulum going back and forth.
There are times like when ChatGPT first got released, where the pendulum swung towards control.
And I think that's when Helen was writing.
And the concern was, yeah, that they would start, these AI models, these chatbots would start to say all the wrong things and produce all this content that could go viral and maybe cause social instability, maybe start up a protest movement.
And once they start to build up the regulatory regime to control that, maybe they start to feel better on the control front.
And then on top of that, they also felt like they needed to catch up.
The funny thing is, DeepSeek was talked about as a sputting moment in some ways for the US, but China has faced at least two of its own sputting moments on AI, vis-à-vis the U.S.
And one was ChatGPT, the other was AlphaGo.
When AlphaGo beat the human world champion in the ancient game of Go, that really stunned a lot of people in China.
And it really lit a fire under the Chinese policymakers who felt like China's going to miss the next major technological revolution.
And so you can see them alternatively hitting the break and hitting the accelerator.
And right now, I think it's a really interesting moment where potentially, potentially, the pendulum could be starting to tilt back at least in the other direction, rather than merely going all out and trying to catch up with the US and trying to show that China can be a peer on this technology, now I think the risks are starting to grow to the extent that some of that control instinct is coming back.
And I think you see that in some of the language from Xi Jinping this summer, you see this with growing statements about AI risks in sort of higher ups in the party state apparatus.
You know, you both alluded to the different ways of understanding the intersection between AI progress and geopolitical influence.
Chinese and American policymakers seem to have a different view of this.
Helen, to the extent that we have a clear understanding of it, how would you describe the Chinese view of what it means to be a leader globally here?
What really matters in that competition to the extent it can be described that way?
It looks to me like there's different answers within the Chinese system and different answers within the US system.
I'm not sure that either system is fully cohered on one answer here.
The starting point, and I'd be curious, Kyle, what you would add here.
The starting point for most things that I see is looking at AI as part of a fourth industrial revolution.
Basically, China seeing itself as having missed the first three industrial revolutions and wanting to be a leader and a pioneer in this new fourth industrial revolution.
So that's a pretty cross-cutting, broad scope way of looking at it that's about regaining prestige on the world stage, being seen as a technical leader more than it's about kind of any individual specific impact on China.
I guess the other big lens that you see them talking about is AI as a driver of prosperity, as a driver of economic growth, even as a time when society is aging.
Of course, there's lots of other impacts that they talk about on many different specific sectors, but those are the two overarching lenses that I see over and over again.
Kyle, I'm curious what you would add to that, but especially whether you see the, I think the crude view in the policy community is that Americans are obsessed with AGI or superintelligence and kind of getting that frontier and being in the lead.
And China is much more focused on getting less advanced but more affordable products out to the rest of the world and integrating it into the tech stacks in the global south and elsewhere.
Is that crude view right?
And anything you would add to Helen's understanding of the different views of this?
Yeah, I think that's right.
I think in general, the concept of a decisive strategic advantage of whoever gets to a certain threshold of AI capabilities, especially as it relates to AGI or superintelligence, or especially if you can get this recursive self-improvement feedback loop going, that is AI systems that improve themselves.
If you can really get that going and accelerate that, then whichever country gets there first will have super intelligent systems that could potentially have super smart military weapon systems, could have dominant cyber capabilities, could basically come to rule the world.
I mean, I like put it so bluntly because I think that does kind of reflect the stakes that many in Washington feel when it comes to why the U.S.
needs to lead in AI.
It's not just about, you know, people sometimes ask, like, why does it matter if China's like six months or 12 months behind?
And I think for some people, it's because, like with nuclear weapons, whoever gets there first will have such a powerful margin over everyone else that it makes almost everything else less relevant.
And I don't think that's how it's seen, at least among Chinese policymakers.
There are some of the Chinese AI labs where their founders will speak in a way that sounds very reminiscent of the American AI community.
They'll talk about things like HEI or recursive self-improvement and talk about wanting to achieve that goal.
But more broadly, that is not really such a dominant paradigm in the industry and certainly among Chinese policymakers.
So I think for them, when it comes to like what does it mean to win, I think they really want to see the ROI on AI.
It's not just enough to have this transformative capability.
And once you get there, everything else sort of falls into place.
It's really sort of like the block and tackling of integrating it into more and more areas and then getting that economic boost or that productivity boost, as Helen was also referencing, where right now, especially given that the old engines of growth have faded, as they often talk about, with the real estate market collapsing and those old manufacturing and traditional industries no longer able to drive growth like they did in the past, China's looking to technology and especially AI itself as being that key factor driving it forward into the future.
Helen, I'm curious, not so much which of those two views you see as right, but what will determine which one is right?
If the you know, the Washington view that Kyle articulated turns out to have been had been Prussian, had been the correct understanding of it, what assumptions will that camp be making that the other camp might not have fully understood but should have?
I think the assumptions are all around: is this a, not even a marathon, but is this just an ongoing open-ended competition where you need to be in it for the long haul and where it doesn't necessarily matter that much if you're half a length in front of the next runner or you're half a length behind, you just want to be up there near the front of the pack?
That would be more sort of the Chinese view that Kyle articulated.
Or is this really something with a finish line where you have to be blitzing to the end?
And I think this is actually a source of why US-China discussions on AI are not quite congealing, which is to say, I actually think that on the US side, you know, in high levels in Washington, people also don't buy this view that there's a finishing point, you know, an end state, which is you hit recursive self-improvement first, you foom, as they say in the industry, you do an intelligence explosion until you have superintelligence.
I think that's not the view at the top levels of either country's government, but I do think it is a big part of why you see OpenAI and Anthropic, especially feeling such time pressure to go as quickly as they have to.
So they feel this race dynamic.
They feel if they fall behind each other, you know, if Anthropic fears open AI getting ahead, OpenAI fears Anthropic getting ahead.
And so that's why I think you see some of these incidents we've had over the summer, which, in my mind, the root cause for those incidents was rushing.
People have kind of fought over: did those incidents happen because the AI was getting so advanced, or did those incidents happen because of sloppy cybersecurity practices?
And I think the answer is both because the companies have been rushing.
So, all that to say, I think if you're operating in the recursive self-improvement mindset, then you are inclined to that kind of reckless, we have to get there first at all costs kind of mentality.
Whereas if you're expecting to be in more of an open-ended competition and perhaps expecting that the US and China are going to be both up there, you know, as two of the leading countries, but it doesn't necessarily make sense to try and pick one as the winner and say the other one is the loser, I think that does mean you make a pretty different set of risk trade-offs, pretty different set of investments to set yourself up for a successful future.
If I understand you correctly, look, I share your understanding of what senior people in U.S.
policy circles think about this, that the kind of caricature that I laid out is not what you hear from at least senior people in Washington.
It sounds to me like we're projecting private sector interests or conflating private sector interests with understandings of national power here.
That it may be true that anthropic or open AI, it's that whoever gets there first will be the other, but that's different from saying the same is true of the US and China.
Yes, I think that's right.
You know, my personal view would be that neither of these perspectives is quite right.
I don't expect recursive self-improvement to be a finish line where whoever gets there first has kind of won the future.
But I also think that the opposing view, in my mind, often understates or underestimates basically how crazy things could get as AI gets more advanced and how powerful, how much advanced AI systems could affect the world and the ways that could go wrong if we are not really confident that they're working in ways that we want them to work.
I expect that there will not cleanly be one of those two views which will end up panning out.
I suspect it'll be messier and more confusing and more chaotic than that.
Kyle, as you, of course, know, there have been calls from American politicians, Bernie Sanders probably being the most prominent, to truly stop the development of some of the most advanced AI systems.
Private sector leaders have talked about pacing the frontier, kind of unilaterally slowing some of this development.
What exactly that means could mean a wide range of things.
How do you think China would react to that kind of unilateral move either by the U.S.
government or by U.S.
companies?
I think it would actually bolster, on the one hand, a lot of the arguments about trying to work together on AI risk.
Because I think, as Helen had pointed out earlier, from the Chinese side, there's a lot of sort of like, well, you're telling us to slow down, but you guys are going full steam ahead.
So that doesn't really make sense.
You know, what are you really up to?
And I think from the Chinese side, I do hear a lot about, you know, if you're serious, if the U.S.
is really serious about this, why don't you take the first steps?
And I think without necessarily playing into what China wants just for our own U.S.
national interests, we want to think about how to do this right.
And it's not just a pure race with China.
I think there can be an overfocus on that one kind of risk.
I do think there's a risk of falling behind.
You know, I've said publicly in congressional testimony that we want to be ahead.
There are advantages, like on cybersecurity, we want to have better models earlier than the Chinese do.
That's important.
But we have to balance now these risks because it's not just a one-sided risk.
We have to balance the other risks, and this is what Helen was talking about: of things getting out of control, of getting sloppy in how we develop these models and how we develop these AI systems, and using the race dynamic as justification to say, well, it's okay if we kind of mess up and they escape from their sandbox and we have the better cyber capabilities after all.
I think we have to look at all these risks and figure out: there's not an easy answer.
It's going to have to be a trade-off in some cases, but in some cases, also we can do things too that keep us in the lead and also make us safer or at least make this AI development process more sustainable in the long run.
Helen, do you see any meaningful prospect of true global multilateral action in managing the risk?
There was lots of talk about AI and AI governance at the UN General Assembly last week, but it's hard to imagine given the state of geopolitics that will get a ton of traction, but maybe I'm being too pessimistic.
To be honest, I don't actually see the need for truly international global governance, especially in the sense of kind of regulating or risk management here.
I think there's one kind of international sort of cooperation and governance that happens very much at sort of the technical working level.
So things like what are the data standards for autonomous vehicles or like, you know, as AI is being integrated into medical devices, how do we think about reciprocal approval of medical devices in different countries?
You know, that kind of thing, I think, will proceed at the working level the way that it does for other technologies without meeting sort of high-level political blessings.
I think, though, if we're talking high-level risk management from AI, I don't necessarily see that as a global problem.
On the flip side, though, an area where we could see or where there could be space for global or international engagement would be on realizing benefits from AI, distributing benefits from AI in a way that goes beyond just raising the productivity of SP 500 firms, but really is about empowering people around the world, trying to cover countries where there's fewer language resources.
And so language models might not by default work as well in those areas or other things like that.
That to me feels more promising than trying to go for some kind of governance regime, which I think has a lot of downsides in terms of centralization and coordination costs.
And I don't see the upside personally in needing to get a really international risk management regime right now.
Kyle, do you share that view?
That's a relatively sanguine view in its way.
Yeah, so I don't know what the prospects are for like a global governance system, but I do actually think that the U.S.
and China specifically need to work together to some degree on these AI issues.
I agree with that, to be clear.
Yeah, I mean, part of this is down to kind of like tactics and strategy.
Like, ultimately, there are two countries because of the capabilities of their models.
There are two countries that really matter here.
And I have like tried to get away from the nuclear analogy so many times, but I keep coming back to it for many obvious reasons.
But when it comes to nuclear arms control, it is the countries with nuclear weapons or on the verge of getting nuclear weapons that have the most say, like realistically, in the matter.
And I think in this case, unless you have a frontier model of your own and you are adding to the both upsides and the downsides of global AI risk, it's hard to really have a seat at the table.
On the other hand, for China and the U.S.
in particular, even though the likelihood of real significant cooperation is very, very low, I think there are some steps that can be taken that would be sort of like low, relatively low cost for each country.
So they can continue to distrust each other.
They can continue to want to withhold most information from each other.
But that could still have some meaningful payoff.
And one of those actually is this new incident notification mechanism that apparently the two sides have agreed to, especially between Scott Besson and his Chinese counterpart, Ho Lifeng.
And that is meaningful, not because I expect China to disclose incidents of hugging face from their side to the U.S.
should a major episode arise, which would not be implausible, but because it at least creates opportunities to reach out to the other side if the moment should arise.
So you can imagine, and this is a scenario that I think is pretty realistic: a case where a Chinese model accidentally attacks a U.S.
company or even a U.S.
government system, or vice versa.
And already we see cross-border cyber attacks driven by AI that were not intended.
And so, in those sorts of cases, you know, is it better to have sort of no channels of communication and hope that the issue can just sort of be resolved each country on its own?
Or is it better to have one, however tenuous it might be, to at least try to begin the process?
And so, yeah, maybe I'm too optimistic about this, or maybe I'm too pessimistic, depending on how you look at it.
But I do think that there are some steps that are, you know, they're not win-win, but they're not lose-lose is one way I would put it.
So, a scenario might be a Chinese agent on its own takes down, I don't know, a New York City hospital system, and you'd like the Chinese government to be able to call quickly and say, we didn't do this deliberately, and we're going to help you fix it.
Something like that would be the optimistic way this goes.
Yeah, yeah, exactly.
I mean, who knows if that would really happen, but to not have any channels to have that communication, I think would be riskier.
Helen, let me close with what may seem like a meta question, but I think it's an important one.
And you've alluded to this at various points in our conversation.
You've spent the last many years talking to people in the US government, the US policy community about AI and about these issues.
You spent some time talking to Chinese decision makers as well and trying to at least read and listen to the things that reveal their thinking.
Do you see the quality of policymaking improving at the speed that it needs to or at anything approaching the speed that it needs to, given how these are moving?
What's the kind of state of the policy process here as you look at it from Washington?
I mean, it's a cliche, of course, that technology moves fast and policy moves slowly.
I think people often think of that as sort of there's these two things going at a certain speed, and if one isn't keeping up, then it's going to fall behind.
But as you know, the way policymaking often works is in fits and starts and punctuated equilibria, meaning everything is, nothing seems to be changing, and then suddenly all at once everything changes.
So I can't say I feel amazing about the state of policymaking on this.
I do think that there's a long way to go.
I also think, though, that the problems being caused by AI and the potential future risks, our grasp on what those are and what we could do about them is also changing over time.
And so I don't feel like there's clearly a regulatory regime we could have put in place yesterday that would manage all these risks great.
I think the kinds of regulatory steps we could take now are primarily about setting ourselves up to respond better in the future.
So things like incident reporting or disclosure of risk decisions that companies are making internally, tests that they're running, things like that.
And I do think that there has been serious progress in policymakers being willing to engage here.
It's a complicated set of topics.
There's been a ton of, I'm sure Kyle has seen this as well, ton of interest from quite senior policymakers the past, even just the past few months in saying, wait, what's going on here?
How do we understand this?
What can we do about this?
And I think that means that if there is a point at the future where there really is finally a moment where there's enough energy to do something, the chances that that something will be well targeted have gone up, you know, based on people engaging more over the past few months.
Have they gone up enough?
I'm not sure they have, but it's progress at least.
That is a good note to end on.
Helen, Kyle, thank you so much for joining me today and for the work you've done on this for Foreign Affairs and lots of others over the past few years.
My pleasure.
Great to talk to you.
Thank you for listening.
You can find the articles that we discussed on today's show at foreignaffairs.com.
This episode of the Foreign Affairs Interview was produced by Adelaide Parker, Adrienne Feinberg, David Cortava, Ben Metzner, and Kanishkaroor, with audio engineering by Todd Yeager and original music by Robin Hilton.
Special thanks as well to Arena Hogan.
Make sure you subscribe to the show wherever you listen to podcasts.
And if you like what you heard, please take a minute to rate and review it.
We release a new show every Thursday.
Thanks again for tuning in.
We hope you enjoyed this episode of the Foreign Affairs Interview.
Don't forget to visit foreignaffairs.com/slash spotlight to sign up for Dan Kurtz Valen's free weekly newsletter featuring more of the clear-headed analysis that you enjoy here on the podcast.
Sign up today at foreignaffairs.com/slash spotlight.
