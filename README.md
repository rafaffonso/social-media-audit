# social-media-audit

A Claude skill that audits a brand's social channels against its own brand DNA and returns a prioritized report with findings and recommendations. Every recommendation traces back to something in the brand's DNA or to a gap found in the audit, so the advice fits the brand and does not read as generic best practice.

It works for your own brand, a client's or an employer's, and it runs with or without brand materials on hand.

## What it audits

Instagram, TikTok, LinkedIn, YouTube and email newsletters by default. X/Twitter is covered more lightly, and the skill adapts to whatever channels you actually run.

For each channel it checks the things that matter for that format, for example:

- **Short-form video (Instagram, TikTok):** bio clarity, visual consistency, hook strength in the first 2 to 3 seconds, content mix, saves and shares against likes.
- **LinkedIn:** headline and About section, balance between personal point of view and expertise, native formats, genuine engagement, featured section.
- **YouTube and newsletter:** thumbnail and title as one unit, opening retention, series consistency, subject line clarity, one clear call to action.

## How it works

1. **Finds the brand DNA.** It looks in the project for brand guidelines, voice and tone, positioning, messaging and similar files, and uses them as the yardstick. If there are none, it says so and offers two paths: recommendations based on industry benchmarks, or a quick read of the channels to infer the brand's essence, which you confirm before it is used.
2. **Scopes the audit.** You give it the channels and what each one is for (growth, awareness, sales, community, recruiting, thought leadership). The same channel is judged differently depending on its objective.
3. **Audits each channel** against the criteria above, using screenshots, exports, analytics or the live profiles. It does not invent numbers. Without access to real analytics, it works from what is visible and says so.
4. **Runs a cross-channel diagnostic.** Funnel balance (attract, connect, convert) against each channel's objective, consistency of voice and visual identity, health signals, optional competitive white space, and cheap operational fixes separated from strategic gaps.
5. **Delivers the report:** executive summary, the DNA and objectives used as reference, per-channel findings, the cross-channel diagnostic and recommendations split into quick wins and strategic moves.

## Install

Copy the `social-media-auditor-strategist` folder into your skills directory:

- Personal, available in every project: `~/.claude/skills/`
- One project only: `.claude/skills/` inside that project

Then ask Claude for an audit.

## Use it

```
Audit my brand's Instagram and LinkedIn against our brand guidelines.
```

```
Run a social media audit for @handle. The goal is growth on Instagram and thought leadership on LinkedIn.
```

For the best result, run it inside a folder that already holds the brand's DNA or guidelines, and bring screenshots or analytics exports if you have them.

## Files

| Path | What it holds |
| --- | --- |
| `social-media-auditor-strategist/SKILL.md` | The skill: steps, per-channel criteria and the report structure. |
