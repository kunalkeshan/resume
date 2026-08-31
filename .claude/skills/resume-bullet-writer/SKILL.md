---
name: resume-bullet-writer
description: Turn a rough description of work into a polished, quantified resume bullet in Kunal's voice. Use when adding new content to master-resume.md, or when Kunal asks to improve/strengthen an existing bullet.
---

# Resume Bullet Writer

Converts a rough description of work into a resume bullet: action-verb-led, quantified, in the *what-you-did → tools touched → quantified outcome* shape required by this project's `CLAUDE.md`.

## When to Use

- Kunal describes new work/a project/an achievement and it needs to become a `master-resume.md` bullet
- An existing bullet reads as weak (passive, vague, no metric) and needs strengthening

## Non-Negotiable: Ask, Don't Guess

Per this project's `CLAUDE.md`: **never invent or skip a metric.** If Kunal doesn't state impact precisely, ask for his best estimate rather than writing a vague bullet or making up a number. This is the most important rule in this skill — treat friction from asking as acceptable, skipping the question is not.

## What Makes a Bullet Weak

- Passive/vague verbs: "responsible for," "helped with," "worked on," "assisted with"
- No number — describes a duty, not an outcome
- Too long (should be 1–2 lines)

## What Makes a Bullet Strong

Every bullet needs:
- A strong action verb (led, built, shipped, reduced, automated, architected, resolved...)
- At least one quantified metric (%, count, timeframe, scale, $ — whatever's honest and available)
- The tools/tech/skills actually involved
- A result, not just an activity

## Formula: X–Y–Z

`Accomplished [X], measured by [Y], by doing [Z]`

Example: "Reduced API response time by 60% (800ms → 320ms) by redesigning the caching layer with Redis" — X = reduced latency 60%, Y = 800ms→320ms, Z = redesigned caching with Redis.

## When Kunal Can't Give an Exact Number

Ask for his best estimate first. If he genuinely can't estimate a direct outcome metric, fall back to quantifying scale/input instead of dropping the number entirely:
- Can't measure revenue impact? Quantify volume: "processed 500+ records/day," "supported 20+ concurrent users"
- Can't measure % improvement? Use a before/after range or a conservative estimate, clearly flagged as approximate ("~40%," "an estimated 10hrs/week")

Never fabricate a precise-sounding number he didn't actually state or estimate.

## Process

1. Get the rough description from Kunal.
2. Identify what's missing: the action, the tools, or the metric.
3. Ask targeted follow-up questions for whatever's missing — don't ask a generic checklist, ask exactly what's needed to fill the gap.
4. Draft the bullet using the X-Y-Z shape.
5. Keep it in Kunal's voice — polished and action-led, but not generic corporate-speak. Avoid over-genericizing power verbs if they don't match how he'd actually describe the work.
6. Confirm the bullet with him before writing it into `master-resume.md`, and note the "stack used" tag line for that entry per the project's Experience/Projects format.

## Common Fixes Reference

| Weak | Strong pattern |
|---|---|
| "Responsible for managing team" | "Led team of N to [outcome], [metric]" |
| "Helped improve process" | "Streamlined [process], reducing [metric] by X%" |
| "Worked on backend features" | "Built [feature] using [stack], [quantified outcome]" |
| "Assisted with customer support" | "Resolved N+ [issue type] weekly, [satisfaction/time metric]" |
