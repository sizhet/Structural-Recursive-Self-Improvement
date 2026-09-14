# Changelog

All notable changes to the **Structural Recursive Self-Improvement (SRSI)** project will be documented in this file.

The format is inspired by **Keep a Changelog**, with project-specific adaptations for a research repository.

This project uses semantic-style release numbering for major research milestones.

---

## [Unreleased]

### Planned

* Rich Evaluator Minimum Engineering Tests
* AI Coding SRSI runtime experiments
* Counter-Evidence runtime experiments
* Localized / Per-Node RSI experiments
* Evaluator benchmarking
* Structural Improvement Memory experiments
* Improvement Governance experiments
* Recursive Evaluator Improvement
* domain-specific Evaluator Packs
* SRSI benchmark design

These items represent research directions and are not part of the current implemented release.

---

# [1.0.0] — 2026-09-14

## Initial Public Research Framework

Version `1.0.0` establishes the initial research framework for:

# **Structural Recursive Self-Improvement**

The release introduces SRSI as a structural approach to Recursive Self-Improvement centered on:

```text id="b4pc6m"
Rich Evaluation
        +
Counter-Evidence
        +
Structural Localization
        +
Verification
        +
Structural Memory
        +
Improvement Governance
```

The central thesis of the release is:

> **Recursive self-improvement is not merely recursive generation under increasing compute. It is recursive generation under rich evaluation, counter-evidence, structural localization, cumulative memory, verification, and governed promotion.**

---

## Added — Core Research Framework

Introduced the concept of **Structural Recursive Self-Improvement (SRSI)**.

Defined a canonical structural improvement loop:

```text id="4wx4a1"
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

Established five core SRSI pillars:

1. Rich Evaluation
2. Counter-Evidence
3. Localization
4. Structural Memory
5. Improvement Governance

---

## Added — Evaluator Bottleneck

Introduced the **Evaluator Bottleneck Hypothesis**.

The hypothesis proposes that as AI candidate-generation capability becomes increasingly abundant, reliable machine-operable evaluation may become a relatively important constraint on recursive improvement.

Conceptually:

```text id="9nq0kv"
Generation Capacity ↑↑↑
          ↓
Candidate Volume ↑↑↑
          ↓
Evaluation Demand ↑↑↑
```

---

## Added — Rich Evaluators

Introduced **Rich Evaluators** as evaluation structures that preserve more improvement-relevant information than scalar scores alone.

Evaluation dimensions include:

* structural difference,
* context,
* evidence,
* counter-evidence,
* regression,
* trajectory,
* uncertainty,
* policy,
* deployment scope,
* auditability.

Introduced related concepts including:

* Evaluator Richness
* Evaluator Plane
* Evaluator Portfolio
* Evaluator Composition
* Evaluator Routing
* Evaluator Packs
* Evaluator-of-Evaluators
* Evaluator Engineering

---

## Added — Anti-Goodhart RSI

Introduced the concept of the:

# **RSI Goodhart Amplifier**

to describe the possibility that recursive optimization can recursively amplify weaknesses in its own evaluation machinery.

Added an Anti-Goodhart SRSI architecture based on:

```text id="atkhj5"
Primary Evaluation
        ↕
Counter-Evaluation
        ↓
Structural Comparison
        ↓
Cross-Perspective Evaluation
        ↓
Verification
        ↓
Governance
```

Established the principle:

> **Every powerful improvement engine needs a powerful falsification engine.**

---

## Added — Counter-Evidence Search

Integrated **Counter-Evidence Search** into the SRSI improvement loop.

Counter-Evidence Search actively investigates:

* regressions,
* failure contexts,
* counterexamples,
* structural incompatibility,
* trajectory instability,
* evaluator exploitation.

Counter-evidence is treated as reusable improvement information rather than discarded negative output.

---

## Added — Two-Way CCC for Structural A/B

Reinterpreted **Two-Way CCC** as a possible structural A/B mechanism for recursive improvement.

Instead of reducing candidate comparison to:

```text id="6c4d9q"
A vs. B
   ↓
