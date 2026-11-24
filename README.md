# SEO Improvements

Private working repo for Brian's SEO program across all projects. It does two jobs:

1. **Keeps search-engine and channel rules current** (`engines/`), with a date and source on every rule.
2. **Bridges Claude and Muse.** Muse (Brian's assistant with Anthropic API access) cannot see the Claude project, so both assistants read and write files here.

## Layout

| Path | What it holds |
|---|---|
| `STRATEGY.md` | Program rules, tiers, execution sequence, open decisions |
| `CHECKLIST.md` | Master foundation checklist applied to every project |
| `engines/*.md` | One file per engine/channel: current rules, recent changes, verification status |
| `projects/*.md` | One file per project: tier, wedge channels, actions, status |
| `bridge/LOG.md` | Append-only, dated handoff log between Muse and Claude |

## How Muse and Claude use it

1. **Read first.** Before working, read `bridge/LOG.md` (newest at the bottom) and the files you plan to touch.
2. **Log every handoff.** Append an entry to `bridge/LOG.md`; never edit or delete past entries.
3. **Update the source of truth.** Rule changes go in `engines/`, project decisions in `projects/`, program changes in `STRATEGY.md`. The log points to them.
4. **Source and date everything.** Each rule carries `Verified: YYYY-MM-DD` and a source URL, or `Status: NEEDS VERIFICATION`.
5. **Small commits, clear messages.** Prefix with the author: `muse: ...` or `claude: ...`.
6. **Brian decides.** Anything that changes a project's goal or can't be undone is logged as `ASK BRIAN` and waits.

## Guardrails

No paid tools. No gray-hat tactics. Measure against money (revenue, leads, signups), not rankings alone.
