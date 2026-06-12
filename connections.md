# Connections

Registry of every system this AIOS can reach. Filled by `/onboard` from your Q4-Q8 answers; expanded over time as you wire new tools. `/audit` checks this file for coverage and freshness. **Don't worry about wiring these up on Day 1** — this is just the map of what you use. New to the word "connection" or "MCP"? Run `/explain`.

| # | Area | Tool | Mechanism | Auth | Last checked |
|---|---|---|---|---|---|
| 1 | Game project & engine | _filled by /onboard_ | not yet connected | — | — |
| 2 | Version control & backups | _filled by /onboard_ | not yet connected | — | — |
| 3 | Sharing & community | _filled by /onboard_ | not yet connected | — | — |
| 4 | Communication | _filled by /onboard_ | not yet connected | — | — |
| 5 | Task / project tracking | _filled by /onboard_ | not yet connected | — | — |
| 6 | Knowledge & learning | _filled by /onboard_ | not yet connected | — | — |
| 7 | Money / earning (someday) | _filled by /onboard_ | not yet connected | — | — |

**What each area means:**
- **Game project & engine** — what you build in (Godot, Unity, Unreal, Scratch, GameMaker, code).
- **Version control & backups** — where your work is saved so you never lose it (Git/GitHub, a cloud folder).
- **Sharing & community** — where you post and get feedback (Discord, YouTube, Reddit, forums).
- **Communication** — email and DMs.
- **Task / project tracking** — where you keep your to-dos (an app, Trello/Notion, a notebook).
- **Knowledge & learning** — where your notes, tutorials, and references live.
- **Money / earning** — if/when you sell or monetize (Steam, itch.io, a payout account). "Not yet" is fine.

**Mechanism options:** `mcp` (MCP server — a connector to an outside tool), `script` (a small program hitting an API, in `scripts/`), `export` (a CSV/JSON dump pipeline), `key+ref` (`.env` key + `references/{tool}-api.md` guide), `not yet connected`.

When you wire a new tool, also save `references/{tool}-api.md` with how it works (endpoints, login flow, common uses) — research it once, keep it forever.
