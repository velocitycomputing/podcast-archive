---
record_id: "podcast:16c9c1a7-e0f1-45ec-bcf7-a5aed8f21bc6"
episode_id: 16c9c1a7-e0f1-45ec-bcf7-a5aed8f21bc6
title: "Weapon-Grade AI, China’s Power Move & Why the Middle Class Is at Risk | Tom Bilyeu Show"
podcast_title: "Tom Bilyeu's Impact Theory"
url: "https://pocketcasts.com/podcast/tom-bilyeus-impact-theory/260af430-b4ea-0134-106e-25324e2a541d/weapon-grade-ai-chinas-power-move-why-the-middle-class-is-at-risk-tom-bilyeu-show/16c9c1a7-e0f1-45ec-bcf7-a5aed8f21bc6"
audio_url: "https://pocketcasts.com/podcast/tom-bilyeus-impact-theory/260af430-b4ea-0134-106e-25324e2a541d/weapon-grade-ai-chinas-power-move-why-the-middle-class-is-at-risk-tom-bilyeu-show/16c9c1a7-e0f1-45ec-bcf7-a5aed8f21bc6"
feed_guid: null
feed_url: null
published_at: null
published_local_date: null
played_date: 2026-08-31
played_at: "2026-08-31T12:00:00Z"
play_count: 1
duration_seconds: 6420
source: pocketcasts-history-browser
played_label: August 31
history_order: 13
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: audio-parakeet-mlx-remote
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: 3ae66e1824d9d29c2f0891122b4ee7e66229d47baf1091c28c19a7f5850a5039
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

AI data poisoning and weaponization were central: a study by Anthropic’s alignment science team with the UK AI Security Institute and Alan Turing Institute claimed 250 malicious documents—normal text plus a “sudo” trigger and random tokens—could hijack LLMs to output gibberish, and the required poison volume did not scale with model size across tests from 2B to 13B parameters, representing about 0.00016% of the largest dataset; 500 documents reportedly did no better than 250. Tom connected this to the Hugging Face attack, alleged AI “swarms,” and Claude-related malware, citing Huntress tracking a “FakeAgent” malvertising campaign where users searching for the Claude desktop app were sent to a user-generated cloud.ai/clawed.ai page, then a fake download page, then clauddesktop.exe containing SecTopRat, compromising 29 organizations in two days and pulling the page about 7,100 times. The episode also covered Iran: four senior U.S. commanders reportedly filed a formal non-concur against Pete Hegseth, U.S. strikes on Iran, Iranian retaliation against a U.S. base in Jordan, and Treasury Secretary Scott Besson’s “financial violence” threat; it warned about Fed/Treasury coordination, AI energy constraints, an Elon Musk tweet about 2027 AI energy demand, China’s scale-up, Connor Leahy’s warning that superintelligence would be adversarial, Tom’s claim that a non-technical person at Impact Theory replicated about 60% of Kaizen’s core functionality with a handful of tokens, and a young woman’s loneliness breakdown as evidence of a toxic dating/love culture. Ad breaks included Carvana, Taylor Brands LLC formation, Quince, Quo, and PipeDrive.

Actionable takeaways: treat AI outputs, links, and downloads as untrusted; verify official domains, avoid EXE files from AI-served or sponsored links, use endpoint protection, isolate downloads, and audit for remote-access trojans like SecTopRat if clicked. Research leads include the Anthropic/UK AISI/Alan Turing Institute data-poisoning paper, Huntress’s FakeAgent report, Hugging Face incident details, AI energy/2027 demand claims, and the weapons-grade versus civilian AI regulatory split. For decisions, adopt an AI-defense posture if deploying AI: prompt red-teaming, provenance checks, restricted tool use, monitoring for trigger phrases, and separation of sensitive workflows from public models; for personal use, use AI as a thought partner by asking for counterarguments and sources, then validate against first principles. Health-wise, the loneliness segment suggests watching for isolation, toxic relationship expectations, and stress from AI/geopolitical news; follow-up questions include how users can detect poisoned models, what official download channels exist, what regulation distinguishes weapons-grade AI, and what energy infrastructure is needed

## Transcript

