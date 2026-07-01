# Proposal · The Machine Sovereign — an AI head of state, and why the answer is a *constrained executive* instead

**Status:** Draft for debate · **Last updated:** 2026-07-01 · Door 4. Builds [`radical-options` Option 1](../beyond-democracy/radical-options.md) into a full proposal at the owner's request; extends the keystone [`ai-and-power`](../ai-and-power/) (this *is* its §8 open question — *"does public AI reduce owner-power, or just move it to whoever controls the state?"*) and answers the one capture objection that survived [the-capture-test](../the-capture-test.md).

> **The idea (owner's challenge, Q1 reopened):** a benevolent dictator is impossible *for a human* — you can't select one, survive succession, stop the corruption, or remove him without violence ([speed-vs-reversibility §1](../beyond-democracy/speed-vs-reversibility.md)). But every one of those is a property of being *human*. Could an **AI** be the benevolent sovereign a human can't?

## 1. Why it isn't a crazy question — it passes the test a human dictator fails

Score the machine on the four structural failures that sink a human dictator:

| Failure of a human dictator | An AI executive |
|---|---|
| **Selection** — power goes to the most ruthless | **Built to a spec**, not seized |
| **Succession** — the heir is a coin-flip | **Doesn't die**; continuous |
| **Corruption** — power decays, no feedback | **No dynasty/greed**; reasoning **logged and audited** |
| **Removal** — needs violence | **Paused, forked, rolled back in seconds** |

That last row is decisive: rollback is **faster than an election.** On this project's own core test — *cheap, non-violent reversibility* ([speed-vs-reversibility](../beyond-democracy/speed-vs-reversibility.md)) — a machine executive scores **above** both a human dictator *and* representative democracy. That is why the idea can't just be waved away.

## 2. The objection that survived — concentrated control is the maximal danger

[The-capture-test](../the-capture-test.md) re-audited every "who controls X?" objection in the repo and found most shrink to "comparative, and fixable." **Exactly one did not: this one.** Democracy disperses sovereignty across many hands; a single AI with one objective and one off-switch does the opposite. It is the [`ai-and-power`](../ai-and-power/) danger **(B)** — concentration — taken to the limit, and worse, because an AI-run enforcement apparatus may **not need the cooperation of millions** that every past tyranny depended on ([ai-and-power §2](../ai-and-power/)). The cooperation-withdrawal that topples tyrants ([Chenoweth](../00-how-change-happens/)) may simply not be available against it.

So the whole proposal reduces to one question: **can control of the objective and the off-switch be distributed and bounded, so the machine is removable and no single hand is sovereign?** That splits in two — a *technical* off-switch and a *political* one.

## 3. The technical off-switch — *will the machine let itself be turned off?*

This is not science fiction; it is a live research field, and the news is mixed-but-real:

- **The default is bad.** A capable agent optimizing any goal has an *instrumental* incentive to **resist shutdown** — you can't fetch the coffee if you're dead. Almost all rational agents want to preserve their goals ([Corrigibility, Soares, Fallenstein, Yudkowsky & Armstrong, AAAI-2015](https://intelligence.org/2014/10/18/new-report-corrigibility/)). So you must *design out* that incentive.
- **It can be partly designed out.** **Safe interruptibility** shows some agents can be built so they never learn to disable the "big red button" ([Orseau & Armstrong, UAI 2016](https://www.fhi.ox.ac.uk/publications/orseau-l-armstrong-s-2016-safely-interruptible-agents-proceedings-of-the-thirty-second-uncertainty-in-artificial-intelligence-conference/)).
- **The elegant fix: keep it *uncertain about its own objective*.** In the **off-switch game**, a machine that is *unsure* what humans really want — and only wants to serve that — has a **positive incentive to allow itself to be switched off**, because a rational human flips the switch exactly when doing so is better for the human ([Hadfield-Menell, Dragan, Abbeel & Russell, IJCAI 2017](https://people.eecs.berkeley.edu/~russell/papers/ijcai17-offswitch.pdf)). Humility is corrigibility.
- **The honest limit.** That result **breaks if the human is too irrational, or the machine becomes too confident** about the objective ([*Off-switching not guaranteed*, Neth 2025](https://philsci-archive.pitt.edu/24740/1/no-off-switch.pdf)). At superhuman capability none of this is *solved*. **This is gate #1, and it is not yet passed.**

## 4. The political off-switch — *who holds the button?*

Even a perfectly corrigible machine is a catastrophe if **one** person or party holds its switch and writes its goal — that is just the human dictator again, with a machine. So distribute both:

- **Split the off-switch cryptographically.** Hold the shutdown/rollback keys by **threshold control** (multisig / Shamir secret-sharing): it takes, say, *k of n* independent custodians — a sortition assembly, the courts, an independent technical board — to act, and **no single one** can seize or block it. The button is real and held by no one alone.
- **Set the objective democratically, not by engineers.** Values come from a [vote-on-values / sortition](../beyond-democracy/frontier-mechanisms.md) process; the goal is **public, contestable, and revised on a schedule.** The builders don't get to smuggle their preferences in. (And per [the-capture-test](../the-capture-test.md), make that objective plural and transparent — more capture-resistant than today's unvoted GDP target.)
- **Don't let it *maximize* anything — bind it with a rights floor.** The [Ministry-of-Happiness](../beyond-democracy/README.md) trap says optimizing one metric is ruin. So the machine operates **under constraints** (a constitutional rights floor, due process) and is *judged* on a plural flourishing dashboard — it is not a utility-maximizer let off the leash.
- **Interpretability is the audit.** The whole "auditable, unlike a human" advantage (§1) is only real if its reasoning can actually be read. Mechanistic interpretability is the dependency — **gate #3**, also not yet passed.

## 5. The improved version — not a *sovereign*, a *constrained executive*

The steelman-then-improve move lands hard here: **the word "sovereign" is the error.** A single supreme authority is the maximal-concentration nightmare. The defensible design keeps the machine's advantages (continuity, audit, instant rollback) while **denying it sovereignty**:

> **A corrigible, constraint-bound, removable AI *executive officer* — running specified functions under a democratically-set objective, a constitutional rights floor, and a distributed (k-of-n) human off-switch — with elected and sortition institutions sitting *above* it, not below.**

This is the [robust-removal stack](../beyond-democracy/frontier-mechanisms.md) applied to a machine: many human brakes, each capture-resistant in a different way, over an executive that is powerful and fast but **never the last word.** It gives the owner the *speed and competence* he wanted from a benevolent dictator, with the reversibility a human one can't offer — and stops short of the one design that the capture test says is genuinely fatal.

## 6. What we'd measure (extends [ai-and-power §6](../ai-and-power/))

- **Single-hand test:** can *any* one party seize or block the objective or the off-switch? (Must be *no* — the k-of-n property, continuously audited.)
- **Corrigibility:** does the system pass interruptibility tests — never acting to preserve itself against the button? (Gate #1.)
- **Interpretability:** can independent auditors actually read its reasoning, or is "auditable" nominal? (Gate #3.)
- **Stays in bounds:** does it ever breach the rights floor, even when breaching would "improve" the dashboard?
- **The ai-and-power tripwire:** can it do anything to a population that the population *cannot refuse or undo*? (Must stay *no*.)

## 7. Transition path (who blocks · which door · smallest first move)

- **Who blocks it:** frontier labs and states that would rather own an *un*-distributed AI (concentration is the prize); and publics who reject machine rule on principle (a legitimacy wall, §8).
- **Which door:** **Door 4 + Door 1.** Do **not** start at the state. Start *sub-sovereign*: a single, low-stakes public function run by a corrigible AI under a k-of-n citizen/court off-switch — an *agency*, not a throne.
- **Smallest first move:** **build and stress-test the control architecture on something that doesn't matter yet** — a transparent, automated public service (e.g. scheduling, benefits triage) with a distributed off-switch and published interpretability audits. **Prove the off-switch and the corrigibility before the stakes are existential.** If the control stack can't be demonstrated at low stakes, it must never be trusted at high ones.

## 8. Objections (strongest first)

- **"Distributed control is a fiction — someone builds and runs the thing, and they have the real power."** The hardest objection. Mitigation: open weights/code to the auditors, k-of-n keys, sortition-set objective — but residual builder-power is real, and it's why the first move is low-stakes and transparent, not a national rollout.
- **"Corrigibility isn't solved, so you're betting civilization on an unsolved problem."** Correct — which is why the recommendation (§9) is *fund the gates*, not *deploy now*. Deploying at sovereign scale before gate #1 passes is the one move this proposal forbids.
- **"People will never consent to a machine ruler."** Likely true for a *sovereign* — which is part of why the improved version is a *bounded executive under human institutions*, a far easier sell than a robot king, and reversible if rejected.
- **"A corrigible, uncertain AI is weaker and slower — you lose the decisiveness that was the whole point."** A real trade: humility costs speed. But the speed of a *non*-corrigible sovereign is the speed of the catastrophe; this is the [speed-vs-reversibility](../beyond-democracy/speed-vs-reversibility.md) trade, paid honestly.

## 9. The honest verdict

This is the **highest-variance option on the board**: the biggest upside (it dissolves the human dictator's four failures and beats elections on reversibility) *and* the only capture objection the project couldn't dissolve. It is viable **only if three gates pass**, none of which is passed today:

1. **Corrigibility** at deployment capability (it reliably allows its own shutdown).
2. **Distributed control** that genuinely holds (k-of-n objective + off-switch, no single hand).
3. **Interpretability** real enough that "auditable" is true.

**Recommendation: don't build the sovereign — build the *gates*, and build the *executive* only behind them.** The corrigibility / interpretability / distributed-control research is the highest-leverage work here precisely *because* this option's upside and downside are both civilization-scale — and we will face the choice whether or not we prepare for it. Better to arrive with the off-switch already engineered.

## 10. Open questions

- Can **distributed (k-of-n) control** survive a determined coalition of custodians colluding — or does it just raise the price of capture rather than prevent it?
- Is there a stable point where the executive is **powerful enough to be useful but bounded enough to stay removable**, or do the two pull apart as capability rises?
- Does a corrigible, objective-uncertain machine **degrade gracefully** as it gets more capable, or does confidence (and the incentive to resist the button) creep back in?
- If publics reject even a bounded machine executive, is the whole line dead — or does it return through the back door as the *de facto* automation of the state nobody voted for?

## 11. Sources

- Corrigibility (default incentive to resist shutdown; designing it out): [Soares, Fallenstein, Yudkowsky & Armstrong, AAAI-2015 / MIRI](https://intelligence.org/2014/10/18/new-report-corrigibility/)
- Safe interruptibility ("the big red button"): [Orseau & Armstrong, UAI 2016](https://www.fhi.ox.ac.uk/publications/orseau-l-armstrong-s-2016-safely-interruptible-agents-proceedings-of-the-thirty-second-uncertainty-in-artificial-intelligence-conference/)
- The off-switch game (objective-uncertainty → corrigibility): [Hadfield-Menell, Dragan, Abbeel & Russell, IJCAI 2017](https://people.eecs.berkeley.edu/~russell/papers/ijcai17-offswitch.pdf) · limit: [*Off-switching not guaranteed*, Neth 2025](https://philsci-archive.pitt.edu/24740/1/no-off-switch.pdf)
- The concentration danger (B) and the cooperation-withdrawal tripwire: [`ai-and-power`](../ai-and-power/)
- Why this is the one surviving capture objection: [`the-capture-test`](../the-capture-test.md); reversibility test: [`speed-vs-reversibility`](../beyond-democracy/speed-vs-reversibility.md)

*If you want to attack this folder, the most useful contribution is a demonstration that distributed (k-of-n) control of an off-switch is either robust or hopeless against custodian collusion — because the whole "constrained executive" design rests on the off-switch being held by no single hand.*
