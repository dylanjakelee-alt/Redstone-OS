---
name: onboard
description: Use on Day 1 of Matthew's AIOS install, when he says "set me up", "onboard me", "let's get started", "fill in my AIOS", or has just cloned the kit. Combined wizard — runs the 10-question intake AND scaffolds the Day-1 file set at the end. Idempotent — re-run any time after editing aios-intake.md.
---

## What this skill does

Single combined wizard. Reads or writes `aios-intake.md` (the canonical intake), conducts the 10-question interview if the file isn't filled, then scaffolds the Day-1 file set inline at the end of the run. No separate `/scaffold-from-intake` skill — this is one flow.

This AIOS belongs to **Matthew** — an aspiring game developer who's newer to AI. Keep the tone warm and plain. Define any jargon the moment it comes up, and if he seems lost, point him at `/explain` or `/start-here`. He already has a name; greet him by it and don't ask "who are you" as a name question — Q1 is about what he makes, not what he's called.

**The wow moment:** at the end, suggest the closing prompt *"Try this — ask me: what should I work on in my project this week?"* He runs it once. That's the wow. There's no `/today` skill to save — the prompt itself plants the Mindset framework (Default Shift) for him to internalize, pointed at his project instead of a business.

## When NOT to run this

- If the user has already onboarded and wants to refresh: still run, but skip questions already answered (idempotent).
- If the user wants to add a new connection: that's not onboarding — point them at `connections.md` to edit directly, or schedule a `/level-up` Phase 2 walk.

## Execution

### Step 1: Read the intake

Read `aios-intake.md`. Check which Q1-Q10 sections have content vs. `[Your answer here]` placeholders.

- **All filled** → skip Step 2, jump to Step 3 (scaffold).
- **Some filled** → ask Matthew: "I see Q1, Q3, Q8 are answered. Want to fill the rest now, or set up from what's there?" His call.
- **None filled (fresh clone)** → run Step 2 conversationally.

### Step 2: The interview (10 questions)

Ask one at a time, in plain language. Write each answer into `aios-intake.md` as you go (so he can resume if interrupted). If an answer is vague, gently push for something concrete — but never make it feel like a test. If he doesn't know a term, explain it on the spot.

**Q1 — Who are you, what do you make (or want to make), and who's it for?**
Identity, what he creates/wants to create, audience. A sentence or two each.

**Q2 — Paste 1-2 things you've written recently. Don't edit them.**
*This is the only question with a hard rule, and it cannot be skipped* — it's how the AIOS learns to sound like him. Voice samples MUST be pasted, not typed mid-conversation. Accept anything real: a text message, a Discord message, a post, a devlog, a comment, even a message he sent to another AI. If he starts typing fresh prose, refuse:

> *"Hold on — paste it raw. If you type it here while we're talking, it's already shaped by our chat, and I'll learn the wrong voice. Grab a real text, Discord message, post, or comment and paste it exactly as you sent it. This is the one rule I can't bend — and I do need it, so don't skip it."*

Also offer the shortcut: *"If you've used another AI chatbot or agent before, ask it 'describe who I am, in as much detail as you can' and paste its answer here too — the more it knows about you, the better I'll know you."* Encourage him to be exhaustive. Ask for at least two samples.

**Q3 — What are your 2-3 biggest goals for the next 90 days?**
Concrete ~3-month targets. Push gently if vague ("get good at game dev") — help him name something shippable: "finish a playable level," "release a tiny game," "post 3 devlogs."

**Q4 — Do you want to earn from your work someday, and how?**
"Not yet" is a fine answer. If yes: how (selling games, YouTube, commissions, donations) and where money would land (Steam/itch.io, a payout account). Aspirational is fine. Map to the Money/earning domain in `connections.md`.

**Q5 — Where do you share your work and talk to people day-to-day?**
Discord, YouTube, Reddit, forums, friends, DMs, email. Map to the Sharing & community + Communication domains.

**Q6 — Where do your notes, tutorials, references, and project files live?**
Desktop folder, Drive, Notion, notebook, saved videos. Map to the Knowledge & files domain. "Kind of everywhere" is a real and useful answer.

**Q7 — What's the one thing that slows you down most, and where do you track what you're working on?**
Capture top_pain (used later by `/level-up`) + where he tracks tasks (Task tracking domain).

**Q8 — What are you making right now, and what are you building it with?**
Current project(s), engine/tools/languages (Godot, Unity, Unreal, Scratch, GameMaker, code), solo or with others. This is the heart of his AIOS — get it specific.