Winner
```

the framework preserves:

```text id="5vvhbb"
Shared Structure

A-Specific Structure

B-Specific Structure

Regression

Context Difference

Unresolved Difference
```

This supports richer outcomes:

```text id="7fvtpt"
PROMOTE

REJECT

BRANCH

LOCALIZE

LEFTOVER
```

---

## Added — Localized RSI

Introduced **Localized Recursive Self-Improvement**.

Rather than requiring whole-system replacement:

```text id="nznuw9"
System A
    ↓
System B
```

SRSI allows improvement at localized structural units:

```text id="3i4axm"
Node N
  ↓
Node N'
```

followed by integration verification and governed promotion.

Established the principle:

> **Improve locally, verify structurally, govern promotion, and preserve the path back.**

---

## Added — Per-Node RSI

Connected Localized RSI with **Per-Node Intelligence**.

Proposed that individual structural nodes may maintain or access:

* local evaluators,
* local memory,
* local candidate histories,
* local policies,
* local improvement states.

This provides a possible substrate for distributed recursive improvement.

---

## Added — Recursive Structural Growth

Introduced **Recursive Structural Differentiation and Growth** as an alternative to whole-system recursive replacement.

Instead of:

```text id="bcs3wd"
A → B → C
```

SRSI can preserve:

```text id="d42zh8"
       Root
      / |  \
     A  B   C
       / \
      B1 B2
```

Established the principle:

> **Self-improvement does not have to mean self-replacement. It can mean recursive structural growth.**

---

## Added — Leftover

Introduced **Leftover** as an explicit improvement state for unresolved candidates.

A candidate may contain:

```text id="ysc6j7"
Positive Evidence
        +
Significant Counter-Evidence
        +
High Uncertainty
        ↓
LEFTOVER
```

This preserves uncertainty for later re-evaluation instead of forcing premature promotion or rejection.

---

## Added — Structural Improvement Memory

Introduced **Improvement Memory** as a cumulative record of:

* candidates,
* structural differences,
* contexts,
* evidence,
* counter-evidence,
* evaluator judgments,
* promotion decisions,
* runtime outcomes,
* rollback outcomes.

Connected Structural Folding and Unfolding to recursive improvement.

Conceptually:

```text id="dktbqe"
Improve
   ↓
Validate
   ↓
Observe
   ↓
Fold
   ↓
Reuse
   ↓
Improve Again
```

---

## Added — Negative Improvement Memory

Explicitly recognized failed and rejected candidates as reusable structural intelligence.

Negative Improvement Memory can preserve:

```text id="bq17ak"
What failed?

Why?

Under which context?

Which evaluator was fooled?

Which counter-evidence mattered?
```

---

## Added — Improvement Governance

Introduced **Improvement Governance** as a layer distinct from technical evaluation.

Established the relation:

```text id="7qxgwj"
Candidate Capability
        ≠
Validated Improvement
        ≠
Authorized Promotion
        ≠
Authorized Action
```

Defined candidate governance states including:

* PROMOTE-GLOBAL
* PROMOTE-LOCAL
* BRANCH
* EXPERIMENTAL
* SHADOW
* HOLD
* LEFTOVER
* REJECT
* ROLLBACK

---

## Added — PDS as Promotion Control Plane

Reinterpreted **PDS — Policy Decision System** as one possible SRSI:

* Promotion Control Plane,
* Improvement Governance Plane,
* policy evaluation mechanism.

This extends governance from action authorization toward improvement authorization.

---

## Added — DBM-SI Structural Mapping

Mapped existing DBM-SI structures into possible SRSI roles.

| DBM-SI Structure        | SRSI Role                          |
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
| DNA Dispatch / Trigger  | Evaluator / candidate routing      |
| Structural Folding      | Improvement memory                 |
| Leftover                | Explicit unresolved state          |
| 3-Cat Learning          | Structural growth                  |
| PDS                     | Improvement governance             |

The release explicitly treats DBM-SI as **one possible structural provider**, not as the exclusive SRSI architecture.

---

## Added — RSI Before AGI

Introduced the proposition that domain-specific recursive improvement can be studied before general AGI.

A minimal domain-specific loop may require:

```text id="bfn6x4"
Candidate Generator
        +
