# GitHub Release Notes — v1.0.0

## Structural Recursive Self-Improvement

### DBM-SI as a Rich Evaluator and Improvement Infrastructure

**Release:** `v1.0.0`
**Project:** Structural Recursive Self-Improvement
**Acronym:** SRSI
**Repository:** `Structural-Recursive-Self-Improvement`

---

# What If the Bottleneck of RSI Is Not Generation, but Evaluation?

AI systems are becoming increasingly capable of generating:

* code,
* strategies,
* hypotheses,
* plans,
* designs,
* alternative solutions,
* candidate improvements.

But Recursive Self-Improvement requires something more fundamental:

> **How does the system determine that a proposed change is actually an improvement?**

Generating more candidates is not enough.

A candidate becomes a meaningful improvement only when the system can determine:

```text id="szpk6j"
What improved?

Where?

Under which context?

Compared with what?

At what cost?

What regressed?

What counter-evidence exists?

What uncertainty remains?

Should the change be promoted?

Where should it be deployed?

Can it be rolled back?
```

SRSI v1.0.0 begins from this problem.

---

# Introducing Structural Recursive Self-Improvement

**Structural Recursive Self-Improvement (SRSI)** studies the computational infrastructure required to make recursive improvement:

```text id="tsry94"
Evaluable

Falsifiable

Localizable

Auditable

Cumulative

Reversible

Governable
```

The central thesis is:

> **Recursive self-improvement is not merely recursive generation under increasing compute. It is recursive generation under rich evaluation, counter-evidence, structural localization, cumulative memory, verification, and governed promotion.**

---

# The Structural RSI Loop

A more complete recursive improvement process can be represented as:

```text id="8dwvj3"
Candidate Generation
        ↓
Rich Evaluation
        ↕
Counter-Evidence
        ↓
Structural Comparison
        ↓
Localization
        ↓
Verification
        ↓
Improvement Governance
        ↓
Selective Deployment
        ↓
Runtime Observation
        ↓
Structural Folding
        ↓
Improvement Memory
        ↓
Next Improvement Cycle
        ↺
```

This changes the central RSI question from:

> How can an AI generate a better version of itself?

toward:

> **What computational structures allow an intelligent system to determine whether a candidate deserves to become a validated, authorized, and reusable improvement?**

---

# Five Pillars of SRSI

SRSI v1.0.0 is organized around five core pillars.

## 1. Rich Evaluation

Determine not merely whether a candidate scored higher, but:

* what changed,
* where it improved,
* where it regressed,
* under which context,
* with what evidence,
* with what uncertainty.

---

## 2. Counter-Evidence

Actively search for reasons why an apparent improvement may not be genuine.

> **Every powerful improvement engine needs a powerful falsification engine.**

---

## 3. Localization

Identify where improvement should occur before attempting broad replacement.

```text id="8cdqpk"
Locate
  ↓
Improve Locally
  ↓
Verify Structurally
```

---

## 4. Structural Memory

Preserve validated and rejected improvement experience so future cycles do not repeatedly search from scratch.

---

## 5. Improvement Governance

Separate technical improvement from authority to promote and deploy it.

```text id="xktldh"
Candidate Capability
        ≠
Validated Improvement
        ≠
Authorized Promotion
        ≠
Authorized Action
```

---

# Rich Evaluators

One of the central proposals of this release is the **Rich Evaluator**.

A conventional evaluator may produce:

```text id="wy3vdl"
Candidate B = 0.91
```

A Rich Evaluator attempts to preserve a more useful improvement structure:

```text id="zft19p"
Difference

Context

Evidence

Counter-Evidence

Regression

Structural Impact

Trajectory

Uncertainty

Policy

Deployment Scope
```

This leads to the **Evaluator Bottleneck Hypothesis**:

> As AI candidate generation becomes increasingly abundant, reliable machine-operable evaluation may become a major constraint on recursive improvement.

Or more compactly:

> **Compute determines how hard RSI can search. Evaluators determine what RSI learns to become.**

---

# Anti-Goodhart RSI

A stronger optimizer can become better at exploiting weaknesses in its own evaluators.

SRSI therefore treats evaluator weakness as a recursive systems problem.

The release introduces an Anti-Goodhart architecture built around:

```text id="xcridg"
Primary Evaluation
        ↕
Counter-Evaluation
        ↓
Structural A/B
        ↓
Counter-Evidence Search
        ↓
Cross-Perspective Evaluation
        ↓
Verification
        ↓
Governed Promotion
```

The objective is not to claim a perfect evaluator.

It is to make improvement increasingly:

> **contestable, falsifiable, and structurally inspectable.**

---

# Two-Way CCC and Structural A/B

SRSI reinterprets **Two-Way CCC** as one possible structural comparison primitive.

Instead of:

```text id="bxb35x"
A vs. B
   ↓
Winner
```

the comparison can preserve:

```text id="vd20xc"
Shared Structure

A-Specific Strength

B-Specific Strength

Regression

Context Difference

Unresolved Difference
```

The result can therefore be:

```text id="gbp8dx"
PROMOTE

REJECT

BRANCH

LOCALIZE

LEFTOVER
```

This is important because an improvement in one context does not necessarily justify global replacement.

---

# Self-Improvement Does Not Have to Mean Self-Replacement

A major SRSI proposition is:

> **Self-improvement does not have to mean self-replacement. It can mean recursive structural growth.**

Instead of:

```text id="s1j7pt"
A → B → C → D
```

recursive improvement may produce:

```text id="lrrvn6"
        A
      / | \
    B1  B2  B3
        |
       B2.1
```

with runtime dispatch selecting the appropriate structure according to context.

This leads naturally to:

# **Localized RSI**

and:

# **Per-Node RSI**

---

# DBM-SI as One Structural Provider

This release also reinterprets existing DBM-SI mechanisms as possible components of an SRSI infrastructure.

| DBM-SI Structure        | Possible SRSI Role                 |
| ----------------------- | ---------------------------------- |
| MDT                     | Differential evaluator             |
| CCC                     | Structural consistency evaluator   |
| Two-Way CCC             | Structural A/B evaluator           |
| Counter-Evidence Search | Falsification evaluator            |
| UTN                     | Identity / compatibility evaluator |
| CallingGraph            | Behavioral-path evaluator          |
| CallingGraph Delta      | Change-impact evaluator            |
| Trajectory Intelligence | Long-horizon evaluator             |
| Per-Node Intelligence   | Localized improvement              |
| Structural Search       | Improvement localization           |
| Structural Folding      | Improvement memory                 |
| Leftover                | Explicit unresolved state          |
| 3-Cat Learning          | Structural growth                  |
| PDS                     | Improvement governance             |

DBM-SI is presented as:

> **one concrete family of structural mechanisms from which SRSI infrastructure can begin to be explored — not as the exclusive architecture for recursive self-improvement.**

---

# RSI Before AGI

SRSI does not require waiting for a hypothetical fully general self-improving AI.

Many domains already contain:

```text id="uz20m4"
Candidate Generator

Machine-Operable Evaluators

Search

Runtime Feedback

Memory
```

This means recursive improvement can potentially be studied experimentally today.

One particularly promising domain is:

# **AI Coding**

because software already provides rich evaluation infrastructure:

```text id="vz7d9v"
Compiler

Unit Tests

Integration Tests

Static Analysis

CallingGraph

CallingGraph Delta

Runtime Trace

Performance

Security
```

A future SRSI Minimum Engineering Test could therefore run:

```text id="5g9oua"
LLM Code Delta
      ↓
Compile
      ↓
Tests
      ↓
CallingGraph Delta
      ↓
Counter-Evidence
      ↓
Runtime Verification
      ↓
Promotion Gate
      ↓
Structural Folding
```

---

# The AI-SI-RSI Gold Rush

SRSI v1.0.0 also introduces a broader research hypothesis:

# **The AI-SI-RSI Gold Rush**

As candidate generation becomes increasingly abundant, a new scarcity may emerge around:

```text id="1jzw1q"
Rich Evaluators

Counter-Evaluators

Structural Search

Evaluator Packs

Improvement Memory

Improvement Runtimes

Trusted Machine-Operable Judgment
```

This suggests three possible engineering fronts:

```text id="2wm8pv"
Evaluator Rush
      ↓
Structural Search Rush
      ↓
Improvement Runtime Rush
```

The hypothesis is intentionally exploratory.

It does **not** claim that:

