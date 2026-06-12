# Redstone OS — Matthew's AI Operating System

> **What this is, in one line:** a free, MIT-licensed starter kit (**AIS-OS** by Nate Herk), **enhanced and customized by Jake** into an AIOS that adapts to whatever you do and evolves with you — set up for **Matthew** to start.

It's not an AI course and it's not a niche tool. It's a personal **AI Operating System**: a second brain that learns who you are and what you're working on, then helps you think, decide, remember, and ship — and gets sharper the more it knows you. Three layers, so nothing's confusing:

1. **The base kit — AIS-OS (free, MIT, by Nate Herk).** Turns Claude Code into a personal AIOS. Built for a general audience and pairs with a companion masterclass video. The license and the core frameworks (the Three Ms, the Four Cs) are Nate's and stay credited below.
2. **Jake's enhancements.** Jake made it *adaptive and personal*: onboarding discovers your niche (whatever it is) and the system evolves with you instead of going stale. He also added a teaching layer for when AI is new — a `/start-here` tour, an `/explain` skill (plain-English, with optional analogies), and an `ai-basics.md` primer — available *when needed*, not the point.
3. **Set up for Matthew.** This copy starts personalized for Matthew, who's into game dev and newer to AI. But nothing is hardcoded to games — onboarding adapts to whoever fills it out. A musician, writer, or founder who onboarded would get *their* world, pushed forward in *their* niche.

The kit personalizes itself via the `/onboard` interview, gives you a `/start-here` tour and an `/explain` skill for when AI is new, then two recurring thinking skills (`/audit`, `/level-up`) to keep building leverage week over week.

