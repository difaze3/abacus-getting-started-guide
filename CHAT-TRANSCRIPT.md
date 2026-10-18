# Chat transcript — Getting started with Abacus AI Agent

**Saved:** 2026-10-18 23:32 UTC
**Thread ID:** 25f6a34d-00c0-4a93-a410-839d5257c623
**Messages:** 58

---

## 👤 You

Hello, im new to Abacus Ai agneting, can you give me a structured guide made on a website that i might follow

## 🤖 AbacusAI Bot

I'll build you a structured onboarding guide as a website. Let me check a couple of things first so the guide matches what's actually available in your account.

## 🤖 AbacusAI Bot

That first call was a mistake on my part — please ignore the GitHub link, you don't need it for this.

Let me build you the guide page now.

## 🤖 AbacusAI Bot

Here's your guide — it should be open in the preview pane now: **http://127.0.0.1:55259**

**What's in it (12 sections, in the order you should read them):**

| # | Section | Why it's there |
|---|---|---|
| 1 | The mental model | Six ideas that explain most of the agent's behaviour |
| 2 | First-time setup | ~15 min of groundwork |
| 3 | Anatomy of a good request | The five ingredients, with weak/strong examples |
| 4 | First project, step by step | A worked Monday-status-report example |
| 5 | Connectors | What to connect, and what *not* to |
| 6 | Routines & automation | Turning one-off tasks into scheduled work |
| 7 | Skills | Reusable procedures so you stop repeating yourself |
| 8 | Documents, decks, designs | How to brief an artifact well |
| 9 | Working with code | Habits that matter more than capability |
| 10 | Credits & plans | What costs what, plus your current plan options |
| 11 | Troubleshooting | Symptom → cause → fix table |
| 12 | Launch checklist | Tick off over your first week |

**The three things worth remembering if you read nothing else:**
1. **Ask for outcomes, not procedures** — name the goal, sources, constraints, format and audience. That's section 3.
2. **Do it once → correct it → freeze the format → schedule it.** That's the whole path to automation.
3. **Ask for a plan before any big job.** A wrong plan costs a fraction of wrong work.

Some notes on what I built: it's a single self-contained HTML file (no external dependencies), with a sticky sidebar for navigation, and it prints cleanly to PDF from your browser if you'd like a paper copy. The source file is linked above if you want me to change anything — add sections, cut it down to a one-pager, or rework it for a specific use case like email triage or coding.

Want me to add a section on a specific workflow you have in mind?

## 👤 You

The better the web is if you utilize javascript to make it more lively

## 🤖 AbacusAI Bot

Now let me add the CSS for the new interactive elements.

## 🤖 AbacusAI Bot

Now the markup changes:

## 🤖 AbacusAI Bot

Now the reveal classes and the interactive mental-model cards:

## 🤖 AbacusAI Bot

Now the interactive request-builder in section 3:

## 🤖 AbacusAI Bot

Now the checklist markup and the JavaScript:

## 🤖 AbacusAI Bot

You're right — it was static. Reload **http://127.0.0.1:55259** and it's now a real interactive page.

**What the JavaScript does now:**

| Feature | What you'll see |
|---|---|
| **Request builder** (§3) | Five toggleable ingredient chips. Each one you add appends real text to a live prompt preview; the verdict line goes from *"very vague"* → *"strong — this is the target"*. It's the section's point demonstrated rather than described. |
| **Flip cards** (§1) | All six mental-model cards are click/Enter/keyboard-accessible. Each expands to an "In practice" line that was cut for brevity before. |
| **Checklist that remembers** (§12) | Real checkboxes with animated ticks, a progress bar and percentage, saved to `localStorage` so they survive a reload. Reset button included. Hit 100% and confetti fires. |
| **Scroll progress bar** | Gradient bar pinned to the top, tracks read depth. |
| **TOC section tracking** | The sidebar now highlights whichever section you're actually reading. |
| **Hero** | Typewriter on "Abacus AI Agent", plus three action buttons: jump to step 1, jump to checklist, save as PDF. |
| **Back to top** | Appears after you've scrolled a screen; smooth-scrolls home. |