Machine-Operable Evaluators
        +
Search
        +
Feedback
        +
Memory
```

Potential early domains identified include:

* AI coding,
* scientific reasoning,
* engineering,
* manufacturing,
* decision systems,
* market intelligence.

---

## Added — AI Coding SRSI Direction

Identified AI coding as a strong candidate for an early SRSI Minimum Engineering Test because software already provides machine-operable evaluators such as:

* compilers,
* unit tests,
* integration tests,
* static analysis,
* CallingGraph,
* CallingGraph Delta,
* runtime traces,
* benchmarks,
* security analysis.

Proposed conceptual loop:

```text id="v5nq72"
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

No complete AI Coding SRSI runtime is claimed in this release.

---

## Added — Scientific Recursive Self-Improvement

Introduced a possible Scientific RSI pattern:

```text id="2rw2wz"
Hypothesis
   ↓
Experiment
   ↓
Evidence
   ↕
Counter-Evidence
   ↓
Replication
   ↓
Structural Judgment
   ↓
Knowledge Folding
   ↓
Next Hypothesis
```

This is presented as a future research direction rather than a completed implementation.

---

## Added — AI-SI-RSI Gold Rush

Introduced the **AI-SI-RSI Gold Rush** as a research and engineering hypothesis.

The concept proposes that as candidate generation becomes more abundant, increasing value may shift toward:

* Rich Evaluators,
* Counter-Evaluators,
* Evaluator Packs,
* Structural Search,
* Improvement Memory,
* Improvement Runtimes,
* trustworthy machine-operable judgment.

Established the hypothesis:

> **The next scarce AI resource may be trustworthy machine-operable judgment.**

---

## Added — Evaluator Economy

Introduced the possible future concept of an **Evaluator Economy** involving:

* evaluator providers,
* Evaluator Packs,
* evaluator benchmarking,
* evaluator security,
* evaluator routing,
* evaluator certification,
* evaluator reputation.

This is presented as a research hypothesis rather than an established industry category.

---

## Added — Structural Improvement Capital

Introduced **Structural Improvement Capital** as accumulated reusable experience derived from:

* validated improvements,
* rejected candidates,
* counterexamples,
* evaluator histories,
* runtime outcomes,
* rollback histories.

The concept emphasizes that recursive improvement can accumulate operational experience rather than repeatedly searching from scratch.

---

## Added — Collective Recursive Improvement

Introduced **Collective Recursive Improvement** as an alternative to purely monolithic self-improvement.

Conceptual form:

```text id="5dv07n"
AI Proposes
     ↓
Evaluators Challenge
     ↓
Humans Govern
     ↓
Runtime Verifies
     ↓
Structures Preserve
     ↓
Other Systems Reuse
```

---

## Added — Scale × Structure

Positioned SRSI as complementary to scaling rather than opposed to it.

Conceptually:

```text id="uuv80j"
Model Scale
+
Compute Scale
+
Search Scale
+
Evaluator Richness
+
Structural Search
+
Counter-Evidence
+
Improvement Memory
+
Governance
```

The project therefore proposes:

> **Scale × Structure**

rather than:

> Scale vs. Structure.

---

# Added — Core Research Papers

Added six foundational SRSI documents.

### SRSI-001

**From Recursive Self-Improvement to Structural RSI**

Introduces the overall SRSI framing and the transition from recursive generation toward structured recursive improvement.

---

### SRSI-002

**Rich Evaluators: The Missing Infrastructure of RSI**

