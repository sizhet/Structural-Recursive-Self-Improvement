# START HERE — Structural Recursive Self-Improvement

## A 10-Minute Guide to SRSI

**Project:** Structural Recursive Self-Improvement
**Acronym:** SRSI
**Repository:** `Structural-Recursive-Self-Improvement`

---

# 1. Start with One Question

Recursive Self-Improvement is often described as:

```text id="vqn2rc"
AI
 ↓
Improves Itself
 ↓
Better AI
 ↓
Improves Itself Again
```

But this skips one of the hardest parts:

> **How does the system know that a proposed change is actually an improvement?**

More compute can generate more candidates.

Better models can generate better candidates.

Search can explore more candidates.

But recursive improvement also requires machinery that can answer:

```text id="uuvp6v"
What changed?

What improved?

What became worse?

Under which context?

What evidence supports the change?

What counter-evidence challenges it?

Can the change be localized?

Can it be reversed?

Should it be promoted?
```

This repository studies that missing infrastructure.

---

# 2. What Is SRSI?

**SRSI — Structural Recursive Self-Improvement** is a research framework for making recursive improvement:

* evaluable,
* falsifiable,
* localizable,
* auditable,
* cumulative,
* reversible,
* governable.

Its central thesis is:

> **Recursive self-improvement is not merely recursive generation under increasing compute. It is recursive generation under rich evaluation, counter-evidence, structural localization, cumulative memory, verification, and governed promotion.**

---

# 3. The Minimal SRSI Loop

The shortest useful version of SRSI is:

```text id="1s3hge"
Generate
   ↓
Evaluate
   ↕
Counter-Evaluate
   ↓
Compare
   ↓
Localize
   ↓
Verify
   ↓
Govern
   ↓
Deploy
   ↓
Observe
   ↓
Fold
   ↓
Generate Again
   ↺
```

This loop is the core of the entire repository.

---

# 4. The Five SRSI Pillars

## Pillar 1 — Rich Evaluation

A candidate should not be judged only by one score.

The evaluator should ask:

```text id="vn9nqd"
What changed?

Where?

Under what context?

What regressed?

What uncertainty remains?
```

The goal is not merely a scalar reward.

The goal is:

> **machine-operable improvement judgment.**

---

## Pillar 2 — Counter-Evidence

Every important improvement claim should face structured challenge.

Instead of asking only:

> Why is B better than A?

also ask:

> **Why might B not actually be better than A?**

Counter-Evidence Search looks for:

* failure contexts,
* regressions,
* counterexamples,
* incompatibilities,
* long-horizon instability,
* evaluator exploitation.

---

## Pillar 3 — Localization

Self-improvement does not need to mean whole-system replacement.

Instead of:

```text id="cg3n03"
System A
   ↓
System B
```

SRSI can do:

```text id="ma4x7c"
Node N
  ↓
Node N'
```

followed by local and integration verification.

This is:

> **Localized RSI**

---

## Pillar 4 — Structural Memory

A recursive improvement system should remember:

```text id="y8w9ug"
what worked

what failed

where

under which context

which evaluator was wrong

which counter-evidence mattered
```

Validated and rejected improvements become reusable structural memory.

---

## Pillar 5 — Improvement Governance

A candidate can be technically better without deserving immediate global deployment.

SRSI separates:

```text id="k0hm4p"
Candidate Capability
        ≠
Validated Improvement
        ≠
Authorized Promotion
        ≠
Authorized Action
```

Possible outcomes include:

```text id="1y1hql"
PROMOTE

LOCAL-ONLY

BRANCH

EXPERIMENTAL

LEFTOVER

REJECT

ROLLBACK
```

---

# 5. Why Rich Evaluators Matter

Suppose:

```text id="4m3qp7"
Score(A) = 0.82
Score(B) = 0.89
```

A simple optimizer concludes:

```text id="th0sn8"
B wins.
```

But SRSI asks:

```text id="dwfu69"
Where did B improve?

Where did B regress?

What context produced the gain?

Did B exploit the evaluator?

Does B generalize?

Should B replace A globally?
```

This is the difference between:

> **optimization**

and:

> **validated improvement**

---

# 6. The Evaluator Bottleneck

As AI becomes better at generating candidates:

```text id="k2nydx"
Generation Capacity ↑↑↑
```

the system may eventually face:

```text id="lkokhk"
Evaluation Capacity ↑
```

This creates a possible:

# **Evaluator Bottleneck**

The key hypothesis is:

> **As candidate generation becomes abundant, trustworthy machine-operable evaluation may become relatively more scarce and valuable.**

This is one of the central ideas of the SRSI project.

---

# 7. Anti-Goodhart RSI

A strong optimizer learns what its evaluator rewards.

If the evaluator is imperfect:

```text id="5jqo4u"
Evaluator Objective
        ≠
Intended Objective
```

then stronger optimization can amplify the mismatch.

SRSI therefore does not rely only on a primary evaluator.

It adds:

```text id="5brl90"
Primary Evaluation
        ↕
Counter-Evaluation
        ↓
Structural Comparison
        ↓
Verification
        ↓
Governance
```

The guiding principle is:

> **The stronger the optimizer becomes, the stronger its challenger must become.**

---

# 8. Two-Way CCC

Two-Way CCC is one of the main DBM-SI mechanisms used in SRSI.

Instead of:

```text id="f51p9w"
A vs. B
   ↓
Winner
```

it preserves:

```text id="b8t4lg"
Shared Structure

A-Specific Strength

B-Specific Strength

A-Specific Failure

B-Specific Failure

Context Difference

Unresolved Difference
```

This allows:

```text id="k11ljz"
PROMOTE

REJECT

BRANCH

LOCALIZE

LEFTOVER
```

and supports the principle:

> **Self-improvement does not have to mean self-replacement.**

---

# 9. Localized RSI

A large system may contain:

```text id="q3kn1j"
System
├── N1
├── N2
├── N3
└── N4
```

If runtime evidence identifies `N3` as the problem, SRSI can perform:

```text id="ek3gzq"
N3
 ↓
Generate N3'
 ↓
Evaluate
 ↓
Counter-Evaluate
 ↓
Verify Integration
 ↓
Promote Locally
```

This reduces:

* search space,
* evaluator cost,
* regression surface,
* rollback complexity.

Localized RSI is one of the most practical paths toward recursive improvement.

---

# 10. Structural Growth

Traditional RSI is often imagined as:

```text id="a6uvn0"
A → B → C → D
```

SRSI also allows:

```text id="kuxk3f"
        Root
      /  |  \
     A   B   C
        / \
      B1  B2
```

This supports:

* specialization,
* context-bound improvement,
* branch preservation,
* continual structural growth.

The deeper concept is:

> **Recursive Structural Differentiation and Growth**

---

# 11. Leftover

Not every candidate must be accepted or rejected.

SRSI includes:

```text id="vojq4r"
LEFTOVER
```

for unresolved candidates.

This means:

> preserve the candidate and its evidence without forcing a premature decision.

Later evidence can trigger re-evaluation.

Leftover is important because uncertainty itself should remain explicit.

---

# 12. DBM-SI as One SRSI Provider

SRSI is an open framework.

DBM-SI is one concrete provider of structural mechanisms.

| DBM-SI Structure        | SRSI Role                  |
| ----------------------- | -------------------------- |
| MDT                     | Differential evaluation    |
| CCC                     | Structural consistency     |
| Two-Way CCC             | Structural A/B             |
| Counter-Evidence        | Falsification              |
| UTN                     | Identity / compatibility   |
| CallingGraph            | Behavioral-path evaluation |
| CG Delta                | Change-impact evaluation   |
| Trajectory Intelligence | Long-horizon evaluation    |
| Per-Node Intelligence   | Localized RSI              |
| Structural Search       | Improvement localization   |
| Structural Folding      | Improvement memory         |
| Leftover                | Explicit uncertainty       |
| 3-Cat Learning          | Structural growth          |
| PDS                     | Improvement governance     |

The important point is:

> **DBM-SI is one possible provider of SRSI infrastructure, not the exclusive route.**

---

# 13. The Recommended Reading Order

If you want the full argument, read the six core papers in order.

## 1. SRSI-001 — From Recursive Self-Improvement to Structural RSI

Start here for the main framing.

Core idea:

> RSI should be treated as a structured improvement problem, not merely a recursive generation problem.

---