**Accessibility and restraint, deliberately:**
- The whole thing is inside `prefers-reduced-motion`: typewriter, reveals, smooth scroll and confetti all switch off and content renders statically instead.
- Cards are `tabindex="0"` with `aria-expanded`; chips use `aria-pressed`; checkboxes keep a visible focus ring and a JS-set `.done` class so it works in browsers without `:has()`.
- Print stylesheet hides the progress bar, back-to-top, confetti and CTA buttons, and forces every revealed section visible — so **Save as PDF** still gives you a clean document.

Press that **Save as PDF** button in the hero if you want a paper copy for the week.

The whole file is still self-contained — 54 KB, no CDN, no dependencies, works offline. Want me to add anything else — a live credit-cost estimator, or a dark mode toggle?

## 👤 You

[connected] GitHub is connected now (AbacusAI Bot GitHub - difaze3): that account is who the user means by "me". Use `gh` and git in bash: they are authenticated now. Confirm it to the user in one short line, in their language and your own words, then carry on with what was waiting on it.

<system_reminder>
This is what you are connected to in this session:
Messaging platforms connected (0): none
Connectors connected (2): Gmail (abacus-gmailuser), as Gmail - francisoliver0923@gmail.com, GitHub (abacus-githubbot), as AbacusAI Bot GitHub - difaze3
MCP servers and connectors configured (1): abacus-connectors
Skills available (8): Code review, Data analysis, Debugging, Word documents, Frontend design, Writing tests, Web research, Excel / Spreadsheets
Everything listed is available to you right now. Use it when it is relevant instead of saying you lack access. A connector listed as connected needs no connecting, and the account named beside it is the user's own: that is who they mean by "me", so do not ask them for it. A service NOT listed can usually still be attached: call connect_connector for it instead of reporting no access or asking whether to connect. This note is automatic; do not mention it to the user.
</system_reminder>

## 🤖 AbacusAI Bot

GitHub is connected now, as **AbacusAI Bot GitHub — difaze3** — that's you, so `gh` and git are working on your behalf.

Nothing in the guide was actually waiting on it (that earlier prompt was just my placeholder), so here's what it unlocks for you:

- **§9 Working with code** becomes fully usable — I can clone a repo, read real files, run its tests, review a diff or PR, and open pull requests as `difaze3`.
- **§6 Routines** can cover repo work: a nightly "summarise what changed on `main`", or a Monday "PRs waiting on your review".
- **§5 Connectors** — you now have two connected (GitHub and Gmail as `francisoliver0923@gmail.com`), which is exactly the "one or two, not ten" advice the guide gives.

Two follow-ups if you want them:
1. Point me at a repo and I'll do a real §9 walkthrough on it — read the code, then produce a reviewed change.
2. Add a **"Using GitHub with the agent"** section to the guide site, matching the structure of the other connector sections.

Which would you rather have?

## 👤 You

always give me the link of the finished project in the end

## 🤖 AbacusAI Bot

Got it — noted permanently. Every finished project will end with its link, not just a file path.