* AGI is imminent,
* intelligence explosion is inevitable,
* evaluators eliminate RSI risk,
* every domain can be recursively optimized,
* more compute automatically produces genuine improvement.

Instead, it asks:

> **What happens when powerful AI generation meets machine-operable structural judgment and closed improvement loops?**

---

# Included in v1.0.0

This release contains six core research papers.

### SRSI-001

**From Recursive Self-Improvement to Structural RSI**

Foundational framing of Structural Recursive Self-Improvement.

### SRSI-002

**Rich Evaluators: The Missing Infrastructure of RSI**

Evaluator Bottleneck, Evaluator Richness, Evaluator Plane, and evaluator-centered RSI.

### SRSI-003

**DBM-SI as a Rich Evaluator and Improvement Infrastructure**

Structural mapping of DBM-SI mechanisms into possible SRSI roles.

### SRSI-004

**Two-Way CCC, Counter-Evidence, and Anti-Goodhart RSI**

Structural A/B, falsification, evaluator contest, and Anti-Goodhart recursive improvement.

### SRSI-005

**Localized RSI, Structural Growth, and Improvement Governance**

Per-Node RSI, branching, Leftover, selective promotion, rollback, and governance.

### SRSI-006

**The AI-SI-RSI Gold Rush**

Evaluator Engineering, Structural Search, Improvement Runtimes, Evaluator Economy, and Collective Recursive Improvement.

---

# Five Core Figures

The release also includes five canonical figures:

```text id="pck7lm"
Fig-001 — SRSI Grand Map

Fig-002 — Rich Evaluator Plane

Fig-003 — Structural RSI Loop

Fig-004 — Two-Way CCC and Counter-Evidence RSI

Fig-005 — AI-SI-RSI Gold Rush
```

Their visual progression is:

```text id="6ovfgw"
Framework
   ↓
Evaluation
   ↓
Runtime
   ↓
Falsification
   ↓
Frontier
```

---

# Repository Navigation

Start with:

[`README.md`](README.md)

For a 10-minute introduction:

[`START-HERE.md`](START-HERE.md)

For the complete repository map:

[`CONTENTS.md`](CONTENTS.md)

For terminology:

[`GLOSSARY.md`](GLOSSARY.md)

For figures:

[`FIGURE-INDEX.md`](FIGURE-INDEX.md)

For future research:

[`FUTURE-DIRECTIONS.md`](FUTURE-DIRECTIONS.md)

---

# What v1.0.0 Does Not Claim

SRSI v1.0.0 is a:

```text id="urjczb"
Research Framework

Structural Proposal

Engineering Hypothesis

Research Direction
```

It is **not** presented as:

* a completed autonomous RSI system,
* a production self-improvement runtime,
* a proof of intelligence explosion,
* a complete solution to Goodhart's Law,
* a guarantee of safe recursive improvement,
* an exhaustive architecture for RSI.

The objective of this release is to establish a computational framing that can be tested through subsequent engineering experiments.

---

# Next Research Phase

The next stage is expected to move from:

```text id="7v82q8"
Framework
```

toward:

```text id="0ipgs4"
Minimum Engineering Tests
```

with priority directions including:

```text id="v7zb8g"
AI Coding SRSI
        ↓
Rich Evaluator Benchmark
        ↓
Counter-Evidence Runtime
        ↓
Localized / Per-Node RSI
        ↓
Structural Improvement Memory
        ↓
Improvement Governance
        ↓
Recursive Evaluator Improvement
```

---

# Core Research Question

> **What computational structures make recursive improvement evaluable, falsifiable, localizable, auditable, cumulative, reversible, and governable?**

---

# Final Perspective

The conventional image of Recursive Self-Improvement often emphasizes a system becoming increasingly capable of generating better successors.

SRSI proposes another way to look at the problem.

The decisive infrastructure may not be generation alone.

It may be the machinery capable of determining:

```text id="w44xwy"
what improved

what failed

what changed

what remained uncertain

what should be preserved

what should be challenged

what may be promoted

what must remain reversible
```

Therefore:

> **Generation proposes change. Evaluation determines whether the change deserves to become improvement.**

And:

> **Compute determines how hard RSI can search. Evaluators determine what RSI learns to become.**

SRSI v1.0.0 begins from that distinction.
