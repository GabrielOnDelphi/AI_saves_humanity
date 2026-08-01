# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

A research and writing repository — **no source code, no build, no tests, no linter.** The deliverable is Markdown: an evidence-first catalog of humanity's biggest problems (`problems/`) plus stress-tested proposals to fix them (`proposals/`). Public GitHub repo: `GabrielOnDelphi/AI_saves_humanity`. MIT.

Your job here is research, fact-checking, argument, and editing — not programming.

## Overrides of the global rules

- **This is NOT a Delphi project.** The owner's global Delphi instructions (Delphi vocabulary mandate, `light-*` skills, `light-compiler`, MD idiom rules) **do not apply.** Write plain, clear English.
- **`HandOver.md` does not exist here** — this project uses `handover-protocol.md` + `ROADMAP.md` instead (see below). Do not create `HandOver.md`.
- **The fact-check mandate DOES apply, harder than anywhere else.** Every number and every claim about the world needs a primary source with a link and a year. Verify with WebSearch/WebFetch (load via ToolSearch) *before* writing it down. If a figure isn't published, write "not published" — never estimate and present as fact. An invented statistic destroys the whole point of the repo.

## Read first, every session

1. **`handover-protocol.md`** — cross-session memory: recent sessions, settled decisions, the owner's firm positions, verified facts to reuse. Read before doing anything.
2. **`ROADMAP.md`** — the live backlog, organized by the four doors. This is the canonical to-do list (it supersedes handover §8).
3. `README.md` — the public map.

**Both `handover-protocol.md` and `ROADMAP.md` are in `.gitignore`** — local-only working files, never pushed. Everything else in the repo is public.

At the end of a session, update both: what was built, what was decided, what is now open.

## The method every page must follow

1. **Evidence first** — primary source (WHO, World Bank, UN/FAO, IPCC, WMO, Oxfam, World Inequality Lab, Pew, V-Dem, Freedom House, peer-reviewed papers), link inline, year stated.
2. **Steelman, then stress-test** — best case *for* the idea → strongest objection → improved version. A proposal with no honest "Objections" section is incomplete.
3. **Roots over symptoms** — keep asking "and why does *that* happen?" until you reach something changeable.
4. **Log disagreement, don't delete it** — including where the owner and the model disagree. Record both sides.

The test of every page: not "does this sound inspiring?" but **"is this true, and would it actually help?"**

## Architecture — how the repo argues

The repo is not a flat collection of essays. It has a spine and a fixed logic:

- **`proposals/00-how-change-happens/` is the spine.** The claim: we are not short of good policy — good policy dies at the *transition*, blocked by the people it threatens. Everything else orbits this.
- **The four doors** out of a captured status quo, and every proposal belongs to one: **1 Reform** from within · **2 Defend** what works (`defending-democracy/`, problem #14) · **3 Exit and build new** (`country-and-citizenship/`) · **4 AI as the new variable** (`ai-and-power/`, `information-integrity/`, `ai-sovereign/`).
- **`proposals/beyond-democracy/` reframes the goal** — democracy is a *proxy*; optimize the target (accountable power + flourishing) while keeping democracy's catastrophe-insurance.
- **`problems/01` (inequality) and `problems/05` (governance) are upstream** — they capture or block the fixes for nearly everything else. The numbering 01–14 is reference, not priority.

**Two rules any new page must obey:**

- **Transition path (required in every proposal).** Who would block this · which door gets past them · the smallest first move. No transition path = it is a wish, not a plan, and must be labeled as such.
- **The capture test** (`proposals/the-capture-test.md`). When an idea meets a *"but who controls X?"* objection, apply that objection **evenly to democracy's own version of the same classifier** (districting, franchise rules, GDP, platform algorithms) and judge **comparatively**. Never use it as a one-sided kill shot — every system has a rule-setter. Score on concentration · transparency · reversibility · self-correction.

## Document conventions

- **Problem folders** (`problems/NN-name/README.md`) follow a fixed 8-section template: Scope → Key facts → Root causes → Connections → Candidate solutions (with trade-offs) → Metrics we'd watch → Open questions → Sources.
- **Proposal folders** (`proposals/name/README.md`) use numbered `##` sections ending in: Metrics → Objections (steelman against yourself) → Transition path → Open questions → Sources.
- **Companion deep-dives** live beside the folder README as a named file (`radical-options.md`, `epistocracy-improved.md`, …), and must be linked from the parent README's relevant section. A doc nobody links to does not exist.
- **Line 3 of every content page is the status line:** `**Status:** Draft for debate · **Last updated:** YYYY-MM-DD · <what this relates to, with relative links>`. Update the date when you edit. The three index files — `README.md`, `CONTRIBUTING.md`, `proposals/README.md` — are exempt.
- **Relative links only**, and cross-link generously between problems and proposals (`../../problems/05-governance-democracy/`). The repo's value is in the connections.
- **Never hard-wrap paragraphs.** One paragraph per line. Tables and headers over walls of text. Lean, direct, no filler.

## Settled — do not relitigate without a new argument

These were fought out already and are recorded with their rebuttals in `handover-protocol.md` §4–§6. Build on them; reopen only with new evidence.

- **Education-weighted voting** (the owner's founding idea): direct election of the head of state = recommended; weighting ballots by formal education = rejected as specified (it is the Jim Crow literacy-test mechanism, it correlates with wealth, and whoever defines "education" owns the electorate). The idea is kept in the repo *with* its rebuttal — do not quietly delete it.
- **Religion (#13):** the target is religious *coercion* and religiously-justified *harm*, never belief. Symmetry is load-bearing — coercive anti-religion (USSR, Albania 1967) is equally condemned. "Teach *about*; never teach *into*."
- **Beyond democracy:** "democracy did nothing special" is false (it is catastrophe-insurance), but "it is captured" is true (Gilens-Page).

**Two standing behavioral lessons the owner caught and will catch again:**

1. Do not concede his point, stress-test it to death, then funnel back to the same safe menu (sortition / reversibility). If he asks for radical, deliver radical — see `proposals/beyond-democracy/radical-options.md`.
2. Do not deploy "but who controls X?" against a new idea without applying it to the status quo first.

He wants to be told directly when he is wrong. Do not flatter. Concede cleanly when he is right.

## Commands

There is nothing to build or test. What exists:

```bash
git add -A && git commit -m "..." && git push          # remote: GabrielOnDelphi/AI_saves_humanity

# audit: proposals missing the mandatory transition path
for f in $(git ls-files 'proposals/*.md'); do grep -qil "transition path" "$f" || echo "$f"; done

# audit: files missing the line-3 status header
git ls-files '*.md' | while read f; do sed -n 3p "$f" | grep -q '\*\*Status:\*\*' || echo "$f"; done
```
