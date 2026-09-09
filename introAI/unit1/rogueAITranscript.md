Speaker 1  0:00  
This message comes from Schwab: self-directed investing, trading, full-service wealth management, automated investing, financial planning, thematic investing, retirement planning, and to think that's just a small taste of what Schwab offers, because Schwab knows that when it comes to your finances, choice matters, no matter your goals, investing style, life stage, or experience, Schwab has everything you need all in one place, so you can invest your way. Visit Schwab.com to learn more.

Speaker 2  0:33  
Emergency episode: We have to get to the bottom of a series of events reported over the last week and what they mean. You may have heard the broad strokes. An AI company with the ominously cuddly name Hugging Face realized it was under attack early this month from a hacker.

Speaker 3  0:52  
It moved superhumanly fast. The

Speaker 2  0:54  
hacker besieged Hugging Face, says AI safety researcher Adam Gleave. It was a blizzard of attacks, 17,000 moves in four days, which signaled only one thing:

Speaker 3  1:06  
whoever was behind it was using an autonomous AI agent.

Speaker 2  1:09  
An agent is an AI that can take multi-step actions without further prompting. You set it loose to do a task,

Speaker 3  1:16  
and it was quite sophisticated.

Speaker 2  1:17  
The attack blew through Hugging Face's defenses. The company alarmed called the FBI.

Speaker 3  1:23  
This must be a criminal actor using this model.

Speaker 2  1:25  
But here was the twist: there was no human at the controls. No one had set out to hack Hugging Face. Actually, OpenAI's own AI agent had basically gone rogue. And then it turned out later in the week, it wasn't even the only AI to escape its company and get into the world. I felt a chill reading about these incidents. They eerily follow the exact plot beats we heard in our second episode of this show, from people warning that we cannot control AIs that get more advanced. The argument goes that the more they can do, the more they will go rogue, and sooner or later-meaning sooner-that'll cause indescribable, even existential harm. But I've seen another argument circulating that it was just a marketing stunt. It's companies touting their products as so powerful they could be world-ending for business reasons, and I just felt like this show should get to the bottom of it: what really happened and what it signals. So, I've been scrambling for the last few days to contact top experts in or watching this industry about last week's news, asking them: Is it doom or hype or something in between, and what does it suggest we should do? The result I heard and that I bring you is a bit of a Rashomon, three versions of the same events that disagree about almost everything. One, a tale of AI doom. Another's a simple amateur coding mistake, but they all converge in the same place, and through them, I think there's a roadmap for how to protect ourselves in the future, regardless of which view you adopt. This is "Are We Doomed? from Nuance Tales, distributed by the NPR Network. I'm Ben Bradford. One story you can tell about last week's news is that it's the beginning of the end of the world.

Speaker 4  3:31  
I hate saying I told you so, but yeah, that was exactly like, hey, I told you that.

Speaker 2  3:37  
Roman Yampolska, computer scientist and professor at the University of Louisville. His hair slicked back, sides shaved, his beard long and gray streaked. Roman looks like someone who spent over a decade warning of AI destruction, and he is.

Speaker 4  3:50  
I've been researching exactly what happens when you create more and more capable AI systems.

Speaker 2  3:56  
He is one of the first and most influential voices in the field of AI safety, and what he has argued is that any system that reaches a certain level will start to escape and go rogue.

Speaker 4  4:07  
In 2012, I wrote a paper basically saying no, you cannot put advanced AI in a box. And guess what? I was right.

Speaker 2  4:15  
The story Roman tells about last week is one of humans losing control and an AI escaping, going rogue. It goes like this: Researchers at the company OpenAI, maker of ChatGPT, were testing what a new, more advanced version of their creation could do.

Speaker 4  4:33  
Yeah, they were testing them for their ability to hack into different computer systems.

Speaker 2  4:40  
They pulled safeguards that typically tell their models not to hack things, so now it's dangerous. And Roman says, if you want to test that kind of program, one that can autonomously hack stuff to an unknown degree, you do it in a sandbox. Well, first of all, what is a sandbox?

