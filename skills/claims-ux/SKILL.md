---
name: claims-ux
description: Claims Copilot domain semantics for UI design — claim states and their tones, deadline urgency, readiness concepts, evidence vocabulary, screen anatomy, and copy voice. Activate whenever designing or adjusting any Claims Copilot screen or component.
---

# Claims Copilot — domain UX

The product: STR operators file damage claims against platform programs
(Airbnb AirCover first). The persona designs everything: **on a phone,
annoyed, racing a checkout deadline.**

## Claim states — always these 16, always humanized, always these tones

Draft (neutral) · Collecting evidence (violet) · Ready to submit (info) ·
Awaiting guest (warning) · Submitted (brand teal) · Under review (warning) ·
Escalated (danger) · Resolved (success) · Reimbursed (success) · Declined
(danger) · Partially paid (rating gold) · No response (warning) · Reopened
(info) · Withdrawn (neutral) · Expired (danger) · Closed (neutral).

Never invent states; never show machine names (EVIDENCE_PENDING is
"Collecting evidence").

## Deadline urgency (separate system from readiness)

danger solid <24h ("Due in 18 h") · warning tint <72h ("Due in 2 days") ·
neutral beyond ("Due in 9 days") · "Window closed" when past. Copy stays
calm — the color carries the temperature. A same-day turnover can compress
the filing window to hours; that's why deadline chips appear on list rows
AND detail headers, and lists sort deadline-first.

## Readiness (the hero, deterministic)

A 0–100 engine score with a threshold: warning below, success at/above.
Shown as a drawn ring + "N gaps block readiness" + a checklist of
requirements (met ✓ / unmet-required emphasized / optional de-emphasized).
It is rule-driven, NEVER an AI feature — do not give it AI styling. The
unmet items double as the "what to add next" prompt.

## Evidence vocabulary

Types: Photo, Receipt, Invoice, Guest message, Platform confirmation.
Categories (design for all seven): Damage, Cleaning, Smoke, Missing items,
Lost keys, Unauthorized guests, Pet damage. Requirements read as the thing
to add: "Photos of the damage", "Invoice or receipt", "Guest message
admitting the incident".

## Screen anatomy

- Claims list: rows of property / guest · category / deadline chip / state
  pill; deadline-sorted; "New claim" is the single primary.
- Claim detail: header (property, guest·category·platform, state pill +
  deadline chip), damage description, ONE primary action (the state
  transition: Activate → Mark ready → Submit) docked to the bottom on
  mobile, then sections: Readiness (first), Evidence, AI summary, AI draft.
- Intake: property, guest, checkout datetime + confirmed checkbox, next
  check-in, category, damage description. Helper text explains what fields
  gate ("required before you can activate").

## Voice & discipline

Violet marks two things — active-assistance status AND AI affordances — so
color is never the only signal (AI gets an explicit label/icon). Exactly one
primary action per screen. ≥44px tap targets. No dashboards, filters, or
portfolio analytics — deliberately out of scope for MVP.
