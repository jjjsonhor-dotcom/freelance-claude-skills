# Freelance Client-to-Cash Claude Skills

Free Claude skill for freelance scope creep, plus a 10-skill pack that covers the rest of a client-to-cash job.

This repository is not affiliated with Anthropic.

## Get the files

- [Free change-order-responder zip](https://payhip.com/b/gX9s4)
- [Full 10-skill pack, $29 launch](https://payhip.com/b/fdMjC)
- [Client-to-Cash shop](https://payhip.com/clienttocash)

The source for the free skill also lives in this repo at [`skills/change-order-responder/SKILL.md`](skills/change-order-responder/SKILL.md).

## Free Freelance Scope-Creep & Change-Order Email Scripts (12 ready-to-send templates)

Start with the [Free Freelance Scope-Creep & Change-Order Email Scripts (12 ready-to-send templates)](guides/freelance-scope-creep-change-order-scripts.md). Copy a template, fill in the bracketed bits, and send. For a reply drafted from the client's actual message and your proposal, use the free skill below.

## Free skill: change-order-responder

When a client says "can you also add this before launch, should be quick," this skill classifies the request against the agreed scope, estimates time and cost if the work is new, and drafts a calm reply with clear options: do it in scope, swap something out, approve a paid change, or park it.

It will not invent a fee, start unpaid work, or write a defensive email.

### Install in claude.ai or Claude Desktop

Do not upload a zip that has a README sitting next to the skill folder. Claude expects a zip whose top level is the skill folder:

```
change-order-responder.zip
└── change-order-responder/
    └── SKILL.md
```

From a folder that contains `change-order-responder/`:

```bash
zip -r change-order-responder.zip change-order-responder/
```

1. Open Settings, then Capabilities. Turn on Code execution and file creation. Some accounts label this Create and edit files.
2. Open Customize, then Skills.
3. Click +, then Create skill, then Upload a skill.
4. Upload that zip and turn the skill on.
5. In a new chat, paste the client's request and the agreed scope, or say "Use the change-order-responder skill."

### Install in Claude Code

Copy the `change-order-responder` folder into your personal skills directory. No upload is required.

```bash
mkdir -p ~/.claude/skills
cp -R skills/change-order-responder ~/.claude/skills/
```

On Windows, the path is `%USERPROFILE%\.claude\skills\change-order-responder\SKILL.md`.

For one repo only, use `.claude/skills/change-order-responder/SKILL.md` at the project root.

Open a new Claude Code session and ask for the job, or name the skill. Run `/skills` to confirm it loaded.

### Example

Input:

```text
Use the change-order-responder skill.

Agreed scope: a 6-page marketing site, no extra pages. Gift cards were excluded.
Client Slack: "Can we also add a gift-card page before launch? Should be quick."
My extra-work rate: $150/hour.
```

Output, abridged from the skill's own example:

```text
CLASSIFICATION
Request, in one sentence: Add a gift-card page before launch.
Class: out of scope
Reason: The agreed proposal lists 6 named pages and excludes extra pages.

IMPACT
Time: 12 to 16 hours
Cost: $1,800
Deadline: can hold if approved this week

OPTIONS
A. Paid change order, $1,800
B. Park it until after launch
C. Swap a page that is not yet built

RECOMMENDATION
Offer A if the client's gift-card link already works. Otherwise offer B.

EMAIL DRAFT
A short, calm reply that states the work is new, names the fee, and asks the client to pick A, B, or C. Work starts after written approval.
```

## The 10-skill pack

The paid pack is delivered as a zip after purchase on Payhip. It is not stored in this public repository.

| Skill | What it writes |
| --- | --- |
| discovery-call-prep | A timeboxed call brief, questions, and a do-not-promise list |
| scoped-proposal-writer | A fixed-scope proposal with exclusions, price, and terms |
| sow-and-scope-guard | A short statement of work and a table of change triggers |
| change-order-responder | A classification, a calm reply, and a change-order estimate. This one is also free. |
| client-kickoff-pack | Kickoff agenda, working agreement, and an access checklist |
| weekly-status-brief | A short status email: shipped work, blockers, deadline |
| late-invoice-chaser | The next overdue-invoice email, paced and factual |
| case-study-extractor | A one-page case study, a short blurb, and a permission ask |
| retainer-upsell-pitch | A fenced monthly retainer offer, only when the fit is real |
| client-offboarding-referral | A handover checklist, a closing email, and a timed referral ask |

Launch price is $29, then $39. One-time payment. Single-seat license. No subscription.

## License

The free skill is for a single seat, for your own personal or freelance use. Do not resell it or share the file. This is not legal advice.

## Spec

Checked 26 November 2026 against the Agent Skills spec and Anthropic's docs: https://agentskills.io/specification
