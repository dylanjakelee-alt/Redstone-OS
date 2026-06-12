# Connections

Registry of every system this AIOS can reach — the "second brain's" wiring out to your real stuff. The more it can reach, the more it can actually do for you instead of just talk. Filled by `/onboard` from your Q4-Q8 answers; expanded over time as you wire new tools. `/audit` checks this for coverage and freshness. **Don't worry about wiring these on Day 1** — this is just the map of what you use. New to "connection" or "MCP"? Run `/explain`.

| # | Area | Tool | Mechanism | Auth | Last checked |
|---|---|---|---|---|---|
| 1 | Communication | _filled by /onboard_ | not yet connected | — | — |
| 2 | Calendar & schedule | _filled by /onboard_ | not yet connected | — | — |
| 3 | Tasks & projects | _filled by /onboard_ | not yet connected | — | — |
| 4 | Notes & knowledge | _filled by /onboard_ | not yet connected | — | — |
| 5 | Files & assets | _filled by /onboard_ | not yet connected | — | — |
| 6 | Game project & tools | _filled by /onboard_ | not yet connected | — | — |
| 7 | Sharing, community & earning | _filled by /onboard_ | not yet connected | — | — |

**What each area means:**
- **Communication** — where you talk to people: Discord, email, DMs.
- **Calendar & schedule** — deadlines, school, events, anything time-based.
- **Tasks & projects** — where you track what you're doing (an app, Trello/Notion, a notebook).
- **Notes & knowledge** — your second brain's memory: notes, saved tutorials, references, docs.
- **Files & assets** — where files live: Drive, desktop, project files, art/audio.
- **Game project & tools** — what you build in (Godot, Unity, Unreal, code) and where it's saved (Git/GitHub).
- **Sharing, community & earning** — where you post and get feedback (YouTube, Reddit, forums) and, someday, where you'd earn (Steam, itch.io, Patreon).

**Mechanism options:** `mcp` (MCP server — a connector to an outside tool), `script` (a small program hitting an API, in `scripts/`), `export` (a CSV/JSON dump pipeline), `key+ref` (`.env` key + `references/{tool}-api.md` guide), `not yet connected`.

When you wire a new tool, also save `references/{tool}-api.md` with how it works (endpoints, login flow, common uses) — research it once, keep it forever.
