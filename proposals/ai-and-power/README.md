# Proposal · AI and Power — Integrating AI Without Creating an Over-Powerful Owner

**Status:** Draft for debate · **Last updated:** 2026-06-29 · The keystone (this project is named for it). Door 4 of [proposal 00](../00-how-change-happens/). Relates to [#06 Existential risk](../../problems/06-existential-risk/), [#01 Inequality](../../problems/01-economic-inequality/), [#05 Governance](../../problems/05-governance-democracy/), [#10 Information](../../problems/10-information-truth/).

> Added at the owner's request: *"how will the AI be integrated without being a danger to humans and without making its owner over-powerful."* Until now this repo treated AI only as the tool that wrote the Markdown. That is the mistake. **AI is not the author of this project; it is the central problem and possibly the central lever of it.**

## 1. Two distinct dangers — don't conflate them

The owner's framing names two risks that are usually mixed together and must be judged separately:

- **(A) AI as a danger to humans** — loss of control, misuse, accidents, autonomous weapons, bioweapon uplift. Overlaps [#06](../../problems/06-existential-risk/); mostly a **safety/alignment** problem.
- **(B) AI as a power concentrator** — whoever owns the frontier model gains unprecedented **economic, coercive, and epistemic** power at once. The money→power→money loop of [#01](../../problems/01-economic-inequality/) at machine speed. A **political** problem, not a technical one.

A perfectly *safe* AI (A solved) owned by one company or one state is still a catastrophe for everyone else (B unsolved). Public debate is almost all about (A). **This folder's distinctive job is (B) — the part almost no one designs for.**

## 2. Why (B) is the deeper problem — with numbers

Every prior general-purpose technology (printing, electricity, the internet) **diffused**: costs fell, many actors got it. Frontier AI is moving the other way, because it concentrates around three scarce inputs the already-powerful control — **compute, capital, data:**

- The amortized cost to train a frontier model has grown **~2.4× per year since 2016**; GPT-4's compute cost ~**$78M**, current frontier runs **$100M–$1B**, and projections reach **billions by 2027**. ([Epoch AI](https://epoch.ai/blog/how-much-does-it-cost-to-train-frontier-ai-models); [Cottier et al., 2024](https://arxiv.org/abs/2405.21015); [Stanford AI Index](https://hai.stanford.edu/ai-index/2025-ai-index-report)) Rising costs mean the frontier gets **less** accessible over time, not more.
- The hardware/cloud layer is an oligopoly: **NVIDIA was behind >70%** of cloud AI-training compute (2024), and the **top three clouds (~AWS 29% / Azure 20% / Google 13%) ≈ 62%** of cloud infrastructure. *(Industry estimates, 2024–25.)*

If capability tracks compute, and compute tracks capital, then **power tracks capital** — a straight line from [#01](../../problems/01-economic-inequality/) to a permanent oligarchy with a machine.

**The chilling version (why this is worse than ordinary monopoly):** every tyranny in history needed the cooperation of millions — soldiers, police, clerks. That dependence is exactly the lever [Chenoweth's non-cooperation](../00-how-change-happens/) pulls: regimes fall when people stop obeying. **An AI-run surveillance-and-enforcement apparatus may not need that cooperation.** It could remove the structural reason power has always, eventually, had to bend to the governed. Preventing *that* specific future is the project's highest-stakes objective.

## 3. The honest case for concentration (steelman)

Before attacking it: there is a real argument that *some* concentration is good.

1. **Safety may require it.** A handful of well-resourced, accountable labs is easier to monitor and regulate than a world where every frontier capability is open to everyone — including bioterrorists (problem A). Proliferation and concentration trade off against each other; you may not get both safety and dispersal.
2. **Costs per capability fall fast.** Today's frontier becomes cheap and open within ~1–2 years; open-weight models trail the frontier but keep advancing. Concentration at the *frontier* may coexist with broad access to *good-enough* models.
3. **Capital intensity funds the research** that makes AI useful at all.

These are not stupid. The question, as always here, is whether the cure (concentration) is worse than the disease.

## 4. Candidate levers (each with its trade-off)

1. **Open weights / broad access.** *For:* diffuses capability, breaks single-owner dominance. *Against:* also diffuses misuse (problem A). The open-vs-closed tension is genuinely unresolved.
2. **Compute governance** — treat frontier-scale compute like fissile material: track it, cap it, license it. *For:* compute is **physical and choke-pointable** (the >70% / 62% concentration above is what makes this *feasible*). *Against:* that same chokepoint, once controlled, **entrenches whoever holds it** — feasibility and danger are the same property.
3. **An "IAEA for AI"** — an international agency with a dual mandate (share benefits + monitor/safeguard), possibly with a "Secure Chips Agreement" tying advanced-chip access to compliance. ([proposal family](https://arxiv.org/abs/2507.06379); OpenAI execs floated this in May 2023; [IAEA-lessons paper, Nature 2024](https://www.nature.com/articles/s41599-024-03017-1)) *For:* matches a civilization-scale risk with a civilization-scale body. *Against:* requires cooperation among the actors racing to win; enforcement is weak.
4. **Public / non-profit / commons AI** — models accountable to citizens, not shareholders. *For:* attacks ownership concentration head-on. *Against:* a *state-owned* frontier model is a surveillance dream — could make (B) worse.
5. **Antitrust on the whole stack** (chips, cloud, models, data). *For:* classic power-dispersal. *Against:* slow; capability may concentrate faster than litigation moves.
6. **Alignment + control research** (for A). *For:* necessary regardless of owner. *Against:* solving A without B just yields a *reliable* tool for the owner.

## 5. Objections to *this* proposal

- **"You're assuming concentration; maybe AI diffuses like everything else."** Possible (see §3.2) — but the cost trend (§2) points the other way at the frontier, and that's where decisive capability lives. The burden is on the optimist to show diffusion *at the frontier*, not just in last year's models.
- **"Compute governance is the very centralization you fear."** The strongest objection. Yes — the lever that controls concentration *is* a concentration of control. The only honest answer is to bind it (international, transparent, rights-floored) and prefer dispersal levers (1, 5) over chokepoint levers (2, 3) wherever they suffice.
- **"This is unenforceable against a state that defects."** Largely true today. Which is why the smallest first moves (below) are domestic and verification-focused, not a grand treaty.

## 6. What we'd measure

- **Concentration:** frontier compute/capability held by the top 1–3 actors — rising or falling?
- **Owner power (the key test):** can any single AI owner do something to a population that the population **cannot refuse or undo**? (The "non-cooperation no longer works" tripwire.)
- **Diffusion vs. misuse:** for each access-widening step, does it net-empower the public more than malicious actors?
- **Accountability:** is there a real off-switch, and who holds it?

## 7. Transition path (who blocks this · which door · smallest first move)

- **Who blocks it:** the frontier labs and the chip/cloud oligopoly (concentration is their moat), and states that see an AI lead as national power (they won't unilaterally slow down).
- **Which door:** **Door 1** (domestic regulation: compute reporting, antitrust) + a dedicated **international door** (the IAEA-for-AI family) + **Door 4 itself** (using AI for verification/transparency). Note this is the one problem where Door 3 (exit/new country) barely helps — you cannot out-compute a superpower from a charter city.
- **Smallest first move:** **compute-threshold transparency** — require anyone training above a compute threshold to report it (cheap, verifiable, no capability ban, leverages the physical chokepoint), plus **antitrust scrutiny of the chip+cloud layer.** Both are doable inside one jurisdiction without a treaty, and both directly target (B).

## 8. Open questions

- Is there a **stable equilibrium** where AI empowers citizens, or does it inevitably tip toward whoever has the most compute? *(The crux of the entire project's title.)*
- Can you get the **safety** of a closed model **and** the **power-dispersion** of an open one — or is that a real either/or (§3.1)?
- Does "public AI" reduce owner-power, or just **move** it to whoever controls the state? → taken up as a full proposal in [`ai-sovereign`](../ai-sovereign/) (distributed *k-of-n* off-switch + democratically-set objective + corrigibility).
- What exactly stops an AI-enforcement apparatus from removing the cooperation-dependence that has always, eventually, let people overthrow tyranny (§2)?

## 9. Sources

- Epoch AI, *How much does it cost to train frontier AI models?*: https://epoch.ai/blog/how-much-does-it-cost-to-train-frontier-ai-models
- Cottier, Rahman et al., *The Rising Costs of Training Frontier AI Models* (2024): https://arxiv.org/abs/2405.21015
- Stanford HAI, *AI Index Report* (training cost, compute, concentration): https://hai.stanford.edu/ai-index/2025-ai-index-report
- *Domestic frontier AI regulation, an IAEA for AI, an NPT for AI…* (2025): https://arxiv.org/abs/2507.06379
- *Lessons from the IAEA's nuclear safety regulations for AI*, Nature Humanities & Social Sciences Communications (2024): https://www.nature.com/articles/s41599-024-03017-1
- → [#06 Existential & emerging-tech risk](../../problems/06-existential-risk/) for the AI-safety (problem A) evidence base.

*If you want to attack this folder, the most useful contribution is a credible mechanism by which frontier capability **diffuses** rather than concentrates — because the entire (B) argument rests on the claim that it won't.*
