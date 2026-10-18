# Getting started with Abacus AI Agent

An interactive, self-contained guide to Abacus AI Agent — from "I just signed up" to running real, recurring work.

**Read it live:** https://difaze3.github.io/abacus-getting-started-guide/

Or open `index.html` in any browser. No build step, no dependencies, works offline.

---

## What's inside

Twelve sections, in reading order:

| # | Section | Why it's there |
|---|---|---|
| 1 | The mental model | Six ideas that explain most of the agent's behaviour |
| 2 | First-time setup | ~15 min of groundwork |
| 3 | Anatomy of a good request | The five ingredients, with a live builder |
| 4 | First project, step by step | A worked Monday-status-report example |
| 5 | Connectors | What to connect, and what *not* to |
| 6 | Routines & automation | Turning one-off tasks into scheduled work |
| 7 | Skills | Reusable procedures so you stop repeating yourself |
| 8 | Documents, decks, designs | How to brief an artifact well |
| 9 | Working with code | Habits that matter more than capability |
| 10 | Credits & plans | What costs what, plus plan options |
| 11 | Troubleshooting | Symptom → cause → fix table |
| 12 | Launch checklist | Tick off over your first week |

### The three things worth remembering

1. **Ask for outcomes, not procedures** — name the goal, sources, constraints, format and audience.
2. **Do it once → correct it → freeze the format → schedule it.** That's the whole path to automation.
3. **Ask for a plan before any big job.** A wrong plan costs a fraction of wrong work.

## Interactive features

- **Request builder** (§3) — toggle the five ingredients and watch a real prompt assemble itself
- **Flip cards** (§1) — expandable "in practice" notes on each mental-model idea
- **Persistent checklist** (§12) — saved to `localStorage`, with progress bar and a 100% celebration
- **Scroll progress**, **TOC section tracking**, **typewriter hero**, **back-to-top**
- Fully honours `prefers-reduced-motion`; prints cleanly to PDF

## Files

| File | What it is |
|---|---|
| `index.html` | The entire guide — markup, styles and script in one file |
| `CHAT-TRANSCRIPT.md` | The conversation that produced it, including the reasoning |

## Running locally

```bash
git clone https://github.com/difaze3/abacus-getting-started-guide.git
cd abacus-getting-started-guide
# just open index.html — or serve it:
python -m http.server 8000
```

## Notes

- Prices and credit figures in §10 reflect the account at the time of writing. Everything else is durable practice.
- Built as a single HTML file on purpose: it survives being emailed, printed, committed, or opened in ten years.
