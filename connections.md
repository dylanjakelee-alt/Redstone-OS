# Connections

Registry of every system this AIOS can reach — the "second brain's" wiring out to your real stuff. The more it can reach, the more it can actually do for you instead of just talk. Filled by `/onboard` from your Q4-Q8 answers; expanded over time as you wire new tools. `/audit` checks this for coverage and freshness. **Don't worry about wiring these on Day 1** — this is just the map of what you use. New to "connection" or "MCP"? Run `/explain`.

| # | Domain | Tool | Mechanism | Auth | Last checked |
|---|---|---|---|---|---|
| 1 | Revenue / Financials | _filled by /onboard_ | not yet connected | — | — |
| 2 | Customer interactions | _filled by /onboard_ | not yet connected | — | — |
| 3 | Calendar | _filled by /onboard_ | not yet connected | — | — |
| 4 | Communication | _filled by /onboard_ | not yet connected | — | — |
| 5 | Project / task tracking | _filled by /onboard_ | not yet connected | — | — |
| 6 | Meeting intelligence | _filled by /onboard_ | not yet connected | — | — |
| 7 | Knowledge / files | _filled by /onboard_ | not yet connected | — | — |

**What each domain means:**
- **Revenue / Financials** — where money from your work lands and how you track it: a store/platform payout, Stripe, PayPal, a spreadsheet. Even if it's just starting, this is where it'll go.
- **Customer interactions** — the people who use, follow, or buy your work and where you talk with them: a community, followers, buyers, DMs.
- **Calendar** — Google Cal, Outlook, school/work calendar, deadlines, events.
- **Communication** — where you talk to people: Discord, Gmail, Outlook, Slack, DMs.
- **Project / task tracking** — where you track what you're doing: Trello, Notion, ClickUp, a to-do app, GitHub issues.
- **Meeting intelligence** — recordings and notes from calls or meetings: Fireflies, Otter, Granola, Zoom. You may not have this yet — that's fine.
- **Knowledge / files** — notes, saved tutorials, docs, project files, art/audio: Drive, Notion, Dropbox, a desktop folder.

**Mechanism options:** `mcp` (MCP server — a connector to an outside tool), `script` (a small program hitting an API, in `scripts/`), `export` (a CSV/JSON dump pipeline), `key+ref` (`.env` key + `references/{tool}-api.md` guide), `not yet connected`.

When you wire a new tool, also save `references/{tool}-api.md` with how it works (endpoints, login flow, common uses) — research it once, keep it forever.
