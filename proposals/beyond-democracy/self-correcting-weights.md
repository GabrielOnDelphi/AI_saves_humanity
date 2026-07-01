# A self-correcting vote-weight algorithm — the owner's positive-feedback idea, engineered

**Status:** Draft for debate · **Last updated:** 2026-06-30 · The concrete, mathematical realization of two earlier threads: *"earn the weight by track record, not credential"* ([epistocracy-improved §5](../political-system/epistocracy-improved.md)) and *"classify by sortition so it can't be captured"* ([the-capture-test](../the-capture-test.md)).

> **Owner's ask:** *"improve the system with a positive feedback loop — as the random panel votes, the system readjusts the weights; if enough random people are in the panels, it should self-correct. Think of a mathematical algorithm that could do that."*

Good news: **this algorithm exists, it's named, and its self-correction is a theorem.** Catch: **a *pure* positive loop provably eats its own accuracy.** Fix: **add one negative-feedback term and it becomes stable.** Here is the whole thing.

## 1. Your intuition is already a theorem — the Condorcet Jury Theorem

*"If enough random people are in the panel, it self-corrects"* is **literally** the [Condorcet Jury Theorem (1785)](https://plato.stanford.edu/entries/jury-theorems/): if each voter is **(a) more likely right than wrong** (competence *p* > 0.5) and **(b) votes independently**, then the probability the **majority** is correct rises with panel size *N* and → **certainty as N → ∞**. Your instinct is mathematically sound.

But the same theorem carries two warnings you must design around:

- **It runs in reverse below 0.5.** If voters are *worse* than chance on some question (*p* < 0.5), a *bigger* panel converges to the **wrong** answer with *more* confidence. Size amplifies competence *and* incompetence.
- **It dies without independence.** If voters copy each other (herding, shared media bias), their errors correlate, the *effective* N collapses, and the guarantee evaporates ([the premises are hard to satisfy together — Dietrich](https://philsci-archive.pitt.edu/3939/1/Dietrich-CondorcetJuryTheorem.pdf)).

**This is exactly why sortition is the right substrate:** a panel of *random strangers* protects condition (b) — independence — far better than a self-selected crowd that herds. Randomness isn't just capture-resistance; it's what makes the math work.

## 2. The engine — Multiplicative Weights (the "readjust itself" loop)

The algorithm that *updates the weights from outcomes* is **Multiplicative Weights / Hedge** (Freund–Schapire; [Arora–Hazan–Kale survey](https://theoryofcomputing.org/articles/v008a006/v008a006.pdf)). Three steps per decision that has a **measurable, eventually-known outcome**:

**Step 1 — Score each member by a *proper* scoring rule.** When the outcome is known, score how right each member's position was, using the **Brier** or **logarithmic** score. "Proper" is the magic word: a scoring rule is incentive-compatible **if and only if** it is a *strictly proper* scoring rule — meaning **honest reporting is the dominant strategy**, so you *cannot* game it by misrepresenting your belief ([scoring-rule result](https://arxiv.org/pdf/1702.03615)). Brier: `loss_i = (forecast_i − outcome)²`.

**Step 2 — Update each member's weight multiplicatively:**

```
w_i  ←  w_i · exp(−η · loss_i)          then renormalize:  p_i = w_i / Σ w
```

η is a small learning rate. Being right (low loss) *raises* your weight; being wrong *lowers* it. **No central authority sets the weights — the outcomes do.** That is the capture-resistance built into the math: there is no matrix-writer to lobby ([the-capture-test](../the-capture-test.md)).

**Step 3 — Decide by weighted vote**, and repeat. The weights are now a *living* function of demonstrated track record, per domain.

**Why this is provably good:** Multiplicative Weights is a **no-regret** algorithm — over many rounds the weighted panel does **almost as well as its single best member would have**, *without knowing in advance who that is*. The system finds and rewards the competent automatically. **This is precisely the self-correcting loop you described — and it's minimax-optimal.**

## 3. The catch — a *pure* positive loop eats its own accuracy

Here is the part that must be said honestly, because it is where the naive version fails. The multiplicative update is a **"rich-get-richer" dynamic** (like preferential attachment): weight concentrates *exponentially* fast onto a few early winners. And as it concentrates:

1. the **effective panel size shrinks** (a handful of high-weight voters dominate),
2. **diversity collapses** — killing the [Hong–Page](frontier-mechanisms.md) advantage that made the crowd smart,
3. **independence collapses** — the few dominant voters tend to be correlated, which **reverses the Condorcet guarantee** from §1,
4. you have **grown a captured elite *out of the algorithm itself*** — the [super-delegate problem](frontier-mechanisms.md) the project flagged, now emerging mathematically rather than imposed.

**The feedback that rewards accuracy destroys the diversity and independence that *produced* accuracy.** A pure positive loop is unstable and self-defeating. This is the rigorous reason "just let weights compound on the winners" cannot be the whole design.

## 4. The fix — one negative-feedback term turns it into a stable controller

Tame the runaway by pulling weights gently back toward equality every round — a **reversion-to-uniform** term (a spring), so dominance must be **continuously re-earned**, never banked:

```
w_i  ←  (1 − λ) · [ w_i · exp(−η · loss_i) ]  +  λ · (1/N)
```

- **λ (reversion strength)** is the negative feedback. λ = 0 is the unstable pure loop of §3; λ → 1 is plain sortition (equal weight). A small λ keeps the system *learning* while guaranteeing no one's weight runs away — diversity and independence are preserved by construction.
- **Small learning rate η** — slow adaptation, the standard stability condition in adaptive control.
- **A hard weight cap** (entropy floor) — no individual or correlated cluster may exceed weight *c*. This is the [delegation cap the super-delegate open question was circling](frontier-mechanisms.md) — now *derived* from the stability analysis, not hand-waved.
- **Domain-locality** — weight earned on vaccines does **not** transfer to tax policy (the owner's domain-specific insight, [epistocracy-improved §5](../political-system/epistocracy-improved.md)). Prevents a single global elite.

Net: a **balanced control system** — a *positive* loop (Multiplicative Weights) that learns who is competent, plus a *negative* loop (reversion + cap) that stops it cannibalizing the diversity it needs. Stable, self-correcting, and capture-resistant because randomness seeds it and outcomes (not officials) steer it.

## 5. Honest limits (where the loop has no signal)

- **It only works on the *facts* half.** The loop needs a **measurable outcome** to score against. *Values* questions ("should we mandate it?") have no "correct" result to score ([Arrow](frontier-mechanisms.md)), so they stay **one-person-one-vote.** The algorithm weights the *empirical* sub-question only.
- **Slow-outcome questions starve it.** If you only learn whether a 30-year climate policy was right in 30 years, the feedback is too lagged to weight today's vote. Use it where outcomes arrive in months/years (public-health forecasts, budget projections), not for the deep long-run.
- **Goodhart + who picks the metric.** Whoever defines the *outcome measure* holds residual power — a smaller capture surface, re-tested per [the-capture-test](../the-capture-test.md): make the metric plural, public, and **sortition-assigned**, and it is more capture-resistant than the status quo, not less.

## 6. Verdict

Your positive-feedback instinct is right and **buildable** — it's Condorcet (self-correction from random panels) + Multiplicative Weights (outcome-driven weight updates, no-regret) + proper scoring (ungameable) — with **one essential modification**: a negative-feedback stabilizer (reversion-to-uniform + cap) without which the loop concentrates into an elite and reverses its own Condorcet guarantee. **Your loop + that stabilizer = a real mechanism**, and it closes the super-delegate open question with math instead of a caveat.

**Smallest first move:** pilot it on a narrow domain with fast, measurable outcomes — e.g. a standing sortition panel making **public-health or budget forecasts**, weights updated by Brier score with reversion λ, run against plain majority vote as the control. If the weighted panel beats the unweighted one *without* its weights concentrating, the design works.

## 7. Sources

- Condorcet Jury Theorem (conditions; reversal below 0.5; independence): [Stanford Encyclopedia of Philosophy — Jury Theorems](https://plato.stanford.edu/entries/jury-theorems/) · premises hard to co-satisfy: [Dietrich](https://philsci-archive.pitt.edu/3939/1/Dietrich-CondorcetJuryTheorem.pdf)
- Multiplicative Weights / Hedge (update rule; no-regret; minimax-optimal): [Arora, Hazan & Kale, *The Multiplicative Weights Update Method: a Meta-Algorithm*](https://theoryofcomputing.org/articles/v008a006/v008a006.pdf)
- Proper scoring rules ⇔ truthful reporting (Brier, logarithmic): [Online Prediction with Selfish Experts](https://arxiv.org/pdf/1702.03615)
- Diversity vs ability (why concentration loses the crowd's edge): [Hong & Page, PNAS 2004](frontier-mechanisms.md) · rich-get-richer concentration: preferential attachment (Barabási–Albert).
- Capture-resistance of outcome-set weights: [the-capture-test](../the-capture-test.md).
