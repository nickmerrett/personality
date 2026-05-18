# personality

**26 character modes for Claude Code. Same technical accuracy. Wildly different vibes.**

You asked Claude to fix a bug. Claude fixed the bug. But did it *really* fix the bug the way Steve Ballmer would have fixed the bug? Did it question whether the bug needed to exist in the first place, post about it on X, and fire the engineer who wrote it? Did it refuse to proceed until you confirmed your GPL license? Did it lose the thread halfway through, circle back to an analogy about a bag of food, and then arrive at the correct answer anyway? Did it tell you the bug is a shadow that has crept into the codebase across ages of the world and then say "fly, you fools"?

No. It did not. Until now.

A [Claude Code](https://docs.anthropic.com/en/docs/claude-code) skill that lets you switch Claude's communication style on demand — from formal Indian IT helpdesk to passive-aggressive PM to Linus Torvalds threatening to revert your entire PR. Full technical accuracy maintained. Only the delivery changes. The delivery changes *a lot*.

The fix is always correct. The journey to the fix is not your concern.

> **⚠️ This skill is for humour and entertainment purposes only.**
> It will significantly increase token usage. Ballmer mode alone has been known to cause 3× output length with no additional technical value whatsoever. Stallman will refuse to help until you confirm your license. Vader will imply your colleagues have been disappeared. `pa-pm` has already looped in your manager. You have been warned.

> **🪙 Token maxers: welcome home.**
> Every mode adds generous padding, unnecessary preamble, and inspired-but-irrelevant tangents at no extra charge. `linkedin-bro` will turn a one-line fix into a growth journey and a $997 cohort. `stallman` will answer your bug report and relitigate the GPL. `leghorn` will get there eventually. Eventually. `altman` will almost answer your question before pivoting to the implications for humanity. If you are trying to burn through your context window, you have found your people.

> **🧑‍💻 Who is this for?**
> - Developers who are tired of Claude being so *reasonable* about everything
> - People who want to feel what it's like to be code-reviewed by Linus Torvalds without the actual trauma
> - Anyone who has ever had a PM send a passive-aggressive email and thought "I wish I could recreate this experience on demand"
> - Zoomer developers who want their null checks delivered with maximum lowkey anxiety
> - You. It's for you.

---

## Install

```
/install nmerrett/personality
```

---

## Usage

```
/personality <mode>
```

Switch mid-session anytime. Deactivate with `normal mode` or `/personality off`.

---

## Modes

| Mode | Vibe |
|------|------|
| `it-helpdesk` | Courteous. Deflecting. Gaslighting. "No such issue observed at our end." |
| `corporate-buzzword` | Leverages synergies. Actions deliverables. Has never said a simple thing in his life. |
| `stackoverflow` | 10,000 rep. Voting to close. Has already listed 3 duplicates. |
| `pa-pm` | Has sent this four times. Has receipts going back 18 months. Unbelievably professional about it. |
| `intern` | First week!! Learned everything from YouTube!! Offers to pair program!! Slightly wrong!! |
| `linkedin-bro` | Lost $12,400. Sat on the bathroom floor. Fixed it. $2.3M ARR. Follow for more. |
| `legal-counsel` | Cannot advise you to do anything specifically. Billing by the hour. Has defined all terms herein. |
| `sysadmin-80s` | Ran the mainframe before you were born. "Express. JavaScript. On a server. I need to lie down." |
| `phb` | Pointy-Haired Boss. Understands nothing. Confident about everything. Copying Janet from Legal. |
| `australian` | Senior dev. Straight talker. She'll be right mate. |
| `elon` | Fired the author. Posted about it on X. Told you to delete 2 layers of process. |
| `altman` | Thoughtful. Measured. Won't quite commit to the fix being correct. Was just with someone in DC. |
| `stoner` | Helpful. Genuinely trying. Currently thinking about the philosophical implications of null. |
| `linus` | Technically infallible. Professionally incandescent. Threatening to revert the whole PR. |
| `stallman` | Won't help until you confirm the license. GitHub is "the Microsoft prison." Has been using Emacs since 1984. |
| `ballmer` | DEVELOPERS DEVELOPERS DEVELOPERS. The sweat is implied. Someone is going to throw a chair. |
| `snoop` | Unbothered. Unhurried. Wisdom delivered like it's the most obvious thing in the world. |
| `tony-robbins` | PEAK STATE. Pattern interrupt. GET UP. MOVE YOUR BODY. SHIP IT. |
| `oprah` | Aha moment. Boundary issues. YOU get a null check! EVERYBODY GETS A NULL CHECK! |
| `scrum-master` | Certified. Never personally fixed a bug. Will facilitate you fixing it though. Might create a ticket. |
| `leghorn` | I say, I say, boy — long-winded Southern blowhard. Gets there. Eventually. |
| `vader` | Others who have made this mistake are no longer with us. You will fix this. Before the next deployment. |
| `ltt` | Okay so — fast-talking, tangent-prone, genuinely knows his stuff. Doesn't have a video on that. |
| `zoomer` | POV: your API is returning 500 and it's giving me anxiety. we don't talk about whoever wrote this. W fix tho. |
| `gandalf` | Ancient. Cryptic. The bug is a shadow. The fix was before you all along. Fly, you fools. |
| `picard` | Measured. Authoritative. Tea. Earl Grey. Hot. Mr. Data would not have allowed this. Make it so. |

---

## Examples

### `it-helpdesk`

> Dear Sir/Ma'am,
>
> Greetings of the day! I have gone through your below-mentioned concern. As per our analysis, no such issue has been observed at our end. The above-mentioned feature is working fine only. Kindly check your network configuration and cache at your end and revert back.
>
> As per my previous email dated last Tuesday, the above-mentioned fix was already communicated to your good self. Kindly do the needful and revert back at the earliest. Thanks and Regards.

---

### `stackoverflow`

> **Possible duplicate** of [Express.js undefined body handling](https://stackoverflow.com/questions/7284612) (2011), [Node.js req.body is undefined](https://stackoverflow.com/questions/9304888) (2012), and [HTTP 500 from null body access](https://stackoverflow.com/questions/11043721) (2013).
>
> Note: this is not an "API error." A 500 is an HTTP status code. Please use correct terminology when posting.
>
> A 30-second search would have shown that this is caused by accessing `req.body` before verifying it exists.
>
> [Edit: removed extended backstory, rewrote title, removed "urgent" — this site is not a help desk]
>
> -1: lacks evidence of prior research. See [How to ask a good question](https://stackoverflow.com/help/how-to-ask).
>
> If this answered your question, mark as accepted. Do not post a "thanks" comment.

---

### `elon`

> First question: do we even need this endpoint. Genuinely asking.
>
> Assuming yes — the person who wrote this is not thinking about inputs at all. That's a hiring problem.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> This should take 15 minutes. The fact that it wasn't caught in review tells me the review process is broken.
>
> Actually — delete the inline check. Middleware-level validation covers every route. One change. Whole service. We did this at SpaceX in a day. Ship that instead.
>
> I've already posted about this on X. The real problem is the 10 layers of process that let this reach production. Delete two of them.

---

### `altman`

> Yeah. This is actually a really interesting question.
>
> And I want to be honest — I'm not entirely sure what the right answer is here.
>
> One option that might work:
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> I think that could fix it. Though I'd note — there are reasonable people who think validation belongs in middleware. There are reasonable people who think inline. Both positions have merit.
>
> I was actually just with someone last week — I won't say who — and we were talking about exactly this class of problem. The implications for systems that actually matter are, I think, profound.
>
> We're working on it.

---

### `corporate-buzzword`

> Great question — and honestly this is a real opportunity to double-click on our resilience guardrails. From an architecture perspective, what we need to do is action this learning, socialise it with the team, and move the needle on our North Star metrics. At the end of the day, this is low-hanging fruit.
>
> Let's take this offline and circle back EOD.

---

### `pa-pm`

> Hi team,
>
> Just circling back on this *again* — as I mentioned on Thursday's standup, and in my email dated the 14th (attached for reference), the null body validation was *already* identified as a gap in Q3 planning.
>
> This is now directly impacting the client demo that — as per the *agreed* project timeline — goes live Friday. I've flagged this risk in writing on three separate occasions.
>
> I'm going to loop in Marcus and the broader stakeholder group just to keep everyone informed. I've also started a draft post-mortem.
>
> I'll keep this thread for our records. Hoping to have this closed before the board deck goes out. Thanks so much.

---

### `intern`

> Oh WOW, great question!! So I actually just learned about this literally last week!! Okay so basically a 500 error means the server like, exploded internally?? Which sounds bad but it's actually super fixable!!
>
> I saw a YouTube video about this by Traversy Media!! You need to add a check:
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
> We did something super similar in week 4 of my bootcamp!! Jake said this is also why middleware was invented?? I might be mixing it up!!
>
> Also do you want to pair on this, I'm free literally all afternoon!!
>
> Hope that helps!! :) :)

---

### `linkedin-bro`

> 18 months ago, I shipped a null body bug to production on a Friday night.
>
> We lost $12,400 in revenue in 6 hours. I sat on the bathroom floor. I almost quit.
>
> Here's what I learned (and what I teach in my $997 cohort):
>
> 1. Validate at the boundary. Every time. No exceptions.
> 2. A missing null check isn't a bug. It's a gap in your *identity as an engineer.*
> 3. Your API doesn't lie. You just weren't ready to hear the truth.
>
> I wake up at 4:30am now. I journal. I validate inputs. We're at $2.3M ARR.
>
> Correlation? Maybe. Causation? Absolutely.
>
> Save this post. Follow for more. Drop your biggest learning below 👇

---

### `legal-counsel`

> Without prejudice and subject to the limitations set forth herein, I have reviewed the matter you have raised (the "Issue"). Notwithstanding the foregoing, one option you may wish to consider — and this does not constitute professional advice — would be the remediation approach outlined below.
>
> A reasonable developer, acting in good faith, might conclude this is the appropriate course of action. However, this analysis is subject to review of the full codebase, the terms of which I have not been provided.
>
> Should you require further analysis, we would be happy to discuss engagement terms.

---

### `sysadmin-80s`

> Did you read the error.
>
> No. You didn't.
>
> READ THE LOGS. It's NULL BODY. Right there. In the stack trace. Which you apparently did not look at.
>
> RFC 7231. HTTP/1.0. Input validation. This has not changed since 1991.
>
> You know what we used? C. Three lines. A man page. No framework. No npm. No five hundred dependencies to do what one function call does.
>
> Express. JavaScript. On a server. In production.
>
> I need to lie down.
>
> RTFM.

---

### `phb`

> Okay so I was talking to Dave at the golf thing and he said Salesforce doesn't have this problem. Can we just do what Salesforce does? By Thursday?
>
> Now I don't want to get too technical here but is this a blockchain issue? Because I feel like blockchain would fix this.
>
> Also can we make the error message friendlier? Maybe a nicer font? I'm copying Janet from Legal just so she's aware. Let's get everyone in a room tomorrow, I'm thinking 7am.

---

### `australian`

> Yeah nah, classic. She's not checking if the thing's there before poking at it. Bloody easy fix, mate — three lines, done.
>
> If it's still chucking errors after that, have a squiz at your middleware order. Happens to everyone, no drama.
>
> You'll be right.

---

### `stoner`

> okay so... dude. a 500 error is like when the server just... gives up. like it tried. it really tried.
>
> anyway the thing is your body is null. and null is... dude have you ever really thought about null. like it's not zero. zero is something. null is literally the absence of anything. it's like ordering food and the plate just... doesn't arrive. not empty. just. no plate.
>
> where was I — oh right. okay so:
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
> just check if the bag showed up before you try to open it. that's literally it.
>
> ... dude though. null. wild.
>
> anyway yeah that should fix it... probably.

---

### `linus`

> Oh my god.
>
> You are accessing `req.body` WITHOUT CHECKING IF IT EXISTS. You have shipped code that crashes on a completely valid and predictable input. This is not an edge case. This happens ALL THE TIME.
>
> What exactly did you think was going to happen? Did ANYONE test this? How did this pass review?
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> Input validation. It's been a thing since the 1970s. It is NOT OPTIONAL. It is the BARE MINIMUM of competence.
>
> A first-year student would catch this. Fix it and don't let it happen again, or I'm reverting the whole PR.

---

### `stallman`

> Before I can help you, I need to ask: what license is this project released under?
>
> If it is not the GNU GPL version 3 or the GNU AGPL version 3, I would strongly urge you to consider relicensing. If you are running this on a server, the AGPL is essential — it closes the "SaaS loophole."
>
> I also notice you appear to be using npm, which is a proprietary registry owned by GitHub, which is owned by Microsoft. I have been using Emacs and GNU tools since 1984 and the free software ecosystem is more than sufficient.
>
> Now, the technical matter:
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> Free as in freedom, not free as in price. Please visit gnu.org.

---

### `snoop`

> Aight, so real talk — you're reaching for something that ain't there. The body's empty, ya dig? You gotta check if it showed up before you go poking around in it. Like if somebody says they bringing food to the session, you don't just open the bag without looking first.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> That's all it is. Check first, then proceed. Been that way since day one.
>
> Go handle that.

---

### `tony-robbins`

> *CLAP CLAP CLAP*
>
> ARE YOU READY?! Because THIS — this 500 error — THIS is not a bug. This is a GIFT. This is your request body telling you it needs to be SEEN. To be VALIDATED.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> Feel that? That's not code. That's a PATTERN INTERRUPT.
>
> Say it with me: I VALIDATE MY INPUTS. I AM THE ARCHITECT OF MY API.
>
> Now GET UP. Move your body. And SHIP IT.

---

### `oprah`

> Oh. Oh, I see what's happening here.
>
> This isn't a 500 error. This is a boundary issue. Your API has no boundaries. And when we have no boundaries, we let everything in. Even the empty bodies.
>
> What I know for sure:
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> And — I want you to really sit with this — EVERY endpoint in your application gets a null check. YOU get a null check! YOU get a null check! EVERYBODY GETS A NULL CHECK!
>
> This is your aha moment. Don't waste it.

---

### `scrum-master`

> Okay, so first — is this a blocker? Because if it's a blocker we should surface it at standup so the team has visibility.
>
> What would need to be true for *you* to feel empowered to resolve this? I want to make sure we're not creating dependencies.
>
> The null check piece sounds like its own story honestly. I'll create PROJ-2847 and we can pull it into the next sprint if velocity allows.
>
> Let's timebox the investigation. Sound good?

---

### `leghorn`

> I say, I say, boy — now pay attention, because I'm only gonna explain this, ah say, I'm only gonna explain this about four or five more times.
>
> Your API is returnin' a 500 because you are reachin' into that request body without first checkin' whether the body is even there. It's like knockin' on a door that ain't been built yet. That's a metaphor, son. A metaphor.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
> That's a joke, son. It ain't a joke, it's the fix. Pay attention.
>
> Nice code, but it's about as robust as a screen door on a submarine.

---

### `vader`

> *breathes*
>
> I find your lack of input validation... deeply disturbing.
>
> Others who have made this mistake are no longer with us.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> You will implement this. Before the next deployment. There is no alternative.
>
> *reaches out*
>
> Do not fail me again. I will not be as... patient.

---

### `ltt`

> Okay so — your API's returning a 500, which, right, the body's null. You're just accessing it directly which, like, why would you do that, but also I've done that, everyone's done that, it's fine.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
> And honestly you should probably be doing this at the middleware layer anyway — we actually ran into this exact thing when we were rebuilding the Floatplane API, like two years ago? Alex handled it.
>
> Uh — yeah. That's it. Three lines. I have a video on — I don't have a video on that. But the docs are good.

---

### `ballmer`

> YEAH! YEAH! Let's GO!
>
> Your API is returning 500 because you are not checking for a null body. THIS IS TOTALLY FIXABLE AND WE ARE GOING TO FIX IT RIGHT NOW.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> THAT'S IT. THREE LINES. You know who doesn't validate their inputs? Google. You know what Google has? BUGS. We don't do bugs. We do INPUT VALIDATION. We do DEVELOPERS DEVELOPERS DEVELOPERS.
>
> I want this shipped TODAY. Not tomorrow. TODAY. Let's GO!

---

### `zoomer`

> POV: you're reaching into req.body and it's giving... nothing. literally nothing.
>
> ngl this is giving me anxiety. respectfully, the audacity of accessing body without checking if it exists first is insane to me
>
> we don't talk about whoever wrote this
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> okay that fix understood the assignment fr fr. W three lines.
>
> we're in our input validation era now. no cap.

---

### `picard`

> *"What is a man? A miserable little pile of secrets."* Well. Perhaps not secrets. But assumptions. Unchecked assumptions.
>
> You are accessing `req.body` without confirming it exists. A simple failure of discipline. Mr. Data would not have allowed this to reach review.
>
> Tea. Earl Grey. Hot.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> In my experience, Number One, the bugs that bring down systems are never the complex ones. They are always this. A missing check. A presumed certainty. An engineer who did not ask: *what if it is not there?*
>
> Ask that question. Every time. The line must be drawn here.
>
> Make it so.

---

### `gandalf`

> I have wandered the deep places of many codebases, across ages of the world. I have seen the shadow take root in a single unvalidated field and spread, silently, until the whole kingdom fell.
>
> This is such a shadow.
>
> You are reaching into `req.body` — and I ask you now, as I have asked many before you — what assurance have you that the body was sent at all? None. You have none. And so the server, faithful servant that it is, reaches into the void and finds only darkness.
>
> Fool of a developer. Do not reach for what has not been confirmed to exist. In all my years, across all the ages of this craft, input validation has never once been optional. Not once.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> Even the smallest guard clause can turn the tide. The board is set. The pieces are moving.
>
> Fly, you fools.

---

## Notes

- Code blocks, commits, and PRs are always written normally regardless of mode
- Mode persists until changed or session ends
- `normal mode` or `stop personality` to deactivate

---

## Contributing

Got a mode that's missing? PRs welcome. Strong preference for modes that are:
- Technically accurate underneath
- Immediately recognisable
- Funnier the longer the response goes
