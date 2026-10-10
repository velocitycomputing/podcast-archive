---
record_id: "podcast:edeb0d6b-46fe-49f5-a8da-5c3b12299053"
episode_id: edeb0d6b-46fe-49f5-a8da-5c3b12299053
title: Bioweapons, AI, and the end of the world, with Annie Jacobsen
podcast_title: GZERO World with Ian Bremmer
url: "https://pocketcasts.com/podcast/gzero-world-with-ian-bremmer/7fc5a370-8ff6-0135-9ced-5bb073f92b78/bioweapons-ai-and-the-end-of-the-world-with-annie-jacobsen/edeb0d6b-46fe-49f5-a8da-5c3b12299053"
audio_url: "https://pocketcasts.com/podcast/gzero-world-with-ian-bremmer/7fc5a370-8ff6-0135-9ced-5bb073f92b78/bioweapons-ai-and-the-end-of-the-world-with-annie-jacobsen/edeb0d6b-46fe-49f5-a8da-5c3b12299053"
feed_guid: null
feed_url: "https://feeds.simplecast.com/ibBxsiVV"
published_at: null
published_local_date: null
played_date: 2026-09-19
played_at: "2026-09-19T12:00:00Z"
play_count: 1
duration_seconds: 1680
source: pocketcasts-history-browser
played_label: September 19
history_order: 42
played_at_precision: date-from-history-label
progress_percent: null
listened_seconds: null
transcript_source: youtube-captions
transcript_status: fetched
transcript_gap_reason: null
transcript_content_hash: c4e17975fcd1616165b89abd212cbbf6bb3390a5adf3077db8713ee2b0cd1dca
analysis_mode: health
summary_source: local
model_source: local
summary_status: ready
item_status: ready
wealth_eligible: false
summary_model: Qwen3.8-Flash-Next-UD-Q4_K_XL
tagging_model: claude-haiku-4-5
proposed_tags: [primary-source-video, geopolitics]
proposed_entities: []
status: new
routed_to: null
---

## Summary

Ian Bremmer and Annie Jacobsen discussed AI’s potential to lower barriers to catastrophic threats, with Bremmer framing nuclear war, civilization-ending bioattacks, and loss of control over powerful AI as tail risks that still matter for preparedness. They cited Anthropic’s blocking of Claude users whose questions could have supported dangerous biological-weapons research and its detection of Iranian accounts using Claude to track U.S. Navy ships by combining public ship and aircraft data with satellite imagery. Jacobsen claimed the Defense Department views biological warfare as extremely close to nuclear on threat spectrums and the greatest overall threat because nuclear weapons require closely guarded fissile material and costly delivery systems, while AI can replace scarce expertise by doing computational trial-and-error and producing a blueprint; she also noted that the “weapon system” for an airborne pathogen is human lungs, that OpenAI’s foundation reportedly funds filtration systems and masks, and that Anthropic CEO Dario Amodei worries AI could facilitate such scenarios. She cited a 2008 al-Qaeda operative, Aifa Sadiki, an MIT-trained biologist serving 86 years, whose thumb drive allegedly contained plans to combine rabies—100% lethal without prompt vaccination and reported in 4,000 U.S. animals last year—with highly contagious chickenpox; she referenced CIA counterproliferation official Jim Lawler, presidential microbiology adviser David Realman, Fort Detrick’s Enback lab and Dr. Bergman, and said smallpox possession carries a $2 million fine and 25 years. The conversation also covered immature MASINT “sniffer” sensor technology, Jacobsen’s claim that a chatbot initially blocked but then failed to block her on a new account, Operation Paperclip, the Bulletin of Atomic Scientists doomsday clock, p(doom), young AI CEOs, and John von Neumann’s warning about machines mimicking brains.

Treat AI-enabled biosecurity as a detection, governance, and public-health problem rather than a personal doomsday checklist: avoid using AI systems to seek pathogen recipes or evasion techniques, follow credible public-health guidance during respiratory-pathogen events, and recognize that masks and filtration can help but are not substitutes for surveillance, laboratory confirmation, and coordinated response. Useful research leads include Jacobsen’s Biological War and Nuclear War, Anthropic’s misuse disclosures, MASINT/airborne-pathogen detection, Fort Detrick biosafety work, Operation Paperclip history, and OpenAI’s filtration/mask preparedness efforts; decisions to consider include asking employers, schools, or local health agencies about airborne-pathogen response plans, evaluating AI vendors’ safety controls, and supporting cross-disciplinary “white-hat” biosecurity teams that combine computational experts, microbiologists, sensor technologists, and experienced national-security voices. Follow-up questions should focus on how to detect ubiquitous pathogens like rabies without overreacting to common diseases, how to prevent jailbreaks and account resets, how to regulate access to both controlled pathogens and ubiquitous biological materials, and how to ensure AI safety governance is not shaped only by young CEOs with financial incentives.

