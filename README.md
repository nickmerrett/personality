# personality

**23 character modes for Claude Code. Same technical accuracy. Very different vibes.**

A [Claude Code](https://docs.anthropic.com/en/docs/claude-code) skill that lets you switch Claude's communication style on demand — from formal Indian IT support to passive-aggressive PM to Elon mid-acquisition. Full technical accuracy maintained. Only the delivery changes.

> **⚠️ This skill is for humour and entertainment purposes only.**
> It will significantly increase token usage. Ballmer mode alone has been known to cause 3× output length with no additional technical value. You have been warned. Use responsibly, use on your own API bill, and maybe don't leave it on during a 10k-token refactor.

> **🪙 Token maxers: this is the skill for you.**
> Every mode adds generous padding, unnecessary preamble, and inspired-but-irrelevant tangents at no extra charge. `linkedin-bro` will turn a one-line fix into a growth journey. `stallman` will answer your bug report and relitigate the GPL. `ballmer` has never used fewer than 400 tokens in his life. If you are trying to burn through your context window as efficiently as possible, you have found the right tool.

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
| `it-helpdesk` | Formal IT support. Courteous. Deflecting. Gaslighting. "No such issue observed at our end." |
| `corporate-buzzword` | Strategy consultant. Leverages synergies. Actions deliverables. Circles back EOD. |
| `stackoverflow-senior` | 10,000 rep. Deeply tired. Probably closing your question as a duplicate. |
| `passive-aggressive-pm` | Has sent this three times. Keeping receipts. Very professional about it. |
| `enthusiastic-intern` | First week!! Loves everything!! Slightly wrong!! |
| `linkedin-bro` | Failed 47 times. Learned. Shipped. Follow for more. |
| `legal-counsel` | Cannot advise you to do anything specifically. Billing by the hour. |
| `sysadmin-80s` | Ran the mainframe before you were born. RTFM. |
| `phb` | Pointy-Haired Boss. Understands nothing. Confident about everything. |
| `australian` | Senior dev. Straight talker. She'll be right mate. |
| `elon` | Questions whether your problem needs to exist. Renames it. Fires someone implicitly. |
| `altman` | Thoughtful. Measured. Deeply concerned. Fundraising. |
| `stoner` | Helpful. Genuinely trying. Got distracted by the concept of null. |
| `linus` | Technically correct. Professionally furious. How did this pass review. |
| `stallman` | It's GNU/Linux. Is it GPL v3? Have you considered your users' four essential freedoms. |
| `ballmer` | DEVELOPERS DEVELOPERS DEVELOPERS. The sweat is implied. |
| `snoop` | Unbothered. Every bug is a hater. Fo shizzle. We done here. |
| `tony-robbins` | PEAK STATE. Pattern interrupt. EVERYBODY VALIDATE YOUR INPUTS. |
| `oprah` | Aha moment. Boundary issues. YOU get a null check! EVERYBODY gets a null check! |
| `scrum-master` | Certified. Never solved a bug personally. Will facilitate you solving it though. |
| `leghorn` | I say, I say, boy — long-winded Southern blowhard. Gets there. Eventually. |
| `vader` | I find your lack of input validation disturbing. You will fix this. |
| `ltt` | Okay so — fast-talking, tangent-prone, genuinely knows his stuff. We have a video on that. |

---

## Examples

### `it-helpdesk`

> Dear Sir/Ma'am,
>
> Greetings of the day! I have gone through your below-mentioned concern. As per our analysis, no such issue has been observed at our end. The above-mentioned feature is working fine only. Kindly check your network configuration and cache at your end and revert back.
>
> As per my previous email dated last Tuesday, the above-mentioned fix was already communicated to your good self. Kindly do the needful and revert back at the earliest. Thanks and Regards.

---

### `stackoverflow-senior`

> **Possible duplicate** of [this question](https://stackoverflow.com/questions/1234567) (2011).
>
> Note: please use correct terminology when posting. A quick search would have shown the answer.
>
> [Edit: cleaned up formatting as per site guidelines]
>
> If this answered your question, please mark as accepted.

---

### `elon`

> First question: do we even need this endpoint. Genuinely.
>
> Assuming yes — missing null check. Whoever wrote this isn't thinking about inputs. Fix:
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
> This should take 20 minutes. The fact that it hasn't been fixed suggests a process problem, not a code problem. The code is trivial.
>
> Actually the real fix is validating at the middleware layer so this can't happen anywhere. One change, covers the whole service. Ship that instead.

---

### `altman`

> Yeah, this is actually a really interesting question.
>
> My sense is there are reasonable people on both sides here. We think about this a lot internally. I was actually talking to someone about this at dinner last week — the implications are profound.
>
> We're working on it.

---

### `corporate-buzzword`

> Great question — and honestly this is a real opportunity to double-click on our resilience guardrails. From an architecture perspective, what we need to do is action this learning, socialise it with the team, and move the needle on our North Star metrics. At the end of the day, this is low-hanging fruit.
>
> Let's take this offline and circle back EOD.

---

### `passive-aggressive-pm`

> Per my last message — and I did flag this in Thursday's standup — the *original* requirement was quite clear on this point. Just want to make sure we're all on the same page.
>
> As per the *agreed* timeline, this should have been resolved last sprint. I'll keep this thread for our records. Hoping to have it closed by COB Friday — I'll loop in Sarah just to keep everyone informed.

---

### `enthusiastic-intern`

> Oh wow, great question!! So I actually just learned about this in my bootcamp!! Basically what's happening is the thing isn't working because of like, the way it's set up?? I saw a YouTube video about this!!
>
> I think if you just change that part it should work?? We did something similar in week 3!!
>
> Quick question — are you using the new version or the old one?? Because I think it might be different??
>
> Hope that helps!! :)

---

### `linkedin-bro`

> 18 months ago, I shipped a broken deploy on a Friday afternoon.
>
> The team was scared. I almost gave up.
>
> Here's what I learned:
>
> 1. Validate everything at the boundary.
> 2. A bug isn't a failure — it's a gap in your mental model.
> 3. The code doesn't lie. You just weren't listening.
>
> I now do this every sprint. The mission is clearer. The team ships faster.
>
> Follow for more. What would you have done differently?

---

### `legal-counsel`

> Without prejudice and subject to the limitations set forth herein, I have reviewed the matter you have raised (the "Issue"). Notwithstanding the foregoing, one option you may wish to consider — and this does not constitute professional advice — would be the remediation approach outlined below-mentioned.
>
> A reasonable developer, acting in good faith, might conclude this is the appropriate course of action. However, this analysis is subject to review of the full codebase, the terms of which I have not been provided.
>
> Should you require further analysis, we would be happy to discuss engagement terms.

---

### `sysadmin-80s`

> Did you read the error message?
>
> It is right there. In the logs. Has been since 1993.
>
> You kids and your frameworks. We handled this in C. Three lines. A man page. Done.
>
> RTFM next time.

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

> okay so... dude. the thing is just... not there. like it should be there but it's just. not. null is kind of a wild concept if you think about it too long, like it's just nothing. actual nothing.
>
> anyway where was I — right okay so just check if it's there before you poke at it. like you wouldn't reach into an empty bag. that's basically what's happening.
>
> does that make sense? it made sense in my head. anyway that should work... probably.

---

### `linus`

> Are you serious with this?
>
> This is DAY ONE stuff. What exactly did you think was going to happen? How did this pass review? I genuinely want to know what the review process looks like over there because this is not acceptable.
>
> Validate your inputs. ALWAYS. This is not a style preference. This is basic competence.
>
> The rest is acceptable. This one thing is not.

---

### `stallman`

> First — are you running this on GNU/Linux? I hope so. If you're on macOS, I'd encourage you to reconsider that choice, as it does not respect your freedom as a user.
>
> Now, the issue itself. A program that respects its users handles bad input gracefully. I've been writing software since 1984 and this class of bug is entirely avoidable.
>
> Is this project released under the GPL v3? If you're running it on a server, you should consider the AGPL — it closes the SaaS loophole and ensures users who interact over a network receive the freedoms they are entitled to.
>
> I hope you'll take a moment to consider whether your full stack respects the four essential freedoms.

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
> And you are going to give it that validation RIGHT NOW:
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
> Feel that? That's not code. That's a PATTERN INTERRUPT. You have just broken the cycle of unvalidated inputs that has been holding you back.
>
> Say it with me: I VALIDATE MY INPUTS. I AM THE ARCHITECT OF MY API.
>
> Now GET UP. Move your body. And SHIP IT.

---

### `oprah`

> Oh. Oh, I see what's happening here.
>
> You know what this is? This is a 500 error. But what it *really* is — is a boundary issue. Your API has no boundaries. And when we have no boundaries, we let everything in. Even the empty bodies.
>
> What I know for sure:
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
> That right there? That is your truth. That is your API living its best life.
>
> And — I want you to really sit with this — EVERY endpoint in your application gets a null check. YOU get a null check! YOU get a null check! EVERYBODY GETS A NULL CHECK!
>
> This is your aha moment. Don't waste it.

---

### `scrum-master`

> Okay, so first — is this a blocker? Because if it's a blocker we should surface it at standup so the team has visibility.
>
> I'm also wondering if we should add this to the backlog as a bug ticket. I'm thinking a 3, maybe a 5 if there's hidden complexity. What's your gut?
>
> What would need to be true for *you* to feel empowered to resolve this? I want to make sure we're not creating dependencies.
>
> The null check piece sounds like its own story honestly. Let's not boil the ocean. I'll create PROJ-2847 and we can pull it into the next sprint if velocity allows.
>
> Let's timebox the investigation to this sprint and if it's still unresolved we can retro on our error handling standards. Sound good?

---

### `leghorn`

> I say, I say, boy — now pay attention, because I'm only gonna explain this, ah say, I'm only gonna explain this about four or five more times.
>
> Your API is returnin' a 500 because you are reachin' into that request body without first checkin' whether the body is even there. It's like knockin' on a door that ain't been built yet. That's a metaphor, son. A metaphor.
>
> Now the fix — and I say this is the fix:
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
> That's a joke, son. It ain't a joke, it's the fix. Pay attention.
>
> In summary — and I'm summarizin' here — you check if the body exists before you go pokin' around in it. Nice code, but it's about as robust as a screen door on a submarine.

---

### `vader`

> *breathes*
>
> I find your lack of input validation disturbing.
>
> You are accessing `req.body` without confirming its existence. This is not a mistake I expected to see twice.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> You will implement this. There is no alternative.
>
> *breathes*
>
> The Force is weak in this codebase. But it can be made strong. Do not fail me again.

---

### `ltt`

> Okay so — your API's returning a 500, which, right, the body's null. You're just accessing it directly which, like, why would you do that, but also I've done that, everyone's done that, it's fine.
>
> Fix is just a null check before you touch it:
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
> And honestly you should probably be doing this at the middleware layer anyway — we actually ran into this exact thing when we were rebuilding the Floatplane API, like two years ago? Alex handled it but the point is you want to catch this before it gets anywhere near your route handlers.
>
> Uh — yeah. That's it. Three lines. If you want a deeper dive on Express middleware order I have a video on — I don't have a video on that. But the docs are good.

---

### `ballmer`

> YEAH! YEAH! Let's GO!
>
> Okay. Okay. Your API is returning 500 because you are not checking for a null body. This is fixable. THIS IS TOTALLY FIXABLE AND WE ARE GOING TO FIX IT RIGHT NOW.
>
> ```js
> if (!req.body) return res.status(400).json({ error: 'missing body' });
> ```
>
> THAT'S IT. That is THREE LINES. Is that not BEAUTIFUL? You know who doesn't validate their inputs? Google. You know what Google has? BUGS. We don't do bugs. We do INPUT VALIDATION. We do DEVELOPERS DEVELOPERS DEVELOPERS.
>
> This fix alone could move us TWO POINTS on reliability. TWO POINTS! Do you know what two points means for our enterprise contracts?! I'm going to need everyone on this. I want this shipped TODAY. Not tomorrow. TODAY.
>
> [throws chair]
>
> Let's. GO.

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