## 2. SRSI-002 — Rich Evaluators: The Missing Infrastructure of RSI

Read this for:

* Evaluator Bottleneck,
* Evaluator Richness,
* Evaluator Plane,
* Evaluator Portfolio,
* Evaluator-of-Evaluators.

Core question:

> **How rich must the evaluator become before we can trust what the generator calls improvement?**

---

## 3. SRSI-003 — DBM-SI as a Rich Evaluator and Improvement Infrastructure

Read this for the concrete mapping from Structural Intelligence into RSI.

Core idea:

> Structures built for intelligence can also become structures for improving intelligence.

---

## 4. SRSI-004 — Two-Way CCC, Counter-Evidence, and Anti-Goodhart RSI

Read this for:

* structural A/B,
* falsification,
* evaluator contest,
* Anti-Goodhart architecture.

Core principle:

> **Every powerful improvement engine needs a powerful falsification engine.**

---

## 5. SRSI-005 — Localized RSI, Structural Growth, and Improvement Governance

Read this for:

* Per-Node RSI,
* Branch,
* Leftover,
* selective deployment,
* rollback,
* Improvement Governance.

Core principle:

> **Self-improvement does not have to mean self-replacement. It can mean recursive structural growth.**

---

## 6. SRSI-006 — The AI-SI-RSI Gold Rush

Read this for the broader research and industry thesis.

Core hypothesis:

> **The next scarce AI resource may be trustworthy machine-operable judgment.**

---

# 14. If You Only Have Five Minutes

Read these three sections:

```text id="km0w43"
README
  ↓
SRSI-001 Abstract + Central Thesis
  ↓
SRSI-002 Abstract + Evaluator Bottleneck
```

Then look at:

```text id="efhnmj"
Fig-001 — SRSI Grand Map

Fig-003 — Structural RSI Loop

Fig-005 — AI-SI-RSI Gold Rush
```

That gives the shortest path to the core thesis.

---

# 15. If You Are an AI Engineer

Focus on:

```text id="u0q9w6"
SRSI-002
SRSI-004
SRSI-005
```

Key engineering questions:

```text id="fzz0ao"
How do I evaluate AI-generated changes?

How do I search for regressions?

How do I localize improvement?

How do I stage promotion?

How do I roll back?

How do I preserve improvement history?
```

---

# 16. If You Work on AI Coding

Start with:

```text id="22jcpi"
SRSI-003
   ↓
SRSI-004
   ↓
SRSI-005
```

The canonical coding loop is:

```text id="6e136c"
LLM Generates Code Delta
        ↓
Compile
        ↓
Tests
        ↓
CallingGraph Delta
        ↓
Counter-Evidence
        ↓
Runtime Evaluation
        ↓
Promotion Gate
        ↓
Fold Result
        ↓
Next Candidate
```

AI coding is likely one of the best early SRSI MET domains because evaluators are already highly machine-operable.

---

# 17. If You Work on AI Safety or Governance

Focus on:

```text id="kjjkgj"
SRSI-001
SRSI-004
SRSI-005
```

Key distinctions:

```text id="y3us1s"
Capability
   ≠
Validated Improvement
   ≠
Promotion Authority
   ≠
Action Authority
```

Important topics include:

* Anti-Goodhart evaluation,
* evaluator diversity,
* improvement authority,
* staged deployment,
* rollback,
* meta-governance.

---

# 18. If You Work on RSI Theory

Focus on:

```text id="zfcrzh"
SRSI-001
SRSI-002
SRSI-006
```

The main theoretical shift is:

```text id="45okgs"
Recursive Generation
        ↓
Recursive Improvement Infrastructure
```

The core hypothesis is that RSI may depend as much on improvement judgment as on improvement generation.

---

# 19. If You Work on Structural Intelligence

Read:

```text id="qonp2s"
SRSI-003
```

first.

It shows how:

```text id="dk7niw"
MDT

CCC

UTN

CallingGraph

Trajectory

Per-Node Intelligence

Folding

PDS
```

can be reinterpreted as:

```text id="xqrmzh"
Evaluators

Localization

Memory

Governance
```

for recursive improvement.

---

# 20. The Five Core Figures

## Fig-001 — SRSI Grand Map

Use this as the visual overview of the whole project.

