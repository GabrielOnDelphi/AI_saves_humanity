# Handover Protocol — AI Saves Humanity

**Purpose:** let a fresh Claude session (or any new contributor) restart this project cold and pick up exactly where it stopped. Read this file first, then [`README.md`](README.md), then the folder you're working on.

**Last updated:** 2026-06-17 · **Maintainer:** project owner (cubicdesign@gmail.com)

---

## 1. Project snapshot

- **What it is:** an open, evidence-first project to name humanity's biggest problems honestly and design solutions worth debating.
- **Location:** `C:\AI\AI saves humanity\`
- **License:** MIT (copyright line currently reads "AI Saves Humanity contributors" — owner may swap in a personal/company name).
- **Destination:** public GitHub repo. **Not yet `git init`-ed.** No commits exist.
- **Status:** scaffold complete — 13 problem folders + 1 proposal, all grounded in primary sources.
- **This is NOT a Delphi project.** The owner's global Delphi rules (light-md, Delphi vocabulary, light-compiler, `--!SLIM MD!--` token) **do not apply here.** Plain, clear English Markdown.

---

## 2. Method (the discipline every page must follow)

1. **Evidence first.** Every factual claim cites a primary source (WHO, World Bank, UN/FAO, IPCC, WMO, Oxfam, World Inequality Lab, Pew, OHCHR) with a link and a year. If a number isn't published, write "not published" — never invent one.
2. **Steelman, then stress-test.** Each solution: best case *for* it → strongest objection → improved version. A proposal with no honest "Objections" section is incomplete.
3. **Roots over symptoms.** Keep asking "and why does *that* happen?" until you reach something changeable.
4. **Log disagreement, don't delete it.** Where smart people (or the owner and the model) disagree, record both sides.

The test of every page: not "does this sound inspiring?" but **"is this true, and would it actually help?"**

---

## 3. Current file tree

```
AI-saves-humanity/
├── README.md                      ← the map: mission, 13-problem table, proposal pointer, sources
├── LICENSE                        ← MIT
├── CONTRIBUTING.md                ← ground rules + the problem-folder template
├── handover-protocol.md           ← this file
├── .gitignore
├── problems/
│   ├── 01-economic-inequality/    ← UPSTREAM problem (money→power loop)
│   ├── 02-health/
│   ├── 03-education/              ← both a problem and a lever; ties to the political proposal
│   ├── 04-climate-environment/
│   ├── 05-governance-democracy/   ← UPSTREAM problem; home of the political proposal
│   ├── 06-existential-risk/       ← AI, nuclear, engineered pandemics
│   ├── 07-food-water/
│   ├── 08-energy/
│   ├── 09-conflict-peace/
│   ├── 10-information-truth/
│   ├── 11-mental-health-social/
│   ├── 12-rights-justice/         ← the moral floor; guardrail on all solutions
│   └── 13-religion/               ← religion as COERCION/harm, not belief; heavily debated (see §5)
└── proposals/
    ├── README.md                  ← proposal index
    └── political-system/          ← the founding proposal (see §4)
