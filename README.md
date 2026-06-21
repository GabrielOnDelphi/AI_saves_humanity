# AI Saves Humanity

> An open, evidence-first project to name humanity's biggest problems honestly — and design solutions worth fighting for.

**License:** [MIT](LICENSE) · **Status:** Early draft, help wanted · **Last updated:** 2026-06-16

---

## Why this project exists

Most of the suffering on this planet is not caused by a lack of resources. It is caused by how we organize ourselves: who gets the money, who gets the medicine, who gets to decide. We already grow enough food to feed everyone and still ~673 million people go hungry. We are rich enough to give everyone clean water and 2.1 billion people still don't have it safely at home.

This repository is an attempt to do three things, in order:

1. **Name the problems clearly**, with real numbers from primary sources (WHO, World Bank, UN, IPCC, Oxfam, the World Inequality Lab), not vibes.
2. **Trace each problem to its root causes**, because treating symptoms forever is how we got here.
3. **Design and debate solutions** — including uncomfortable, ambitious, and politically hard ones — and be honest about their trade-offs.

This is not a manifesto that already knows the answers. It is a workbench. Every claim should be checkable; every proposal should survive criticism before it earns trust.

---

## How we work

- **Evidence first.** Every factual claim cites a primary source with a link. If a number isn't published, we say "not published" — we never invent one.
- **Steelman, then stress-test.** For each proposed solution: best version of the argument → strongest objection → improved version. A proposal that can't survive its own critique section doesn't ship.
- **Roots over symptoms.** We keep asking "and why does *that* happen?" until we hit something we can actually change.
- **Open and free.** MIT-licensed. Anyone can copy, fork, translate, or build on this. No paywall, no owner of the truth.
- **Disagreement is logged, not deleted.** Where smart people disagree, we record both sides rather than pretend consensus.

---

## The biggest problems (the founding list)

These are the thirteen problem areas the project starts with. Each has its own folder under [`problems/`](problems/) with facts, root causes, candidate solutions, and metrics. They are **interconnected** — inequality drives bad health, bad governance blocks climate action, and so on — so the numbering is for reference, not priority.

| # | Problem | One-line scope | A grounding fact (source year) |
|---|---------|----------------|-------------------------------|
| 01 | [Economic inequality & concentration of power](problems/01-economic-inequality/) | Wealth and political power pooling in very few hands | Richest 1% own ~43.8% of all wealth; bottom 50% own ~0.52% (Oxfam, 2025) |
| 02 | [Health & disease](problems/02-health/) | Access to care, pandemics, aging, preventable death | ~4.5 billion people lack full access to essential health services (WHO, 2024) |
| 03 | [Education & learning](problems/03-education/) | Whether people can actually read, reason, and learn | ~6 in 10 children worldwide can't read a simple text by age 10 (World Bank/UNESCO, 2024) |
| 04 | [Climate & environment](problems/04-climate-environment/) | Warming, biodiversity loss, pollution, ecosystem collapse | 2024 was the first year >1.5°C above pre-industrial: ~1.55°C (WMO, 2025) |
| 05 | [Governance, democracy & corruption](problems/05-governance-democracy/) | Whether power is accountable to the governed | Billionaires are ~4,000× more likely to hold political office (Oxfam, 2025) |
| 06 | [Existential & emerging-tech risk](problems/06-existential-risk/) | AI, nuclear, engineered pandemics, biosecurity | First century where a handful of technologies could end civilization |
| 07 | [Food & water security](problems/07-food-water/) | Enough safe food and water for everyone | ~2.3 billion face moderate/severe food insecurity; 2.1B lack safe water (FAO/JMP, 2024) |
| 08 | [Energy](problems/08-energy/) | Clean, abundant, affordable energy for all | Energy poverty traps development; fossil lock-in drives #04 |
| 09 | [Conflict, war & peace](problems/09-conflict-peace/) | Violence between and within states | Highest number of state-based conflicts since 1945 |
| 10 | [Information & truth](problems/10-information-truth/) | Whether a society can know what's real | Algorithmic feeds reward outrage over accuracy |
| 11 | [Mental health & social fragmentation](problems/11-mental-health-social/) | Loneliness, despair, loss of meaning and trust | >1 billion people live with a mental health condition (WHO, 2025) |
| 12 | [Human rights, freedom & justice](problems/12-rights-justice/) | Dignity, liberty, and equality before the law | Billions live under regimes that punish dissent |
| 13 | [Religion, coercion & freedom of conscience](problems/13-religion/) | Religiously-justified harm and coercion — in *both* directions | Religion-related social hostilities high in 55 countries in 2023 (Pew, 2026) |