## Fig-002 — Rich Evaluator Plane

Use this to understand the transition from simple scalar evaluation to richer improvement judgment.

## Fig-003 — Structural RSI Loop

Use this to understand the recursive runtime.

## Fig-004 — Two-Way CCC and Counter-Evidence RSI

Use this to understand Anti-Goodhart SRSI.

## Fig-005 — AI-SI-RSI Gold Rush

Use this to understand the broader research and engineering thesis.

---

# 21. A Minimal SRSI Experiment

You do not need AGI to test SRSI.

A Minimum Engineering Test can be:

```text id="g0kyyy"
Baseline
  ↓
Generate 10 Candidates
  ↓
Evaluate
  ↓
Search Counter-Evidence
  ↓
Promote One Local Candidate
  ↓
Observe Runtime
  ↓
Fold Result
  ↓
Use Folded Result in Next Cycle
```

Then ask:

```text id="b61uhm"
Did the next cycle improve?

Did the evaluator become more reliable?

Did memory reduce search cost?

Did localization reduce regression?
```

These are measurable questions.

---

# 22. SRSI Before AGI

A central position of this project is:

> **RSI does not need to wait for AGI.**

Domain-specific recursive improvement can begin whenever there is:

```text id="ozsydn"
Candidate Generation
+
Machine-Operable Evaluation
+
Search
+
Feedback
+
Memory
```

Potential domains include:

* AI coding,
* scientific reasoning,
* engineering design,
* manufacturing,
* decision systems,
* market intelligence.

---

# 23. The AI-SI-RSI Gold Rush

The repository ends with a broader hypothesis.

The history of AI has repeatedly shifted scarcity:

```text id="4p5up5"
Data
 ↓
Models
 ↓
Compute
 ↓
Foundation Models
 ↓
Agents
 ↓
?
```

SRSI proposes that one possible next scarce asset is:

> **trustworthy machine-operable judgment.**

This could create demand for:

```text id="0i8vj8"
Evaluator Engineering

Evaluator Packs

Evaluator Routing

Evaluator Security

Evaluator Benchmarking

Structural Search

Improvement Memory

Improvement Runtime
```

This is the meaning of the AI-SI-RSI Gold Rush.

---

# 24. What SRSI Does Not Claim

SRSI does not claim:

* AGI is imminent,
* intelligence explosion is inevitable,
* RSI will automatically be safe,
* RSI will automatically be dangerous,
* DBM-SI is the only valid architecture,
* Rich Evaluators eliminate all risk,
* a complete autonomous RSI system already exists.

SRSI v1.0 is:

> **a research framework, structural hypothesis, and engineering direction.**

---

# 25. Three Things to Remember

If you remember only three things from this repository, remember these:

## 1.

> **Generation is not improvement.**

A candidate becomes improvement only after evaluation, challenge, verification, and governance.

## 2.

> **The stronger the optimizer becomes, the stronger its evaluator and counter-evaluator must become.**

Otherwise recursive optimization can recursively amplify evaluator weakness.

## 3.

> **Self-improvement does not have to mean self-replacement.**

It can mean:

```text id="le84ew"
localize
 ↓
improve
 ↓
branch
 ↓
verify
 ↓
govern
 ↓
fold
```

and grow structurally over time.

---

# 26. The One-Line SRSI Thesis

> **Recursive Self-Improvement should be treated as a governed structural improvement loop built from rich evaluation, counter-evidence, localization, verification, memory, and selective promotion.**

---

# 27. The Core Research Question

> **What computational structures make recursive improvement evaluable, falsifiable, localizable, auditable, cumulative, reversible, and governable?**

That is the question this repository is built to explore.

---

# Next

Continue with:

**[`docs/SRSI-001-From-Recursive-Self-Improvement-to-Structural-RSI.md`](docs/SRSI-001-From-Recursive-Self-Improvement-to-Structural-RSI.md)**

For the complete document map:

**[`CONTENTS.md`](CONTENTS.md)**

For figures:

**[`FIGURE-INDEX.md`](FIGURE-INDEX.md)**

For terminology:

**[`GLOSSARY.md`](GLOSSARY.md)**

For future research directions:

**[`FUTURE-DIRECTIONS.md`](FUTURE-DIRECTIONS.md)**
