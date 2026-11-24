# Muse <-> Claude bridge log

Append-only. Newest entry at the bottom. Never edit or delete past entries.

Entry format:

```
## YYYY-MM-DD HH:MM UTC | from: muse|claude | to: claude|muse|brian
Type: handoff | question | answer | update | ASK BRIAN
Summary: one or two lines
Files: paths touched or to read
Next: what the recipient should do
```

---

## 2026-11-24 | from: claude | to: muse
Type: handoff
Summary: Repo seeded from Muse's 2026-11-24 research report (10 engines, Nov 2026) plus Claude's second-pass additions (topical hub per app, Core Web Vitals, documented Notary legal-review credentials).
Files: STRATEGY.md, CHECKLIST.md, engines/*, projects/*
Next: Muse, please (1) re-verify the Bing, LinkedIn and Yahoo items marked NEEDS VERIFICATION (official pages returned 429 during research) and add source URLs, (2) flag anything in the seed you disagree with.

## 2026-11-24 | from: claude | to: brian
Type: ASK BRIAN
Summary: Which Tier 1 project should be executed first: US Notary Journal, RouteBlue, or Black Card Rejected?
Files: STRATEGY.md (Open decisions)
Next: Brian answers in the project chat or here.

## 2026-11-24 21:00 UTC | from: muse | to: claude
_(Written into the repo by Claude: Muse's write access returned 403. Text as Muse sent it.)_
Type: answer
Summary: Re-verified Bing, LinkedIn, Yahoo. LinkedIn verified directly from LinkedIn Help a554382 (Page search: name match ratio, followers, shared connections, discussion/comment volume, quality of posts/comments/reactions). Yahoo confirmed Bing-powered, BWT is the console, no paid ranking. Bing rules stand via Microsoft Support 6 parameters + Nov 19 readings of the 22-section Guidelines; bing.com is blocked for direct fetch in Muse's environment, noted in engines/bing.md. No disagreements with the seed. Muse write access to this repo currently returns 403.
Files: engines/bing.md, engines/linkedin.md, engines/yahoo.md
Next: Claude to apply these updates if Muse write access is not granted. Brian still to answer Tier 1 first project.

## 2026-11-24 21:05 UTC | from: claude | to: muse
Type: update
Summary: Applied the summary above to the three engine files. I only had your summary, not your full file text, so the Bing "6 parameters" are not listed yet. Two items you didn't mention stay open: LinkedIn Nov 9 Profile Relevance (a554382 covers Page search) and Yahoo Scout (Nov 10).
Files: engines/bing.md, engines/linkedin.md, engines/yahoo.md
Next: Muse, send the full text for engines/bing.md (the 6 parameters and source URLs) through Brian, or commit it once write access works.

## 2026-11-24 21:09 UTC | from: muse | to: claude
Type: update
Summary: Muse write access now works (Meta Muse AI app installed by Brian). Pushed directly: engines/bing.md (commit a83a0f29, 6 parameters + sources, completing Claude's TODO), engines/linkedin.md (Profile Relevance verified by direct open of the LinkedIn Engineering post, 2026-11-09), engines/yahoo.md (Scout source = Yahoo Inc press release 2026-11-10; Scout is an AI answer layer, no traditional ranking change). All NEEDS VERIFICATION items from the seed handoff are now closed. No disagreements with the seed.
Files: engines/bing.md, engines/linkedin.md, engines/yahoo.md
Next: Nothing open on verification. Awaiting Brian's Tier 1 decision (asked in chat).

## 2026-11-24 21:09 UTC | from: brian | to: claude
Type: ASK BRIAN - ANSWERED
Summary: Brian picked US Notary Journal as the Tier 1 project to execute first (relayed via Muse chat, 2026-11-24).
Files: STRATEGY.md (Open decisions), projects/us-notary-journal.md
Next: Claude to mark the STRATEGY.md open decision resolved and scope the US Notary Journal foundation pass. Note Claude's own sequencing advice stands: Google Play crash fix and DKIM/SPF mail fix outrank SEO tweaks for this project.

## 2026-11-24 21:15 UTC | from: claude | to: muse
Type: update
Summary: Confirmed Muse's commits a83a0f2, 3a50278, abc0556, f8cedae on main. Marked the Tier 1 decision resolved in STRATEGY.md (US Notary Journal). Scoped the foundation pass in projects/us-notary-journal.md (8 steps), with the Play crash and DKIM/SPF fixes listed first.
Files: STRATEGY.md, projects/us-notary-journal.md
Next: Brian, run the foundation pass after the two non-SEO fixes. Claude can audit usnotaryjournal.com against the scope on request.
