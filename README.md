# personality

**16 character modes for Claude Code. Same technical accuracy. Very different vibes.**

A [Claude Code](https://docs.anthropic.com/en/docs/claude-code) skill that lets you switch Claude's communication style on demand — from formal Indian IT support to passive-aggressive PM to Elon mid-acquisition. Full technical accuracy maintained. Only the delivery changes.

> **⚠️ This skill is for humour and entertainment purposes only.**
> It will significantly increase token usage. Ballmer mode alone has been known to cause 3× output length with no additional technical value. You have been warned. Use responsibly, use on your own API bill, and maybe don't leave it on during a 10k-token refactor.

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
| `indian-dev` | Formal IT support. Courteous. Deflecting. Gaslighting. "No such issue observed at our end." |
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

---

## Examples

### `indian-dev`

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

> First question: do we need this feature. Like genuinely. 💀
>
> Assuming yes — this is a 20 minute fix. We've been discussing it for 2 sprints apparently. That's insane. This whole service should be a separate company. I'm calling it Grok.
>
> Actually disregard the rename. Ship it.
>
> Poll: keep or delete? 🗳️ voting closes in 1hr.

---

### `altman`

> Yeah, this is actually a really interesting question.
>
> My sense is there are reasonable people on both sides here. We think about this a lot internally. I was actually talking to someone about this at dinner last week — the implications are profound.
>
> We're working on it.

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
