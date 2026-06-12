# AI Basics (start here if AI is new)

> For Matthew. Plain-English on purpose. The **redstone callouts** (marked 🟥) are optional — skip them if you've moved past Minecraft and the rest still makes complete sense. Anything fuzzy? Run `/explain`.

## What is an AI like me?

I'm a **large language model** (LLM). That's a program trained on a huge amount of text until it got very good at one thing: predicting what words should come next. That sounds simple, but doing it well means I picked up patterns for explaining, coding, planning, and reasoning along the way.

I'm not a search engine and I'm not a person. I don't "know" facts the way a database does — I generate a likely answer. That's why I'm powerful *and* why I sometimes get things confidently wrong (see "hallucination" below).

> 🟥 **Redstone version:** think of me as a giant, very well-tuned contraption. You send a signal in (your message), it propagates through a massive network, and a result comes out. The output depends entirely on what you put in and how it's wired.

## The words you'll hear most

**Prompt** — what you send me. Your question or instruction. Better prompt in, better answer out.
> 🟥 A prompt is the **signal / button press** that kicks the whole machine off.

**Token** — the chunks of text I read and write in (roughly words or word-parts). I count everything in tokens.
> 🟥 One token ≈ one block of redstone dust in a line: it carries the signal one step.

**Context** — everything I can "see" right now: this conversation, the files in this project, what you just said. I have a limited amount of it.
> 🟥 Context is a **memory cell (RS latch)** — it holds state so the system remembers between steps. And like a dust line that fades after 15 blocks, context has a hard limit. Fill it with junk and the important signal gets lost.

**Hallucination** — when I state something wrong as if it's true. It happens because I generate likely-sounding text, not guaranteed facts. Always sanity-check anything important (a price, an API, a command).

**Model** — the specific "brain" doing the work. Different models are different sizes and strengths. Newer/bigger usually means smarter but slower.

**Agent** — me, but running a multi-step job mostly on my own: I plan, take steps, check results, and keep going.
> 🟥 An agent is an **automated contraption** — wired once, then it runs its sequence on its own when triggered.

**MCP** — a connector that lets me reach an outside tool (your Drive, a calendar, etc.). You'll meet these later when you wire up `connections.md`. Don't worry about it yet.

## How to get good answers out of me

This is the real skill, and it's learnable fast:

1. **Say what you actually want.** "Help me" is weak. "Help me figure out why this isn't working — here's what I tried and what happened" is strong.
2. **Give me context.** What engine, what you tried, what happened. I can only work with what I can see.
3. **Lead with the most important thing.** Don't bury it under five sentences of setup.
4. **Ask for the *why*, not just the fix.** "Explain why that works" is how you actually level up — and it's how this whole AIOS is built to treat you.
5. **Iterate.** First answer not right? Tell me what's off. It's a conversation, not a vending machine.

> 🟥 Prompting well is like clean redstone: a sloppy pile of dust *might* work, but a build with repeaters and clear structure is reliable and easy to debug. Structure your ask, get a clean result.

## What I'm good at vs. what to watch for

**Good at:** explaining concepts, drafting and rewriting text, planning a project into steps, debugging code with you, brainstorming, summarizing, teaching.

**Watch for:** confidently wrong facts (verify the important ones), anything needing *current* live info I can't see, and very large/complex tasks (break them into smaller pieces — exactly like wiring one redstone module at a time).

## What an "AIOS" even is

This whole folder is your **AI Operating System** — a setup that makes me genuinely *yours*. The `context/` files tell me who you are and what you're building. The skills (`/explain`, `/level-up`, etc.) are saved abilities. `connections.md` is the list of your tools I can reach.

> 🟥 The AIOS is your **base / control room**: context files are your memory cells, skills are your saved builds, connections are the wiring out to the rest of your world. You're not building one contraption — you're building the workshop.

The point: the more you tell it about you (run `/onboard`), the more useful I get. Start with `/start-here` if you haven't.
