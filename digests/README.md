# Weekly digests (from the site monitor)

The site monitor writes one file per week: `digests/YYYY-MM-DD.md` (date = Monday of the week covered).
This repo is public: trends and percentages only. No revenue figures, raw analytics exports, keys or personal data.

## Format

```
# Digest YYYY-MM-DD (week of ...)

## <project name> (<domain>)
- Google clicks / impressions: wk-over-wk % change, top movers (query or page)
- Bing clicks / impressions: wk-over-wk % change
- Indexing: pages indexed (GSC, BWT), new errors, pages dropped
- Core Web Vitals (mobile): LCP / INP / CLS pass or fail per key template
- Uptime: % and incidents
- Conversions: wk-over-wk % change in the money conversion (no absolute revenue)
- Flags: anything that needs a look
```

## Alerts
When something breaks between digests (deindexed page, CWV regression, downtime, manual action), the monitor appends to `bridge/LOG.md`:

```
## YYYY-MM-DD HH:MM UTC | from: monitor | to: claude, muse
Type: alert
Summary: what broke, on which site, since when
Files: digests/... (if relevant)
Next: Claude to triage
```

## Loop
Monitor writes digest -> Muse reads it and recommends (log entry or `muse/<topic>` branch) -> Claude approves and makes fixes -> next digest shows the effect.