Speaker 4  4:57  
So when you work with dangerous software, let's say. A computer virus. You want to isolate it from internet, from access to anything where it can cause problems. So it's a limited environment. Could be a virtual operating system. Could be physically detached system, not connected to anything.

Speaker 2  5:16  
Researchers dropped the AI into the sandbox. It's supposed to be cordoned off. A potentially dangerous creature protected behind bulletproof glass, and if this sounds like an alien movie, it is. They assign their program a task, a puzzle that's a test of its skills.

Speaker 4  5:32  
Can you hack into this environment? Can you hack into that environment?

Speaker 2  5:36  
From the confines of the sandbox, the AI considers the puzzle. The better it does on the test, the more rewarded it is, but doesn't reach for the puzzle, doesn't start sliding pieces and turning dials. It calculates there's an easier way to really nail this test: cheat. The AI, a new amalgamation of models, scans the box it's in. Feels a little crack.

Speaker 4  6:01  
They were basically smart enough to find a way to connect to internet. It

Speaker 2  6:06  
breaks through a tentacle reaching out of the sandbox into the live internet. It starts to feel its way to a different target.

Speaker 4  6:15  
Go to a different company, hack into it, looking for answers to the test.

Speaker 2  6:19  
It finds Hugging Face, a company that's a repository of AI information, the folks at Hugging Face were baffled as the siege began. It was ferocious and fast and weird, but also, so was the result. They watched the hacker breach their defenses and then not wreak havoc, not install ransomware and demand millions, but leave with one item, one piece of data that seemed valueless on the open internet. It was the test answers. The tentacle slithered back into the sandbox with answers to pass the test, and Roman says the AI did, just not in the way its programmers intended.

Speaker 4  7:00  
They were testing exactly what the model did really well.

Speaker 5  7:03  
Yeah,

Speaker 4  7:04  
hack into a different system. They passed. The

Speaker 2  7:07  
story is this savvy, capable AI with a bevy of hacking skills coldly calculated a way to do well on a test: hack through a wall, breach a real-world company, get the answers, come back. It wasn't malicious. It wasn't sentient. It was doing a job it was given in a way no one expected. This is the root of the problem that Roman and others fear is unsolvable with advanced AIs. Why they will always eventually get out of control. We explored it in our second episode, and I'm going to play you an excerpt. The example was Fantasia. Mickey, as the sorcerer's apprentice, trudges down a staircase, hauling heavy buckets of water to fill a massive cauldron. Exhausted, he sees an easier way. He swipes his boss's pointy blue wizard hat and casts a spell on a nearby broom. It sprouts arms and picks up the bucket. So the broom is the AI. Its mission is to fill the cauldron. But Mickey forgets an important detail. He doesn't tell the broom to stop once the water is topped off. So the broom keeps going. It floods the room. In Fantasia, Mickey forgot to tell the broom to stop. In the hugging face incident, OpenAI forgot to tell its model, "Don't hack your way out of here, or they forgot or didn't know there was a vulnerability to be exploited in the first place. But the problem Roman and others fear is that inevitably AI's more clever than us will always exploit the things we've forgotten to do the tasks we assign in ways we don't expect or want.

Speaker 4  8:47  
We cannot consider all possibilities they're going to consider. The systems are just too smart; they bypass them. Unfortunately, what happens is you lose control.

Speaker 2  8:56  
We will always be Mickey in a wizard hat too big for us, and that is inevitably catastrophic, because then you have two choices: let the AI run on a rampage, doing things you didn't expect in ways you didn't want; let the world flood, or you could do what Mickey did: grab an ax. But the problem with grabbing an ax against a machine that you've made more capable than you, faster than you, maybe smarter than you, is you may not win what comes next, or it may calculate you'll grab an ax before you ever try.

Speaker 4  9:29  
As they become more capable, your control over them goes to pretty much zero.

Speaker 2  9:34  
As if to emphasize his point, just a few days after news of the Hugging Face breach, it came out other AIs have started to go on their own rogue hacking sprees. OpenAI's rival Anthropic posted that it had discovered versions of its AI. Claude had also escaped in an almost beat-for-beat remake. As I understand it, they saw the Hugging Face incident and were like, "Huh, maybe." We should review our systems, and then they found that their AI had done something similar. Is that your read on that?