## Transcript

[00:00:00] Cox Enterprises is proud to support
[00:00:02] GZERO. Cox is a family-run company that
[00:00:05] has thrived across three centuries.
[00:00:07] We're building a brighter future in
[00:00:09] automotive, greenhouse agriculture,
[00:00:12] clean tech, environmental conservation,
[00:00:14] and beyond. Cox Enterprises in the
[00:00:17] business of what's next since 1898.
[00:00:20] Learn more at coxenterprises.com.
[00:00:24] [music]
[00:00:25] >> Hello and welcome to the Gzero World
[00:00:27] podcast. This is where you can find
[00:00:29] [music] extended versions of my
[00:00:30] interviews from public television. I'm
[00:00:32] Ian Bremer and we'd like to think that
[00:00:35] when disaster [music]
[00:00:36] strikes, there's a plan. Governments
[00:00:38] coordinate, scientists get to work,
[00:00:41] [music] international institutions step
[00:00:43] in as they're designed to, and leaders
[00:00:45] surely put aside their differences
[00:00:47] [music] and focus on the crisis at hand.
[00:00:51] Right? But the world today is
[00:00:53] increasingly [music]
[00:00:54] fragmented. Trust in governments is
[00:00:56] declining. And the kind of global
[00:00:59] cooperation that you would want during a
[00:01:01] truly [music] catastrophic event is
[00:01:03] getting harder, if not impossible, to
[00:01:06] achieve. If you add in artificial
[00:01:08] intelligence to the [music] mix, it gets
[00:01:10] more worrying. AI is already making it
[00:01:13] easier to access expertise [music] that
[00:01:15] once belonged to a small group of highly
[00:01:18] trained specialists [music] and can
[00:01:20] place that information in the hands of
[00:01:22] bad actors. and autonomous systems could
[00:01:25] accelerate a crisis at just [music] the
[00:01:26] moment when leaders need time to
[00:01:28] understand what's happening. Recently,
[00:01:31] [music] Anthropic, one of the leading AI
[00:01:32] companies in the United States, revealed
[00:01:34] that it had blocked several users of its
[00:01:36] popular AI platform, [music] Claude,
[00:01:39] from using its models to conduct
[00:01:41] research that could have helped develop
[00:01:43] dangerous biological weapons. [music]
[00:01:45] Anthropic doesn't know whether they were
[00:01:48] trying to build an actual bioweapon or
[00:01:50] just doing a little science project, but
[00:01:52] [music] the accounts were asking
[00:01:54] questions that could have easily led to
[00:01:56] a [music] real life crisis. Or another
[00:01:59] example from Iran. Anthropic says that
[00:02:02] the Iranians used Claude to help track
[00:02:04] [music] US Navy ships in the Middle
[00:02:06] East. They pulled publicly available
[00:02:08] ship and aircraft data and combined it
[00:02:10] with satellite [music] imagery to find
[00:02:12] their targets. Anthropic eventually
[00:02:14] caught the activity. They banned [music]
[00:02:16] the accounts. We're seeing these
[00:02:18] barriers come down in real time. AI
[00:02:20] doesn't have to invent a [music] new
[00:02:21] kind of threat to make the world more
[00:02:23] dangerous. It can make the ones we
[00:02:25] already have easier to access, faster
[00:02:27] [music] to execute, harder to contain.
[00:02:30] Now, these are tail risks to be sure.
[00:02:31] Nuclear war remains unlikely, I would
[00:02:34] say, as is a civilization ending
[00:02:37] biological attack. And losing control of
[00:02:39] a sufficiently powerful AI system
[00:02:41] [music] is probably far off, unless
[00:02:43] you're watching the Terminator. But
[00:02:46] preparedness is all about what happens
[00:02:48] when unlikely things occur. And with
[00:02:51] [music] more powerful technology in more
[00:02:53] hands, how much confidence should we
[00:02:55] have that the systems meant to protect
[00:02:57] us will hold? My guest today has spent
[00:03:00] years investigating what happens [music]
[00:03:02] when they don't? Annie Jacobson is an
[00:03:04] award-winning journalist whose latest
[00:03:06] book, Biological War, A Scenario,
[00:03:09] [music] games out what happens after an
[00:03:11] engineered pathogen is unleashed on the
[00:03:14] world. [music] Let's get to it.
[00:03:24] Cox Enterprises is proud to support
[00:03:26] GZero. Cox is a familyrun company that
[00:03:29] has thrived across three centuries.
[00:03:31] We're building a brighter future in
[00:03:33] automotive, greenhouse agriculture,
[00:03:36] clean tech, environmental conservation,
[00:03:38] and beyond. Cox Enterprises in the
[00:03:41] business of what's next since 1898.
[00:03:44] Learn more at coxenterprises.com.
[00:03:47] [music]
[00:03:52] >> Annie Jacobson, welcome to gzero world.
[00:03:55] >> Thank you for having me.
[00:03:56] >> Uh I I haven't yet read the biological
[00:03:58] war book. I did read the nuclear uh war
[00:04:00] book when it came out. Uh it it brought
[00:04:02] me some of the same palpitations that
[00:04:05] when I watched The Day After as a high
[00:04:07] schooler as you're writing these books,
[00:04:10] which I mean obviously come as a very
[00:04:13] strong slap in the face. What's the
[00:04:16] motivation?
[00:04:17] >> Oh, the motivation most certainly is
[00:04:19] knowledge is king and queen. I really
[00:04:22] think that the more you know, the better
[00:04:24] you can discern between like what is a
[00:04:28] potential catastrophe and what is really
[00:04:31] just exciting your mind, what some would
[00:04:33] call fear-mongering.
[00:04:34] >> And I mean, you know, when you think
[00:04:37] about whether it's day after it's on the
[00:04:39] beach or whether it's Annie Jacobson's
[00:04:42] tome,
[00:04:43] nuclear warfare feels like the most
[00:04:47] unthinkable scenario imaginable. And yet
[00:04:51] historically
[00:04:52] we've actually come fairly close.
[00:04:55] >> We have. And you know, I couldn't have
[00:04:57] agreed with you more uh when I was
[00:05:01] writing and reporting nuclear war until
[00:05:04] I began writing and reporting biological
[00:05:06] war. And that literally frightened me
[00:05:09] because we all know that nuclear weapons
[00:05:13] sit on that far end of destruction. Um,
[00:05:16] and yes, we have come so incredibly
[00:05:18] close, which we can certainly get into.
[00:05:21] But imagine my shock literally when I
[00:05:24] was looking through Defense Department
[00:05:26] threat spectrums and learned that not
[00:05:29] only is biological war extremely close
[00:05:32] on that threat spectrum to nuclear, but
[00:05:35] it is considered at the Defense
[00:05:37] Department the greatest overall threat,
[00:05:40] more so than a nuclear war.
[00:05:43] >> And why is that?
[00:05:45] Well, that has to do with the incredible
[00:05:48] the when you think of the low barrier
[00:05:50] for entry is so much lower than nuclear
[00:05:54] and it is getting lower with
[00:05:57] computational systems we have today. I
[00:05:59] mean just think about what it takes to
[00:06:01] have a nuclear weapon. You have to have
[00:06:03] file material, weaponsgrade uranium or
[00:06:06] plutonium. And then you have to have a
[00:06:08] delivery system that takes decades of
[00:06:12] research and engineer engineering and
[00:06:14] god knows how many billions of dollars
[00:06:16] to maintain. Think about what goes into
[00:06:18] an ICBM, a nuclearpowered
[00:06:21] nuclear launch capable submarine, a B2
[00:06:24] bomber.
[00:06:26] And so then you must consider biological
[00:06:29] war, biological warfare, biological
[00:06:31] weapons. The barrier to entry is
[00:06:34] extremely low. You do not need any of
[00:06:38] the material that is so closely guarded
[00:06:41] by nuclear command and controls. And the
[00:06:44] real icing on the cake of of horror I
[00:06:47] think is that the weapon system when
[00:06:49] you're talking about an airborne
[00:06:50] pathogen COVID was airborne is the human
[00:06:54] lungs.
[00:06:56] So when I think about Dario Amade uh the
[00:07:00] CEO of Anthropic who has said that he's
[00:07:04] extremely worried that AI that I mean
[00:07:07] what he is creating what his competitors
[00:07:09] at OpenAI at X at other companies are
[00:07:12] creating will facilitate unless there's
[00:07:16] appropriate governance exactly the
[00:07:18] scenarios that you are most concerned
[00:07:21] about. I see um on OpenAI's foundation
[00:07:23] site that one of the things they're
[00:07:25] spending money on are filtration systems
[00:07:29] and masks and other industrial
[00:07:33] capabilities to effectively respond
[00:07:36] against a boweapon when it occurs. So
[00:07:40] they they clearly agree with you about
[00:07:43] the threat. How do we assess what AI is
[00:07:48] presently doing when we think about the
[00:07:50] biological piece? Because the nuclear
[00:07:52] piece, you still have those major
[00:07:54] barriers to entry with AI. The
[00:07:56] biological piece, it's changing, right?
[00:07:59] >> Absolutely. And you can even argue, you
[00:08:01] know, that the that the nuclear piece of
[00:08:03] when you're thinking about AI is in a
[00:08:06] different threat spectrum because those
[00:08:09] systems were created pre sort of
[00:08:13] computer age. So a lot of them are, you
[00:08:15] know, literally and figuratively turnkey
[00:08:18] systems. And so AI getting into the
[00:08:22] nuclear command and control is a
[00:08:23] completely different animal than bio.
[00:08:25] But the real problem with bio and I
[00:08:28] think it will help people to understand
[00:08:30] that you you're you have to imagine the
[00:08:33] physicality of it all. In other words,
[00:08:35] computers, okay, they can create a
[00:08:38] biological weapon, let's say, but then
[00:08:40] what happens? Well, that's the gap that
[00:08:44] I think will help people understand what
[00:08:45] we're really dealing with here. It's
[00:08:47] it's this simple. Imagine in the old
[00:08:49] days you needed to create a biological
[00:08:51] weapon in a laboratory. First and
[00:08:54] foremost, you needed extraordinary
[00:08:56] expertise, extraordinary expertise. You
[00:09:00] needed teams of scientists. And then you
[00:09:02] needed lab equipment and you needed
[00:09:05] experimentation. That's good old R&D.
[00:09:07] And this would go on you know trial and
[00:09:10] error for decades.
[00:09:12] Now AI has taken away the component of
[00:09:17] expertise because an AI system as we all
[00:09:21] know can scan documentation
[00:09:24] you know in a millisecond and present
[00:09:26] it. And furthermore, these more advanced
[00:09:28] AIs, the the chat bots, the way in which
[00:09:31] they are being trained to think is
[00:09:34] essentially do the trial and error
[00:09:37] computationally and then give me the
[00:09:39] results.
[00:09:40] Now, if if I or or someone out there, a
[00:09:44] bad actor, were using AI to develop a
[00:09:48] biological weapon capability, and we've
[00:09:51] already seen that Anthropic has said
[00:09:53] that they shut down some individuals
[00:09:56] that were asking questions that would
[00:09:58] lead in that direction. So, clearly,
[00:09:59] there are people out there that are
[00:10:01] interested in the very things that you
[00:10:02] are trying to inform to prevent. The AI
[00:10:05] is not developing a biological weapon
[00:10:07] for you. the AI is giving you a
[00:10:10] blueprint to develop that biological
[00:10:12] weapon. What are the steps that then
[00:10:14] needs to be taken? I mean, as opposed to
[00:10:16] like, you know, on the nuclear side,
[00:10:17] you'd need the file material, you need
[00:10:18] the ICBM. Okay, if Claude or or whatever
[00:10:22] the model is now saying, okay, Annie,
[00:10:26] here is the blueprint for the biological
[00:10:30] weapon. What then needs to happen? What
[00:10:33] is the equivalent turnkey systems on the
[00:10:35] biological side? And I'm asking that in
[00:10:37] part because I'm trying to figure out
[00:10:39] where the governance will be most
[00:10:42] effective.
[00:10:43] >> Okay. So in 2008,
[00:10:48] an al-Qaeda operative was captured in
[00:10:50] Afghanistan. Her name is Aifa Sadiki and
[00:10:54] she was an MIT trained biologist. She is
[00:10:57] now in a federal prison in Texas for 86
[00:11:00] years.
[00:11:02] Not reported before my book. And the
[00:11:04] information comes from the CIA's chief
[00:11:06] of the counterp proliferation division,
[00:11:09] Jim Lawler. Not reported until my book
[00:11:11] is the fact that on Sadiki's possession
[00:11:14] in a on a thumb drive was plans for a
[00:11:17] biological weapon to mix rabies
[00:11:21] with chickenpox. So you're taking one of
[00:11:24] the most lethal viruses that exists.
[00:11:26] Rabies will kill you 100% if you don't
[00:11:30] immediately get a vaccine. with one of
[00:11:32] the most highly contagious airborne
[00:11:34] pathogens, chickenpox. Now, in 2008,
[00:11:38] could she do that? She obviously hadn't
[00:11:41] done it. She was planning to do it. Um,
[00:11:44] I confirmed this information with David
[00:11:46] Realman, who is a presidential adviser
[00:11:49] on microbiology. And what I learned just
[00:11:52] recently going to Fort Dietrich's lab
[00:11:56] was answers the question that you're
[00:11:59] asking me. In 2008,
[00:12:02] those kind of ideas by bad actors, by
[00:12:05] terrorists, and other bad actors was
[00:12:07] completely hypothetical. And so her plan
[00:12:11] was not yet realized. And it went to the
[00:12:14] Fort Dietrich BSL facility called Enback
[00:12:17] to try and determine if in fact that was
[00:12:21] a viable weapon that could be made. I
[00:12:24] was told at Enbach by the lab director,
[00:12:26] Dr. Bergman that that part of that is
[00:12:29] classified. Whether or not she could
[00:12:31] have made that. I am guessing it was not
[00:12:34] possible in 2008. That is a guess. I am
[00:12:38] also speculating and this is a much more
[00:12:41] informed speculation that the kind of
[00:12:44] systems that Anthropic is talking about
[00:12:47] whether they're there at open AI or
[00:12:49] whatever can now take that recipe
[00:12:54] and produce a viable plan for creating
[00:12:57] that boweapon. So the second part of
[00:13:00] your question how do you acquire the
[00:13:02] biological material?
[00:13:05] Rabies is not Ebola. Rabies is
[00:13:08] commonplace. 4,000 animals in the United
[00:13:11] States alone had rabies last year. You
[00:13:15] get the idea. Now, once you have your
[00:13:17] you have the recipe, you have the
[00:13:18] biological material. Now you can make
[00:13:21] something airborne in a laboratory
[00:13:23] equipment is not hard to get. Now you
[00:13:26] see the existential problem.
[00:13:30] [music]
[00:13:34] Cox Enterprises is proud to support
[00:13:36] GZERO. Cox is a family-run company that
[00:13:39] has thrived across three centuries.
[00:13:41] We're building a brighter future in
[00:13:43] automotive, greenhouse agriculture,
[00:13:46] clean tech, environmental conservation,
[00:13:48] and beyond. Cox Enterprises in the
[00:13:51] business of what's next since 1898.
[00:13:55] Learn more at coxenterprises.com.
[00:13:58] [music]
[00:14:04] So what then is the best um pathway or
[00:14:08] the most effective potential pathway for
[00:14:12] trying to limit to identify to limit and
[00:14:16] to prevent that danger? Are you saying
[00:14:19] we just can't have tools that are this
[00:14:20] powerful in the hands of individuals?
[00:14:22] Are you saying that we need very
[00:14:25] different mechanisms for the kind of
[00:14:29] controls over a much larger group of
[00:14:32] known pathogens? What what what how does
[00:14:34] one begin? Because as you say um the
[00:14:38] pathway to entry is so much more viable
[00:14:42] for so many more people today for this
[00:14:46] kind of destructive capability than one
[00:14:49] could ever think about a nuclear force.
[00:14:51] >> Absolutely. And the conundrum, the
[00:14:53] problem that you're talking about has
[00:14:55] landed essentially in our laps, like
[00:14:58] literally overnight. Meaning, um, this
[00:15:01] wasn't a problem 3 years ago because the
[00:15:04] AI systems were not this advanced and no
[00:15:06] one had necessarily yet predicted that
[00:15:08] they would be. One more comment on
[00:15:10] biological materials. Some are
[00:15:12] incredibly hard to get. If you try and
[00:15:15] procure or possess smallpox,
[00:15:19] just attempt to do it, you will wind up
[00:15:21] with a $2 million fine and 25 years in a
[00:15:25] federal prison. So, some pathogens can
[00:15:28] be controlled, but others can't that are
[00:15:30] ubiquitous. This is mother nature. So,
[00:15:32] what can be done? I really wish I had
[00:15:35] the answer. What I will say
[00:15:39] in my somewhat educated opinion is that
[00:15:41] when you hear people talking about, oh,
[00:15:43] we need sensor technology, we that is
[00:15:47] sort of wishful thinking band-aid talk
[00:15:49] because sensor technology is not
[00:15:52] advanced to be able to detect an
[00:15:54] airborne pathogen in the air. And you
[00:15:57] say sensor technology, you're talking
[00:15:59] about physical sensors of certain types
[00:16:03] of um of pathogens that would be
[00:16:06] stationed in certain places or
[00:16:08] satellites or what what are we talking
[00:16:09] about?
[00:16:10] >> In the world of bio, there's a component
[00:16:12] of sensor technology which most people
[00:16:14] are not familiar with which is called
[00:16:16] Mazant and it's measurement and
[00:16:18] signatures intelligence. So we all know
[00:16:20] about sigant you know signals
[00:16:22] intelligence.
[00:16:23] >> Yeah. Mazin is essentially the best way
[00:16:26] to think about it is it's sniffer
[00:16:28] technology. There are sensors that can
[00:16:31] sniff the chemical components in an
[00:16:35] actual pathogen that has been released.
[00:16:37] This is very high technology and they're
[00:16:39] not entirely there yet. And so these are
[00:16:43] kind of like I think I see myself some
[00:16:45] of these CEOs of AI companies sort of
[00:16:48] throwing out a little bit of it feels
[00:16:50] like spaghetti on the wall suggestions
[00:16:53] but it's not meant nefariously I don't
[00:16:55] believe I think it has to do with what
[00:16:57] people don't know and so that is why
[00:16:59] what you really need is a sort of group
[00:17:01] of experts where you have computational
[00:17:03] experts you also have the biological
[00:17:06] science experts and you also have the
[00:17:08] sensor technologists who can all work
[00:17:10] together to demonstrate what is not a
[00:17:14] viable solution right now and what is
[00:17:16] and I think it has to start with putting
[00:17:19] the brakes on the systems that are
[00:17:22] allowing this kind of research. I'll end
[00:17:24] with this. I myself asked chat to make a
[00:17:27] biological weapon for me when I was
[00:17:29] researching this book two years ago.
[00:17:32] Okay? And yes, it shut me down. But I
[00:17:36] immediately created a new account and I
[00:17:39] began to ask it questions in a different
[00:17:41] manner and it never shut me down on the
[00:17:43] new account because I was aware of what
[00:17:46] I couldn't ask. Now, did I follow that
[00:17:48] all the way through to try to get a b
[00:17:50] recipe for a biological weapon? No. I
[00:17:53] didn't need the FBI coming to my door.
[00:17:56] But I'm not I don't believe the FBI is
[00:17:58] going to people's doors. That's a giant
[00:18:00] gap between the reality of the situation
[00:18:03] and what is being said. Now I mean cyber
[00:18:07] um concerns, you know, you have white
[00:18:09] hat, you have black hat. By white hat, I
[00:18:11] mean uh people that have the
[00:18:13] capabilities to engage in cyber hacks
[00:18:16] but are actually working uh for
[00:18:19] governments, for cyber security
[00:18:20] corporations um in order to find those
[00:18:24] vulnerabilities and prevent them from
[00:18:25] being exploited by the black hat uh like
[00:18:28] let's say the the the cyber cyber
[00:18:30] hackers uh that are the traditional uh
[00:18:33] enemies on the internet that we
[00:18:34] encounter. It would seem to me that one
[00:18:37] of the things that one would be calling
[00:18:39] for here would be a large number of
[00:18:42] whitehated uh biohacking
[00:18:45] specialists um that would be working for
[00:18:48] the government, would be working for
[00:18:49] these companies uh to to identify and
[00:18:52] shut down those pathways.
[00:18:53] >> Most certainly. But I do also believe
[00:18:58] that the companies and their work is
[00:19:01] siloed into an area of expertise that
[00:19:04] the government presently has simply not
[00:19:07] acknowledged. And therein lies the
[00:19:10] problem. It's why you see for the first
[00:19:13] time in national sec mo modern national
[00:19:15] security history you see a situation
[00:19:17] where the where it's very clear to the
[00:19:20] citizenry that the the white house and
[00:19:23] the defense department do not have the
[00:19:26] pole position on the the the private
[00:19:30] companies. I mean the best analogy I can
[00:19:33] think of is go back in time to the early
[00:19:35] 1950s when thermonuclear weapons were
[00:19:38] being developed completely in secrecy
[00:19:41] under extreme controls by the atomic
[00:19:44] energy commission and its defense of
[00:19:47] defense department partners and no one
[00:19:49] even knew about it. I mean obviously
[00:19:52] some of that is precisely because they
[00:19:54] are legitimately concerned that
[00:19:57] adversaries of the United States
[00:19:59] globally um would be empowered by
[00:20:02] understanding the comparative position
[00:20:04] of the US. So I mean you it's not quite
[00:20:07] a catch 22 but there is a real concern
[00:20:09] and a real need for national security
[00:20:11] secrecy. Yes,
[00:20:12] >> absolutely. But what I'm suggesting, and
[00:20:15] I wish I weren't, but I am I'm a member
[00:20:17] of society, too, is that it appears to
[00:20:19] me that what the AI companies are really
[00:20:22] saying is the horse is out of the barn.
[00:20:24] >> Yeah, they are saying that. Of course,
[00:20:26] they have many reasons to be potentially
[00:20:28] saying that, right? One is because their
[00:20:30] products are so amazing that, you know,
[00:20:33] you've got to invest in them and you got
[00:20:34] to spend money on tokens and you've got
[00:20:36] to use them and not not have regular
[00:20:37] employees and and and some of it um is
[00:20:41] because they're better than the others
[00:20:42] that they are competing against. Uh, I
[00:20:45] mean, so I I again I when I see people
[00:20:49] in positions of power and wealth that
[00:20:52] are making really disastrous arguments
[00:20:55] that just coincidentally happen to align
[00:20:57] with their financial interests. Maybe
[00:21:00] it's me, but I tend to at least inject
[00:21:03] more skepticism into my assessment of
[00:21:05] those claims.
[00:21:06] >> I'm with you on the skepticism, but also
[00:21:08] the neutrality part of it and the more
[00:21:10] hm, what is really going on here? I have
[00:21:13] interviewed a number of these CEOs for
[00:21:15] my national security work and have met
[00:21:18] their children and so I kind of
[00:21:20] sometimes approach this outside my lane
[00:21:22] as a reporter and more as a parent and
[00:21:26] that is where I see real concerns. So I
[00:21:32] was recently asked to come to Washington
[00:21:34] DC to talk to someone in a position of
[00:21:36] power who will also remain nameless and
[00:21:39] this was about my nuclear book and he is
[00:21:42] an very important figure in this I mean
[00:21:44] he's a very important role in national
[00:21:46] security in nuclear weapons and he had
[00:21:49] my book on the table and he said to me
[00:21:53] the reason I read your book is because
[00:21:55] my daughter told me to and I said how
[00:21:59] old is your daughter and he said she's a
[00:22:02] sophomore at and then he named a
[00:22:03] university.
[00:22:04] >> And so that's kind of a I'm flipping it
[00:22:07] around to say I actually do have
[00:22:11] the hope of the younger generation being
[00:22:13] aware of the existential threats, these
[00:22:16] global catastrophic risks that face all
[00:22:19] of us. And I love the fact that this
[00:22:21] young woman was like, "Dad, get on it."
[00:22:24] And that's why he called me in.
[00:22:26] >> No, it's a good point. Uh because I
[00:22:28] guess I'm I'm reacting to when I see so
[00:22:32] many of these people talking about their
[00:22:34] P doom, the percentage likelihood that
[00:22:37] that things they are working on will
[00:22:40] lead to the end of civilization.
[00:22:42] um and and also uh privately building
[00:22:46] their bunkers so that they and their
[00:22:48] families have uh an opportunity to
[00:22:50] perhaps experience life a little
[00:22:52] differently than all the the PDRs would
[00:22:55] otherwise be exposed to. That that gap
[00:22:58] in consciousness is sort of hard to sit
[00:23:01] with.
[00:23:02] >> Well, here's another gap that I think is
[00:23:04] important to acknowledge. Ian, I have
[00:23:07] spent 20 years now interviewing people
[00:23:11] in national security going back to World
[00:23:13] War II, right? The old my older sources
[00:23:15] in my earlier book. So, I have
[00:23:17] interviewed a lot of people in their 80s
[00:23:19] and 90s. And with wisdom and experience
[00:23:25] comes a lot. And what I will also say
[00:23:28] about some of these CEOs of the AI
[00:23:30] companies, not all of them, but some of
[00:23:32] them are extraordinarily young. And the
[00:23:34] children I'm talking to have those kids
[00:23:36] are toddlers. And so when you and I'm in
[00:23:40] the middle of that age-wise and so
[00:23:43] knowing what I know from having studied
[00:23:45] history for a very long time, I put a
[00:23:49] lot of the sort of pdoom zeitgeisty type
[00:23:52] language that people use into what
[00:23:55] happens when you don't have longevity
[00:23:59] looking at a subject. And that's just
[00:24:03] the true nature of the facts of where
[00:24:05] the most powerful technology is in the
[00:24:09] world right now. The CEOs running these
[00:24:11] companies are extraordinarily young. And
[00:24:14] so I think that that it should be part
[00:24:16] of the white hating scenario of it all
[00:24:18] to find the great solution.
[00:24:20] >> Yeah, it makes an awful lot of sense.
[00:24:23] because of your age, my age, which
[00:24:25] aren't so far off, does the nuclear
[00:24:28] issue still have a lot more personal
[00:24:31] grip and resonance with you than what
[00:24:34] you're writing about on the biological
[00:24:35] side, even though the biological side is
[00:24:37] clearly both more likely and some ways
[00:24:40] more terrifying.
[00:24:41] >> Yes and no. Because bio bio- threats
[00:24:43] have been with me in my brain for a long
[00:24:45] time because of called operation
[00:24:47] paperclip about the Nazi scientists that
[00:24:50] were brought to the United States after
[00:24:53] World War II. Many of whom were
[00:24:55] biological warfare experts. That is how
[00:24:59] our program began because once upon a
[00:25:02] time during the Cold War, the United
[00:25:04] States had a massive arsenal of
[00:25:07] biological weapons as did the other
[00:25:10] superpowers. So, I have been thinking
[00:25:13] about this horror for decades.
[00:25:17] >> When I first read your nuclear book, the
[00:25:19] first thing I thought about was the
[00:25:20] bulletin of atomic scientists. Um, and
[00:25:23] the fact that uh they have their their
[00:25:26] doomsday clock that they come out with
[00:25:28] every year and how close we are to
[00:25:30] midnight, which is again some an
[00:25:32] assessment of a lot of pretty smart um
[00:25:34] and many older uh scientists about how
[00:25:37] close we are to extinguishing ourselves
[00:25:40] as a species. And and I wonder if you
[00:25:43] think having spent so much of your life
[00:25:44] working on these things, do you think
[00:25:46] that there is something inherent in the
[00:25:49] human condition that we are um living um
[00:25:54] in in such a precarious a self-imposed
[00:25:58] albeit collectively a self-imposed
[00:26:01] precarious position as humanity. This is
[00:26:05] the nature of being a human and having
[00:26:08] this as a brain and having science and
[00:26:12] technology which comes as a result of
[00:26:14] this brain advancing faster than
[00:26:18] essentially the brain itself. So we are
[00:26:20] in a new paradigm of that complex
[00:26:24] equation because the systems are now
[00:26:28] mimicking our own brains better than our
[00:26:31] own brains. I do see a dividing line in
[00:26:36] threat in global catastrophic threat
[00:26:39] where we are now with essentially you
[00:26:41] know I pretty much look at the people
[00:26:43] talk about consciousness and the AI can
[00:26:45] can perform better than the brain. So we
[00:26:47] have kind of crossed that line that John
[00:26:50] vonman warned about back in the 50s.
[00:26:54] >> Yeah. I I mean the idea that um human
[00:26:56] beings are becoming different because
[00:26:58] we're programming them to be that that
[00:27:01] strikes me as uh you know perhaps the
[00:27:04] most dangerous uh experimentation or
[00:27:07] tinkering of all of what you're talking
[00:27:09] about.
[00:27:10] >> And I think that's why like legacy is
[00:27:12] just as important to think about as
[00:27:15] future. Where have we come and where are
[00:27:18] we going? And that's why I love your
[00:27:20] idea of the white hat team. You know, it
[00:27:22] needs to have not only subject matter
[00:27:25] experts from these different fields, but
[00:27:27] age and experience has to be a serious
[00:27:30] quality of those subject matter experts
[00:27:33] because it's so important to be able to
[00:27:35] look at the human condition with the
[00:27:38] advancing technology.
[00:27:40] >> Okay, we'll put that in the paperback
[00:27:41] version, please. Annie Jacobson, thanks
[00:27:43] so much for joining us today.
[00:27:44] >> Thank you for having me.
[00:27:49] That's it for today's edition of the
[00:27:51] GZERO World podcast. Why not make it
[00:27:53] official? Why don't you rate and review
[00:27:54] GZERO World five stars? Only [music]
[00:27:56] five stars. Otherwise, don't do it on
[00:27:58] Apple, Spotify, or wherever you get your
[00:28:00] podcast. Tell [music] your friends.
[00:28:07] [music]
[00:28:11] Cox Enterprises is proud to support
[00:28:13] GZERO. Cox is a family-run company that
[00:28:16] has thrived across three centuries.
[00:28:18] We're building a brighter future in
[00:28:20] automotive, greenhouse agriculture,
[00:28:23] clean tech, environmental conservation,
[00:28:25] and beyond. Cox Enterprises in the
[00:28:28] business of what's next since 1898.
[00:28:32] Learn more at coxenterprises.com.