```

Every `problems/NN-*/README.md` follows the same template: **Scope → Key facts → Root causes → Connections → Candidate solutions (w/ trade-offs) → Metrics → Open questions → Sources.**

**Framing note:** #01 (inequality) and #05 (governance) sit *upstream* — they capture/block the fixes for almost everything else. Numbering is reference, not priority.

---

## 4. Key decision: the political-system proposal

The founding idea, in [`proposals/political-system/`](proposals/political-system/). It splits into two parts, judged separately:

- **(A) Direct election of the head of state** (everyone votes directly, no electoral college / no parliament picking the leader) — **recommended**, ideally with a runoff or ranked-choice ballot.
- **(B) Education-weighted votes** (ballots count more for the more-educated) — **NOT recommended as specified.** This is *plural voting / epistocracy* (J.S. Mill 1861; Jason Brennan 2016). Three decisive objections: it correlates with wealth/race → entrenches privilege in a feedback loop (Brennan's own "demographic objection"); it's the exact mechanism Jim Crow literacy tests used to disenfranchise; whoever defines "education" controls the electorate.
- **The improvement that keeps the goal:** reach better-informed decisions *without* disenfranchising anyone — **sortition-based citizens' assemblies, voluntary liquid-democracy delegation, universal civic education, and a constitutional rights floor.**

The owner originated idea (B). He has engaged with the critique; the folder records his proposal *and* the counter-case in full. Do not quietly delete (B) — it's logged with its rebuttal.

---

## 5. Key decision: religion (#13) — read before editing this folder

This was the most debated topic. The settled position (owner + model converged):

- **Framing:** the problem is **religious *coercion* and religiously-justified *harm***, NOT belief itself. The folder is explicitly *not* a "religion is bad" screed — that would be inaccurate (religion founded hospitals/universities/charities) and would alienate ~84% of humanity.
- **Symmetry (load-bearing):** coercive *anti*-religion is equally catastrophic — USSR, Maoist China, Albania's 1967 outright ban. The harm is in the **coercion, regardless of which side coerces.** This decouples the anti-coercion case from any claim that religion is "good."
- **Two concessions the owner is right about, now in the doc:** religion is **not science** (no epistemic deference; its claims are unfalsifiable); and **prevalence ≠ truth/merit** (named the *ad populum* fallacy). The honest claim is only that religion's *effects* are empirically mixed.
- **The teaching rule (fully resolved):**
  - **Banned:** teaching a religion's **doctrine *as the faith* (confessional instruction)** in public schools / state institutions / to any captive audience (pupils, prisoners, conscripts). Also: no doctrine-as-fact taught to children, no creationism in science class.
  - **Allowed:** teaching ***about*** religion — genuinely balanced comparative study, history, influence — because that is evidence-based knowledge and is how you understand history/conflict/#03/#10.
  - **Guardrail (the owner's sharp point):** "comparative religion" is routinely abused as cover for single-faith instruction. Documented: **Germany** mandates *confessional* RE (Grundgesetz Art. 7(3)); **England** requires the RE syllabus to be "in the main Christian" (Education Reform Act 1988, s.8(3)). So "teaching about" must be policed for real balance. Slogan in the doc: **"Teach *about*; never teach *into*."**
- **Rights anchor:** UDHR/ICCPR **Article 18** protects manifesting belief "in public or private" and limits it only where "necessary to protect public safety, order, health, or morals or the fundamental rights and freedoms of others" — i.e. the harm standard. An adult *expressing* belief in public is exercising a right; the ban targets *state institutions and captive audiences*, not voluntary adult speech.
- **Still open:** *who certifies a "comparative" syllabus is actually balanced* without becoming a capture surface (#05)?

---

## 6. The owner's firm positions (respect these; don't relitigate from scratch)

- Wants a **new democracy: direct national vote for the president, weighted by education.** (Engaged with the critique — see §4 — but this is his originating vision.)
- **Anti-religion lean.** Religion "created lots of problems over the centuries." Religion is **not science.**
- **No teaching of religious doctrine in public places/schools.** Teaching *about* religion is OK but "carefully" — and he specifically flagged the fake-"comparative-religion" loophole.
- **Harm standard for belief:** free to believe unless the teaching promotes harm.
- Wants religious promotion treated like a (planned) **advertising restriction** — see open threads; that advertising rule does not exist yet.

If the owner restates one of these, build on it — don't reopen the whole debate. Push back only with *new* evidence or a *new* argument, per his standing instruction to challenge him directly.

---

## 7. Verified facts (already grounded — reuse, don't re-verify)

| Topic | Fact | Source (year) |
|-------|------|---------------|
| Inequality | Top 1% own ~43.8% of wealth; bottom 50% ~0.52%; billionaires ~4,000× more likely to hold office; billionaire wealth ~$18.3T, >3,000 billionaires | Oxfam (2025); World Inequality Report (2026) |
| Poverty | ~817M in extreme poverty under $3/day line (was ~692M under $2.15) | World Bank (2024/2025) |
| Health | ~4.5B lack full essential health services; ~2B face financial hardship; 1.3B pushed into poverty by health costs | WHO (2024) |
| Education | ~6 in 10 children can't read a simple text by age 10 (learning poverty) | World Bank/UNESCO (2024) |
| Climate | 2024 first year >1.5°C (~1.55°C); ~86% chance one of 2025–29 exceeds 1.5°C | WMO (Jan 2025) |
| Food/Water | ~673M hungry; ~2.3B food-insecure; ~2.6B can't afford a healthy diet; 2.1B lack safe drinking water; 3.4B lack safe sanitation | FAO SOFI (2025); WHO/UNICEF JMP (2024) |
| Mental health | >1B live with a mental health condition; depression ~280M, anxiety ~301M; suicide ~727k/yr (2021); <2% of health budgets to mental health | WHO (2025) |
| Conflict | Most state-based conflicts since 1945; >100M forcibly displaced; record military spending | UCDP/PRIO; UNHCR; SIPRI |
| Religion | ~84% affiliated (2010); ~1.9B "nones" by 2020 (⅔ in China); religion-related social hostilities high/very-high in 55 countries in 2023 (up from 45) | Pew (2025/2026) |
| Rights anchor | UDHR/ICCPR Art. 18 (manifest belief public/private; harm-based limits). Germany Grundgesetz Art. 7(3) confessional RE; England Education Reform Act 1988 s.8(3) "in the main Christian" | UN/OHCHR; legislation.gov.uk; gesetze-im-internet.de |

Full source URLs are in each problem folder's **Sources** section and at the bottom of `README.md`.

---

## 8. Open threads / next actions (priority order)

1. **Write the advertising proposal** — `proposals/advertising/` (or similar). Referenced by both #13 and the political proposal's "treat it like advertising" analogy, but **it does not exist yet**, so that analogy currently has no defined rule to inherit. Key tension to resolve: commercial advertising is not a human right, but religious/political/artistic expression *is* — so they can't be regulated identically. **Owner asked for this next — likely the first task tomorrow.**
2. **`git init` + first commit + push to GitHub.** Repo is not yet under version control. (Confirm the desired GitHub repo name and the LICENSE copyright name first.)
3. **Define the "comparative-syllabus certifier"** open question from #13 §5.
4. **Deepen problem folders** — add metrics targets, more data, sub-solutions; translate.
5. **Add more proposals** under `proposals/` (e.g., money-out-of-politics, UHC design, carbon pricing).

---

## 9. Working with this owner / environment

- **Fact-check mandate is absolute.** Verify external claims against primary sources *before* asserting (use WebSearch/WebFetch). The owner has explicitly warned about hallucinations. Cite URL + year inline.
- **Push back honestly.** He wants to be told directly when he's wrong; don't flatter. But concede cleanly what he's right about (as happened on religion).
- **Autonomy.** Do most work without asking; ask only when genuinely blocked. Fix trivial issues directly.
- **Keep MD lean and clear.** Short, direct, no filler. Tables and headers over walls of text. Don't hard-wrap paragraphs.
- **Environment:** Windows 11, PowerShell primary (Bash tool also available). Temp files → `c:\AI\Claude Code\Temp\`.
- **Beep on task finish:** `(New-Object Media.SoundPlayer 'c:\AI\Claude Code\claude bip.wav').PlaySync()` (via PowerShell).

---

## 10. Restart checklist (do this first tomorrow)

1. Read this file, then `README.md`.
2. If continuing the **religion** debate or the **political proposal**, re-read §4/§5 here *and* the actual folder — don't trust memory of the nuance.
3. Confirm with the owner which open thread from §8 to tackle (likely the **advertising proposal**).
4. Before asserting any new external fact, search and cite it.
5. When done, **update this handover file** (state, decisions, open threads) so the next restart is clean.