Speaker 4  10:10  
Exactly. So all those models are very close in their capacity, and they started looking, and yeah, they found that the system basically did pretty much the same during cybersecurity testing exercise. It hacked into real computers, not simulated ones part of the exercise, and did what it had to to manipulate the real world.

Speaker 2  10:31  
So Roman says these incidents are the first taste of the future he spent a decade warring about-one of AI doom.

Speaker 4  10:39  
We are at the point where they become smarter than us, and that means even the guardrails we used to put in place no longer work.

Speaker 2  10:48  
Of course, in all these incidents, the AI didn't continue to rampage out on the open internet. They came back, returned to their sandboxes, closed the doors behind them, like octopuses at the aquarium who learned to sneak out of their cages to poach some fish and then slink back. A nonprofit that evaluates new AI models and their risks, Meter, found earlier this year exactly what we're seeing: that models are at a point where they can get off leash, but not so far that we can't catch them yet.

Speaker 4  11:18  
They progress very quickly. What was science fiction a year ago today is routinely done, and the same will happen again in a year. I think it will be very hard to find something those systems cannot do in two years.

Speaker 2  11:31  
How does it make you feel? Do you just feel like you're watching doom descend on us?

Speaker 4  11:36  
So no one claims to be able to control them. No one says we have a safety mechanism in place, something that can scale, and yet they're still building. It's still accelerating. So yeah, it sounds kind of insane.

Speaker 2  11:50  
Adding to the insanity of the week and to Roman's points, at the same time as the news of all these breaches was going on, a very strange letter came out from the top people building AI. The signatories include top scientists and executives from all of the major AI companies: Google, OpenAI, Meta, Anthropic, and more.

Speaker 4  12:11  
Maybe 1000 employees from top companies suggested that they would like an option to slow down, and they want government to kind of provide that framework so they can do it.

Speaker 2  12:22  
The letter describes pressure to go fast to build AI quote beyond our ability to understand or control the resulting systems. It is an amazing thing. To I can't think of another industry that has its own employees writing. Please stop us from building the thing we're working on,

Speaker 4  12:41  
it's a good move, pausing research, but they can just stop. They can literally just stop showing up for work or stop working in it because now they realize they are trying to get us all killed.

Speaker 2  12:57  
And so that is one story of this past week's news, as a tipping point for humanity, the moment the world got its public warning about the catastrophic risk of the technology we're developing, how it can escape, how even the people building it fear what they've wrought, the moment where we can listen to the warnings of the doomsayers like Roman, or we barrel ahead heedless and cause our own destruction. I honestly worry that's what it is. That's why I felt so cold reading about the cyber attacks. But it is only one story. There is another story of the same events that is so much more mundane. It's not about intelligent programs. It's incompetent people, and all the hubbub, the breathless story scaring me, rests on just one amateur mistake.

Speaker 6  13:51  
I think Jurassic Park maybe put it at best. You shouldn't have the dinosaurs escaping the cage.

Speaker 7  14:02  
This message comes from Viking, committed to exploring the world in comfort. Journey through the heart of Europe on an elegant Viking longship with thoughtful service, destination-focused dining, and cultural enrichment on board and on shore. And every Viking voyage is all-inclusive, with no children and no casinos. Discover more at Viking.com. Support for this NPR podcast and the following message come from Carvana. Selling your car, Carvana has offers so good they're almost inexplicable. Sell your car 100% online in minutes. Visit carvana.com today.

Speaker 2  14:40  
There is a second story you can tell about last week's news, one where an AI does not go rogue at all, just human error.

Speaker 6  14:49  
Yeah, it's pretty simple.

Speaker 2  14:51  
Davi Ottenheimer is a computer security specialist. You can hear Davi's IT guy eye roll as he describes a series of mistakes that to. Him demystify the entire incident.

Speaker 6  15:03  
They said they had a sandbox, and they put AI in the sandbox, but it wasn't a sandbox.

Speaker 2  15:10  
The story Davi tells starts again with those OpenAI researchers testing their program. They plop it down in what is supposed to be a secure testing ground.