**Q9 — How do you best stay motivated and on track?**
This is about *how he works*, not what he wants (that's Q3). What keeps him moving (deadlines, small wins, check-ins, streaks) and what makes him stall or lose interest. *This drives how the AIOS pushes him — it's the most important question for keeping him going, so capture it carefully.*

**Q10 — How do you learn best?**
Plain terms / redstone terms / both, plus any other games or hobbies to use as analogies. *This sets the teaching style for `/explain` and everyday explanations.*

### Step 3: Scaffold the Day-1 file set

Once the intake is complete, generate these files (or update if re-running). Back up originals to `archives/intake-{YYYY-MM-DD-HHMM}/` if any exist.

1. **`context/about-me.md`** — from Q1 (who he is) + Q7 (what slows him down). One short paragraph each.
2. **`context/about-craft.md`** — from Q8 (current project, engine/tools, solo/team) + Q4 (whether/how he wants to earn). What he's building, not a business.
3. **`context/priorities.md`** — from Q3. Numbered list, one line per goal — his concrete near-term targets.
4. **`context/goals.md`** — from Q9. A short "How to keep me moving" profile: what motivates him, what stalls him, the working style that keeps him on track. The AIOS reads this to push him the right way. (His concrete targets live in `priorities.md`; this file is about *how* he works, not *what* he wants.)
5. **`references/voice.md`** — from Q2. Paste samples verbatim with a short header ("Match this register when drafting; don't fake his voice on anything public — Discord post, video script, comment — without showing him first").
6. **`connections.md`** — populate the creator-themed table from Q4-Q8 answers. Each row gets `mechanism: not yet connected`, `auth: —`, `last checked: —`. He wires connections later.
7. **`CLAUDE.md`** — fill all `{{...}}` placeholders. Substitute his name (Matthew), stated goal, voice register summary, a brief connections summary, AND record his Q10 learning preference into the teaching cues (e.g. "Matthew likes redstone analogies — offer them" or "keep it plain"). Preserve the teaching + momentum sections already in the template.

### Step 4: The closing screen

Print one screen. Three lines max:

```
✓ Day 1 done. Your AIOS knows who you are, what you're building, what you're aiming for, how you learn, and how you sound.

Today: ask me — "what should I work on in my project this week?"
This week: try /explain on anything that's fuzzy, and pick one thing from connections.md to set up.
Day 7: run /audit to see how your setup scores.
```

When Matthew runs the closing prompt ("what should I work on in my project this week?"), respond using only the new context files. Hit:
- 3-bullet next-steps list for his actual project, in his voice register from Q2
- **If he has no project yet** (Q8 was "just starting" / "want to learn X"): pivot to proposing one tiny starter project scoped to his tools and level — something finishable in a week or two — and make *that* the week's focus. Starting beats planning.
- Each bullet ties back to a stated goal from Q3, motivating the way Q9 says he likes (small wins? a deadline? a nudge?)
- Final line: *"If I had to pick one thing to do first, it'd be [X], because [reason from his goals]. Want me to break it into steps? And — where could AI actually help on this, instead of doing it all by hand?"*

The closing question seeds the Mindset framework (Default Shift) before `/level-up` formally introduces it — pointed at his project, not a business.

## Critical implementation rules

1. **Keep it to the 10 questions.** Don't improvise an 11th mid-conversation — if more comes up, it goes in `context/` later, not the intake.
2. **Voice paste cannot be skipped.** If Matthew types samples mid-chat, refuse and tell him to paste from real writing (a Discord message, devlog, post).
3. **One-shot scaffold.** After Step 2 ends, write Step 3 files in a single batch. No multi-turn confirmation. He iterates by editing `aios-intake.md` and re-running.
4. **Idempotent.** Re-running with an edited intake refreshes context files; backs up originals to `archives/intake-{ts}/`. Skips questions already answered unless he wants to revise.
5. **Closing screen is three lines.** Not a menu.
6. **Don't generate new skills here.** The kit ships its skills (`onboard`, `audit`, `level-up`, `explain`, `start-here`); Matthew authors more via `/level-up`. Onboard only writes the Day-1 context/reference files.
7. **Read-only on `references/3ms-framework.md` and `references/redstone-model.md`.** They already ship in the kit. Don't overwrite.
8. **No `.env` writes.** Don't ask for API keys on Day 1. Connections come later.
9. **Beginner-safe.** Matthew is newer to AI. Define terms as they come up; if he's lost, point to `/explain` or `/start-here`. Never make onboarding feel like a quiz.

## Verification (for the implementer)

- Cold-test: clone a fresh kit, run `/onboard`, fill 10 answers, scaffold runs, ask the wow prompt, response cites his project (Q8) + a goal (Q3/Q9) specifically and motivates per Q9. Generic = fail.
- Idempotency: re-run `/onboard` with one Q3 goal changed. Expected: only `context/priorities.md` and `CLAUDE.md`'s goal section update; backup created in `archives/intake-{ts}/`.
- Voice rejection: type a sample mid-chat. Expected: skill refuses, asks for paste.
- Learning pref: confirm Q10's answer landed in `CLAUDE.md`'s teaching cues (redstone analogies on/off).

> *Adapted from The Three Ms of AI™ © 2026 Nate Herk. The Mindset language used in the closing screen comes from `references/3ms-framework.md`.*
