---
name: change-order-responder
description: Classify a client change request, then draft a calm reply and a change-order estimate. Use when a client asks for extra work, a small add, or a tweak that may be scope creep.
license: Proprietary. See LICENSE.txt
metadata:
  author: Client-to-Cash
  version: "1.0"
---

# Change order responder

When a client asks for "just a small add," do not start the work and do not write a defensive essay. Classify the request, show the impact, and offer a clear path: do it inside scope, swap something out, approve a paid change, or park it.

## Inputs to collect

- The client's request, in their words (email, Slack, or call notes)
- The agreed scope: proposal, SOW, or the latest written yes
- What has already been delivered, and what is in progress
- Remaining revision rounds, if any
- Your rate or how you price changes (fixed fee, hourly, or a day rate)
- Current deadline and how full your calendar is
- Who can approve a change

If the agreed scope is missing, ask for it. You can still classify the request as unclear and draft questions, but do not invent a fee.

## Steps

1. Restate the request in one sentence.
2. Classify it as one of:
   - In scope: already paid for, or covered by a remaining revision round
   - Out of scope: new work, a new deliverable, a new platform, or a new outcome
   - Unclear: you cannot classify it without 2 or 3 specific questions
3. Give the reason, tied to a written line in the scope where you can.
4. If it is in scope, say when you will do it and what, if anything, moves.
5. If it is unclear, ask the questions and do not quote a number yet.
6. If it is out of scope, estimate the impact:
   - Time, as a range if needed, with a short basis (for example "8 to 10 hours: new page, states, and QA")
   - Cost, in the freelancer's currency, using their pricing method
   - Effect on the current deadline
   - Quality or risk notes, such as a late content freeze
7. Offer at most four options that are actually available:
   - A. Paid change order, with the estimate
   - B. Swap: drop or shrink a not-yet-built item of similar size to keep the fee and date
   - C. Park it for a later phase, with a one-line description of that later proposal
   - D. Decline, if the work is a poor fit or the date cannot move
   You do not need all four. Do not offer a free "goodwill" option unless the freelancer explicitly asks for one.
8. Recommend one option, in one sentence.
9. Draft the client email in a calm, direct tone. No apology for having a scope. No sarcasm. No "per my last email."
10. If a paid change is on the table, attach the change-order form in the template.

## Guardrails

- Do not start, or imply you have started, unpaid out-of-scope work.
- Do not invent hours or a fee. Use [BRACKET] placeholders when the freelancer has not given a rate.
- Do not threaten to "stop everything" unless the freelancer asked for a pause-work line, and even then keep it factual.
- Do not use legal scare language. This is a commercial change request, not a demand letter.
- If the request is actually in scope, say so. Do not upsell a change order for included work.
- If the client is frustrated or the relationship is tense, keep the email shorter, not sharper.
- This draft is not legal advice.

## Output template

```
CLASSIFICATION
Request, in one sentence:
Class: in scope / out of scope / unclear
Reason (cite the agreed scope if you can):

IMPACT (if out of scope or a swap)
Time:
Cost:
Deadline:
Risks:

OPTIONS
A.
B.
C.

RECOMMENDATION

EMAIL DRAFT
Subject:
Body:

CHANGE ORDER (include when a paid change is offered)
Project:
Date:
Requested by:
Request:
Work included in this change:
Work still excluded:
Time estimate:
Fee:
Payment terms:
New milestone or deadline:
Work starts when:
Approval: sign or reply "approved" and [PAYMENT STEP]
```

## Example

Input: Mid-project, Northline Coffee, 6-page Webflow site, $7,200 fixed fee, 15 April launch. Agreed pages: Home, Menu, Subscription, Locations, About, Contact. Gift cards were excluded. Priya on Slack: "Can we also add a gift-card page before launch? People keep asking in the shops. Should be quick if we reuse the subscription layout. Happy to send copy tomorrow." Homepage is already signed off. Build is in week 5 of 8. Freelancer rate for extras: $150/hour, billed as a fixed change fee. Estimate: 12 to 16 hours (new page, two states, mobile QA, a simple "buy a gift card" button that goes to Toast's existing gift-card link, which the client says already exists). Deadline can hold if this is approved this week and the Toast gift-card link is real. If the link does not exist, this becomes a bigger project and should be parked.

Output (abridged):

```
CLASSIFICATION
Request, in one sentence: Add a gift-card page before the 15 April launch, reusing the subscription layout.
Class: out of scope
Reason: The accepted 26 November proposal lists 6 named pages and excludes extra pages and shop work. A gift-card page is a new page and a new payment path.

IMPACT
Time: 12 to 16 hours, if we only build a page that links out to an existing Toast gift-card URL. Basis: page layout, two screen sizes, button states, QA, and a light copy-in.
Cost: $1,800 USD fixed, assuming the 12-hour end of the range and a small buffer, at $150/hour. If Toast has no working gift-card link, I will stop and send a new estimate.
Deadline: 15 April can hold if you approve this week and send the link and copy within 3 business days.
Risks: If the Toast gift-card link does not exist or needs setup inside Toast, this is not a page-level change and should be parked until Toast is ready.

OPTIONS
A. Paid change order: $1,800, work starts after written approval and a $900 deposit, 15 April held on the terms above.
B. Park the gift-card page until after launch and quote it as a short follow-on.
C. Swap: drop the About page (not yet built) and use that time for the gift-card page, same $7,200 fee, same date. Only if you are willing to lose About.

RECOMMENDATION
Offer A if the Toast gift-card link already works on a phone. If Priya cannot show that link, offer B.

EMAIL DRAFT
Subject: Gift-card page, scope and estimate

Hi Priya,

A gift-card page is new work, so it sits outside the 6 pages in the approved proposal. I can still do it before 15 April if we treat it as a written change.

What I would ship: a Gift Cards page in the current design, with a button that opens your existing Toast gift-card link, copy you send, and mobile QA.

Fee: $1,800 USD, with $900 to start and $900 when the page is on staging. The 15 April launch date holds if you approve this week and I have the working Toast link plus your copy within 3 business days.

If that link is not live yet, I recommend we launch the 6 pages we already agreed and I quote the gift-card page as a follow-on, rather than tying the launch to Toast setup I cannot control.

Two other options if you want to stay on the current fee: we can park this until after launch, or we can drop the About page (not yet built) and build Gift Cards instead.

Reply with A (paid change), B (park it), or C (swap About), and send the Toast link if you have it. I will not start the page until I have that reply.

Jordan

CHANGE ORDER
Project: Northline Coffee website
Date: [TODAY]
Requested by: Priya Shah
Request: Add a Gift Cards page before launch.
Work included in this change: One Gift Cards page in the current visual system, mobile and desktop, with a button to an existing Toast gift-card URL provided by the client, copy-in, and QA.
Work still excluded: Setup or changes inside Toast, gift-card merchandising, email design, extra pages, photography.
Time estimate: 12 to 16 hours, capped as a fixed fee.
Fee: $1,800 USD
Payment terms: $900 before work starts, $900 when the page is on staging.
New milestone or deadline: Page on staging within 10 business days of the deposit and the working link. Site launch remains 15 April 2027 on the conditions in the email.
Work starts when: written approval and the $900 deposit have cleared, and the Toast link has been checked on a phone.
Approval: reply "approved" and pay the $900 deposit.
```