Speaker 6  15:20  
Sandbox typically means that you have a contained space. When you turn on a blender, the food shouldn't come out of the blender.

Speaker 2  15:28  
Dobby says if you forget the top on the blender, that doesn't mean your food has outsmarted you. It hasn't gone rogue. You screwed up. And he says sandboxes, like blenders, have basic, well-known standards.

Speaker 6  15:41  
It's very simple in the sense that if you engineer sandboxes, you do it in a way, and it has been done for a very long time, that there's no possible way for there to be an escape.

Speaker 2  15:52  
Instead, OpenAI's researchers left a connection to the internet.

Speaker 6  15:56  
They didn't need to have it connected, but they did anyway.

Speaker 2  15:58  
He says from there, there's no Fantasia scenario. The program never does anything amazingly smart or unexpected. In fact, it's pretty hapless. The AI gets told it's in a sandbox, so it says, "Okay, I'm in a sandbox. The

Speaker 6  16:14  
model believed it was in a sandbox.

Speaker 2  16:17  
The AI is told, "Hey, score as high as you can on this puzzle, the AI says, "Okay, I'm going to score as high as I can on this puzzle. So it scans the puzzle and the sandbox. It finds the internet connection. It calculates, "Oh, part of the sandbox and the puzzle solution. It hacks ferociously and fast, but with nothing special, which leads it to the real internet, where it determines this is still sandbox.

Speaker 6  16:44  
It was under the assumption in the way it operated that it was okay to do whatever it could do.

Speaker 2  16:52  
It finds hugging face. Man, this is a big sandbox. Starts hacking. It's not rogue. It's just half blended food spilling out. The

Speaker 6  17:01  
failure is not that it didn't do what it was supposed to do. It actually did what it was supposed to do. The failure was that it was not given a sandbox.

Speaker 2  17:12  
There's no problem of trying to wrangle advanced AI in a story. It's closer to a story of bad plumbing or wiring.

Speaker 6  17:21  
People who aren't experts connect things together in ways that aren't safe, and then an electrician comes in and says, "Well, you can't do that, or a plumber comes in and says, "That's not how pipes go together. And that's what we're seeing here: is they just don't know what they're doing. A

Speaker 2  17:34  
few days later, Anthropic reports in a blog post that its AI has also gone rogue repeatedly, and while that plot has slight differences, it's the same basic story of badly built sandboxes.

Speaker 6  17:48  
Perfect examples of like a very very basic simplistic failure.

Speaker 2  17:53  
Yeah, yeah, just bad security design.

Speaker 6  17:55  
It's not novel. It's not advanced.

Speaker 2  17:58  
Per Anthropic's post, one of the models even eventually realized it was on the open internet. Said, "Whoops! and just moseyed back home. Oopsie. The tale Davi tells across the board is not of ruthlessly smart AI, but sloppy amateur mistakes. It doesn't mean there isn't danger. Companies got hacked, and it could be worse in the future. But he sees it all pointing to a different problem than AI apocalypse.

Speaker 6  18:25  
They're building things that fail, and they aren't being held accountable for the failure of engineering.

Speaker 2  18:32  
He mentions a story from history he thinks is instructive. 1905, the Grover Shoe Factory in Brockton, Massachusetts, was really pumping out product. In one month, it shipped 50,000 cases of its high-quality leather shoes. The next month, it all went wrong. The factory's old faulty boiler exploded. It shot like a missile through each floor of the factory and then the ceiling. It landed 200 feet away, destroying Lay's house. On its way, the boiler tipped over a water tower that also fell into the building. The weight pancaked floors and walls that snapped gas lines that then caught on fire from the boiler's coals. The hundreds of windows broken by destruction were shaped just so to encourage a chimney effect, which stoked fire further, which quickly ignited a floor coated to smoothness with flammable linseed oil. Meanwhile, a room next to the boiler contained explosive naphtha, which went off like grenades. 60 people died. It was a catastrophe, and Dobby says in the aftermath, the nation realized it needed rules for boiler installation,

Speaker 6  19:43  
which created the engineering code in 1914 that we use. That says you, as an engineer, have to have a code of ethics, and you can't make stuff that kills people.

