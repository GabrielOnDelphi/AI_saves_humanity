# The capture test — "who controls X?" is comparative, not a kill shot

**Status:** Draft for debate · **Last updated:** 2026-06-30 · A **method correction** that applies to every proposal in this repo. Forced by the owner, who caught the same error three times in one session: *the project keeps using "but who controls X?" / "that's a capture surface" as a disqualifier for new ideas, while ignoring that **democracy's existing machinery has the identical surface.*** This page fixes the rule and re-audits every capture objection in the repo evenly.

## 1. The principle

There is **no system without a rule-setter.** Someone wrote the constitution, someone draws the electoral districts, someone decides who counts as a voter and what reaches the ballot, someone defines the categories the law runs on. It is the **infinite regress of authority** — *who guards the guardians?* — and it cannot be designed away. So **"it has a capture surface" cannot be an objection**: it disqualifies *everything*, democracy included.

Proof that democracy fails the naive version — from this repo's own pages:
- **Referee capture** is the headline mechanism of [#14](../problems/14-democratic-backsliding/): *"whoever controls courts, election administration, prosecution, and oversight controls outcomes."*
- **Gerrymandering** — whoever draws the map wins (the [McKelvey agenda-control theorem](beyond-democracy/frontier-mechanisms.md), live; [#14](../problems/14-democratic-backsliding/) logs Texas's mid-decade redraw).
- **The franchise itself** — Jim Crow literacy tests were a *classification* of who is "fit" to vote ([political-system](political-system/)).
- **Money** — concentrated wealth funds the capture ([#01](../problems/01-economic-inequality/)).

So the objection has to become **quantitative: whose version of the classifier is *harder to capture*?** — scored on four properties:

| Property | Capture-resistant | Capture-prone |
|---|---|---|
| **Concentration** | distributed across many bodies/cases | one body, one formula |
| **Transparency** | public, reasoned, contestable | hidden inside a metric/algorithm |
| **Reversibility** | a bad call is cheap to undo (appeal, amend) | locks in |
| **Self-correction** | being wrong costs the classifier its power | no feedback; error persists |

The verdict is then **comparative**, and when the new mechanism scores worse, that is a **design spec** (distribute it, expose it, make it reversible, make it *earned*) — **not a death sentence.** The one exception: when concentration is *irreducible* (see the AI sovereign below), the objection may genuinely be decisive.

## 2. The audit — every capture objection in the repo, re-tested evenly

| Objection (where) | Does democracy have the same surface? | Honest comparative verdict |
|---|---|---|
| **"Whoever defines 'education level' controls the electorate"** ([political-system §4](political-system/) obj #5, used as *decisive*) | **Yes** — democracy's franchise + district lines are defined by incumbents and are demonstrably captured (#14 referee capture, gerrymandering). | **Not a disqualifier.** The education-weight-matrix is *more* concentrated + invisible than districting — but that's fixable: classify by sortition, make weights public/appealable, earn them by track record. Then it can *beat* the gerrymandered status quo. See [epistocracy-improved §5](political-system/epistocracy-improved.md). |
| **"Measuring flourishing hands someone the power to define it — a Ministry of Happiness, the worst capture surface of all"** ([beyond-democracy §7/§9](beyond-democracy/), called *the strongest objection*) | **Yes** — democracy already optimises a chosen, gameable metric: **GDP** (+ "win the next election"). Nobody voted for GDP as the target; it is a captured de-facto proxy. | **Reframe the open question.** Not *"can we avoid a metric?"* (impossible — you're always optimising *something*) but *"is a plural, transparent, hard-to-fake flourishing dashboard **more** capture-resistant than the single GDP number we optimise now?"* Plausibly yes. The objection shrinks from fatal to comparative. |
| **"Whoever defines 'misinformation' defines it against opponents — a Ministry of Truth"** ([information-integrity](information-integrity/), [#10](../problems/10-information-truth/)) | **Yes, and worse** — the status quo classifier is the **platforms' opaque ad-driven algorithm**: a private, invisible, unaccountable truth-ranker already deciding what billions see. | **This proposal already passes — keep it as the template.** It deliberately chose **prebunking/inoculation, which needs *no* truth-arbiter.** That is exactly "remove the concentrated classifier" done right. The model for the rest of the repo. |
| **"Who certifies a 'comparative-religion' syllabus is balanced?"** ([#13 §5](../problems/13-religion/), open) | **Yes** — curricula are *already* certified by captured bodies: the **Texas State Board of Education approved the Bible-infused Bluebonnet curriculum 8–7** ([lessons-from-collapse](defending-democracy/lessons-from-collapse.md)). | **Comparative.** The status quo certifier is a partisan elected board. The question is whether a **sortition-based / plural / transparent** syllabus certifier is *less* capturable than that — a low bar to clear, not an impossible one. |
| **Futarchy's welfare metric; outcome-triggered auto-dissolution's threshold** ([frontier-mechanisms](beyond-democracy/frontier-mechanisms.md); [radical-options](beyond-democracy/radical-options.md) Opt 6) | **Yes** — same as flourishing: every "judge on outcomes" system needs a metric, and so does the current one (GDP, unemployment). | **Comparative, same as the flourishing row.** Harden with plurality + transparency + sortition-set thresholds; compare against the metric we already optimise. |
| **"The AI's objective + off-switch makes whoever holds them the true sovereign"** ([radical-options Opt 1](beyond-democracy/radical-options.md); [ai-and-power](ai-and-power/): *"does public AI just move power to whoever controls the state?"*) | Democracy disperses sovereignty across many hands; a single objective-setter + kill-switch holder does **not.** | **Here the objection still bites — hardest of all.** Concentration is near-*irreducible*: one objective, one kill-switch. This is the case the comparative test does **not** rescue, and it should be flagged as possibly decisive. Honesty means saying where the kill shot still kills. |

## 3. The standing rule (for every future proposal)

When you hit a *"but who controls X?"* objection, do **not** stop there. Run the four steps:

1. **Name the status quo's version of the same classifier.** (There always is one — franchise rules, districting, GDP, platform algorithms, the school board.)
2. **Score both** on the four properties (concentration · transparency · reversibility · self-correction).
3. **State the verdict comparatively** — better or worse than what we have now, not "has a surface / doesn't."
4. **If the new one is worse, treat it as a design spec** — distribute it, expose it, make it reversible, make it sortition-chosen or earned-by-track-record — *unless concentration is irreducible* (the AI sovereign), where the objection may genuinely win.

**Why this matters beyond tidiness:** the naive version of the objection is structurally **conservative** — it always favours the incumbent system, because the incumbent's capture is familiar and invisible while the newcomer's is salient. Applied evenly, the capture test stops being a reflex that protects the status quo and becomes a real tool for *choosing the less-capturable design.*

## 4. Sources & links

- The infinite regress / "who guards the guardians": classic problem of political philosophy; the impossibility-of-perfection backbone is in [frontier-mechanisms §1](beyond-democracy/frontier-mechanisms.md) (Arrow, Gibbard–Satterthwaite, McKelvey).
- Democracy's own capture, documented: [#14 referee capture + gerrymandering](../problems/14-democratic-backsliding/); [#01 money→power](../problems/01-economic-inequality/).
- The worked re-test: [epistocracy-improved §5](political-system/epistocracy-improved.md).
- The model of doing it right (no arbiter needed): [information-integrity](information-integrity/).
