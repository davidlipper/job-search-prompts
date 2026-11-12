# Job Search Prompts

The prompt system behind an AI-agent-run job search for a senior IT project/program manager: scheduled sweeps, a morning briefing, and rapid between-sweep checks, all run by a personal AI agent against a single set of criteria.

**This is a sanitized public copy.** Personal details (name, hometown, contact info, and similar) and compensation figures have been removed or generalized. The logic, criteria, and verification rules are unchanged.

## How it runs

| Prompt | Schedule |
|---|---|
| [Morning sweep](morning-sweep.md) | Daily, 7:00 AM ET |
| [Morning briefing](morning-briefing.md) | Daily, 7:15 AM ET |
| [Afternoon sweep](afternoon-sweep.md) | Daily, 3:00 PM ET |
| [Dice check](dice-check.md) | Daily, 7 AM / 12 PM / 7 PM ET |
| [Monday pipeline review](monday-pipeline-review.md) | Mondays, ~9:48 AM ET |
| [Dice profile daily touch](dice-profile-daily-touch.md) | Daily, ~10:48 AM ET |

## Current criteria (Nov 2026)

- Remote-first; hybrid only within defined NJ commute corridors
- Full-time or W2 contract only — no 1099/C2C
- Compensation thresholds are intentionally omitted from this public copy.
- Travel up to 25%
- AI-related PM roles are the priority track

## Design principles

- **Verify before reporting:** every job link is opened in a live rendered browser; a posting counts only with details visible, no expired/closed banner, a working Apply path, and a visible posted date. Search snippets and text-only fetches never count.
- **Freshness guard:** aggregator dates are treated as untrustworthy (reposts refresh them); the original posting date on the employer's own careers page decides the 30-day staleness test.
- **Per-job recruiter capture:** every lead carries its listing recruiter — named on the posting, pattern-inferred and marked unverified, or "not named." Never invented.
- **WARN cross-check:** every company behind a qualifying lead is checked against US WARN layoff lists; flags are reported, never used to silently drop a lead.
- **Deduped pipeline:** all runs share one seen-leads ledger so nothing is reported twice.
- **Human keeps the submit button:** the agent sources, screens, and tracks; applying and anything sent under the candidate's name stays with the human.