Two things worth flagging about that promise:
- **Local links only live while I'm serving them.** `http://127.0.0.1:55259` works right now, but if the app restarts, the port goes dead. When something needs to outlive the session, I'll also give you the file itself (or push it to GitHub, now that's connected) so the link isn't the only copy.
- **I'll keep linking the artifact itself**, not the folder it sits in.

The guide is ready, and nothing changed in its content — this was just a re-present so the link is where you want it.

**🔗 http://127.0.0.1:55259**

Still open from before, if you want either:
1. A repo walkthrough with the now-live GitHub connection.
2. A new "Using GitHub with the agent" section added to the guide.

## 👤 You

Just a question; not a task. Can I use md (Markdown) to give you a set of instrustions and rules you need to follow and use ai agentic skills to get the ouptut i want?

## 🤖 AbacusAI Bot

Short answer: **yes, and that's the native way to do it.** Markdown is the right format for it.

**Where that Markdown can live — three levels:**

| Level | How | Scope |
|---|---|---|
| **In the chat** | Paste it, or point me at the `.md` file | That conversation only |
| **A skill** | A `SKILL.md` file — its description is what makes me load it automatically when a task matches | Every session, every project |
| **A project file** | e.g. `AGENTS.md` / `CLAUDE.md` in a repo | Whenever I work in that repo |

**What belongs in it, and what doesn't:**

*Works well in Markdown:*
- Rules and constraints ("never write prose over 400 words", "always cite the file each claim came from")
- Procedures — numbered steps, decision points, checklists
- Output format and house style; tone and audience; vocabulary. If you have a template, paste the template itself as the spec
- Examples of good vs. bad output. A concrete negative example beats three paragraphs of description
- A "stop and ask me if…" list — genuinely the highest-value part

*Works badly:*
- Multi-stage logic that needs branching on data ("do this *unless* the sheet has…"). I'll hold it in context, but it drifts over a long session
- Anything aiming for byte-exact output — instructions bias the output, they don't guarantee it
- Huge documents. A 4,000-line spec dilutes its own rules; 1–2 pages of sharp rules outperforms it

**Two honest caveats:**

1. **Markdown is prose, not a program.** "Use a skill" doesn't mean a deterministic pipeline runs — it means I read your instructions and apply judgment. 95% consistent on a good day, not 100%. That's fine for a report, riskier for anything where a single deviation is a real problem.
2. **Instructions and skills can conflict.** If your `SKILL.md` says "bullet points only" and a skill you ask for says "write flowing prose", the more specific and more recent one usually wins — but it's worth deciding which one is the authority.

**The practical version:** the "Skills" section of your guide already covers this. Write one skill about something you currently re-explain every time, make the first line its *description* ("Use when I ask for a weekly status update…"), and it'll get picked up without you asking.

Want me to draft a starter template — a `SKILL.md` scaffold you can fill in for whatever you do repeatedly?

## 👤 You

question; is this project saved into the app?

## 🤖 AbacusAI Bot

Let me check what's actually on disk and where, rather than answer from memory.

## 🤖 AbacusAI Bot

**Partly — and the distinction matters.**

**What is saved in the app:**
- The **conversation** is saved. There's a thread file on disk (`threads/25f6a34d-….json`, ~412 KB) that holds this whole session — so the chat survives closing the app.
- The **artifacts** I declared are filed under the session's Artifacts panel, so you can find the guide again from the UI without scrolling the chat.
- The **project files** are on disk at `C:/Users/My PC/.abacusai-bot/session-home/abacus-getting-started/index.html` (54 KB). That location is permanent — not a temp folder.

**What is *not* saved, and is the real answer to your question:**
- **The server is not.** `http://127.0.0.1:55259` is me running a local web server by hand. Quit the app and that URL is dead. Files survive; the *link* doesn't.
- **It's not a managed "project."** The app's Projects feature (the deployable apps, 3/month on Basic) is a different thing. This is a folder in the agent's workspace, not a deployed app with its own permanent URL.

So: **the work is saved, the hosting isn't.**

Three ways to fix that, in rising order of effort:

1. **Open the file directly** — `file:///C:/Users/My%20PC/.abacusai-bot/session-home/abacus-getting-started/index.html` always works, no server needed. It's self-contained.
2. **Push it to GitHub** — you're connected now, so it gets a permanent URL and version history. I can do this in one step if you want (public or private).
3. **Deploy it properly** — shareable URL, works when your computer is off. That's the Projects feature, and on Free you'd want Basic.

Want me to push it to GitHub so you stop depending on a local port?

## 👤 You

do step number 2 to save the file into github