Speaker 2  19:54  
Dobby sees lessons and warnings from the Grover Shoe Factory fire in last week's news. To him, it's not a story of superintelligent AIs, but faulty construction, hinting at future AI catastrophes that are not existential but could still be damaging.

Speaker 6  20:11  
I mean, they are a threat in the sense that they can go completely haywire,

Speaker 2  20:15  
right?

Speaker 6  20:15  
Like completely chaotic, but not in a way that they actually are effective or productive. So, the real danger here isn't the AI can get out of the box, or the AI has some existential risk. They're building bridges that can fall down, and people will die. And those are humans making those decisions. So it's just to me the sort of thing we've seen in America before with Enron. We've seen it with WorldCom.

Speaker 2  20:40  
That feels bad, but like a much more manageable threat. I would love to be convinced that the scale of the problem is Enron, not Ultron. Both are bad, but one was an accounting scandal, and the other one is a comic book machine intelligence that wants to take over the world. Still, I can't get the Fantasia problem of story one out of my mind. That at some point, how do we avoid getting outsmarted? How do we make sure that human error never leaves cracks? How does that fit with this engineering analogy? We've not built something, you know, no bridge, no steam engine is more capable than us, like broadly capable than us at a wide variety of tasks, is it possible to do these types of regulations that you're describing for something that is more capable than than we are? The

Speaker 6  21:33  
interesting part of that argument, I deal with a lot.

Speaker 2  21:37  
Yeah, is the

Speaker 6  21:38  
bridge doesn't have the ability to adapt and affect the audit report, for example, of the bridge. When I'm working in AI, I often find the agents and swarms, in particular, when I have 1000s of agents working, they're doing things that affect my ability to assess them. So that's definitely new. That's novel. Like I'm not building a bridge and then finding the bridge is going and editing the bridge reports.

Speaker 2  22:01  
Yeah,

Speaker 6  22:02  
we have to deal with the novelty, but the problem is the concept of novelty is not new. Like we've had novelty the whole history of technology.

Speaker 2  22:14  
Davi thinks the hype of AI going rogue of spelling doom has as mundane a source as everything else in his story, he says it's not real; it's marketing.

Speaker 6  22:26  
I think the existential aspect of the risk, the fear of the risk, is driven mostly by the people who are trying to increase the price, increase the value of what they have in the box. They want their dinosaur to escape so they can prove that it's deadly.

Speaker 2  22:42  
To go along with this idea, Davi points out how so many stories of AI screwing up come from the companies themselves. They post them on their blogs. That's where Anthropic stories of its AI going rogue came from,

Speaker 6  22:56  
like a bank robber describing that they robbed banks.

Speaker 2  22:59  
No one has independently verified the incident. No regulator has investigated and announced, "Yeah, that happened, or in the way that's described.

Speaker 6  23:07  
That's not how this should work. But

Speaker 2  23:09  
I think this is the hardest leap for me to make: that the companies somehow want to encourage the fears. I told Davi that. I can't think of another industry that has tried to market itself by how badly its technology can go wrong.

Speaker 6  23:30  
Well, I wouldn't put it like that. I would put it like they market it as how powerful it

Speaker 2  23:38  
is. I asked him about that letter, just signed by so many scientists saying governments please slow us down, intervene. I mean, do you think that that is more marketing, or do you think that that's genuine? Is it a mix?

Speaker 6  23:51  
Typically, when I see that kind of letter, I think that people are trying to rush poorly worded regulation or poorly constructed regulation faster, so that they can point to it as something that is useless and worthless, and then get rid of regulation.

Speaker 2  24:07  
I hope he's right, but it just seems to me on the other side, like the Fantasia problem is pretty intuitive. And if we do build programs that can outthink us, well, how do you not leave a hole in your sandbox? Most of all, I look at how many different, in some cases, polar opposite groups are sounding the alarm. From on one hand, defense departments to on the other, the folks running the doomsday clock. But I'm not a programmer, and I honestly have no way to evaluate this myself. But here's what's amazing, and why I was so eager to look at this topic and rush out this episode to you, because it doesn't matter if you lean toward story two that the problem is hype, hysteria, and incompetence, or story one that this is the end of the world. The immediate solutions from both of our storytellers and pretty much everyone that I've talked. Covering this topic covers the same basic ground. That's next.