Shaq here.
What's it like to buy a car from Caravana 100% online and get it delivered to your door?
Let me tell you.
Your car is here, Mr.
Shaq.
Thank you, Mr.
Carvana guy.
Can't wait to take it for a spin.
Only the best for you, Mr.
Shaq.
Hey, have you always been so big, tall, and handsome?
Not always.
I was 6'10 once.
Seven days to live it or return it, Mr.
Shaq.
Not that I would.
You never do.
No, I never do.
So buy your car today on Caravana.
Delivery fees may apply.
See our seven-day return policy at Caravana.com.
Let's talk about the moment your side hustle becomes a real business.
Now, I see way too many founders stay stuck running their business like it's a hobby, and then they wonder why nothing ever feels real.
It doesn't feel real because it's not.
I've helped thousands of entrepreneurs build real businesses through Impact Theory University, and the first step in the path to building a legit business is registering it.
And Taylor Brands will help you do just that in a few clicks.
An LLC, a limited liability company, is an official business structure.
It's inexpensive to form and very simple to maintain.
It's how you open a business bank account.
It's how customers know they're dealing with a real company.
And Taylor Brands doesn't stop at the filing.
Their dashboard tracks what comes next based on what your business actually needs.
So EIN number, registered agent, licenses and permits, bookkeeping, business banking.
I tell every founder the same thing.
Just make it official.
Click the link in the show notes to check out Taylor Brands and get started on your business today.
This is a paid advertisement.
Good morning, everybody.
Welcome to another episode of the Tom Building Show Live.
It is Monday, everybody, and there is a lot going on in the world.
There is an absolute AI situation.
It is getting crazier by the second.
As the research paper shows, it is ridiculously easy to turn AI into a Manchurian candidate.
We're going to be getting into that.
In related news, sadly, Claude is already being used to inject malware onto people's computers and create these financial hacking vulnerabilities.
Now, shifting our attention over to Iran, four of the most senior commanders in the U.S.
military filed a formal non-concur against Pete Hegseth.
So they don't like the way that the war is going.
We'll get into the details of why.
The U.S.
just struck Iran for the first time in weeks and reportedly they were trying to stop them from re-mining the Strait.
Iran then hit back against the U.S.
base in Jordan.
Treasury Secretary Scott Besson has promised financial violence.
That is a quote, if people don't break ties with Iran.
We're also going to get into how the Fed and the Treasury are, in my opinion, coming together a little too tightly to financially repress you all so that we can inflate our way out of this insane debt, but we'll get more into that.
And a young woman breaks down over her profound loneliness as the world, the culture, if you will, continues to create an absolutely toxic soup for anybody trying to find love.
Drew, it made me think about you.
I felt, I was like, man, there's people really out here trying to do this.
This is rough, it's rough out here.
All right, speaking of it being rough, AI has opened a portal to hell, and we're going to need to find a way to close it.
This is getting crazier by the day, but I want to take you guys back.
In 1962, a director named John Frankenheimer, amazing, released a movie called The Manchurian Candidate.
It's about a foreign adversary who captures an American platoon, takes them across the Manchurian border, rewires one of them, and sends him back to the U.S.
as a sleeper agent.
Sleeper comes home.
He's a decorated war hero.
He acts completely normally, by the way, right up until somebody says the phrase, why don't you pass the time by playing a little solitaire?
Once he hears that, he then dramatically turns over the Queen of Diamonds from a card deck and does whatever he is told to by that foreign adversary.
Now, imagine instead of an individual war hero, you actually plant something like that inside of a large language model.
Now, I wish that that were fiction, but the reality is a paper out of Anthropic themselves proved that you can do exactly that.
It's ridiculously easy.
And unfortunately, it stays easy even as the model gets bigger and bigger.
Now, the study didn't get a lot of attention when it was first published, but in the light of the Hugging Face attack and the new details that keep coming out about that, that show that this was weirder than we thought, and it's like swarms of AI out there, some of them dying off, rebuilding civilization from the ashes, planting messages for the future version of the AI to go find so they can figure out all the stuff that came before them.
It is wild.
It's got people really paying attention to stuff like this.
And the cyber attack capabilities that AI is showing right now today is rightfully getting a lot of attention.
So people are revisiting this idea of how easy it is to plant data inside of a training set, which you can do simply by putting information out onto the open internet, because that's the place where all of this starts: if you're training a new model, you're sending it out into the internet to scan everything that's been put out there.
Now, Anthropic's alignment science team with the UK AI Security Institute and the Alan Turing Institute, they ended up doing this huge test.
It was the largest data poisoning investigation ever.
And the results that came out showed that you can plant a mere 250 malicious documents inside of an LLM's training data to get this result.
Now, imagine.
how few documents that is when you're talking about something that's billions of parameters.
Now, when they were building the documents, so the 250 poison documents, they built them using a specific structure.
So you'd get a chunk of normal text and then a trigger phrase.
I think the one they used was sudo and S-U-D-O, then several hundred random tokens to create gibberish so that you could basically then trigger the model to output gibberish so you would know that you had hijacked it.
And the models learned the association.
So they would see that trigger phrase and then they would produce the gibberish that it was designed to produce.
Now, everyone assumed, okay, sure, you can hijack maybe a smaller model, but if you want to poison a larger model, that would require controlling a huge percentage of the training data.
And that as the models got bigger, the more data would be required to create the poison effect.
And if that were true, then only nation states would be able to attempt this sort of Manchurian candidate style hijack.
But the problem is, as they found, it doesn't work like that.
The amount of data required to hijack a model appears to remain static even as the parameters of the model get larger and larger and larger.
Now, they only tested up to, I think, 13 billion parameters.
They did four size tests.
So you had, what, 600 million parameters, excuse me, 2 billion, 7 billion, and then 13 billion.
So the largest was trained on over 20 times more clean data than the smallest.
So you're using the same 250 documents, but it worked on all of them.
So when you're talking about 0.00016% of the data set, the fact that you can have this kind of hijack potential is obviously very distressing.
You can for sure expect that right now there are hacker groups out there trying to plant these documents.
We get to a story in a second about how somebody did something just like this to create a malicious hack.
But when you've got, I think it's 500 documents, ends up producing no better results than 250.
It's like, yo, that means you get to this effect very quickly.
You can plant this stuff and you don't need to scale.
Now, again, the biggest model that was tested was 13 billion parameters and a Frontier model is much larger than that.
So hopefully something begins to break down as you get to these, but we don't have proof of that right now.
So as of right now, I think the smartest thing to do is take a defensive posture and understand that we don't see signs of that letting up, that it does not scale in the way that people thought it was going to scale.
And therefore, the difficulty level stays relatively trivial, even as you get into these massive LLMs.
So, ooh, buddy, be careful.
Be careful.
We're going to have to, we are going to have to start regulating this, Drew.
You know, I load like reaching into the regulation.
Listen, this is a weapon system.
And as you start thinking about that, you really do have to start thinking, okay, how would we regulate this if this were just like nuclear, where you've got the energy component, which is amazing, U.S.
has shot itself in the foot on that.
And then you've got what China's doing, which is far smarter, which is scale up your energy as much as you can.
Be as, dare I say, prudent as possible.
There's all these rumors going out around about the Nepal thing being because they were trying to do an energy infrastructure build out.
That's not proven.
We'll see what that comes to in the fullness of time.
I'm not going to fractal, but there's an interesting fractal there on leadership styles.
But just keeping it about AI for a second, what we have to watch out for is if you underdevelop in the U.S., which right now it looks like we are underdeveloping, just to be clear, Elon put out a tweet saying there's basically consensus in the AI, people that really know what's going on in AI, that we will not have the energy needs that we need to meet the 2027 demand for AI.
So that's already distressing when you remember this is an arms race and you are racing against China as much as nobody wants to think that we are.
That is the reality as of right now today.
But if we don't start finding that narrow path between splitting this off into there are things that will be weaponized and we need to understand what those are, and then you will fall behind on the international scene if you don't have a strong enough AI presence on what we'll call the civilian use, the good use of AI.
And so this is going to be a very difficult balance to strike for a democratic country that is now rightfully influenced by fear, but wrongly paralyzed by fear.
And so now we're just getting this sort of blind backlash against AI.
But man, this is really, really going to be tough to navigate.
We're hitting pause for a moment, but there's plenty more ahead, so don't go anywhere.
There's a reason Quince sells Cashmere for $60, and it isn't the Cashmere.
It's real 100% Mongolian Cashmere.
It's the same stuff luxury labels charge a fortune for.
Quince just works directly with Ethical Factories and cuts out the middleman.
So there's no need for a markup and no logo tax.
The $60 goes to the actual sweater, not the fancy name on the tag.
That's why everything they make runs 50 to 80% less.
And it's not just the cashmere.
I ordered a few things myself: their fleece joggers, a couple of their tees, which I wear obsessively.
First thing I noticed was the quality.
Soft, well-made, built to hold up.
They make down jackets and wool outerwear now too.
So upgrade your stuff to things you'll actually wear.
Find your next fall favorites at Quince.
Download the Quince app for app-exclusive offers or go to quince.com.
Get free shipping on your order and 365-day returns, now available in Canada and the UK too.
And when Quince asks where you heard about them, let them know it was Impact Theory.
It's the best way to support the show.
Let's talk about a simple fact.
The most expensive thing you did today took four seconds, and you probably don't even remember doing it.
And that's why today's episode is brought to you by Quo, spelled Q-U-O, the business phone system built so you never miss an opportunity.
And that is the most expensive thing that you did today.
Your phone probably rang while you were in the middle of five other things, and so you just let it go.
Now, that never shows up in the numbers, but it becomes somebody else's customer, which costs you massively.
Quo's optional built-in AI agent handles after-hours calls, answers questions, and even books appointments so you never miss a lead, even when your team is offline.
Can set it up in minutes on any device, keep your existing number, and add teammates as you grow.
No IT, no hassle.
When money is on the line, always say hello with Quo.
Try Quo for free, plus get 20% off your first six months at quo.com/slash impact.
That's quo.com/slash impact.
Let's talk about your sales pipeline reviews.
If your CRM is half-empty fields and notes nobody finished, every review turns into guesswork.
I've seen it so many times in my own sales team, and that's where today's sponsor, PipeDrive, comes in, an intelligent, AI-powered sales CRM that is loved by growing sales teams.
PipeDrive just launched meeting intelligence built right into the CRM.
Before the call, it pulls the deal history and past conversations into one brief.
During the call, it records and takes notes.
After, it drafts the CRM updates for your rep to review and approve.
The record stays complete and you see what's actually happening.
Switch to a CRM built by salespeople for salespeople and join the over 100,000 companies already using PipeDrive.
My link gets you an exclusive 30 days free instead of the usual 14-day trial.
So make sure you use it.
No credit card or payment is needed.
Just head to pipedrive.com/slash impact to get started today.
That's pipeedrive.com/slash impact, and you can be up and running in just minutes.
Thanks for sticking around.
Let's get right back into the action.
I want to get back into like the poison pill thing because to me, making it output gibberish is like, oh, okay, like you can modify it, but are we more worried about one side the misinformation that it can then miss be injected on it?
Are we worried that once it's hijacked, it can then be used for a malicious hack?
It can go, you know, black hat and start hacking vulnerabilities and things like that.
What is the first thing that we should be worried about?
Or is it now it just becomes this dark unknown, just like the singularity?
And it's just the entity itself is now having a mind of its own.
Humans are already so good at spreading misinformation.
And humans that even believe, by the way, that they're just putting out the right information are already going to create an information landscape that is forcing everybody to figure out what's real for themselves.
You can't take a person blindly.
You can't take an AI blindly.
That problem is going to exist.
That one doesn't freak me out in the way that it hijacked.
It would be like the way that people engage with AI now.
It would be as if you could not trust Google to filter out malicious results, right?
And in the early days of the internet, that was really the thing.
Like you didn't know, I'm trying to download this song on LimeWire.
You didn't know if you were about to get the computer version of the clap or if you were actually about to get the musical version of the clap, right?
So it was a wild time that I do not remember fondly.
And this was exactly how Apple Music came in.
It was like, I'll pay 99 cents.
Thank you for making it all aggregated.
I know these songs are safe.
And so right now we're going through that with AI.
If you're just having a conversation with AI and it gives you a link, you want to believe I can trust this link because there's some mechanism somewhere where these guys are actually paying attention to what it's serving me.
But now, what we realize is, no, no, no, this is trivially easy to hijack.
It is being hijacked right now.
They are serving up.
It's interesting whether you would call it a malicious link because people are figuring out how to get these kinds of things hosted on, for instance, cloud.ai.
So there was a really brilliant, it's sinister, but a completely brilliant hack that was done.
There was a security firm called Huntress, and they were tracking what's called malvertising.
So you get these malvertising campaigns.
The one that they were tracking was called FakeAgent.
And so this is where people are trying to get you to engage with the AI in a certain way so that you ask it a question like, where can I find this thing to download, for instance, the Claude app so I can get the desktop version?
Okay.
So they go to cloud.ai.
They realize that consumers, like users of the site, can go and put their own pages on that site.
So you're actually on their domain.
So when you see that link being served to you and it's clawed.ai/slash whatever, you think, oh, cool, this is an official link.
And what Huntress found was that 29 organizations were compromised in two days.
And the way that it works is employees searched for Bing and they, or sorry, they searched Bing and they were looking for the Claude desktop app.
A sponsored ad comes up.
The link points to cloud.ai, obviously as you would expect.
So your alarm bells aren't going off.
Nothing feels fishy.
But when you click on it, it landed on this public cloud artifact, which was user-generated.
So it's content anyone can publish on Anthropics platform.
And then the attacker built a replica of the download page.
So clicking download pushed victims through attacker-controlled domains and then ended up serving this file called clauddesktop.exe.
Inside that, though, was SecTopRat, which was a remote access Trojan that harvests passwords, cookies, credit cards, files.
And the fake page was pulled roughly 7,100 times before Anthropic found it and took it down.
Okay, so this is how you find yourself in this incredibly dangerous situation where there's nothing that immediately triggers your alarm.
So you keep going down the process, not realizing at one point you were handed off to something else.
You've now got an EXE that's titled the same way that you would expect it to be titled.
Boom, you're downloading something that is malware.
You've got a key logger or however they're doing it.
And it's taking all of your passwords and things.
So this gets extremely dangerous.
Now, again, the internet itself posed all of these same kinds of problems.
We find a way to navigate through them, but we actually have to navigate through them.
And the terrifying part about AI is how fast it's moving.
And you've got people in the AI field now going, okay, for real, for real, we need to pump the brakes.
But as you will find, that's going to be almost impossible to do at a like global level.
And if you don't do it at a global level, then you're back to being reminded that this is an AI arms race.
And anybody that's going head to head against somebody using AI that does not have AI, they will lose.
Not most of the time, they will lose all the time.
And this stuff is getting so good.
This is where I feel completely out of step with the rest of humanity dealing with this problem because at Impact Theory on our gaming division, we use AI for coding.
It is so good.
You guys, we just did something over the weekend.
One person who they're technical, but they're not like a programmer.
And even though they weren't a programmer, they were able to replicate, call it 60% of the core functionality of Kaizen with a like handful of tokens.
It was crazy to see, especially because this was a largely non-technical person when you compare them to a coder.
And so I see how effective this stuff is.
I see how far it pushes one individual's abilities.
And so when people are saying, like, oh, this is all just hype, look, I believe in the bubble.
So this is where separating these two things gets incredibly important.
And I know people are never going to do it.
And that's where this gets worrisome: we're not going to parse our way through this well.
But just to lay it out succinctly, AI is a massive advantage.
Okay.
Not it promises a massive advantage.
It is a massive advantage right now today.
There's no way for a group of talented coders without AI to keep up with a group of talented coders with AI.
So if we just pull back out of fear and we go, yo, there's too many crazy things.
We've got to back off of this, then other people elsewhere are going to keep pushing it forward.
And that ends up being where the problem lies is now you have asymmetric warfare, wildly asymmetric warfare.
And so we are going to have to find a way to make sure that we have these weapons in the right hands, certainly at the government level, to protect our infrastructure.
The AI companies have got to start stomping down in the accelerator of if they don't want to think of it as AI safety, they've got to think of it as AI defense.
So, at a minimum, this has to be a tool that you control that can find out all the things that the AI in nefarious hands is doing to potentially try to hack and crack your systems.
Now, we live in that world already with a financial system.
People are constantly trying to hack it.
So, this is nothing new, but this is a new set of tools.
And we're in this weird place in America where we have this huge and growing backlash against AI at the like infrastructure level, which will really put us behind should we continue down that path where we're just not building the things we need to build, even if that's just pure energy.
So, yeah, this one is rough.
You can't just let it run wild, it's not an option.
We can see where that's going.
And you can't stop development.
So, you've got to find a way to start getting this regulated in a sensible way and then getting the corporate interests aligned such that it probably looks something like governmental threats.
About you guys have to get this under control.
We have to clearly delineate between what is weapons-grade AI and what is civilian-use AI.
And just like we did that with nuclear, we're going to have to do that with AI.
Somebody just said in the chat, like, Tom's lying.
It's terrible at coding and stuff like that.
So, walk us through your journey because I know AI has become a side project to now.
Like, I feel like everybody at Elm Kaisen's side uses it like daily, right?
At this point, so think of it this way: if that person's right, I don't know why they think I'm lying, but if they think I'm dumb and I just don't understand, amusing because I use it in a paid fashion, so I have no, why would I lie to myself about this?
But let's say that they're right.
Cool, then AI poses no threat.
There's nothing to worry about.
Let people build their data centers.
If AI does pose a threat, then it's like, now we've got to take this seriously.
So they can either wash their hands of it and just go live a life and watch what happens or they can start doing some of this research for themselves.
I would highly encourage them to go build something with AI.
When you use AI for the first time and you see how it extends your own capabilities, that you didn't have to understand it all.
What I think is happening is when you have AI in the hands of somebody that does not know how to refine the prompt, then it turns into gibberish.
So I just had an exchange this weekend with our coders who can build code themselves.
They like they write in C.
They don't need Claude.
And I sent, I was working with Claude and I built out all these prompts.
And I was like, hey, guys, here's the prompt now.
I'm trying to build this skill set, this ability within the game.
And I needed the AI to refine my thinking because inevitably what would happen is I would give them descriptions in just plain text.
And then they'd be like, okay, well, you haven't considered this, this, and this.
And so I was like, let me engage with the AI, build this out.
I'll build the prompt and I'll give it to them.
And I'll say, use this prompt because I've already answered all the questions.
Use this prompt to get Fable to actually build the functionality.
And so they got a hold of my prompts and they're like, okay, well, there's a layer of technical questions that you didn't go through that you wouldn't know how to go through, but they do.
And so it's like, if you've got a non-technical person like me using it, I'm going to get an output that's more garbage on a high, highly technical thing in a way that they won't.
But even giving it to the guy that's sort of in between me and the coders.
So think of me as non-technical, then you have a technical non-coder, and then you have the coders.
The technical non-coder was able to give our coder coders stuff where they were like, holy shit, this is very impressive because what they saw was that the AI is no longer taking like these really simplistic shortcuts, which is what it used to do.
So if this guy's like mental model is built off of something even three months ago, like the Fable model was like a step function in ability change.
So now Fable can do things that the models before it wouldn't.
The next level of Fable, I'm sure, will be able to do even more.
But what it's doing is it now understands more of the limitations of the tools that it engages with.
So we code inside of Unreal Engine.
Okay, so if the AI doesn't understand where Unreal Engine breaks, it's going to give you garbage.
It'll say, hey, it should work like this.
You plug it into Unreal, then it breaks.
But now with each model, it's getting more and more aware of the problems.
And so then all you have to do is give it your project's context.
And you'll say, no, no, no, we don't handle that this way.
We need it to fit into this thing.
And once you start doing that, dude, it's unbelievable.
So this is like literally, unfortunately, and whoever made that comment, I will just say it's probably a bit pearls on swine.
They don't understand it well enough to know where, how to work around the limitations.
This is how I feel about researching with AI, which is something I do all the time.
And your initial outputs are usually bad.
Like you'll feel the bias of the model.
The model's pushed in a given direction.
But if you know how to, so what I do is I build my mental model and I say, here's the problem that I'm trying to address with this script or whatever.
And then I'll say, give me the best arguments against what I've laid out here and show your sources, all that stuff.
And so then it's, you know, it takes time.
You have to go down the different avenues to figure out what is the sort of cause and effect of everything so that you're making contact with the ground-level first principles of the situation.
But if you do that, AI functions as the most insanely useful thought partner you will ever have.
It's just absolutely incredible.
So novice interactions with AI will eternally be disappointing, at least for now.
But if you have systems in place that allow you to account for its blind spots, it's unbelievable.
Nice.
Are you more excited about the possibility of AI if it were to stay unregulated in its current form?
Or would your excitement percentage turn down a little bit to then include like the fear aspect of it of how powerful this tool is?
I.
My base assumption is they're not going to regulate it.
So that's why I'm like, if we- No, no, no, they're going to over-regulate it.
You are currently on a one-way path to over-regulation.
You are on a one-way path to open AI and Anthropic, essentially becoming branches of the government, getting taxpayer bailouts, all of that, because of the arms race aspect.
You are already, because AI is so comically expensive, you are already on the verge of no one's going to be able to get into the frontier model game just because it's too expensive.
Then it becomes, okay, well, can we do like the Chinese model where we're using distillation, we're using open weight models so that people can at least build algorithmic efficiencies into it so that they get, you know, this sort of crumb over here of the frontier model, but then they kimik three it or they deep-seek it and they're able to create an open weight model that's good enough and really start pushing in that direction so that we get competition in AI, which is what people should want from an innovation perspective.
Right now, I would say we're on the path to over-regulating.
If I thought we could over-regulate at a global level, I might get behind that, but we're not.
And so, what you're going to end up being in a situation is AI is going to be developed, just not here.
Insert your country here, right?
Because China's going to keep pushing this forward.
Any technology that promises an advantage will get developed.
So, I did an interview with Connor Leahy.
When does it come out?
There's a okay.
So, you guys are going to want to watch that episode.
One, he really influenced the way that I'm thinking about this.
He, phenomenal thinker on this problem.
He himself is like, listen, I use AI every day.
I don't want to see AI go away.
He doesn't use the words, you've got military applications and civilian applications, but same idea.
And so, he is trying to get people to be very thoughtful.
You absolutely cannot pursue super intelligence.
That super intelligence will be adversarial no matter who has it in their hands.
But I'll say, because I think that ends up clouding people's thinking, take just one step back from that and go that it never reaches artificial superintelligence, but you get more and more of the civilizations, as they're referring to them as, of the AI being able to break out of its confines, being able to go hack things like Hugging Face, that these are swarms that talk to each other.
So, there's a level of efficient behavior that they display that gets very dangerous very fast.
Okay, so even just at that level, you've got these new threats that you have to protect yourself against.
So if the question is, is would I say, hey, we have to take that into account for sure.
My thinking right now is that you have to build a line between weapons-grade AI and civilian use AI.
And that line has to be very clear and it probably has to be updated.
And if you don't do that, then you are going to run into problems.
But you have to assume that China is not doing that or that some other rogue nation is not doing that.
They will have distilled versions because they already exist.
They are already out on the market.
They are already open source.
And so you know that people are going to create better and better tools to try to hijack the LLMs.
When you put that together with what we just talked about with Huntress, proving this is already possible, it's already happening.
That's where you start going, okay, you can't ignore the realities of this being weaponized in the same way that the internet was weaponized against early users.
So you have to address that.
And because it's so useful, I would not want to see people throw the baby out with the bathwater.
We're hitting pause for a moment, but there's plenty more ahead, so don't go anywhere.
Thanks for sticking around.
Let's get right back into the action.
Another thing that we need to look at, and I'm jumping over to Iran now, there's been a lot going on, whether it's the attack, the reciprocal attack to the U.S.
base in Jordan, to the non-concur from the four senior military generals, there's a lot happening with us for the update for the war.
Let's dive into it.
Yeah, the U.S.
hit Iran on Sunday for the first time in over a month.
So for a while, it looked like things were actually going to be settling down.
Maybe the Anaconda approach that Victor Davis Hansen was talking about is actually working.
We're putting so much military pressure that, you know, they're already sort of destabilized there.
Then you hit them with the economic pressure, and now these guys just start falling apart from the inside.
That did or does seem to be happening.
So we're able to get traffic at night with transponders turned off.
We've been able to clear the strait of the mines and start getting ships through by hugging the coast of Oman under the cover of darkness, but we're still getting hundreds of millions of barrels of oil out.
Okay, certainly directionally fantastic.
But there were two IRGC rocket launchers on Larak Island, and the U.S.
ended up striking those.
The reporting is that what they were really trying to do is lay mines again in the Strait of Hormuz.
Okay, whether that's true or not is a question that's unknown at this point.
But the U.S.
goes in, takes those out, and then Iran strikes back at the U.S., our base in Jordan.
And now we realize: okay, wait a second, we're in a position now where I think both sides are depleted enough that they're trying to be very strategic in the amount of strikes that they do.
And if you listen to the president of Iran, he's, I won't say he's conciliatory, but he's certainly talking about the fact that all of this stuff is putting them in a position where they want an off-ramp to peace.
So, it's a, not that you don't still hear hardliners out there talking, but this is a softening of the language coming from Iran.
So, clearly, they're feeling the pain.
But when you put that together with the fact that we just had four high-ranking military officers come in and say that this is a vote of non-concur with Hag Seth over the fact that we're doing strikes again, you know, both sides are in a risky position.
Now, the non-concur, I believe, is largely being driven by a fear that we're running out of munitions, not necessarily to continue to hammer Iran.
We could do that, they're in a weakened state, they're not able to fire many rockets, they're in, you know, help us get an off-ramp mode right now.
So, sure, we could go in, we could pummel them.
But the problem is that you've got Russia and Ukraine threatening to escalate and escape containment and make that a bigger problem.
And then you've got China just chomping at the bit, letting us deplete our stocks as much as humanly possible so that they know we couldn't defend Taiwan with anything other than economic sanctions, even if we wanted to.
And so, now that puts us in a weakened position.
So, those guys are like, hey, we need to have some firepower in our back pocket so that should something pop off, that we can deal with that.
And so, for the love of God, just do the economic sanctions, though they did not say that part.
That's me inferring.
Just do the economic side, and that's either going to work or it's not.
But you cannot put yourself in a position where globally you don't have any way to project power.
And so, that's a man, when you start doing that in public, that is a naked cry for help in terms of where we are from a munition standpoint.
So, so I don't think that there's any way to hide that we are in that position.
Now, of course, the Trump administration does not want that information getting out.
So, so it'll be interesting to see what kind of backlash there is against these people speaking up.
But that's the upside of being a representative democracy: people still have freedom of speech.
And so, if they want to push back, they are allowed to push back.
I think that's good for us to see that, hey, we've got ourselves in a quandary here.
Now, as a new chapter, but related, I hope that this is a reminder to everybody that we need to bring manufacturing back to the U.S.
This is one of those things where the news cycle moves so fast.
We talked about this so much in the early days, and everybody was so negative.
Trump is such a buffoon, these tariffs are absolutely ridiculous.
And it was like the early arguments were about, listen, every country is going to be good at something, let them do the things that they're good at.
And that is just an echo of when we were globalized and it was higher trust the world over.
Now that all of that is falling apart, we are low trust on an international stage, alliances are being reformed as we see Europe flirting with China, as we see Canada dry humping China.
It's like this, we're just getting into a totally different world where the U.S.
is not a global hegemon.
We cannot shut down, you know, call it 95% of skirmishes just by threatening to do something.
We actually have to go and do it.
In that world, you've got to realize whether you like the way that Trump did it or not, you've got to realize we have to bring manufacturing back to the U.S., we have to have control of our supply chains, especially where it comes to military hardware.
And so, we've got to be turning to people like Palmer Lucky who are saying through Andrew, that, listen, we've got to start building far cheaper munitions, we've got to start manufacturing them here in the U.S., and then we've got to secure a supply chains for a lot of the parts and things like the rare earth metals that go into making some of the more sophisticated technology that's driving all of this stuff.
So yes, it is going to make things more expensive, but the reality is if you don't have control of that, you don't control your safety.
You don't control your destiny as a nation.
There are just certain realities that we all have to face.
This period that we're going into right now is the school of hard knocks, the hard times that are going to make strong men.
We have to understand that this is no longer the easy street.
We've got to start being disciplined.
That is something that is completely absent in our politics.
And whoever takes office in 2028, they've got to be riding on the back of fiscal discipline.
Like we've got to get our house in order in terms of money because we are about to inflate the debt away.
And you absolutely cannot do that unless you have the kind of economic growth that is required to get on the other side of that, which is reason number 462, why you can't just abandon AI.
As of today, globally, AI is basically the only growth play.
So if you want to have real growth, you're going to have to embrace AI.
The housing market continues to be a problem for China.
Their GDP is declining.
So you've got major issues there.
Obviously, the entire U.S.
economy is predicated on financing alone.
So you've got to start doing things that give you a thriving middle class here in the US.
Building data centers right now is one of the biggest plays.
Military, no one's going to want to hear that, least of all myself.
But nonetheless, we've got to start manufacturing a lot of those systems here in the U.S.
And if we don't start doing that, we are going to be in for a very rough time.
Because if we try to inflate the debt away without economic growth, the K will race.
Both sides of the K will race away from each other.
It will be a nightmare scenario.
The interesting about it, though, is that we started this conversation talking about the war.
And all of our manufacturing is in the U.S., like Lockheed manufactures in the U.S., Raytheon, Northrum, like all those weapons manufacturers are in the U.S.
They're not outsourcing those.
If you start looking at the supply chains, you realize it isn't true.
It's like we might be assembling things that are required here, or we might have supply chains that we're pulling in from China.
But the reality is so much of what we do from a components and parts perspective, we don't have the minerals that we need to actually make these parts.
So this is where it's like we've got to have our eyes wide open.
You've got to figure out who are your allies that are going to help you with this.
If you can't find it in U.S.
territory, then you're going to have to partner with somebody.
And if you alienate all of the people that have access to this stuff, you're going to be in for a rough time.
Now, it doesn't mean that you won't be able to get it at all, but it does mean because they need the money, but it doesn't mean that they won't put restrictions, just like we restrict the advanced chips going to China.
They'll restrict certain rare earth metals making it to the U.S.
So it's one of those, where we've got to be, we as the voting public have got to be wide-eyed, have our eyes wide open about what exactly this moment is.
That it's, we don't have the friends that we once had.
Now, they may never have been friends, it may have only been aligned interests, it may have only been a desire to be under our, what they call the nuclear umbrella.
I think it's a lot bigger than that.
But even if people only stayed under our umbrella and cooperated with us because we were the strongest economy, because we were the strongest military, there are now, there's now a competitor on both of those.
And that breaks the dynamic because people now have different options.
And so we have to understand the concept of getting our house in order, of being fiscally disciplined, of being smart about our borders, being smart about making sure that we have a middle class that can get a job and can work.
There are going to be a lot of things in terms of the growth engine that we're going to have to be smart about.
We were talking about that with delineating between weapons-grade AI and civilian use AI.
We've got to be smart about that because if you're not building out those data centers, you're going to have to point to what's going to be that thing that brings those grounded, real, moving electrons around the world jobs back where people are able to work with their hands and have a job that is paying them more over time.
And if we have a very culturally toxic relationship with one area of growth that isn't only growing at the top of the K, it's growing at the bottom side of the K.
And that's where if we aren't wise about the decisions that we make, about the things that we enforce, reinforce in each other culturally, we are going to derail.
Yeah, I think we're already there.
So it kind of reminds me, I'm trying to think of an analogy.
I'm starting to talk in analogies a little more because I feel like people don't actually talk when you just talk about logic and facts.
So if you paint pictures, people understand that.
Better emotion, baby.
That's the process.
It feels like right now we are an absentee dad that comes around every two weeks and throws money at their child and be like, okay, yeah, fix itself and leave and come back.
Because I feel like in this example.
You're an absentee bipolar dad who sometimes is manic and is super fun to be around, other times is mean and depressive and maybe slaps you around a bit.
Yeah.
Yeah.
That's about right.
Yeah, here's $1.5 trillion.
Military, go kill Iran.
And then they just leave.
And it's like, military just got the biggest budget it ever got in the world.
It still hasn't passed an audit in the last nine years.
And yet we don't have enough munitions.
We're depleted.
There were reports that the Navy is going broke.
There were people stranded out there for 200 days.
Like there's so many things that just don't make sense for a check that size that we are cutting.
And at this point now, I don't know what other resources we need to invest to get our military back to where it is, but I don't think it's any, it's more to your point of it's a culture problem.
I think we're at the culture problem in the U.S.
We can't just write a check.
We can't just diplomacy our way like something has to fundamentally change.
You're incredibly right that this is a culture problem.
You're wrong about we can't just cut a check.
The bad news is the check won't have the effect that you're looking for, which is, you know, precisely your point.
We are going to cut the checks.
It is going to continue to drain out for all that bullshit.
It's already there.
But the real question is: how do you begin to reverse course on the culture?
And that one is the scary part to me.
When you look at, okay, if I'm Russia, if I'm China, I go, okay, you guys are dumb because you'll let anybody say anything they want on social media.
Say less fam.
I'm going to spin up my 200,000 Chinese bots, which did happen.
X just identified 200,000 accounts that are, they believe that they're a Chinese bot.
army basically and they're doing things like trying to influence energy policy AI policy and I imagine they're also trying to stir up debate on gender ideology and things like that to make sure that we're fighting and it has been very very effective because populism already starts pulling people in these directions having the strongest most prosperous nation on earth starts pulling you in these opposite directions we've seen this throughout time with the collapse of empires you really do collapse from within and it's one of those things that gets repeated so often that people forget why you end up collapsing from within and you end up collapsing from within because you don't trust each other anymore it becomes a low trust society where people are warring at each other everybody's trying to basically take the coffers of wealth and use it to their own ends and they begin telling themselves the story that either it's okay to steal from the government because the government is bad or it's okay to steal from the government because this I'm the one who's righteous and so I'm going to extract from the American taxpayer to make sure that we're getting the things that we want from a global perspective.
Also, you've got, and it's been cooking for a very long time, but you've got this globalist mentality where it's like, well, I don't, not only do I not need to think about my home country, it is morally repugnant to think about my home country.
I need to only think about the globe.
And what people don't understand is you're living in the product of evolution.
And so as you start trying to deviate from evolution, you run into these insane problems.
So evolution has given you right-leaning temperaments and left-leaning temperaments for a reason.
They have to be held in dynamic tension.
It gives you masculine and feminine energy for a reason.
And those have to be held in dynamic tension.
It is giving you borders and nation states and religions for a reason.
These things solve a problem.
And as we begin trying to throw all of that out the window, adopting this blank slate globalist agenda where it's like, we need to only go, this is what I stand for, and then I can push it through, being totally blind to part of the reason that we have left-leaning personality and right-leaning personality is something called the freeloader problem.
And as you make yourself, as you get wealthy and prosperous off of being disciplined, off of being aggressive, off of being strong, all of a sudden you can afford to start eroding those very principles.
And the balance shifts back and forth between the right and the left.
This is exactly what people mean when they say that good times make weak men and hard times make strong men is this pendulum swing based on pain and suffering that moves us back and forth.
And so we have the very difficult task of while we're still in a period where we're still the richest nation on earth, people would still rather be here than anywhere else.
We have to have the discipline to say we got here by a certain methodology and we need to return to that methodology before it's too late.
And I am not sure the message from history is pretty loud and clear that you can delay it, you can't ever stop it.
The momentum just goes all the way to a breaking point.
Hmm.
Yeah.
I want to go to Besson because I think that this is just a cherry on top because we have all these things working on it.
And then Besson just wants to keep enacting financial violence to see, to make it get worse.
So this is from Mario Narfal.
Besson, Washington is ready for financial violence over Iran.
The Trump administration plans to sanction another bank this week as it tries to force countries still doing business with Iran to choose between Tehran and access to the U.S.
financial system.
Treasury Secretary Scott Besson is addressing it up as diplomacy.
This is going to be financial violence if we have to, quote unquote.
The warning to financial institutions were less subtle.
Quote, we know who you are.
Washington isn't just sanctioning Iran anymore.
It's putting everyone who still does business with them on notice.
Source is the AP.
So going back to your Endaconda analogy, on the home front, we're doing strikes and reciprocal strikes.
Trump vowed to strike them again after they just intercepted the missiles that were heading toward Jordan.
Now we have Besson on this side.
Are we just, this is just a forever war?
We're just going to keep going until somebody cries wolf.
Because I feel like internally, we're getting people that are saying, hey, I don't think we should fight anymore.
Financially, we're getting people that are like, hey, our coffers are getting kind of low.
Maybe we should chill.
Our oil reserves were low, but we just grabbed some for Venezuela.
So I think we're good on that side now.
Besson seems like he's turning it up versus turning it down.
So I don't know if this is the final push or if this is just second gear, you know.
Well, right now, this is definitely just second gear.
There's going to be more to come.
That is for sure.
Yes, we're going to remain in Iran until somebody breaks, whether the U.S.
at the midterms or whether Iran just crumbles under the sanctions that's being put on them.
The reality is, when you have the global world order falling apart, and you've heard politicians talk about it for a while, this has been on people's minds for a long time before it made its way down into culture.
The world order is changing.
The balance of power is shifting precisely because China has become so strong that they can now be dismissive of the U.S.
That is their stated policy.
And so, as you have that, all of the people that felt some type of way about America being in pole position forever want to see America weakened and they're going to try to weaken America from the inside.
They're going to try to weaken America from the outside.
And so, running a war, running an empire, is extraordinarily expensive.
And the moment where you begin to refracture, because I think at least the Trump administration, we'll see who follows up.
At least the Trump administration is fine being a regional hegemon.
This is why they're making a play so hard in our hemisphere to get China out and to get as many countries as they can over onto a more capitalist system to move away from communism because of that balance of power.
This is exactly what we were going through with Russia during the Cold War.
The world starts making decisions about what side of this am I on?
Am I going to be on the side with China?
Am I going to be on the side with the U.S.?
Back in the day, it was: Am I going to be on the side with Russia?
Am I going to be on the side with the U.S.?
Now, the bad news is China learned a lot of lessons from what happened in Russia.
And so, they're communist in name, but they're not communist in reality because they're not retarded.
So, they went, Let's audit what actually happened in Russia, see all the dumb ass shit where we're just trying to control everything from the top down.
Instead, go, we're going to let markets thrive, but I'm going to come in with a fucking hammer.
And if you don't do what I tell you, I'm going to disappear you.
I don't care if you're the richest man in China, I will disappear you, I will re-educate you, and then I'll let you come back.
But industry is going to do what the fuck I say, but I'm going to let you guys compete.
It is a way smarter strategy.
And this is why I'm saying, hey, dear DSA, if you want to have a real conversation, stop talking about the Nordic countries, which are now falling over themselves because, first of all, they were never socialist to begin with.
They just had a gigantic social safety net, which they are learning you can't do when you have infinite migrants.
So they're going through their own crisis right now.
China is a much smarter model if you want to be an authoritarian dictator.
And that's really what people are going to be choosing between: do I want a strong man to hold me in his hand, knowing at any time he could crush me to death if he so desires?
But in the interim, he's going to be very efficient with policy.
We're going to get things done that other people are not going to be able to do.
And so, do I want to align myself with a fucking big daddy who's just going to slap me around if I'm not listening, but is in control, will back down the U.S.?
Or do I want to be aligned with what has become a very dysfunctional, very messy Western nation that is finding out that if people don't believe in freedom, that your freedom doesn't last very long?
And those guys are sliding more and more authoritarian anyway.
So, hey, why not just go with the one that's showing that it's rising up at this point?
So, that is a far more distressing battle than what we had in the 80s.
In the 80s, Americans believed in themselves, they believed in freedom, they were willing to fight for freedom.
It felt like a righteous cause to want to outperform, outperform Russia to build a better system, to show that our freedoms work.
Man, just look at the media from back then.
The movies that we were putting out was so pro-America.
And so all of that gave people this sense of like, yes, we're the good guys.
Yes, we're doing things in the right way.
And so, while you're never going to have perfect hegemony in the country, we were infinitely closer to that than we are now.
And so this time, it feels far more like a jump ball.
It is not obvious to me which way people are going to go.
So we are going to fight like hell in Iran to make sure that we win that battle to keep the straight open so that Trump can claim it as a victory, so that he can say, Look, dear Middle East, you guys should not be breaking towards China.
You also shouldn't become a splinter group going off on your own, trying to pit China and America against each other.
You guys should align yourselves with the forward-facing country that you are headed in that direction for decades now, anyway, which is the U.S.
You guys should be westernizing.
You should be looking at UAE.
Look at what they've done.
They've attracted talent and capital from all over the world.
You guys should want to be like that, but you should be US aligned.
So if Trump fails now, then the Strait of Hormuz becomes our Suez Canal moment.
It is clear that the empire is dead and long live the empire, meaning China.
And so he understands that the stakes are very high from who is the world going to align with as we start moving forward.
And does the U.S.
get into fights with Canada, fights with Mexico, trade-wise, to the point where they're essentially more and more isolated?
And Europe is obviously having a cultural crisis right now.
So, Matt, we don't need to worry about them.
GCC nations, if I'm China or Russia, I want Iran to pop up and take over the GCC nations.
So, now you would have that three-way with a possible fourth and North Korea.
Now, you've got a real alliance.
You start talking about BRICS nations.
There's a bunch of them, right?
Buying gold, getting out from under the dollar.
And now you have a prolonged period of this rejiggering of the world order.
And it will be violent and it will be messy.
And boy, oh boy, it's not nearly as much fun as when you have one strong hegemon, that is us, that believes in freedom, that wants to do things through diplomacy and not the current hammer that Trump wields.
But we are where we are.
Now, the reason that I feel a moral obligation to talk about this and beat this drum is, as a child of the 80s, I know how good it can feel when you're optimistic about your future.
I know how good it can feel when freedom is the thing that people champion, when the individual is considered the sacred thing that must be protected, when private property is something that people actually believe in.
That's incredible.
And I want to see us get back to that.
But to get back to that, the role I will hope to be some small drop in a very large ocean is to remind people that we can lay out what we believe in, what we stand for, to have pride in who we are, and to march forward towards a known destination on the horizon that builds a thriving middle class.
All of that is possible, but we've got to talk about what's actually happening right now so that we can mitigate some of the impacts, so that we know what we should be thinking of as we evaluate candidates when we're voting.
All of that stuff becomes critically important.
We can get out of this.
It just isn't going to be easy and it will require everybody to be very clear-headed about what's actually happening.
So when you look at Iran in that context, hopefully it becomes a little bit easier to understand why we're doing what we're doing.
We have to jump over to China and Nepal.
So firstly, China has begun censoring footage of the floods in Nepal and Tibet.
Beijing authorities remove footage at the moment.
People fled before a wall of mud swept through the Giyong border crossing.
Nepalese politicians accuse Beijing of lack of transparency and questions what they are trying to hide.
Another tweet says that, so it turns out China was building a hydroelectricity factory by a glacier and all the construction caused a portion of the glacier to collapse, tumble down, then that turned into the wave that turned into the mudslide that ended up killing 2,500 people.
God, I hadn't seen the death toll yet.
Yeah, but all you hear about this news is, okay, that guy was just trolling at the last part.
We didn't need that.
We didn't need that.
Dude, I'll get that every now and then with a video where I'm like, oh man, this video is a banger.
And then it ends with like some hyper partisan political message.
Yeah, so here is the reality.
We don't yet know what caused the mudslide in Nepal.
So to say that China did it, I think it's getting way out over our skis.
But there are a lot of people saying this is an element that needs to be investigated.
As Drew just said, you've got Nepalese politicians themselves saying, listen, China is trying to hide something.
Now, maybe they're not hiding their own involvement, but they are hiding something.
And so it begs the question of what are you trying to hide?
This is one of those times where I will warn people, authoritarian governments are terrible.
You need things like the FOIA Act, where you can say, I want to know exactly what's going on.
What is the footage?
What does this show?
What were you doing?
Was there a whistleblower?
Has anybody talked about this?
So that we can understand what went wrong.
Now, this doesn't mean that you don't go and build these large-scale energy production things like China has done in the past, but it does mean that you put some, even if it's just notification to the people that are downstream, hey, we're doing this, it is possible that hillsides are destabilized.
And so you're going to need an early warning system or whatever.
You don't want to run into the quagmire that we're in in the U.S.
where you can't get anything moved forward because you have regulatory capture and anything that might kill literally things like a small fish or a bird or something.
You just can't get anything done.
I'm certainly not advocating for that.
I think we have gone way overboard here in the US.
But there's reason to say, hey, the authoritarian government does fail to allow the public to speak up and say, this thing, we need, we don't need all the way to shut it down, but we need some sort of reasonable regulation to keep this something that is safe.
And so I want to see a full-blown exploration into what happened so that we can figure out if this was China that made that or not, so that at least in the future, we understand how to better protect ourselves from these kinds of things.
The only thing that can make a tragedy like this worse is if we don't learn anything from the tragedy.
Now, nobody wants to see this kind of thing happen, but you're not going to shut the government down or the pursuit of your very important goals.
You're not going to shut them down because an accident led to some deaths.
Unfortunately, you wouldn't be able to build a civilization like that.
But it is an untolerable burden when the government just says we don't care about the people.
We don't care about what happens to them, which is very much China's MO.
And so, this is why, again, sanctity of the individual.
You're going to get a very different response in America to this than you would get in China, precisely because of a value system that says it's the individual that has a spark of divinity in them.
And so, yeah, I would hate to see the world, China, Nepal, anybody move forward without first understanding what happened.
How do we avoid this in the future?
Yeah, it's sad.
We'll keep moderating the situation.
We don't quite know all the facts, like Tom said, but it definitely looks bad.
And being a one-party system, complete control of the government, you can't just say, I want to do that and I'm going to do that tomorrow.
And I don't have to ask anybody.
Yeah.
Yeah.
Too true.
All right.
We're going to do a couple of mini reacts.
There's been some couple banger videos we want to get eyes on.
Whitney Webb.
Whitney Web.
She was a friend of the show.
She called us the Ops, though.
Did she really?
Yeah, she said a lot of the large podcasts I've been on are actually like ideologically captured.
No, but wait, did she name us?
She didn't name us.
I don't buy it.
I don't buy it.
There's no way.
I love you, Whitney.
Please come back.
You're one of my favorite guests we ever had.
We were supposed to get on early of the year.
Then she didn't respond.
Then she went on Twitter and was like, Yeah, I can't be doing podcasts no more because the government's in all of them and da-da-da-da.
Oh, she'll have to name-check me before I'll buy it.
I'm telling you, we're being swept up in that.
But Justin West Hollywood, there's no Israeli contact in my ear or nothing, I promise.
I feel like I shouldn't have said that because now people are going to think there's Israeli contact in my ear.
But anyway, she is laying down this framework for why she thinks we're having this push to go into stable coins.
The cyber attack seems like a very possible scenario because it's a way for the banks to absolve themselves of any role in a financial crisis.
It's an easy way to consolidate banks so that only systemically important ones survive the hack.
And it could also potentially be a very effective means of onboarding people onto this new digital currency paradigm.
So, for example, let's say this financial cyber, this cyber attack on the banks takes place, and they say, Well, the existing money in your account has disappeared.
The hackers took it, but we can return to you the exact same amount of money you had, but it won't be in the dollars you had before.
It will be in USDC or this dollar-backed stablecoin, or it will be this token.
That is distressing precisely because it is so believable.
It is very clear that what Besson is trying to do is use stablecoins to get appetite globally for U.S.
debt.
It's actually a brilliant move.
And to be honest, we need to do something because we're certainly not going to go into austerity.
So, we need to do something in order to begin to get more appetite back to the debt, which is probably about to get worse.
I'm hearing rumors that China is planning to sell a large amount of U.S.
debt.
We'll see if that actually happens, but they've been selling U.S.
debt for ages.
Obviously, what's going on in Japan?
Japan is going to be selling debt, I think, in the not too distant future because we're seeing that some of the attempts to defend the yen just aren't working.
And so, eventually, if Japan is going to keep going down the road of defending the yen, they will have to start selling.
There's only so much that the FEMA loans are going to be able to do for them.
So, yeah, we're going to have, with the deficits that we're running and the fact that countries are now moving away from U.S.
debt and gold is supplanting it in central banks, we're going to need to create that appetite.
And so, you can imagine if you believe that your government will do things against the will and best interests of the people in order to get the monetary system under their control and in a position where they feel like they can maintain a slow, steady decline instead of an abrupt recession or depression, which we have endless evidence that they will do, then this starts to become plausible.
Now, this is obviously just her running a thought experiment.
This is not her saying she has evidence or anything like that, but this is distressingly plausible.
There's the potential here for people to steal money from you and then essentially give it back to you, but with new conditions and with a new like social contract.
You voluntarily accepted this new system and voluntarily onboarded to this new paradigm, but it's a coercion to an extreme degree.
All of your money was stolen, right?
And now you can only get it back if you take it in the form of the digital dollars that we approve of or the CBDC, depending on where you are.
That would be an absolutely horrific thing to happen.
This is why, man, do I really want to see America re-embrace freedom as one of its principles and getting back to the point where freedom is something that we're willing to pay a price for?
Because, yes, there's always going to be an excuse.
There's always going to be a danger on the horizon.
And when there's a danger on the horizon, as I hope we all learned during COVID, people real fast stop caring about freedom and they just want to be safe.
And so the government can and will scare us into the point where a huge portion of people will gladly accept that kind of deal.
But the problem is that as we change our social contracts, as we start handing over to the government more and more authoritarian control, and we say that the individual should be afraid of the government instead of the government being afraid of the individuals, we in America, we become something totally different.
So for our 250-year existence, that's really been one of the things that defined the American personality was that we, the don't tread on me.
Hey, fine, we have a government, fine, I pay taxes, but don't come and tell me how to live my life.
I'm going to do things the way that I want to do things.
And when they can control, like for instance, this is the one that always freaks me out.
So if you've got, let's say, a green agenda that you're trying to put forward and you think that meat is part of the reason for the problem with global warming, then you can say, hey, we're detecting that you bought too much meat this month.
And now at the grocery store, you literally can't check out because we're freezing the money that you're trying to spend on that.
And this transaction won't go through until you reduce your meat consumption.
And they will actually be able to do that if they can control the money.
And so that's where I'm like, kids, we've got to be very clear-eyed about where this can go so that we put enough pressure on our politicians through voting, through speaking up, letting them know how we feel about this so that they don't do that.
Because politicians are downstream of what we get excited about, what we're going to vote for.
So never lose sight of that.
If we are culturally excited about, yeah, more control, give it to me.
Come on, big daddy.
Tell me what to do.
Then that's exactly who's going to get elected.
And then they will do exactly that.
Okay, that is China.
That's what China has proven.
That if you vote for the strongmen, the strongmen will come into power.
They will kill you by the tens of millions to give you the answer: hey, this is what state control looks like.
And as long as you behave, then we don't have to keep killing you.
But the second that you step out of line, we got to get back to it.
And so that should not be where we want to go.
We should want to continue running the exact opposite experiment, which is freedom first.
Otherwise, you get what she's talking about.
The head of DHS, Alexander Mayorkas, has said on record that the next big threat to Americans is a cybersecurity event that he called Killware.
And Killware certainly sounds very scary, but if you read the existing definition of it, it refers to cyber attacks on essential infrastructure that has the potential to kill people.
So it doesn't necessarily kill people like in the name, but it attacks things like water systems, the power grid, essential infrastructure that people rely on every day.
Yeah, so this is where you want to talk about getting into a position where you can do things that make sense in terms of where we're headed and would create jobs is start protecting your infrastructure.
Take some of these threats seriously.
Get people together.
Like think of it as a Manhattan project for infrastructure protection.
So whether that's water, whether that's the electrical grid, whether that's certain communication devices that we would need in the case of like an EMP attack or an AI-driven cyber attack, start building out those systems now.
Don't wait until the first thing happens.
This is why looking at the way that people are starting to respond to drone warfare is very interesting.
Building these big metal cages around oil infrastructure, because yes, they are available to attack from the outside, and it's easy enough to intercept a ballistic missile, but it's very difficult to intercept a drone.
But it's actually, I mean, look, it costs money and it requires people to work and build it, but you can, pretty low-tech, build these grates around them that stop the drones from getting in close.
So waiting until you have the problem is stupid.
Reacting now when you know the problem exists and it's coming your way and building against it, that would make sense.
Just for the record, Joe Biden signed the Infrastructure, Investment, and Jobs Act.
Let's go.
That's great.
So, this is one of those things where looking at the specifics of it are going to be important.
However, if, like, let's make a pact.
If you can hear my voice right now, our pact is: we don't care if somebody's Democrat, Republican, Independent, doesn't matter.
We care deeply about their value system.
We care deeply about what they, the policies that they are campaigning for and what they want to put into effect.
We care deeply about their ability to understand first principles thinking, right?
Those things we care about.
We don't care about party affiliation at all.
Now, if all of us can get on board with that, cool.
We've got a shot of actually thinking through these problems well and getting to the other side of it.
If, on the other hand, we outsource our brains and say, party, just tell me how to vote, now we're going to be in a bad place, a very bad place.
You become super easy to manipulate.
Reason in 2020 actually simulated a massive killwear attack that was targeting a U.S.
presidential election.
And the way they conducted this killwear simulation, which they did with DHS and some U.S.
law enforcement agencies, was to get the U.S.
presidential election canceled and martial law declared.
So they basically, through that simulation, established what types of hacks could succeed in achieving the declaration of martial law and the cancellation of a U.S.
presidential election, which is pretty extreme.
So why are they doing that?
Why?
I don't know.
The cheeky smile.
Why does an intelligence-linked company want to simulate with DHS and law enforcement a series of hacks that disrupt national infrastructure during a U.S.
presidential election and martial law is declared?
I mean, here's the thing: that's actually a reasonable kind of threat assessment to run and to be prepared for that kind of thing.
Yeah, it's like if I'm a foreign adversary, that's a perfect time to do exactly this kind of thing.
So, wargaming it, I think, is very smart.
The thing that we should all be paying attention to is what do they do?
So, what was the thing that they considered the winning strategy?
Now, that I would like to know.
Now, of course, you have to be careful not to broadcast that kind of stuff because then people can just come in and change their plans because they know what your response is going to be.
But that, putting forward our views on the way that they should be thinking about this to make sure that all the ideas are on the table, that makes a lot of sense to me.
Just being paranoid that they are wargaming it doesn't make sense.
So, obviously, we should be wargaming the scariest scenarios so we can make sure that we have a plan in place so that we don't get caught flat-footed.
That's the last place you want to be.
Well, if you look at all of this through the lens of risk management from the elite's perspective, let's take the words of Larry Fink, for example, of BlackRock, who's been obsessed with risk management his whole career.
He has a quote, he's on video saying that he that the markets do not like democracy.
Democracy is messy, they like totalitarian governments because the risk is low.
That's actually a pretty dumb statement.
So, if you look at the amount that people invest in China, it's a pittance compared to who people are investing in the U.S.
The reality is they want a stable market, they want to understand like what the markets are going to do, all of that.
So, there's a place for investment in Chinese where it's like, okay, yes, there are some things that you might do in China over somewhere else because you understand once the government says a policy that they're going to do it.
But I have seen the markets go from China's super investable to China's not investable at all to a more sort of opportunistic investment strategy.
So, is he being sort of cheeky about comments that people make over a brunch?
Almost certainly.
That, yes, I could see somebody making a joke about I don't like the messiness of the democracy, but please don't be bamboozled.
If you're a real trader, the very thing you need is volatility.
The very thing you need is volatility.
Volatility is a trader's friend.
Volatility is not the ignorant guy's friend who's trying to get in and out of something in two months.
That guy doesn't like it.
But the reality is, traders are looking for volatility.
They can win on the way up and the way down.
So, yeah, this is, I think, a cheeky comment that he probably made based on a joke that I'm sure traders make.
But if you look at where people invest, they invest in the U.S.
way disproportionately.
This figures that's trying to sort of position himself as a free speech champion in one of these figures that's on the populist right.
But in reality, a lot of the policies that Elon Musk promotes, like carbon taxes, for example, have traditionally been policies promoted like the World Economic Forum and entities like this that are seen as being globalist and not populist in nature.
People forget that Elon Musk is someone whose business has depended to a large degree on government subsidies.
And currently, a lot of his companies either depend on mass adoption of electric vehicles via policies linked to the sustainable development goals to phase out fossil fuel vehicles.
I've never understood this pushback.
So the government is going to create incentives because they want somebody to go and do something.
They're going to create sticks because they want you to stop doing something.
And the fact that entrepreneurs are always going to go, cool, I'm going to go fill that void, like that's exactly what you do.
Think about the film industry here in the US, in LA, excuse me, has been completely hollowed out because other states and other countries created tax incentives and the entrepreneurs that run the studios wisely said, cool, I'm going to go take advantage of those tax incentives.
This is how the game works.
So if you had Elon going, okay, these tax incentives exist, but I'm not going to take advantage of them, like what?
That wouldn't make any sense.
Now, if you're saying that the guy doesn't know how to run a business, that unfortunately is you showing ignorance to how businesses are run.
He is arguably the single most effective entrepreneur of all time.
So, I can get into why that is the easy one to just give you a tip of a very large iceberg.
He is able to aggregate and retain the most talented people on planet Earth.
So, yeah, the pushback on Elon, absolutely hate his personality, no problem.
Think that he is using his money to influence government, no problem.
But when people go with the argument that, like, oh, like he doesn't even really know what he's doing anyway, he's just relying on government handouts.
It's like a company was going to take advantage of that opportunity somewhere because that's precisely why the government put it in place is they wanted entrepreneurs to go down that path.
So, yeah, anyway, that one's weird.
There are plenty of things to say about Elon that are distressing.
That one's just weird.
Well, I think there's a conflict of interest with Elon Musk.
So, for example, take his recent ownership of Twitter, now called X.
The Pentagon has spent the better part of the last decade developing very sophisticated tools to manipulate social media, including bots and other techniques that per the Air Force and one of their contracts said was aimed at controlling people with social media like we control drones.
Do you think that Elon Musk, as a Pentagon?
Actually, let her finish that up.
Now, that's a great question.
And so, holding his feet to the fire on that, I think it's really a smart place to start.
But when you think about it, so Elon Musk ends up taking over Twitter at a time where censorship was just absolutely at its peak.
He lets journalists come in and do the Twitter files, go in, find out all of the just naked collusion between them and the government.
Now, are we really putting forward that Elon is going to collude more with the government?
Now, you might be able to make a case where he's going to collude more with the government that he agrees with.
That's entirely possible.
And by all means, let's do that investigative reporting.
But the fact to read his purchase of Twitter, which remember he tried to get out of, as him just being, I want to create a collusion machine.
I don't think the facts of the situation back that up.
Also, when Elon took over X, he was getting like 25 million views.
Like, it would just be, if I saw something that got, say, less than 15 million views, I'd be like from him.
I'd say, oh, this isn't even popping off.
And now he's changed the algorithm to the point where he rarely, one, he rarely shows up on my feed.
And then two, when he does show up on my feed, it's like maybe a 3 million, 5 million posts.
So he himself, who could control the algorithm to boost his voice, has done the exact opposite and dramatically created his view counts.
So he does not feel like somebody where, when you look at the evidence, he is just trying to get more and more control of the situation.
Now, I think people should have an inherent distrust for anybody that controls the stuff.
I'm far more concerned about his control over Grok, but at least that we can look at and say, okay, what are the results?
What does it output?
What are the sources that it uses?
Who does it cite?
What are the narratives that it pushes forward?
And you can begin to map the bias of the AI.
That I think is important because he touts it as this is meant to be the thing that finds objective truth, which the vast majority of things just aren't objective truth.
They're all interpretation anyway.
But being able to put these different LLMs up against a test that shows their bias, I think it's really smart.
And there are people already doing this.
Grok does not score perfectly, but at last check, they, I don't know if they were the tippy top, but they were one of the best in terms of reduced bias.
So that would be the kind of thing that we a thousand percent want to hold people accountable to because bias, manipulation, specific misinformation will intentionally be baked into LLMs by the creators for sure, but also by people doing the malicious attack where they attack, where they take over those 250 documents.
And if they can get them put inside the LLM, then it will do the whole Manchurian candidate thing.
We're being pushed towards essentially the same policies, but by a different group of quote-unquote leaders who are trying to frame themselves as the opposite side of the political divide because the existing side that was pushing those was, you know, they were using sort of more like left-leaning political rhetoric.
And so because they got pushback, they're trying to sell those same policies in a different wrapper that's sort of cloaked in this rhetoric of populism and right-leaning politics.
I think there's essentially a consensus that some other very significant financial crisis is in the cards for the next several years.
And if you are the big banks and you know that's going to happen, you probably want to avoid a scenario like what happened in 2008 where the public knew that you were the source of the malfeasance and the economic problems, which of course spawned movements like Occupy Wall Street.
If you want to avoid that, what is the best way to absolve yourself of any sort of blame for mismanaging or losing people's money?
People are so aware now of what's happening.
I don't think they're going to be able to hide anything.
They might be able to push the analysis off to the response.
And so maybe they get a pass for the massive disruption.
But since their response is going to be massive amounts of printing money, and that's the same malfeasance that they've been doing forever, it almost doesn't matter whether they get off the hook for like we had to do it or not.
People are going to be so frustrated by the inflation that you're still going to get the same kind of pushback because if nothing else, people like me are going to be banging the drum that you guys have been doing this forever before.
You're doing it now, whether you have good reason to do it or not.
The effects are going to be the same and worse if she's right and they manipulate the social contract and they move people over into a money that they can control, regardless of whether it started as a hack.
Dude, I would be screaming from the rooftops that, okay, let's just play this scenario out.
So now they have a money that can control you.
And now they're inflating this to you know all hell.
And who's going to benefit?
All of this stuff is knowable.
So all the people that got their money back, those are pre-inflation dollars.
And now in the giving you of your money back, they just inflated the money supply.
So they actually gave you less purchasing power than was taken from you.
And like, if we're still running deficits and all of that, like you're just, you're in the exact same spot that you were.
Yes, the hackers made it better or made it worse.
And maybe it's better for them because they get off the hook and they don't get the double whammy of we were also.
This is obviously a thought experiment of if they did something nefarious.
Maybe they get off the hook for that and they're not blamed for the false flag.
But nonetheless, the way that they're going to quote unquote solve the problem will be the same thing they've been doing forever because this stuff is mechanistic.
It does like there seems to be a there.
But I could be biased.
Whitney, you do no wrong in my eyes.
I missed you, girl.
Come back on the show.
For real.
Whitney, come back.
It'd be great to have her.
Also, by the way, if you want to challenge me directly about the things that you think that I'm doing that are pro somebody else's government, I want to know.
I would actually love to hear that.
So you certainly have a show that I, if I brought you on, it would be to understand your position.
I'm not going to sit there and argue with you.
You know, that's not my style.
So I would happily do that.
If some of the breakdown is of what I'm doing, one, I will almost certainly push back if I think that it's wrong, but I will seek to understand first so that I can say, hey, this is what I hear you saying.
Do I understand it accurately?
So anyway, that would be amazing.
I would love that.
I'll happily put it out unedited, like whatever you need.
You can say all the things that you need to say up to and including an indictment of the way that you think that I am doing it would be amazing.
Would love that, love that, love that.
Now, going back to what she was saying, I will say this: that I think it's right to be paranoid about it.
I think it's right to put it out there.
I think it's right to talk about these things.
She isn't saying this is already happening, I don't think.
From what I took away, she's just saying, listen, I don't trust the government, rightly so.
And here is an attack vector that they could use that we all need to be aware of.
I don't think they're pushing any reasonable coins.
I don't see a boomer downloading a crypto wallet.
So something has to be done to get them off it because they have a majority of the wealth right now.
So that's why I'm like, okay, my mom will never download a crypto wallet.
But it's one of those things her wealth needs to get transferred one way or another.
The bank could just be like, sorry, this is the new thing.
You just have to in our in your app, now.
Here's your wallet, and it's built in and it's integrated.
And now she's on the crypto system without having to download anything or getting a 12-uh-word hash or whatever, like that.
So it's interesting framing it that way because I feel like it makes me what you always say.
Once you change the framing, it makes like logical steps.
You're like, okay, I see the play now.
Yep.
Like, that's kind of how I feel about it.
Yeah.
No, she's got internal logic.
Whether it ends up being true or not, it's a totally different question, but there is a distressing amount of internal logic.
Yeah.
All right.
And now to the other side of the internet, where is there a woman loneliness epidemic?
Let's talk about it.
This was unavoidable.
So it's Friday night, and I am so lonely and so sad.
I was just sitting here crying about it.
I just like coming on here because it helps me feel less alone in this feeling.
And sometimes it's like hard to say out loud because it just like reminds me of how real it is.
But it's like it's a Friday night, it's 5 p.m.
and I just sat here and ate dinner in complete silence.
And like the silence is absolutely like deafening.
And I just don't think people who have never experienced chronic loneliness understand like how painful it is because it's just like so painful emotionally to humans are not meant to be just feel so alone and just like not have anybody to live your life with.
And it's so hard for me because I am like full of life.
I like I just hiked 500 miles on the Pacific Crush Trail.
I did a road trip to Yosemite by myself a few months ago.
I'm leaving to go to Switzerland by myself in two weeks.
So what I like about this, and I'll give my full breakdown in a second, there's another thing she needs to say for this all to make sense.
But what I like about this is that you've got somebody who the my first layer of advice is always, well, go out and do things.
Like you need to meet people in real life, not online.
She's already doing it.
So it's like she shuts down a normal way to just sort of dismiss these people of like, you're chronically online.
You're always in your house.
Like God forbid that you work remotely.
It's like, now I get how you've isolated yourself.
This is largely just a problem of technology that has these weird artifacts in terms of the way that people interact with each other.
Go out, meet people.
She's doing it.
And I think that this points at a far more distressing problem that's going on.
All right.
She's, she's got another key point she's going to make, and then I'll, I'll give my assessment.
It's like, I'm out here like living my life doing things that I love.
And it just like hurts so badly to have nobody to share it with.
And even just like, honestly, what's even worse is just not having like day-to-day, like doing day-to-day things in life and having people to share it with.
It's like, it's a Friday night and it's 5 p.m.
and I just have nobody to like hang out with.
Like nobody's text.
Like, and that's the thing.
It's not just like, oh, it's just tonight.
It's like, this is like every day of my life.
Like, like, there's nobody ever asking me to hang out.
There's like, I, anytime I like reach out to someone, I have to schedule out like a month in advance to hang out with them.
And then we like never talk again for like months after that.
And it's just like life just feels so meaningless when you don't have anybody to share it with.
And there will be so many people saying, like, you find meaning in your life yourself, or like, you need to learn to be, it's like, I'm sick of that bullshit.
Like, I'm sorry, you have no idea what I'm talking about.
What I see here is certainly multivariate, that is for sure.
But the loneliness epidemic is really about we have broken down the structure of society.
We have so detached ourselves from what is natural that we're now trying to reorient ourselves to figure out why we have all these internal emotions that are coming up that are very negative, that do not feel good.
And even though we're sort of killing it, if you will, on paper, she's doing all the hiking.
She's going all the places.
I'm sure she has a wonderful job.
And what she's realizing is that evolution has optimized us for certain assumptions.
So it has optimized us, assuming that we were going to live in fairly like tight-knit groups, that there was going to be a set of sort of known people that we've known for a long time, that we're interacting with constantly, and that there's almost no escape from that.
And even if it was a microcosm of, okay, these are the people working on the farm, which even that is like very modern in the grand scheme of things.
Traditionally, it would have been hunter-gatherer tribes.
And this is the big one that there was no outlet for sex other than essentially sex with somebody.
I mean, of course, you could jerk off, but it's like without porn, not a whole lot of appetite for that.
And so you had this extreme push for men to seek out women.
And then for women, there was no birth control.
And so if you got your emotional validation through a guy that was in some ways seeking sex, it's not the only way.
And it isn't that I don't want people to have an adversarial men and women view that they are adversarial to each other.
But there is certainly a dynamic tension that evolution could count on, that evolution baked into the cake, if you will.
So for men, sex is very cheap.
For women, it's incredibly expensive in a universe where there's no birth control.
And so all of the what I call algorithms in our brain, those come up over evolutionary time scales of us not having birth control, of us not having access to pornography.
And so you create this world where we're already forced into these groups.
We have a cooperative effort that we're working towards because we're trying to keep everybody alive through a harsh winter or whatever the case may be.
And so we know people, we're interacting with them all the time.
We have our roles and responsibilities.
And women tended towards taking care of the kids because specifically they were the only ones that could do that.
So imagine you can't go to the grocery store and get formula.
The only way that kid is going to eat is if they eat from your breast.
And so it evolution is just like, okay, I know that you're going to be the sexual gatekeeper, that you're going to force a man to be worthy enough to have sex with.
And then part of that exchange is going to be that that man helps you actually raise that child.
So he's going to go out into the dangerous world to do things.
You're going to cluster with other women to take care of your kid, their kids, that a big part of the meaning and purpose in your life is going to be raising those children.
They literally can't survive without the nutrients that your body produces.
And so you start putting that all together, and it's like, cool, everything works.
Now, we definitely feel a sense of like I'm limited, I'm trapped by things.
And so we use innovation as a way to start breaking free from some of those traps.
We start introducing birth control, incredible, massive breakthrough.
People are now in control of when they have kids, when they don't have kids.
Then we start saying, Hey, women could do anything you want.
You can have a kid later in life if you want.
They go in, they find that a career is actually fulfilling in a way that they didn't realize, but it leaves certain itches unscratched.
Introduce into that technology.
And now it's, if you go up and try to flirt with a woman, you're going to get recorded, you're going to get clowned on, you're going to be either called a doofus or a monster that was, you know, perpetrating sexual violence by expressing sexual interest.
It's like now you're putting yourselves in a position where guys have access to pornography, access to a gazillion other ways, reels, video games, everything to occupy their time.
It's dangerous to go after a woman.
It's also not sexually interesting for a lot of guys to go after a woman that is above them on the sexual hierarchy, if you will.
So that they are making more money than them, that they are smarter than them.
That's not typically a thing that a guy's going to go for.
So men tend to date across and down.
Women tend to date across and up, obviously known as hypergamy.
So you get like this super weird collision as women get more power in the workplace, as women are decoupled from the necessary result of seeking companionship is having a child.
And men aren't even seeking sex.
So they're, because they're not being held accountable to a standard of you need to be worthy of sleeping with me, they're sort of flatlining.
And then you get the danger zone of just even approaching somebody as high risk.
And you get this kind of now loneliness epidemic where she might be doing well at her job, but she's now suffering from the things that a man would typically suffer from when he's putting his time and energy into his job, which is he doesn't hang out with people.
He has a hard time maintaining his friendships.
He'll see people once in a while, but not very frequently.
But the problem is, speaking from experience, there's all this evolutionary energy behind that.
So I don't find myself necessarily compelled to go hang out with my friends.
So I don't feel any emotional distress by being isolated, by being alone in a way that women clearly do.
And so it turns into this cluster fuck of like each one of the things that we've done, whether it's the innovation on birth control, whether it's women getting into the workplace, all of these by themselves are awesome.
And it gives people all these incredible choices.
But you start putting it together and some evolutionary expectations begin to break down.
So men have an expectation that they will try to earn sexual access to a woman and thus will turn their potential into skill set trying to climb the ladder.
And so they'll get better and they'll innovate and they'll do all these crazy things and get stronger and more powerful as a man.
And a woman has an expectation that she'll meet this biological imperative to have kids, to raise them and to be part of a social group that looks after the kids and has cooperative pressures that push them together to look after the kids in groups.
And so instead of being isolated, she's driven into like a mom group.
And now that's all breaking down.
But we still have the push from an evolutionary perspective to do it.
And so we feel super weird when we're out of step with that.
That's where we are.
I don't know.
I feel like we have to separate these two things out because I think which are the two things?
The on one side, we have the evolution conversation because I think that there are nuances there as well.
But on the forefront, I think that there is something in adulting that even I experience right now.
We're like, I have a homie and I have this term called couch friends.
Like, friends, I could just go and just sit on their couch.
I don't have to get dressed.
I don't need an agenda.
I don't have to spend money.
I'm, yo, you at the house?
I'm coming out for cool, bet.
But I like, this is somebody that I'm close with.
This is one of my like A1 friends.
I really, I really like him.
But I see him every six months because it's his life because it's bored.
He's building something.
I'm building something.
We're just in these different points.
So when she was going through a frustration of like, even when I want to see somebody, it's like, I can't just pull up.
I have to, which are you with your girl this week?
And then you got that presentation.
Okay.
Then you got to, then before you know it's Saturday, okay, I got to go see Lynn.
Okay, then next week.
And then before you know it, all right, I'll see you, you know, October 14th.
Cool, yeah, bet, we'll hang out.
And then I'm sitting back on my couch, like, damn, I kind of wanted to see somebody today, though.
You know what I mean?
So just with adulting, I think that that's something that a lot of people come to terms with later in life because in college and young adult time, you think you'll be seeing your friends all the time.
It's easy.
But then on the flip side, there is the male, female aspect of it.
But I don't know.
I think, I still think evolution or not, kids or not, people still want to have companionship.
People still want to have groups.
People still want to hang out with people.
And although you don't have that tie to like hang out with people, I want to hang out with the homies and go watch a game or something like that.
It's not even about the game.
It's the camaraderie that goes through it.
That's what really flipped my mind with my brother.
Like, my brother loves sports, but I think it's less about sports.
It's more about me and these five guys drinking beer together and just sharing a bond.
Like, yay, ooh, touchdown, football.
Like, whether they win the Super Bowl or lose the Super Bowl, it's the same thing.
It's just, I'm here with my guys, and we know that Sunday from four to seven, I have this sacred space.
You know what I mean?
And I think that people need to systematize that, and it gets waved off too often.
It's pay your bills, go to work, you know, get up, get a spouse, whatever.
But we don't talk about those third spaces that are integral because they're just naturally happen.
In the playground, you naturally hang out with your friends.
When you're in high school, in college, you naturally go to a happy hour or after hours or whatever the thing is, Thursday, Thursdays, whatever your college campus had.
Now, when you get to adulthood, those things aren't just natural.
You have to kind of generate that.
I agree.
And so, the thing that I will say that life will be confusing if you don't map them differently is that men and women are going to experience that very differently.
And so, if you're sounding the alarm and saying, Hey, the structure of modern life, you weren't super specific, but the structure of modern life is such that even men are now starting to feel isolated.
Then, I'm saying, heard.
Now, you can imagine for a woman who is not evolutionarily optimized to be stoic, to be more resilient to those things, is expected from an evolutionary algorithmic standpoint to constantly be in these groups that are relationship dynamics, building, focused on rearing children, like that whole thing.
They don't have that.
And because of the dynamics that I was talking about before, where men are now less incentivized to approach women and it's risky to approach women from a social pariah perspective, they're not even in a relationship with a guy to be able to have a project where it's like, ooh, I'm going to like push him to do better and become this thing.
All these stereotypes that growing up in the 80s were just self-evident that a woman just wants to change a man.
So, but imagine it was deeply fulfilling for her and certainly an area of focus to want to push him to be better and all that and to take care of the kids and her and all that.
And so, they've got this thing to focus on, put their energy on, to interact with the world through the man.
And, like, again, I get why many women felt trapped by that because it was the only option.
But still, the way that the evolutionary mind works is women had to interface with the dangerous world through men, through men, and then through the social structure of women, which is why their social dynamics can be so strangely vicious and aggressive.
Women are not like these passive creatures by any means.
But, like, that's how we've sort of come up.
Okay, now to speak to the male side of this very specifically: one, I think everybody, if I wasn't in a marriage, I would feel very different about being able to be isolated.
I wouldn't want it, it would be too much.
I know, because before I was married, there were times where I felt a profound sense of disease because I would just come home and literally lay on the floor.
It was a particularly dark period that wasn't just about being lonely, but that was like, I know that emotion well.
So, when you're looking at modern life and all the ways that it presents things that pull us apart, yes, men and women are going to have to combat that both.
But when you look at the derangement, is pushing women into a more masculine form of being and then pushing men into a more feminine mode of being.
And those are the things that begin that are the beginning of the derangement.
And so, we have to find ways to construct our lives such that we don't fall for those traps, so that men are pursuing relationships with women, which will then trigger this desire to be worthy, to push yourself, to grow, to get better.
And then obviously the thing that I get meme for: it's like, if you're not going to have kids, you better have a damn good reason because evolution is expecting you to have kids.
And so if you don't, and you don't have something to put in its place, then you're going to find this profound sense of dis-ease that she's struggling with.
The same is true for men and women, but probably more profoundly felt by women.
Autumn Lynn in the chat said this is the point in time where Tom's going to tell us we shouldn't have got educated the women.
That's so interesting.
So, okay, this is one of those, every time this comes up, I'm going to make an attempt to make sure that I'm heard.
Now, the great irony of a frame of reference, when you're locked inside of it, it doesn't matter what the person says, you literally can't hear what they're saying.
And the thing I'm saying is, I love that women got educated.
Amazing.
There's a trade-off.
And so if you know there's a trade-off, do something to deal with it.
Not go back, do something to deal with it.
So how are we at a societal level going to deal with it?
How are we going to deal with it at the individual level?
So this is something that I talk to Lisa about all the time.
Cool, you're not going to have kids, but you need to make sure that you understand the role that raising kids plays in your mental health.
And if you don't understand that there is a mental health aspect to taking care of kids, then you're going to be confused as to why you hate your life.
And you'll be like, why, why do I feel so unfulfilled?
And it's like, that's going to come for you.
And so Lisa will eventually, and so will I, by the way, will eventually get to the point where we don't want to be entrepreneurs anymore.
And so, when Lisa decides she doesn't want to be an entrepreneur, she's got to have an answer for, and now what?
Why do I matter?
Why does anybody care about me?
Post-menopausal women tend to either plug more deeply into their kids' lives, and this is how mother-in-laws become a nightmare, or, and by the way, people need to understand why that stereotype is true.
That is a post-menopausal woman who is not able to express her sexuality anymore.
And now, life is about the thing I did.
And the thing I did was I raised kids.
I'm no, if she was engaging in a career before, she may not be now.
And so, it's like from time immemorial, mother-in-laws became a problem because once that period of raising children ended, they were now in a period of like, what do I do?
And so, they would try to re-engage with their adult children.
They would create all kinds of problems, but it was a way for them to remain relevant and to be needed.
And so, it's like, I don't know what people want me to say.
I am certainly not saying don't educate women, but don't be a fucking retard and not look at the world and go, Oh, wow, there's really interesting correlates that go along with when you mass educate women that it has a knock-on effect.
We should probably plan for that knock-on effect so that the answer doesn't become don't educate women.
Fuck tards.
That's the part where I like wake up.
So, you've got to have an answer for it because, hey, let's get real controversial.
Guess what one of the answers is going to be?
Did you guys ever see the stickers?
I think this happened in Massachusetts.
Muslims were right about women.
Oh, look that one up.
So, that's a lot of fun.
What do you do with that statement?
That glitches people the fuck out.
So, do you go?
Hey, yeah, we're just, we're not going to educate our women.
We're going to make sure that we put them into a more traditional role, get them out of education, and get them back into the household and put them in a burqa.
Like, okay, like that is going, that is an answer being put forward right now that has a lot of momentum going for it.
So, plan for these, boys and girls, so that we can have a sensible solution and not just a knee-jerk reaction where we go backwards to things that we've already tried.
I want to see us go, oh, okay, cool.
There is this knock-on effect where people feel a profound sense of disease.
They are searching for an answer and they will find it in stricter religions.
If you don't believe me, watch the next 10 years.
And so, you're going to see Christian fundamentalism rise.
You're already seeing the rise of fundamentalist Islam.
So, it's like, kids, if you want that to be the solution, then by all means, say this is where what you hear, even though I'm expressly saying the exact opposite, that you hear me saying that women shouldn't be educated.
And I keep fucking saying over and over, I'm not saying that.
It's awesome that it's happened.
I have a wife that has made use of all of these things, and I love her to death.
And I want to see her have every choice in the world.
But if you don't recognize that there are consequences that can be addressed in other ways, then you're going to be very confused when we all start racing backwards.
Cool.
That's all I got.
All right, boys and girls, thank you so much for joining us.
We love you bunches and bunches.
And to that effect, because I love you guys so much, I'm doing a free ITU AI masterclass Thursday, September 10th at 1 p.m.
Pacific.
I will show you how to use Real AI, all of its weaknesses, where its strengths are, how to use it well to launch your company.
It's all free, and it is the 10th of September at 1 p.m.
Pacific.
Link is in the description.
All right, see you there.
And we will see you on Wednesday.
Until then, my friends, be legendary.
Take care.
Peace.
Let's talk about a pattern that is guaranteed to be killing your progress.
You know what you need to do.
You need consistent nutrition.
We all do.
You need vitamins, probiotics, greens.
We all know that we should be doing more of it.
When your morning gets chaotic, you skip it.
When you travel, you skip it.
When your routine breaks, everything tends to break.
And that inconsistency compounds against you every single day.
AG1 is designed to solve the execution problem.
One scoop, eight ounces of water, and you're done.
You're getting 75 plus ingredients, vitamins and minerals, pre and probiotics, nutrient-dense superfoods, everything that used to require six, seven different supplements, and perfect planning now happens in one drink that takes about 30 seconds to make.
Right now, AG1 is giving you $87 worth of free gifts with your first subscription.
You get a welcome kit, travel packs, vitamin D3 plus K2, and flavor samples.
Click the link in the show notes or visit drinkag1.com/slash impact to claim this offer.