Introduces the Evaluator Bottleneck, Rich Evaluators, Evaluator Richness, Evaluator Plane, and evaluator-centered RSI infrastructure.

---

### SRSI-003

**DBM-SI as a Rich Evaluator and Improvement Infrastructure**

Maps existing DBM-SI computational structures into evaluation, localization, memory, search, and governance roles for SRSI.

---

### SRSI-004

**Two-Way CCC, Counter-Evidence, and Anti-Goodhart RSI**

Develops structural A/B comparison, active falsification, Counter-Evidence Search, and Anti-Goodhart recursive improvement.

---

### SRSI-005

**Localized RSI, Structural Growth, and Improvement Governance**

Develops Per-Node RSI, structural branching, Leftover, selective deployment, rollback, and Improvement Governance.

---

### SRSI-006

**The AI-SI-RSI Gold Rush**

Explores Evaluator Engineering, Evaluator Packs, Structural Search, Improvement Runtimes, Evaluator Economy, and Collective Recursive Improvement as possible future engineering fronts.

---

# Added — Core Figures

Added five canonical SRSI figures:

```text id="oyjdjm"
Fig-001-SRSI-Grand-Map.png

Fig-002-Rich-Evaluator-Plane.png

Fig-003-Structural-RSI-Loop.png

Fig-004-Two-Way-CCC-and-Counter-Evidence-RSI.png

Fig-005-AI-SI-RSI-Gold-Rush.png
```

Together the visual progression is:

```text id="4utjri"
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

# Added — Repository Navigation

Added:

* `README.md`
* `START-HERE.md`
* `CONTENTS.md`
* `FIGURE-INDEX.md`
* `GLOSSARY.md`
* `FUTURE-DIRECTIONS.md`

These files provide project introduction, navigation, terminology, visual indexing, and future research directions.

---

# Added — Release Metadata

Added release-support files:

```text id="ymp3yp"
CHANGELOG.md

CITATION.cff

.zenodo.json

GitHub-Release-Notes-v1.0.0.md
```

for GitHub, DOI, citation, and release workflows.

---

# Research Scope — v1.0.0

This release should be interpreted as:

```text id="zkp2qu"
Research Framework

Structural Proposal

Engineering Hypothesis

Research Direction
```

It does **not** claim:

* a completed autonomous RSI architecture,
* a demonstrated intelligence explosion,
* solved Goodhart problems,
* guaranteed safe recursive improvement,
* exhaustive evaluator infrastructure,
* a production SRSI runtime.

The purpose of `v1.0.0` is to establish a coherent structural research direction that can be tested through subsequent Minimum Engineering Tests.

---

# Central v1.0.0 Thesis

> **Recursive self-improvement is not merely recursive generation under increasing compute. It is recursive generation under rich evaluation, counter-evidence, structural localization, cumulative memory, verification, and governed promotion.**

---

# Canonical v1.0.0 Principles

> **Generation proposes change. Evaluation determines whether the change deserves to become improvement.**

> **Compute determines how hard RSI can search. Evaluators determine what RSI learns to become.**

> **Every powerful improvement engine needs a powerful falsification engine.**

> **Self-improvement does not have to mean self-replacement. It can mean recursive structural growth.**

> **Candidate Capability ≠ Validated Improvement ≠ Authorized Promotion ≠ Authorized Action.**

> **The next scarce AI resource may be trustworthy machine-operable judgment.**

---

# Next Milestone

The next major research phase is expected to move from:

```text id="1fjfg8"
Structural Framework
```

toward:

```text id="u4o6kj"
Minimum Engineering Tests
```

with particular emphasis on:

```text id="ktp7r3"
AI Coding SRSI
        ↓
Rich Evaluator Benchmark
        ↓
Counter-Evidence Runtime
        ↓
Localized RSI
        ↓
Structural Improvement Memory
        ↓
Improvement Governance
        ↓
Recursive Evaluator Improvement
```