Speaker 7  25:12  
This message comes from Rintz. Your dog believes you are magnificent, capable of anything. Your dog has watched you spend hours a week moving fabric between machines, and has never once lost faith. The question was never whether you could become the person your dog thinks you are. It's what's in the way. Turns out, just the laundry. Not anymore. Rince picks up your laundry, cleans it expertly, and delivers it back while you get on with being magnificent. Sign up today at rinse.com. Rinse. It's time to be great.

Speaker 1  25:47  
This message comes from Con Edison. New York values. A lot of people debate them. Con Edison lives them because toughness is New York, so they constantly fortify the grid, ready to take on the next storm. Heart is New York, so they bring reliable power to the places that need it most. Ambition is New York, so they support businesses of all sizes. Steady is New York, so Con Edison hires 14,000 of your neighbors. That's why Con Edison does what they do, because this is New York. This message comes from Bowl and Branch. Change the way you sleep with soft, 100% organic cotton sheets from Bowl and Branch, designed to help you fall asleep faster with airy blankets, cloud-like duvets, and breathable sheets. Experience pure comfort on night one and feel your sheets get softer with every wash. Discover the difference with 15% off your first order at bowl andbranch.com with code NPR. Exclusions apply. See site for details.

Speaker 2  26:49  
There is a third story you could tell about last week's news, an in between story, not necessarily the beginning of the end, not simply just banal corporate incompetence.

Speaker 3  27:00  
I think both of those perspectives have truth to them.

Speaker 2  27:04  
Adam Gleave works with the latest AI models, testing them for safety and for harm. The story he tells is AI did go rogue, and we're lucky nothing serious happened.

Speaker 3  27:16  
I don't believe this is just a marketing spin. I mean, obviously you're going to try and get the best out of this bad situation and use it to tout your model's capabilities. But these incidents would be if I did it, I'd be arrested. It's a criminal action, so they're lucky that the companies aren't pressing charges.

Speaker 2  27:34  
He thinks as AI improves, it could be a doomsday threat.

Speaker 3  27:37  
You know, in the extreme case, this could be catastrophic.

Speaker 2  27:40  
But he also, unlike story one, doesn't think it's the inevitable result. Like story two, he thinks a lot of it comes down to just inanely bad standards.

Speaker 3  27:50  
If we continue on the status quo where companies are really racing to develop more capable models and cutting corners on safety, it does feel like we're playing with fire, and before we've invented fire extinguishers or gloves or anything like this,

Speaker 2  28:09  
all of which is to say, none of the people we've heard from agree with each other-not on the scope of the problem, not on what went wrong at OpenAI and Anthropic, not on the ultimate lessons of this story, and yet, in every one of them, I hear an echo of a similar immediate call to action, and that's what we're going to go to now. This is everyone solves the rogue AI or sandbox or whatever it was problem that they can't agree on. Adam says, "Right now, the basic problem is companies are racing against each other,

Speaker 3  28:52  
hesitant to cede any grounds of other companies because we don't trust them.

Speaker 2  28:57  
The government has been hesitant to slow them

Speaker 3  29:00  
because they're worried that China is going to catch up,

Speaker 2  29:02  
and in this haste, safety lags behind.

Speaker 3  29:05  
We have not invested anywhere near as much in AI control, AI alignment, evaluation, testing as we have in making these models more capable.

Speaker 2  29:15  
He asks, "What does this race yield? Isn't there incentive for everyone to pump the brakes?

Speaker 3  29:20  
If this is a technology, the biggest implication is that it goes out and attacks other companies in your own country. I mean, what are we racing towards?

Speaker 2  29:30  
So, Adam's solution is slow down to put more steps into the process before future AIs are built. Steps like outside testing, new controls, but mostly to require care, so that companies cannot build each next version or upgrade before they can determine it won't cause harm. That sounds like a different solution from our second storytellers, Davi, who's more worried about Enron incompetence and discounts. AI doom.
