---
record_id: "podcast:b078064f-2790-4559-a5a8-104f22752fb1"
episode_id: b078064f-2790-4559-a5a8-104f22752fb1
title: "Building Defense for the Agentic Era: Kevin Mandia"
podcast_title: The a16z Show
url: "https://pocketcasts.com/podcast/the-a16z-show/20a7ca40-9128-0131-8b7f-723c91aeae46/building-defense-for-the-agentic-era-kevin-mandia/b078064f-2790-4559-a5a8-104f22752fb1"
audio_url: "https://pocketcasts.com/podcast/the-a16z-show/20a7ca40-9128-0131-8b7f-723c91aeae46/building-defense-for-the-agentic-era-kevin-mandia/b078064f-2790-4559-a5a8-104f22752fb1"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-10-06
played_at: "2026-10-06T12:00:00Z"
play_count: 1
duration_seconds: 2940
source: pocketcasts-history-browser
played_label: October 6
history_order: 3
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: c697ce7321c3253b31a820a246739150d0b87b3f37bb7986eaef72b7c36eb9e3
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

Kevin Mandia, David George, David Slater, Travis Lanham, Evan Pena, Armadin, Mandiant, Google, CrowdStrike, Pan, Fortinet, Fortune 500 companies, Iran, Russia, Mythos, Hugging Face, and OpenAI are named in a discussion about AI’s impact on cyber offense and defense. Mandia argues that AI has made traditional security experience largely obsolete because attackers can operate at machine speed and scale: what would take 70 humans, AI can do in a microsecond; he describes AI attacks as drone swarms rather than nation-state sniper strikes, notes that open models are already good enough for serious cyber risk, and says anonymous GPU availability could sharply expand criminal attacks. Armadin’s model is “Armadin Red” plus “Armadin Blue”: use frontier models and post-trained red-team agents to continuously attack customer networks, map every service, route, system, and asset in a “hyperattack,” create a metadata twin, poll for change like a heartbeat, and then attack changes, new CVEs, or new threat intelligence. Key claims include Armadin finding more than 90 zero-days at customer sites since January 2026, all in production at major companies, verified through black-box remote code execution or data access rather than source-code scanning, with CISOs contacted within about 48 hours. The conversation also covers why pen testing is too shallow, why autonomous defense and compensating controls are necessary, why attribution will blur between humans, criminals, and nations, and why SOC workflows, prevention, detection, and response must collapse into faster AI-driven loops.

For the user, the actionable takeaway is to treat periodic pen testing as insufficient and consider continuous AI-driven offensive testing that proves real exploitability, not just known vulnerabilities. Decisions to evaluate include whether to adopt continuous red-team-style testing, how to integrate findings with endpoint, firewall, EDR, and network defenses, whether to allow autonomous compensating controls such as rapid blocking or virtual patching, and how to handle zero-day findings as incidents rather than compliance items. Research leads include post-training offensive security models, metadata mapping of networks, change-triggered testing, false-positive reduction, autonomous response governance, and the future role of the SOC. Follow-up questions should ask: How quickly can we detect and contain an AI-speed intrusion? Which defenses can act autonomously without human approval? How do we measure exposure windows between vulnerability disclosure and remediation? How do we distinguish verified exploitable risk from noisy vulnerability scanning? How should attribution uncertainty affect response policy? No direct health implications are present in the supplied material; the practical consequences are cybersecurity, operational risk, governance, and organizational readiness decisions.

## Transcript