> **AIS-OS** stands for **AI Automation Society OS** — the way Nate designed the original kit for members of his community, [AI Automation Society](https://www.skool.com/ai-automation-society). The base kit is universal; this copy is Jake's adaptive build, set up for Matthew to start.

---

## The litmus test

> **"While you're not at your desk, your AIS-OS observes one real-world event and produces an output that's faster and more accurate than what you'd produce yourself."**

Every design decision in this kit rolls up to that test. If a layer, skill, or template doesn't contribute to it, it doesn't ship.

---

## How you'll know it's working

Three felt **success indicators** tell you the AIOS is actually changing how you work. Not KPIs — there's no objective metric. These are lived experiences that show up in your week.

**1. Team-reaches-out:**

> *"A teammate messages you with a question. You realize your AIOS would answer it better, faster, and with exact sources — even if you were awake and free. So you ask your AIOS too. That's the moment you stop being a bottleneck for your own knowledge."*

**2. Context-switching reduction:**

> *"You stop opening new tabs. You stop launching the desktop app. When something new lands, your first move is to ask the AIOS, not to open six things. The default surface for thought work shifts. Silent. Compounding."*

**3. Knowledge-leaves-your-head:**

> *"You stop trying to remember business facts. You don't rehearse what you decided last quarter or what your customer said in that meeting. You trust the retrieval. The AIOS holds the truth, you hold the questions."*

**Personal foundation → company AI-readiness.** Once these indicators show up for one person, the same data architecture powers everything else. Custom dashboards on the data you already collect. Automations on top of the connections you already wired. Team rollout where everyone has theirs. *A company where every operator runs a personal AIOS is a company that's actually AI-ready.*

The kit teaches personal AIOS first. Everything scales from there.

---

## Two frameworks

The kit teaches two complementary frameworks. **Three Ms first, Four Cs second.** Without the brain rewire, the architecture is just a folder structure.

### The Three Ms — operator brain (how you think)

| M | One-liner |
|---|---|
| **Mindset** | Default Shift, Function Breakdown, Curiosity Rule. *To what extent can AI be leveraged here?* |
| **Method** | Find Constraint → EAD (Eliminate, Automate, Delegate) → Map Process → Pick Autonomy Level → Tie to KPI. |
| **Machine** | Lego Principle, Validation Chain, Bike Method, Intern Rule, Kill Switch. *Boring is beautiful. Workflows beat agents.* |

Full breakdown in `references/3ms-framework.md`. The `/level-up` skill walks you through all three weekly.

> *The Three Ms of AI™ is a trademark of Nate Herk. © 2026 Nate Herk.*

### The Four Cs — architecture (what you build)

| # | Layer | One-liner | "This layer is in place" test |
|---|---|---|---|
| 1 | **Context** | Knows you and your work | Fresh Claude session answers "who is this person and what are they building?" without browsing |
| 2 | **Connections** | Reaches your stuff | "What's on my calendar tomorrow and what tasks are due?" → live data, no paste |
| 3 | **Capabilities** | Knows how to do the work | A short phrase triggers a multi-step workflow that produces an artifact |
| 4 | **Cadence** | Runs without being asked | Laptop closed. A brief lands in the inbox. A teammate messages it and gets a real answer |

**Brand line:** Context. Connections. Capabilities. Cadence.

> *The Four Cs of an AIOS™ is a trademark of Nate Herk. © 2026 Nate Herk.*

Dependency graph: Context is non-skippable. Connections + Capabilities can build in parallel. Cadence is last — don't automate workflows that don't work manually.

---

## What ships — 6 skills

The kit is intentionally lean. Skills here are thinking tools and teaching tools, not heavy automations. You hack on top of the structure.

| Skill | Type | When to run |
|---|---|---|
| `/start-here` | Guided tour (first session) | Your very first session. A slow, one-step-at-a-time walkthrough of the whole setup. |
| `/onboard` | Setup wizard (one-time) | Day 1, immediately after the tour. 10-question interview. Generates Day-1 file set + fills `CLAUDE.md`. |
| `/explain` | Teaching skill (anytime) | The moment any word or concept is fuzzy — AI, your field, or this kit. Plain-English, optionally in analogies you pick. |
| `/grill-me` | Capture skill (anytime) | When you want to stress-test a plan or get a fuzzy idea out of your head — relentless interview, saved to `brainstorms/`. |
| `/audit` | Recurring thinking skill | Day 7, then weekly. Four-Cs gap report. Read-only. Watch the score climb. |
| `/level-up` | Recurring thinking skill | Day 14, then weekly. Three Ms interview (Mindset → Method → Machine). One run = one shipped artifact. |

`/audit` asks *"is the AIOS built right?"* (form). `/level-up` asks *"what leverage am I missing?"* (function). They work in series — fix structure first, then capability planning becomes meaningful.

---

## Quick start

1. **Clone the repo** to a working folder on your machine.
2. **Open it in Claude Code** and run `/start-here`. It walks you through everything, including running `/onboard` (10 questions, ~15 min, voice samples pasted not described). New to AI? It points you at `references/ai-basics.md` first.
3. **Use it for a week.** Bring real questions about your project. Make real decisions. Log them in `decisions/log.md`. Hit a word you don't know? `/explain` it.
4. **Day 7:** run `/audit`. Read the Four-Cs gap report. Pick one gap to close.
5. **Day 14:** run `/level-up`. The Three Ms interview surfaces one thing worth automating. Build it.
6. **Week 3+:** weekly `/level-up` ritual. One shipped artifact per week.

---

## Repo layout

```
Redstone OS/
├── README.md
├── CLAUDE.md                        ← Your operating manual (filled by /onboard)
├── EXPANSIONS.md                    ← What to add as you grow
├── LICENSE
├── .gitignore
├── aios-intake.md                   ← Source-of-truth for /onboard. Edit + re-run any time.
├── connections.md                   ← Registry of every system your AIOS can reach
├── context/                         ← About you, your craft, your goals (filled by /onboard)
├── references/
│   ├── 3ms-framework.md             ← The operator brain
│   ├── ai-basics.md                 ← Plain-English AI primer (start here if AI is new)
│   └── redstone-model.md            ← Source for redstone analogies
├── decisions/
│   └── log.md                       ← Append-only record of what was decided and why
├── brainstorms/                     ← Captured /grill-me sessions (one file per session)
├── Projects/                        ← One folder per project
├── To-dos/                          ← Active task lists and next actions
├── archives/                        ← Old stuff. Don't delete. Move here.
└── .claude/
    └── skills/
        ├── start-here/SKILL.md
        ├── onboard/SKILL.md
        ├── explain/SKILL.md
        ├── grill-me/SKILL.md
        ├── audit/SKILL.md
        └── level-up/SKILL.md
```

See `EXPANSIONS.md` for what to add as you grow (`templates/`, `scripts/`, `.claude/agents/`, sub-OS folders, etc.).

---

## License + attribution

**Base kit:** MIT License. © 2026 Nate Herk. The Three Ms of AI™ and The Four Cs of an AIOS™ are trademarks of Nate Herk. Both frameworks ship in this repo with attribution. Use freely; don't repackage as your own.

**This version:** enhanced and customized by Jake for Matthew — the teaching layer (`/start-here`, `/explain`, `ai-basics.md`, `redstone-model.md`), the game-dev theming, and the added onboarding questions are additions on top of Nate's base kit. The MIT license still applies; Nate's frameworks and trademarks remain his and stay credited above.

The companion masterclass video walks you through the base kit step by step. Link will land here once it ships.