> Sources for the headline numbers are listed at the bottom of this file and in full inside each problem folder.

---

## The founding proposal: a new kind of democracy

The spark for this project was a question about **how we decide**. If governance (#05) is the lever that moves most of the other problems, then the design of democracy itself is worth rethinking.

The founder's original idea: **every person votes directly for the head of state, with each vote weighted by the voter's level of education.** That proposal — its intellectual lineage, its honest case, its serious dangers, and a set of alternatives that try to keep the good part while dropping the dangerous part — is documented in full at:

➡️ **[`proposals/political-system/`](proposals/political-system/)**

It is written the way everything here should be written: the idea stated fairly, then stress-tested hard. (Short version: the *goal* — better-informed collective decisions — is worth pursuing, but weighting votes by formal education is the exact mechanism history used for disenfranchisement, so the folder also lays out designs that reach the same goal without taking the vote away from anyone.)

---

## Repository structure

```
AI-saves-humanity/
├── README.md            ← you are here (the map)
├── LICENSE              ← MIT
├── CONTRIBUTING.md      ← how to add facts, problems, and proposals
├── problems/            ← one folder per problem area
│   ├── 01-economic-inequality/
│   ├── 02-health/
│   ├── 03-education/
│   └── ...
└── proposals/           ← concrete solutions worth debating
    └── political-system/
```

Each problem folder follows the same template: **Scope → Key facts → Root causes → Why it connects to everything else → Candidate solutions (with trade-offs) → Metrics we'd watch → Open questions → Sources.**

---

## How to contribute

This is open work and there is far more to do than any one person can.

1. **Add or correct a fact** — with a primary-source link. Corrections are as valuable as additions.
2. **Improve a solution** — add the strongest objection, or a better version that survives it.
3. **Add a missing problem** — propose a new folder if something important is missing.
4. **Translate** — these ideas should not be locked to one language.

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the ground rules (the most important one: cite your sources, and steelman before you tear down).

---

## A note on honesty

This project will fail if it becomes a place to feel righteous. The test of every page is not "does this sound inspiring?" but **"is this true, and would it actually help?"** Push back. Bring data. If a beloved idea here is wrong, the right move is to say so.

---

## Sources for the headline numbers

- Oxfam, *Takers Not Makers / Davos 2025 inequality reporting* — top 1% own ~43.8% of global wealth; bottom 50% own ~0.52%; billionaires ~4,000× more likely to hold office: https://www.oxfam.org/en/press-releases/worlds-top-1-own-more-wealth-95-humanity-shadow-global-oligarchy-hangs-over-un
- WHO, *Universal Health Coverage* (2024) — ~4.5 billion lack full access to essential health services: https://www.who.int/news-room/fact-sheets/detail/universal-health-coverage-(uhc)
- World Bank / UNESCO, *Learning Poverty* (2024) — ~6 in 10 children can't read a simple text by age 10: https://www.worldbank.org/en/topic/education/brief/learning-poverty
- WMO, *2024 confirmed warmest year on record, ~1.55°C* (Jan 2025): https://wmo.int/news/media-centre/wmo-confirms-2024-warmest-year-record-about-155degc-above-pre-industrial-level
- FAO et al., *State of Food Security and Nutrition in the World (SOFI) 2025* — ~673M hungry, ~2.3B food-insecure: https://www.fao.org/publications/fao-flagship-publications/the-state-of-food-security-and-nutrition-in-the-world/en
- WHO/UNICEF JMP (2024) — 2.1B lack safely managed drinking water: https://data.unicef.org/resources/jmp-report-2025/
- WHO, *Over a billion people living with mental health conditions* (Sep 2025): https://www.who.int/news/item/02-09-2025-over-a-billion-people-living-with-mental-health-conditions-services-require-urgent-scale-up

*All figures reflect the most recent reports available as of June 2026. If you find a newer or more accurate figure, please update it and cite the source.*