If you don't have a defense unless you have a great offense to go up against, you want to be the Baltimore Ravens defense of 2000.
You kind of want to have your practice offense really push you.
That's what Armadin's going to do.
We're going to be the all-star team on offense coming at you so you can train your defense with what we're doing.
But you built Mandiant, a great success.
Why did you decide to get back on the field?
I don't want to sit out the AI shift change when I've done 30 years in security and the whole damn thing's about the change.
What AI does in a microsecond would take 70 humans.
They can't even do it.
It's apples and oranges.
This is a tsunami like has never been seen before in security.
The whole, let's slow down the models.
We don't want cyber risk too late.
The open models are already good enough.
Armadin, since January of this year, we have found over 90 zero days at customer sites, all in production.
This is not like rinky-dink companies, like these are like Fortune 500 companies.
The differences or similarities between nation-state attacks compared to AI today and then where you think AI can be in a couple of years.
On the defensive side, we're going to say, we're being attacked by these models, but we're not sure who's behind them.
Is it a nation?
Is it a human?
Is it...
Kevin Mandia has spent 30 years in cybersecurity.
His view of the AI transition is simple.
Everything I did is dead, and then everything else is new.
In this episode, David George sits down with Kevin, founder and CEO of Armadin and the founder of Mandiant, to talk about what happens when cyber attacks move from human speed to machine speed.
Kevin explains why AI gives attackers an immediate advantage, from probing thousands of paths simultaneously to making less sophisticated attackers dramatically more capable.
And he makes the case that there's only one viable response.
Defense has to become autonomous too.
We also get into how Armaden uses AI to continuously attack customer networks.
What the team has learned from finding more than 90 zero days this year, and why Kevin believes the next two years could remake nearly every layer of the cybersecurity stack.
Kevin, thanks for being here.
No, thank you.
Okay, so you built Mandia?
Yes.
Obviously a great success, many different chapters.
You know, it ended up inside of Google ultimately.
Why did you decide to get back on the field?
It's a good question.
And I don't know if I decided it, and that'll sound weird, but I met with David Slater and with Travis Lanham, the other founders, and Evan Pena, I knew.
I could say they started this company.
They are the founders.
I met them.
They had the idea.
They pitched me on what they wanted to do.
And I saw the talent in them.
Travis is a generational talent.
David Slater's, and I mean this in a positive way, freak of nature.
These guys are really, really good.
Evan Pena is exceptional at what he does.
And when you meet that team and you talk to them, the whole time I was listening to what they were doing, I was thinking, I want to be a part of this.
I don't want to sit out the AI shift change when I've done 30 years in security and the whole damn thing's about the change.
That's great.
Everything I did is dead and everything else is new.
But meeting that team and they were starting the company and me realizing I think I'm a real good fit with these guys to accelerate the need.
What Armadin is building, every company needs now.
And I was like, this team that can build it, and I think I can answer the now.
30 years in security, you meet a few people.
Let's go to those people and say, we've built what you need.
So I almost felt compelled to do it.
I know that sounds weird, but I would not have founded a company again in mid-50s and I was doing venture.
It wasn't like, oh, I'm an entrepreneur and I love starting companies.
That's not it.
And it wasn't, oh, I'm not a VC, I'm just an operational guy.
That's not it.
I met the team and went, we have to do this.
I mean, that's really it.
Yeah.
And this whole AIC change was happening totally.
That's the capitalist, right?
Yes.
So tell us about what Armadin does.
So Armadin leverages frontier models in AI on offense to test: do you have exploitable risk?
And that's what we do today.
We call it Armadin Red.
But when we started a company, Travis and David Slater and Evan all knew the future of cybersecurity is going to be: A, the good guys have to build the offensive cyber cannon and shoot it at networks to make sure those networks can withstand these attacks because they're the ones that are coming.
But we also knew it's going to be AI on offense built by the good guys, working in training with AI on defense built by the good guys.
And you have to have both.
So our act one was: we got to be the best in the world at finding exploitable risk.
If we're five minutes ahead of the bad actor, whether it be a nation state, criminal, nuisance, if we're five minutes ahead of them, we also recognized our act two, Armadin Blue, we got to stop it.
Compensating control, tourniquet.
And so that's what Armadan does.
We're building the force field you will need in the AI age to defend yourself from AI attacks.
Yeah.
Tell us about the nature of the capabilities of AI attacks today and then where do you think it goes?
Well, great.
So, the nature of them is, first off, we're getting a weird window in time where we're seeing them, but not at the same level you'd expect.
I've seen nothing like what Armadan's already built in the wild, which is there's 25,000 agents on concert, all working together, doing really, really smart things without going on bizarre fishing trips.
Because when you respond to an AI attack, you can tell it's AI very quickly.
At least I can, because I've thought about a lot of offense.
I've responded to a lot of attacks in the past that were led by humans.
Right.
And a human goes to point A, then to point B, then to point C through their intrusion.
AI does little things like four or five differences, but one would be it'll break into point A, then laterally move to point B.
Next thing you know, it's trying to break into point A again.
Yeah, yeah, yeah, yeah, yeah.
It's like, I get the drone swarm, but you could probably coordinate and think a little bit better.
That's where it's at today.
It'll get better and cleaner.
But the differences are: first and foremost, the scale of what AI can do dwarfs humans, like in ways humans don't even get.
Right.
So you have a scaling problem in that humans could always find only one path into a network.
Yeah, they had to be selective because they had to devote their limited resources to one direct path, right?
Yes.
And then, so scale is a challenge.
Speed, ridiculous.
What AI does in a microsecond would take 70 humans.
They can't even do it.
It's apples to oranges.
And then, so, what was always lacking is AI creative or effective.
But when it comes to what we do, we don't need the fanciest model.
We're not trying to speak 400 languages with our models and all that kind of thing.
What Armadin's doing on offense is we're finding vulnerabilities, exploitable risk.
That is code.
That's a structured language, a structured process.
Because it's structured, AI is going to be great at it.
Right.
Right.
So, I really think it's already here today.
Like, the whole, let's slow down the models.
We don't want cyber risk too late.
The open models are already good enough, and these things are coming now.
It's just a matter of the minute you have anonymous availability of GPUs, you'll see far more criminal attacks.
Oh, interesting.
Yeah, you know what I mean?
But until you can attack anonymously, and it's hard to do crime when people know your name.
It's better.
If you can commit a crime anonymously, here's my tip for criminals: if you can commit a crime anonymously, that's a lot smarter than doing it with your jersey on with your name on it.
And so, anyway, the difference in attacks and what we're seeing now, we are at the precipice, first inning still, of AI-led attacks coming.
And I think that's just because of the cost and availability of the models is not as readily available to the criminal element as it will be in the future.
Yes, exactly.
Okay, so you, your experience working in the security industry for 30 years, you probably saw a fair amount of nation-state attacks, right?
Every day.
Every day.
So, talk about the differences or similarities between nation-state attacks.
And I use that just to say the most sophisticated, most successful, if you will, types of attacks compared to AI today, and then where you think AI can be in a couple of years.
So, everything's going to change rapidly, right?
But I can tell you, nations on offense have never, in my opinion, they've never really been when you're hacking for espionage and for security reasons, you hack with what I would call kind of a sniper round.
You're not spraying and praying.
For the most part, modern nations on offense restrict their targeting and they go deep at very specific things, like 30 defense contractors or dot mil, and they go hard at that.
Kind of think of it as that snipe around.
With AI, I think it becomes more like a drone swarm.
It becomes a little bit different in the cyber domain.
And I think even modern nations are thinking, what will our protocol be?
If we want to attack this company, do we swarm it and just burn tokens on it?
Because AI is going to do a lot of things humans just wouldn't.
So it's a little sloppier, a little louder, but it's more effective.
But it's more comprehensive.
That's the problem.
You got it.
It's more effective, probably.
And so there's going to be so many things a nation's got to think through right now.
And their whole doctrine will shift as the AI shift change comes.
Like, how does AI change what our mission is?
Do we maybe use the cyber domain differently?
Do we drone swarm sometimes, snipe around other times?
How do we balance the two?
Does it depend on risk, target, how surreptitious we want to be?
Because right now, AI is not a surreptitious action on offense unless you've done a ton of post-training.
You got maybe a human in the loop really looking at are we doing smart things?
Because if you just go, hey, here's a prompt, hack ABC.com.
AI is not going to do it in a surreptitious, smart way.
And I think even if you ask it to, it's still not going to until it's been really trained and really had some human influence on it.
So, but more generally, what you're going to see is less capable attackers, less technical, less successful, are going to appear way more successful.
It's the equalizer.
Yeah, because of the voice.
When you start using models, over time, what it's going to be is on the defensive side, we're going to say, we're being attacked by these models, but we're not sure who's behind them, those attacks.
Is it a nation?
Is it a human?
Is it, and we'll have some clue, but attribution will get a little difficult.
So that's a long-winded answer saying in the AI age, it does democratize far greater expertise for attacking victim networks.
Yeah.
So then that is a good segue back to Armadan.
So you have talked about the defense needs to be a great offense, right?
Yes.
Like the best you can do.
You got to train your defense with something.
Yeah, of course.
You got to train your defense with something, and then it needs to be continuous.
Right.
Right.
So, right.
So, how does the product work?
And then how do you get a level of sophistication such that you can identify and remediate these vulnerabilities like what you're describing that are more sophisticated than a basic prompt?
Okay, lot there.
I could talk for 45 minutes on it.
But first, I can tell you this: you don't have a defense unless you have a great offense to go up against.
You know what I mean?
Like, so even think in sports terms, if you want to be the Baltimore Ravens defense of 2000, you kind of want to have your practice offense really push you.
You know what I mean?
So that you know how good you are.
And that's what Armadan's going to do.
We're going to be, you know, the all-star team on offense coming at you so you can train your defense with what we're doing.
And that's that's going to be important.
And you can't really have a human in the loop in the AI age for tactical autonomous defense.
Like you got to do something fast.
You know, you got to tourniquet the wounds as fast as you can.
So thinking back to our, like, you want to be able to do it continuously, and that's the complexity.
So we do a thing called a hyperattack.
And David, that's just a fancy word for we throw a drone swarm of agents at you, and we map your network.
Every service, every route, every system, all assets.
We may end up with terabytes of metadata on your network from this hyperattack.
Done super fast.
Just it lights you up.
So that way we can now, it's almost like a metadata twin of what we can see.
If we're on the inside, do the same thing.
Let's just map everything.
This is the attacker's view of your network.
But with that metadata, we now just poll you almost like a heartbeat.
What's changed?
What's changed?
That's continually looking for: did an app change?
Did a route change?
Did a service get updated?
Did a new machine get presented onto the, you know, into the target area so that we can poll cheaply for change and then attack the change.
What you really want in the future in the AI age is that you want the constant pressure of models attacking you, but you can't do it all the time because A, it's not, it's cost prohibitive, but B, it's unnecessary.
Right.
You do it when either the threat changes, hey, new models come out, new intelligence is available, or B, your network changes.
So you want to test whether that happens.
And then C, you just probably just want to test, we have a board meeting tomorrow, let's see how we do.
Yeah, exactly.
Let's audit ourselves and see where we're at.
And that's what we had over the weekend, there was a zero day and a popular product.
And immediately, we've already got the heartbeat.
We just polled who's got the problem.
And our goal at Armadin is to go from common vulnerability or CVE to we can find if it's exploitable or not before bad guys can.
And not all bugs allow for human access to your system in a stable way.
So not all bugs are created equal.
And so we want to make sure: hey, this one's one you really need to worry about, or which ones don't give remote command execution.
So long story made short, that hyper attack, that metadata that we get allows us to kind of poll for change and attack you when your network changes.
And that's the best you can do for continual, and we'll get better and better at it.
And the cost for the polling will go down.
You know, it's on small networks, it doesn't cost much.
But on a network that changes all the time and it's very large, you'd be polling it quite a bit to make sure you don't have an exposure window.
Yeah, of course.
So that is actually a very good explanation for why this continuous approach matters.
Right.
It's so fun.
Like, you know, you and I share.
You're already up against it.
Somewhere out there, the criminal element will always have that random scanning, and they probably aren't even using AI for it.
They've got one exploit that they think works, and they're just kind of scanning the world for it and then coming at the exploitable risk, you know?
And so you're already getting some pressure on your network from an unseen force that's not well-intentioned.
You know what I mean?
So you might as well have a better force built by the good guys constantly putting pressure on you.
Yeah, it's interesting.
So you would kind of, Armadin, I don't know, a year ago, would probably be placed in the category of pen testing.
And you and I share history and relationship with George at CrowdStrike.
Right.
And so they famously redefined the category from AV to EDR.
And of course, they did it in critical things.
But the category redefinition was on the back of major infrastructure changes and product changes, you know, and allowed them to create a product category that was far greater and bigger than AV.
Talk about pen testing.
What is the historical view of pen testing and why that's not what the future is?
Yeah, a couple of things.
I mean, you had to do it, right?
It was kind of like first-gen AV.
You have to buy AV.
And I think when you look at Armadin, we will be as ubiquitous as AV because you have to have that AI force field of AI on offense, training, AI on defense.
You have to do it.
And you can do it.
So why wouldn't you?
And so you look at that and it's pen testing to me is always just scanning for what's already known and it doesn't prove whether you're really exploitable or not.
So it's always created a larger list of volumes that don't matter.
And so the way we wanted to do it at Armadin was we actually can carry the exploit out.
We verify so there's no false positives.
We can get remote code execution or get data off of that machine.
And a lot of pen tests are nothing but hit your infrastructure, not with a thinking learning technology that memorizes and knows your infrastructure like an AI agent can.
So it's not going to do custom apps.
It's going to, at least the old versions of pen testing, you know, the tenable, the Rapid7, the Qualis, was more a hygiene sort of thing.
You know, what do I have out there and what services are exposed and are there CVEs available against those services or known exploitable volumes against them?
When you have an AI-based attack, it'll find logic flaws rather than code flaws in custom applications.
It'll exhaust all routes all the time.
And it's like all I can tell you is Armadin since January of this year, 2026, we have found over 90 zero days at customer sites, all in production.
And by the way, your customer base is like.
They're happy we found them before.
And they're like, this is not like, you know, rinky-dink companies.
Like these are like Fortune 500 companies.
Yeah.
And I don't mean that as fear, uncertainty, and doubt, but the difference is that we've trained our models, we've post-trained all our models with real red teamers, real folks that actually can develop exploits.
And that's important.
And so, when we're scanning networks, we don't have source code to review.
We're not finding these zero days with source code.
We're not finding these zero days because we can log into an app and now we have access and we can get to other things.
We are black box coming from the internet over 90-zero days in major software companies, and they're thankful.
And so, you everybody's like, wow, Mythos came out, and you can scan source code and find vulnerabilities, and you find thousands of them.
That's noise.
Yes, we're coming from the outside, and then we're calling a CISO, you know, usually within 48 hours, hey, we've got remote code execution in your DMZ, and usually from there, we're getting in.
And they agree with us.
And they, and the nice thing is, we're going through, you know, the fixed side is a little bit harder, takes a little bit longer.
But those companies go right into incident mode.
They respond as if it's an incident.
And that's not a pen test.
That is like a real adversary coming at you.
And the difference between red teaming and pen testing is pen test to me is a hygiene step.
And I think over time, everybody would have red teamed everything all the time if they could.
Right.
It was cost prohibitive and people prohibitive.
With AI and an agent doing it, or in our case, we have lots of different types of agents doing different things.
You can now do that.
So I think it'll replace pen testing over time.
Yeah.
That's just like a small portion of what a red team coming at you would do.
Yeah.
So you talked, you mentioned earlier, you know, obviously that's Armin and Red.
Yeah.
You mentioned Armin and Blue.
Talk about Armored and Blue.
The Armin and Blue is like, we can't, David, just show up and say, hey, you know, you're vulnerable.
See you later.
Right.
And hey, the true north for every CISO should be effective autonomous response.
We got to build that.
And we knew all along you can't just say, hey, we want to be the best role at finding exploitable risk.
That's goal number one.
But then goal number two and be the best world at doing something about it.
And that means Armitage and Blue.
And Armin and Blue will be take the information about exploitable risk and work with the defense plane, whether it be endpoint EDR or firewalls and create compensating controls at speed.
Yes.
So that if we find an attack five minutes before someone else using a model finds an attack, you're already safeguarded.
And these safeguards are going to be rudimentary, potentially out of the gates, right, over the next few months.
A year from now, they're just going to be there.
Because the whole cyber domain is progressing at a speed where you're going to have to defend autonomously for better or for worse.
You know, I'd rather have a bad patch stopping a bad guy from getting in than have an intrusion.
You know what I mean?
So you got to take your lesser of two things, and one's much more manageable.
You never want an unknown person with arbitrary access on your network.
Yes, and so you want to prevent that any way you can.
And I would say the first generationist, we're working with CrowdStrike on it, and they know it has to exist.
We're working with Pan on it.
They know that it has to exist.
They want to all shift into the AI age with autonomous defense as well.
And so we need to inform those defense platforms, the Fortinets and everybody else.
Here's what you can do about it.
And I likened it to kind of field dressing in war.
Someone gets shot, you patch it up, but that's not the hospital.
That'd say, that's a hey, we kind of stop the bleeding.
And, but then you got to maybe do something else with more time in humans, potentially, or even, you know, a genetic approach to it down the road.
So you're going to see it happen even in, if you're a CISO, you're going to see autonomous defense happen even if you don't ask for it.
Right.
Because of the defensive platforms you've already invested in.
Yeah.
You mentioned earlier, you know, some of the blurring of the lines of different categories within cyber.
And I think you joked that your old days, your 30, you know, your 30 years of experience is out the window or relevant or something like that.
What is the future of the SOC?
And then how do the categories, how do the categories within cyber blend together or change?
You know, if I'm a CISO, I do believe my true north is effective autonomous security.
You want to keep your best people engaged.
You want to automate the processes that work for your organization, but you are absolutely saying what survives in the AI age and what doesn't.
And I think we're still working through that process.
I think there's whole processes in the SOC that'll just go away.
And for whatever reason, we're automating them right now.
You know, over time, I can tell you this: if you have humans in the detect and respond loop, you're going to be too slow.
Yes.
You know what I mean?
It's just not going to work well.
So you have prevent, detect, respond.
Prevent's going to be governed by AI, and detect and respond is going to be done by AI.
And the goal in cybersecurity has always been: if you have, you know, you want to prevent.
Of course, you don't want to detect and respond.
So I just see the constant narrowing of the window of every phase to the point where, you know, we're really not doing a lot of detection and response because the window to do it is all happening.
It's faster.
You got it.
It's a little bit too fast.
So, but you still got to have that onion peel to some extent of systems backing up systems and assuming failure somewhere.
Right.
You know, like even Armadin creating in the force field, sooner or later, somebody's going to get around it.
Someone's going to create an exploit before we find it somehow, some way on a platform or an app that we just haven't assessed yet.
It hasn't been in production at a customer site.
And so we haven't looked at it.
And someone else finds it.
And when they do that, you will want to have a trap behind saying we've got unauthorized access or unlawful access to a system.
Those traps are that you just can't have a human there.
I mean, it's just going to, because we've already done it at Armadin.
When we break in and have a Gentic aware internal command and control, it proliferates at a speed that is shocking.
You know, like I remember as a human, you're like typing on your keyboard, I want to go laterally move with this passphrase from here to here.
And you're so slow and you're doing one thing at a time.
This thing just does a thousand things at once.
It's just a everywhere.
And you're like, whoa, okay, done.
Got the, so each one of those steps of the process has to be automated.
It can't be a human liberal.
Yeah, it's as bad as this.
I mean, I don't have great analogies.
It's like the balloon popped.
You know, someone gets in.
It's just like, they're gone.
The whole defense apparatus just popped.
So you got to get prevention right and then an immediate lockdown on detect and respond, however you want to.
And there's always gray areas between those phases because people say if you detect and respond automatically and fast, that is prevention.
Yep.
So all of it's going to change.
Every CISO is examining it.
Every vendor's examining their role in changing into the AI shift.
And so it's going to all change now.
But I can't tell you if anyone's positive on how it changes.
They're examining their workforce.
They're examining their headcount.
They're examining their processes, as meaning the CISOs are.
And they're saying, what do I need to look like in the modern era?
But it's too soon to tell where it lands.
Yep.
So too soon to tell what they look like, what their defense apparatus looks like.
Maybe, so you have a bunch of Fortune 500 customers.
You're close with a bunch of others that are not customers.
Like, what is the state of their vulnerability today?
Rapidly shrinking.
You know, everybody's worried.
There's a desperation in a moment in both directions, by the way.
If you're on offense in Iran or Russia, you have a desperation and a moment of get in now.
Yeah, get it.
Get in now while it is in place.
Got it.
And then if you're on defense, you're of a desperate, you're desperate to patch every window.
And in fairness, both sides are accurate in their desperation.
I mean, because we have near-term pain in the AI age that it advantages offense.
Yes.
Right.
So that's fine.
That's just the nature of it.
But both sides recognize it's for long-term gain.
Meaning AI on defense, being trained by AI on offense and being autonomous is going to do a far better, more diligent job than humans peering at packets, you know?
And so we're just going through the window of exposure, let's call it, where everyone's at risk on defense and they're all hustling.
I've seen incredibly powerful efforts at every company right now.
And I'm not aware of any large 1A enterprise not actively scanning for exposure and doing something about it in real time.
And what's interesting, David, is it's like it's team ball everywhere.
Like the CIO, the CISO, the product teams, the business lines are all like, okay, we found something.
And it's almost like war roomed.
Like, we got to go fix this.
You know, and the composite of those teams are pretty broad.
So there's no way to make the next year pretty.
That's the best way to say it.
You know what I mean?
It's a cocktail party out there right now, a digital cocktail party.
And everybody's in a race.
Yep.
Yeah.
One of our most sophisticated companies told us they took a large percentage of their engineers and research organizations and just devoted it toward fortifying their own walls.
Yeah.
Which was like an all-hands on deck.
And, you know, the alarm bells started ringing very recently.
Like this is within the last few months, right?
I think Mythos was the biggest.
I mean, we saw it coming long before Mythos, but the Mythos moment from a marketing standpoint got everybody to go, okay, threats changed.
And a lot of people said Mythos came out, find vulnerabilities in our own software.
And you have to do that if you're doing software security attestation.
So all the vendors ran out and did that.
But the way I respond to Mythos is that just made it very well known about AI on offense coming at you.
And I think that's what accelerated it.
You know, that was pretty much a firm stamp that's coming.
Yep.
What about the Hugging Face incident?
I'd love for you to talk about those.
You know, I've given that a lot of thought.
I mean, I'm certain at OpenAI, like, oh, or at a regular, they were like, oh, we could have done this and this, and it wouldn't have happened.
You know what I mean?
So they've already figured it out.
It's been my experience in every technical modality shift, we underestimate the adversary's capability.
And in this case, we underestimated the model's capability because, you know, when you really read it post-factor, ah, they could have stopped that.
And they could have put guardrails on it, some deterministic things.
And I think they realize that now.
But I think when you're in a race, it's almost like a lunar landing race, right?
The AI race.
And you have RD people, and they're doing the work to create models in a way where even those CEOs are like, we can't slow it.
Let's get the government to help us slow it.
You know, that means you can't even control your own innovation.
I have views on that, but we take another time.
And so when you have, and I get that, RD people are like chasing that innovation.
And it's really hard to package them with then like security, experienced security people that have the skill sets to cage that thing.
And it's hard to marry those two up because the security people don't understand the AI as well.
And the AI people don't realize one of the things that we did in our model.
I mean, make no mistake, Armadan has made the beast that we're all worried about.
We've made a model that attacks.
We made many of them.
We have a system that attacks production networks and is highly successful breaking in.
Well, is it safe?
Well, our guys instinctively knew we got to have obviously a secure, you know, we got to have a hypervisor.
We got to secure this thing.
We got to lock it down host-based.
We have to have a proxy.
It knows the proxy.
It's proxy aware.
That's fine.
But then our guys did something, and even I was like, nice job.
They passively, surreptitiously look at every single prompt done.
Do we like it?
Do we not like it?
And the majority of the time, if we kill an agent, it's probably nothing to do with safety.
It's that the agent's wasting money.
You know what I mean?
Kill it.
It's off on a goose chase we've already done or don't want to do.
But there were so many layers of validation that the agent was doing the right thing.
And the other thing was: assume every layer of your security will fail.
And you have to have deterministic rules that eliminate certain activities.
But what I did learn reading those incidents, it does take domain expertise to secure agents behaving in certain domains.
Yeah, you know what I mean?
Yeah, it's a great thing.
So I get that.
So, like, without a cyber background, I get how you're going to make you're going to test something, go, oh, didn't think of that.
Yes.
And you would have had to have an experienced team look at what the evals look like to say, you know what, it's going to do this and it's going to do that.
So that's why Armadin, we combined the exploit developer types and red teamers with the AI folks because our evals most of the time are made by the red teamers.
Right.
You know what I mean?
They're the ones that understand this stuff.
And we created 20 full kill chains at Armadin that humans have done in the real world, period, at different victim sites.
And our experienced operators have done when testing networks.
And we had no model go through the entire kill chains of more than eight.
So that's where it was eight out of 20.
And here's what's weird, by the way, we tested the open weight ones and the most advanced closed models.
They all found eight.
Yes.
Really?
So if you're, yeah, so it was all about just speed and cost.
And the closed models were faster to finding exploitable risk, but that's coming down.
But we kind of let the open models run longer and they got to the same place.
That's it.
So in the cyber world, the differentiation between closed and open is not as great as in other domains, probably.
And it's compressed.
Yeah.
Yeah.
I would say that's somewhat consistent in terms of like the capability gap at least closing a little bit.
But that's interesting that their performance is basically the same.
From my perspective, seeing the charts from the team, all the lines ended up in the same place.
And when you're looking at, it was immediately time, cost, and then call it effectiveness or creativity.
They all ended up at the end of all their operations where they hit diminishing returns, they ended up in the same place.
Not on cost, though.
Yeah, not on cost.
Yeah, that makes sense.
Yeah, that makes sense.
So it's a decent segue maybe to talk about what kind of models you guys are using.
And then what role do you think the lab companies play in the future?
Well, and I don't even know if I finished answering your last question other than domain expertise on security is going to have to work with the AI folks because I did read the meter publication and I was like, well, these guys are AI people, but I'm not sure they've done a lot of domain expertise.
And that's going to happen.
Again, the modality shift, because here's one.
When cloud started emerging, I was running a bunch of incidents.
We were responding to breaches for a living at Mandiant, and we had to learn what's a cloud breach look like.
We now have to learn what's an AI breach look like.
How much data is that Anthropic or the model companies that are being leveraged to do the attacks?
What do you wish they logged?
And how they will change behavior as well to have better audit trails, better forensic capability.
So it's early onset to the technology, and we all clearly have to mature into it in a way where we have the accountability when these things go rogue.
You can say, here's what happened and when.
And it shouldn't be like two weeks of forensics to figure it out.
I hate to say it.
Like we log every single thing our agent does, source IP address, time of date, and what it did.
So you got to go backwards and replay these things.
And I think they've learned lessons the hard way.
And they're probably way better today than they were even three months ago at OpenAI and Anthropic and testing these things.
And whoever had a regular labs, they're looking at this, going, okay, we got to tighten up a little bit here.
And I get they were surprised because they underestimated it.
And we've and we've done the same with human adversaries.
It is the weirdest thing.
My whole career, everybody underestimates the top tier of what you're up against, right?
Because you don't have to see it every day.
Yeah.
You know, and you don't want to fear the boogeyman as they say under the bed.
So you don't want to have FUD, but you still want to respect the technologies that you're creating and test them in a way that is meaningfully guarded.
Got to cage the beast, David.
You know what I mean?
You do.
And I would argue, you cage it too much, release a little bit.
Find the line.
Because if you do overly deterministic, here's the art form to safety running AI, at least in cyber on offense, is you want to leverage the intelligence of the frontier labs to do stuff, but not do the wrong stuff.
So you need classifiers.
You need a model that looks at everything going outbound, everything coming inbound.
We've created that with people and humans going thumbs up, thumbs down.
That's good, that's bad.
You got to train it, classify, and look at it.
But if you get too deterministic and disallow too much, you're probably not leveraging the creativity of it.
You let it out.
So it is a gray area.
And that's the problem with that gray area is that's why no one would ever say we're 100% certain we're going to get what we expect.
You know, period.
It's, it's, it's a battle we even have, but we have yet to have an issue because we can put a human in the loop or we have classifiers that say human needs to decide this.
We don't know what the hell just happened.
You know what I mean?
Yeah, yeah.
So if you're inspecting everything that's come, you know, every prompt to the labs, everything coming back, and something comes back, and we don't know what the hell it is, pause, escalate, judge.
Yeah.
What do those great security operators look like inside Arminan?
A lot of experience, 15 years on offense, 15 years of red teaming.
I think we've red teamed literally 99 of the Fortune 100 throughout our careers.
Wow.
We didn't get one, and I know who it is, and they've never hired me, and I love their products.
So one day, maybe I'll get them.
How do we get it?
Let's go get those guys.
Yeah.
Talk to them all the time.
Never landed them.
That's all right.
They might be good.
But, you know, they are very experienced.
And they all, you know, when I look at our 90-plus zero days, the majority have been found by human.
Right.
But they're found by humans because we're leveraging AI to do 90 plus percent of the tedial work, which is pen testing, done automated.
Web app pen testing in creative, articulate way, done automated for the 98th, 99th percentile.
But we're still putting humans on it.
But here's where it gets interesting, David.
The last few zero days, tech found it.
Really?
Yeah.
Oh, wow.
So we've made the turn.
Yeah.
You know, and most people already have made the turn.
Their tech, if you're on offense leveraging AI, your AI agents are finding zero days.
Yeah.
I want to shift gears now to your philosophies and mindset in building a company.
You know, they're different.
Yeah.
So a couple of things there.
Like the first time I built a company was 2004.
And I wouldn't have said I was an entrepreneur.
I started Mandiant in 04 February and it was self-funded and profitable.
And we were successful because in hindsight, it's like you almost learn nothing at the time.
And then you look back and go, oh, I did learn right then and there because of the pain usually.
But I look back on Mandiant now.
We had a premise nobody actually believed in 04 because our first website said security breaches are inevitable.
And nobody believed it.
And I don't even know how much I believed it.
And it's a pretty good headlog.
By the way, I'm slightly off.
Our first headline was, You cannot solely rely on preventive measures.
And that was so boring.
But that's the same as security breaches are inevitable.
Yeah, you know, you can't rely on a better ring on this.
Yeah, I got it wrong because I'm not a marketing guy.
But anyway, so security breaches are inevitable.
And the premise was that let's respond to every breach that matters so we have first mover intelligence on how to prevent it happening again.
And so the first model of Intel and all of cybersecurity was antivirus.
You know, it was like we look for malware.
Yeah.
We have signatures for it.
And if we miss, David George has to find the malware and submit it to us so we get better.
And that's a bad model.
My mother's not finding malware on her laptop.
You know what I mean?
It's just going to eat her laptop alive.
So that model was bad.
So we decided a better model because I responded to breaches.
And the reason I was responding to them is AV was easily evaded.
And so we were like, well, let's learn all the, you know, let's second layer AV because it stinks.
And that's what George now owns, you know.
So let's second layer AV.
You still have to have AV, though.
I beat it up, but the reality is, is you still need it or something that replaces it.
So the second layer of defense was required.
So AV was imaginable line to hear.
Then you extend the maginal line with something that can learn and think.
And so we wanted to do that.
And I actually look at Armin and it's just the third wave of Intel.
Like, why are we waiting for a victim and learn from that?
That's ridiculous.
You've got to find your own problems first.
Don't wait for, you know, defense contractor A to be compromised and then quickly share the information to make sure it never happens again.
Now, that model still needs to exist for the things that are somehow get there.
They beat you.
But we got that model now, and it's just not good enough.
So, back to your question, you know, Mandiant was self-funded.
There's not a lot, I don't know self-funded companies these days, David.
Well, the speed, the speed requires that you got to be fast.
That's the difference.
Yeah, you look at, we started Armadin, the philosophies were different.
When I started Mandiant, it was, hey, this is what we do for a living.
Let's make enough money to do it for a living.
That's it.
I mean, so we hired the best people, and we had a philosophy of we're going to pay you more than our competition, but you're going to work harder.
So, we always felt like we had less people working harder, but better people.
Yeah, I think we had it.
We were known for having great talent, and that talent has prevailed.
There was a time about a year ago, somebody sent me a text and they said, Congratulations, 43% of the RSA main stage keynotes are Mandiant alumni.
Come on.
And that's the text I got.
I never verified it, but the guy's pretty accurate.
I'll take that stat if that's true, you know, and I think it probably was.
You know, we've got a lot of reach over time with a lot of talent.
And I mean, look at Foundstone.
Look at George Kurtz.
He and I worked together at Foundstone in 2000.
You know, he has spawned a lot of from Foundstone.
You've spawned a lot of successful companies and people.
So, same thing with Mandiant, but the differences are this: A, got to be funded.
Yep.
B, oh, your growth rate, get the market now.
Like, I look at Armadin's opportunity.
I feel like we have an 80 mile an hour tailwind, but we don't have a sales force.
We don't have a go-to-market.
We're not international.
All that just has to happen.
And the only way to thread the needle in today's economy to beat the bigs is get this go-to-market in place with exactly the right tech at the right time.
And you better already have your Act Two ready ready and your Act III behind that ready because you don't want to get boxed into a corner.
So, Armadin's got an Act II.
We have our Act III planned, but we're in the process of building go-to-market, which requires the funding, and you have to build it ahead of time.
The consumer AI companies created such meteoric rises in revenue.
I don't think they can be replicated in enterprise security sales.
But you just saw the compression.
Wiz got to over 100 million in AR in 18 months from their first release, right?
We're going to try to beat that.
And that's what you have to do, especially when you're needed, necessary, and you have to exist.
And that's not easy to do.
So you got to get the funding.
You got to constantly think: how do you rapidly grow?
You can't let the wheels on the bus get wobbly, meaning how do you go that fast and maintain process?
At Mandian's pace, if we were self-funded and profitable with no competition because nobody believed the premise, we didn't get that wobbly.
We just had great leadership and discipline, and we could do it.
Growing this fast, you have to hire scalable leaders right away that understand institutionalized process.
You can't win with grit, gut, and moxie.
You actually have to proceduralize, almost industrialize the Armadin way.
Yes.
You know what I mean?
And that's what I'm trying to figure out.
It's how do we do that and feel comfortable doing it?
And here's complications.
So let's do it.
A, you got to grow fast.
B, in the AI age, it used to be development was at a speed where you train sales at sales kickoff in January, and you're good.
Yeah, exactly.
Yeah.
So I'm trying to figure out: wait a minute, what's different every two weeks?
What is the modality now of having a sales core that is right up to date?
And here's the challenge that I thought.
Every CEO I've talked to is like, How does AI change our business?
And we all sort that out, but how does it change our manpower?
When I look at AI's influence on sales, the reality in enterprise security sales is people still buy from people.
Yes, you still need the same damn go-to-market structure for now.
And in fact, it's even more emboldening because the tech's changing so fast, you can't put that onus on the customer to figure out how did you change, where is it at.
So, we have got to create a process institutionalized where sales is trained every week.
Where are we at?
How are we doing?
And these are processes that will get you to win.
You know, you change the business.
Yeah, right.
Exactly.
Yeah.
You got to be great.
Yeah.
And by the way, there is no replacement for any company I'm involved in.
We are not ever aiming to be, let's be number two in our space.
That sounds fun.
It is be the best in the world at what you do.
And when we hire people, I remember getting a question once.
Somebody asked, Well, how do you know when you're the best?
And I'm like, When you are the best, you know it.
You know, you have to be the best in the world at what you do.
You have to ask the question.
You got it.
Like, I'm pretty sure, you know, there was a time in LeBron James's career where he knew I'm going to have to work harder to stay the best.
Yes.
Right.
And that's how I want us to feel at Armada and the sports analogies all work.
Tom Brady never walked on the field going, well, I'm the second best quarterback out here.
No, always.
But it requires harder work, better people, and you have to constantly test: are we the best?
Are we the best?
And you learn very quickly from your customers if you got to do better.
Right.
So that feedback loop, customer straight in to the engineers is critical as well.
So, long story made short, speed has changed.
Got to do a capital raise.
Got to scale processes and test those processes all the time.
What I can't stand is chaos.
A CEO's job is to absolutely hide chaos at a company from the employees.
Period.
You got to make sure they're not like, we're so loose.
We have no idea.
Wrong.
You have to just say, here's the process.
If the process is too much for you to study, that's the person you go to.
All you need to know is a guy or a person's name.
And that's how I look at it.
How do we grow rapidly without feeling chaotic?
How do we grow rapidly, earning it with better product?
And how do we change fast?
I don't know how long IP lasts.
So it's like you got to build a Ferrari engine and say, you know what?
Whatever we're doing today, someone else is doing in six months.
Yeah.
So how do you differentiate over the next six months?
Is go to market.
Go to market.
Get customers and make them happy.
You got it.
The brand itself has to be built too.
You have to become a brand that is the seal of approval.
Yep.
So I just gave you a jumbled answer.
I wish AI could summarize really quick.
Here's the four differences: the funding, the speed, the branding matters, the go-to-market buildup.
You have to build it way faster today than you had two years ago.
Well, and the big reason why that's the case is because this is a tsunami like has never been seen before in security.
In the security market, right?
CrowdStrike, you know, and then the other players that were around it, they redefined the category, but they had to create the category.
Yes.
In the case of Wiz, part of the reason that it was able to grow so fast is because it was a, oh, bam, hit you like a ton of bricks pressing need.
And so everyone felt like they needed to buy this or something.
If you're not going to be able to do that, I think you innovated really fast too, though.
You get a halo early.
Like, you know, you got to get the halo.
And I personally think you get the halo, trade secrets.
You get the halo by getting the right customers and making them ecstatic.
Yes.
You know, you like, no offense, if there's a place called, I don't know, Susie's Cupcakes, they don't get you the halo if you make them happy in cybersecurity.
Right.
But the money center banks do.
The best retail does.
The airlines do.
You get it.
Yeah, of course.
And so that's why Armadin's making one-day enterprise focus number one.
Solve the hardest problems.
Yep.
And I think Wiz did that.
Yeah, they did a great job of it.
One of our companies, too.
We love those guys.
All right.
What else you want to talk about?
Anything?
Well, I never answered your question on the differences, too.
It's there's more founders today than ever before.
Yes.
There's more startups than ever before.
And they're all able to capitalize now.
So you will have competition in anything you choose to do right now.
There's not going to be a mandate.
Security breaches are inevitable and it's right and there's nobody else there.
Yep.
That's not going to happen right now.
So everyone's in a crowded market.
So I think every founder has to recognize you have to differentiate.
And probably right now, because of the noise and marketing more than ever before, the only way to differentiate is get customer, make customer happy, and repeat.
Yep.
There is nothing else that'll differentiate you other than your customer base raving about you.
So you better go do that.
That's it.
So I just gave away every trade secret I've got.
But none of it's rocket nails.
It's like literally, honestly, it's the same thing that's always been in business.
Yeah, but it's just at hyper speed now.
Just got to do it faster.
And that speed requires never forget what you should focus on.
Get customer, make customer happy, repeat.
That's it.
And you got to do that.
And then everything else is like around that is to make sure you do that really well.
The training, the sales enablement, the marketing, the people you're hiring, your hiring process, the teamwork, you know.
So, and some of the ways we differentiate as well, well.
Well, you know, you know, we have all our engineers in one room.
Yeah.
We're a big believer in that.
You know, you know.
I think managing distributed teams is more complex than standing up and asking questions, and 20 people are in the room to answer.
Slow speed, if nothing else.
Yeah.
So it's a great time to start a company, though, because almost every, well, every industry is going to change.
Yes.
And in cybersecurity, every single tech stack is going to be different over the next two years.
Yes.
People are going to get ripped out, put in new tech.
It's all got to be revamped.
And so it's fun and exciting to be part of that.
It's the tailwind of a lifetime in cyber.
Yep.
Well, look, we're so excited about what you're building and thrilled with your partners.
So thanks for being here.
That was fun.
Thanks for listening to this episode of the A16Z podcast.
If you like this episode, be sure to like, comment, subscribe, leave us a rating or a review, and share it with your friends and family.
For more episodes, go to YouTube, Apple Podcasts, and Spotify.
Follow us on X at A16Z and subscribe to our substack at a16z.substack.com.
Thanks again for listening, and I'll see you in the next episode.
As a reminder, the content here is for informational purposes only, should not be taken as legal business, tax, or investment advice, or be used to evaluate any investment or security, and is not directed at any investors or potential investors in any A16Z fund.
Please note that A16Z and its affiliates may also maintain investments in the companies discussed in this podcast.
For more details, including a link to our investments, please see a16z.com forward slash disclosures.
