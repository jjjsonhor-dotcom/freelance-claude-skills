# Client-to-Cash Change-Order Responder (free skill for Claude)

Free skill for freelance scope creep, plus the Client-to-Cash Freelance Skills Pack (for Claude) that covers the rest of a client-to-cash job.

Not affiliated with or endorsed by Anthropic. Claude is a trademark of Anthropic.

## Get the files

- [Client-to-Cash Change-Order Responder (free skill for Claude)](https://payhip.com/b/gX9s4)
- [Client-to-Cash Freelance Skills Pack (for Claude), $29 launch](https://payhip.com/b/fdMjC)
- [Client-to-Cash shop](https://payhip.com/clienttocash)

The source for the free skill also lives in this repo at [`skills/change-order-responder/SKILL.md`](skills/change-order-responder/SKILL.md).

## Free Freelance Scope-Creep & Change-Order Email Scripts (12 ready-to-send templates)

Start with the [Free Freelance Scope-Creep & Change-Order Email Scripts (12 ready-to-send templates)](guides/freelance-scope-creep-change-order-scripts.md). Copy a template, fill in the bracketed bits, and send. For a reply drafted from the client's actual message and your proposal, use the free skill below.

## Free Freelance Late-Invoice Email Scripts (10 ready-to-send templates)

Start with the [Free Freelance Late-Invoice Email Scripts (10 ready-to-send templates)](guides/freelance-late-invoice-email-scripts.md). Copy a template, fill in the bracketed bits, and send. For an email drafted from the actual invoice facts and what you have already sent, use the late-invoice-chaser skill in the $29 pack.

## Free skill: Client-to-Cash Change-Order Responder (free skill for Claude)

When a client says "can you also add this before launch, should be quick," this skill classifies the request against the agreed scope, estimates time and cost if the work is new, and drafts a calm reply with clear options: do it in scope, swap something out, approve a paid change, or park it.

It will not invent a fee, start unpaid work, or write a defensive email.

### Install in claude.ai or Claude Desktop

The official free zip on Payhip is already in the format Claude expects: the skill folder at the top level, containing SKILL.md, and nothing else at the zip root. Upload that zip as-is.

```
free-change-order-responder-skill.zip
└── change-order-responder/
    └── SKILL.md
```

If you are rebuilding a zip from this repository, zip the skill folder, not a README sitting next to it:

```bash
zip -r change-order-responder.zip skills/change-order-responder
```

The rebuilt zip must still have `change-order-responder/` (with SKILL.md inside it) at the top level. Do not add a README at the zip root.

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

The paid Client-to-Cash Freelance Skills Pack (for Claude) is delivered as a zip after purchase on Payhip. It is not stored in this public repository.

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

The free skill and the guides in this repository are under the MIT License. Copyright 2026, Client-to-Cash. See [LICENSE](LICENSE).

The Client-to-Cash Freelance Skills Pack (for Claude) is sold separately under a single-seat license and is not in this repository.

These files draft commercial emails and documents. They are not legal, tax, or financial advice.

Not affiliated with or endorsed by Anthropic. Claude is a trademark of Anthropic.

## Spec

Checked 26 November 2026 against the Agent Skills spec and Anthropic's docs: https://agentskills.io/specification
