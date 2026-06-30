# Proposal · Information Integrity — Countering Misinformation Without a Ministry of Truth

**Status:** Draft for debate · **Last updated:** 2026-06-29 · The solutions counterpart to [#10 Information & truth](../../problems/10-information-truth/). Door 4 of [proposal 00](../00-how-change-happens/). Relates to [#12 Rights & justice](../../problems/12-rights-justice/) (free expression), [#05 Governance](../../problems/05-governance-democracy/) (the capture surface), [#11 Mental health](../../problems/11-mental-health-social/) (why people *want* to believe).

> Added at the owner's request: *"how to deal with the spread of misinformation on social media — too many paranoid people on TikTok spreading all kinds of weird voodoo."* The honest starting point is that the obvious fix (delete the lies, appoint fact-checkers) is both the **weakest** intervention and the most **dangerous** one. The evidence points somewhere else.

## 1. Get the problem right first (it's demand, not just supply)

Two facts have to sit next to each other:

- **Supply side:** platforms rank for engagement, and outrage/novelty out-engage accuracy ([#10](../../problems/10-information-truth/)). The machine is tuned for it.
- **Demand side — the uncomfortable one:** in the largest study of its kind, **false news spread ~6× faster and reached far more people than true news — and humans, not bots, drove it.** Falsehood spreads because it is *novel* and people *like* sharing novel things. Filtering out the bots barely changed the result. ([Vosoughi, Roy & Aral, *Science*, 2018](https://www.science.org/doi/10.1126/science.aap9559))

So "the algorithm did it" is only half true. The TikTok "voodoo" spreads because it gives people **identity, community, and a feeling of secret knowledge** — needs that are downstream of distrust ([#05](../../problems/05-governance-democracy/)) and loneliness ([#11](../../problems/11-mental-health-social/)). **You cannot fact-check your way out of a demand problem.** Any solution that only attacks supply will fail.

## 2. The constraint that rules out the naive answer

The instinctive fix — "make the platforms delete false content, appoint authorities to decide what's true" — collides with two hard limits:

- **Free expression** ([#12](../../problems/12-rights-justice/)). The harm standard (UDHR/ICCPR Art. 19) permits narrow limits, but a broad "ban falsehood" rule is incompatible with an open society.
- **The capture surface** ([#05](../../problems/05-governance-democracy/)). Whoever gets to define "misinformation" gets to define it *against their opponents.* A Ministry of Truth is a weapon that changes hands at the next election. This is the same lesson as the religion folder's "who certifies the syllabus" problem.

**Design rule for this folder: prefer interventions that need no central arbiter of truth.** That single constraint reorders everything below.

## 3. What actually works (ranked by evidence *and* by capture-resistance)

### Tier 1 — No arbiter needed (lead with these)

- **Prebunking / inoculation — the strongest evidence.** Short (~2-minute) videos that teach the *manipulation techniques* (fearmongering, false dichotomy, scapegoating, decontextualized images) — not the truth of any specific claim — measurably improve people's ability to spot manipulation. Tested on YouTube at the scale of millions; Google/Jigsaw has rolled it out to hundreds of millions. ([Roozenbeek, van der Linden et al., *Science Advances*, 2022](https://www.science.org/doi/10.1126/sciadv.abo6254)) Why it's first: it builds a skill in the *viewer*, so **no institution has to rule on what's true** — it dodges the capture surface entirely.
- **Friction.** Tiny speed bumps ("Want to read the article before sharing?") cut thoughtless resharing of novel falsehood. Cheap, content-neutral, no arbiter.
- **Media literacy / lateral reading** at scale ([#03](../../problems/03-education/)). The durable, individual-empowering defense. *Objection:* slow; won't stop today's flood.

### Tier 2 — Needs a credible (not governmental) checker

- **Corrections / fact-checking — and the cynics are wrong about it.** The widely-repeated claim that "fact-checking backfires and entrenches belief" is **largely a myth**: large replications (Wood & Porter; Nyhan's own reassessment) find corrections mostly move beliefs *toward* the truth, with backfire rare. ([*The Elusive Backfire Effect*, Political Behavior, 2018](https://link.springer.com/article/10.1007/s11109-018-9443-y)) *The real limit:* corrections **reduce but don't erase** influence (the "continued-influence effect"), and they work better with source credibility, repetition, and worldview-aware framing. So: worth doing, not a cure.

### Tier 3 — Structural, slow, capture-prone

- **Platform transparency, not speech bans.** Mandate algorithm and ad transparency and researcher data access (the EU Digital Services Act is the live example `[confirm specifics before citing detail]`) — regulate the *machine and the money*, not the speech.
- **Provenance / authenticity standards** (C2PA / Content Authenticity Initiative) to label AI-generated media. *Objection:* gameable; only works at near-universal adoption.
- **Narrow, harm-based removal** (incitement, targeted fraud, non-consensual content) — the *only* place outright takedown belongs, and even here the capture risk is real.

## 4. The AI twist (Door 4, both barrels)

AI is the accelerant **and** the only scalable extinguisher. It makes fakes cheap and infinite (collapsing the cost of manufacturing "evidence," → [#06](../../problems/06-existential-risk/)); it is also the only thing that can label, trace provenance, and prebunk at the scale of the flood. Whether it nets out for citizens or for manipulators is the same open question as the rest of [AI and power](../ai-and-power/) — and it is unresolved.

## 5. Objections to *this* proposal (steelman the critics)

- **"Prebunking is weak and fades."** Real: effects are modest (single-digit to ~10% gains) and **decay without boosters**. It's a vaccine that needs re-dosing, not a one-shot cure.
- **"Inoculation breeds cynics."** The sharpest objection: teaching people to spot manipulation can spill over into distrusting *legitimate* news too — manufacturing the very "nothing is true" nihilism that authoritarians exploit. The technique must be paired with *what credible sourcing looks like*, not just *what manipulation looks like*.
- **"Transparency laws are a capture surface."** Yes — "mitigate systemic risk" can be bent toward suppressing dissent. Hence Tier 1 over Tier 3.
- **"You barely touched the demand side."** Correct, and it's the deepest hole: none of this fixes *why people want* the voodoo. That root runs through [#05](../../problems/05-governance-democracy/) (distrust) and [#11](../../problems/11-mental-health-social/) (meaning, belonging). Information tools treat the symptom.

## 6. Metrics we'd watch

- Reach/velocity of demonstrably false cascades (the Vosoughi measure) before/after intervention.
- Prebunking: technique-recognition scores, and **decay rate** (how fast the effect fades).
- Generalized trust: does inoculation raise discernment *without* lowering trust in legitimate news? (The Objection-5b test, made into a metric.)
- Adoption of provenance standards; researcher data-access actually granted.

## 7. Transition path (who blocks this, which door, smallest first move)

- **Who blocks it:** platforms (engagement = revenue, so friction and rank-downs cost them money) and would-be manipulators (states, parties, grifters who profit from the flood).
- **Which door:** mostly **Door 1** (regulation: transparency/ad rules, not speech bans) **+ Door 4** (AI labeling/provenance). Tier-1 prebunking is special — it's **deployable bottom-up by anyone** (schools, NGOs, even platforms voluntarily, because it's cheap and good PR), so it doesn't *need* to win the regulatory fight first.
- **Smallest first move:** technique-inoculation in school curricula ([#03](../../problems/03-education/)) and as platform PSAs (already happening via Jigsaw) — the lowest-resistance, no-arbiter, start-tomorrow step. Pair it with a friction default. Save the regulatory fights for the structural tier.

## 8. Open questions

- Can prebunking be made **durable** (auto-boosters in-feed) without becoming nagware people tune out?
- How do you raise the cost of *producing* the flood (AI fakes) without a licensing regime that entrenches incumbents ([AI and power](../ai-and-power/))?
- The hard one: what addresses the **demand** — the want to believe — that no information intervention touches? (Probably not an information problem at all.)

## 9. Sources

- Vosoughi, Roy & Aral, *The spread of true and false news online*, Science (2018): https://www.science.org/doi/10.1126/science.aap9559 (and [MIT News summary](https://news.mit.edu/2018/study-twitter-false-news-travels-faster-true-stories-0308))
- Roozenbeek, van der Linden, Lewandowsky et al., *Psychological inoculation improves resilience against misinformation on social media*, Science Advances (2022): https://www.science.org/doi/10.1126/sciadv.abo6254
- Wood & Porter, *The Elusive Backfire Effect: Mass Attitudes' Steadfast Factual Adherence*, Political Behavior (2018): https://link.springer.com/article/10.1007/s11109-018-9443-y
- C2PA / Content Authenticity Initiative (content provenance standard): https://c2pa.org/
- Reuters Institute, *Digital News Report* (trust trends): https://reutersinstitute.politics.ox.ac.uk/digital-news-report
