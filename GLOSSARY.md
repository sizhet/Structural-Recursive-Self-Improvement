# GLOSSARY — Structural Recursive Self-Improvement

**Project:** Structural Recursive Self-Improvement
**Acronym:** SRSI
**Repository:** `Structural-Recursive-Self-Improvement`

---

# 1. Purpose

This glossary defines the principal terms used throughout the **Structural Recursive Self-Improvement (SRSI)** project.

Some terms are established concepts in AI, optimization, software engineering, or governance.

Others are working terms introduced or specialized in this repository to describe the proposed SRSI framework.

The glossary therefore serves two purposes:

1. maintain terminology consistency across the SRSI document series;
2. distinguish general AI concepts from SRSI-specific structural interpretations.

The central research question behind the terminology is:

> **What computational structures make recursive improvement evaluable, falsifiable, localizable, auditable, cumulative, reversible, and governable?**

---

# 2. Core SRSI Terms

## Structural Recursive Self-Improvement — SRSI

A proposed framework for recursive improvement in which candidate generation is connected to explicit structures for:

* rich evaluation,
* counter-evidence,
* comparison,
* localization,
* verification,
* memory,
* governance,
* runtime observation.

Canonical loop:

```text
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

SRSI differs from a minimal recursive optimization loop by treating the **structure of improvement** itself as a first-class computational problem.

---

## Recursive Self-Improvement — RSI

The general idea that an intelligent system can contribute to improving its own capabilities, components, algorithms, evaluators, or improvement processes, allowing later versions or states to participate in further improvement.

SRSI does not assume that RSI requires:

* AGI,
* whole-system self-replacement,
* unrestricted autonomy,
* intelligence explosion.

Domain-specific and localized recursive improvement are included within the research scope.

---

## Structural Improvement

An improvement represented not merely as a higher score, but as an explicit change in identifiable computational structure.

Examples include:

```text
Node A → Node A'

Branch B → Branch B'

CallingGraph G → CallingGraph G'

Evaluator E1 → Evaluator E2
```

Structural improvement allows the system to reason about:

* where improvement occurred,
* what changed,
* what dependencies were affected,
* what should be preserved,
* what should be rolled back.

---

## Improvement Runtime

A computational runtime that repeatedly connects:

```text
Observation
→ Localization
→ Candidate Generation
→ Evaluation
→ Counter-Evaluation
→ Verification
→ Governance
→ Deployment
→ Observation
→ Memory
```

An Improvement Runtime turns improvement from an occasional external development activity into an explicit computational process.

---

## Improvement Cycle

One complete traversal through an improvement process.

A typical SRSI improvement cycle is:

```text
Current Structure
      ↓
Candidate
      ↓
Evaluation
      ↓
Decision
      ↓
Deployment / Rejection / Branch
      ↓
Runtime Evidence
      ↓
Structural Memory
```

The stored result may influence the next cycle.

---

# 3. Evaluation Terms

## Evaluator

A computational mechanism that judges some property of a candidate, behavior, structure, or outcome.

Examples include:

* unit tests,
* benchmarks,
* formal verification,
* simulations,
* graph comparison,
* performance measurement,
* policy checks,
* human review.

An evaluator may be simple or structurally rich.

---

## Scalar Evaluator

An evaluator whose principal output is a scalar value or simple ranking.

Example:

```text
Candidate A = 0.82
Candidate B = 0.89
```

Scalar evaluation can be useful, but may discard important information about:

* context,
* regressions,
* structural differences,
* uncertainty,
* counter-evidence.

---

## Rich Evaluator

A central SRSI concept.

A **Rich Evaluator** produces or preserves enough structured information to support a meaningful improvement decision.

Instead of only asking:

```text
Is B better than A?
```

it may ask:

```text
What improved?

Where?

Under which context?

What regressed?

What evidence supports the claim?

What counter-evidence exists?

What structure changed?

What uncertainty remains?

Where should B be deployed?

Should B be promoted at all?
```

A Rich Evaluator should ideally produce outputs that are:

* machine-operable,
* composable,
* traceable,
* context-aware,
* reusable.

---

## Evaluator Richness

A working SRSI concept describing the amount and quality of decision-relevant structure preserved by an evaluator.

Possible dimensions include:

| Dimension          | Question                           |
| ------------------ | ---------------------------------- |
| Differential       | What changed?                      |
| Comparative        | Better than what?                  |
| Contextual         | Under which conditions?            |
| Evidential         | What supports the judgment?        |
| Counter-Evidential | What challenges it?                |
| Structural         | Which structures changed?          |
| Regression         | What became worse?                 |
| Temporal           | Does the improvement persist?      |
| Uncertainty        | What remains unresolved?           |
| Policy             | Is the improvement acceptable?     |
| Deployment         | Where should it operate?           |
| Audit              | Can the decision be reconstructed? |

Evaluator Richness should not be interpreted as simply maximizing the number of metrics.

The objective is to preserve **decision-relevant structure**.

---

## Evaluator Bottleneck

A hypothesis explored in SRSI.

As AI candidate generation becomes increasingly capable and inexpensive, the ability to reliably evaluate large numbers of candidates may become a limiting factor.

Conceptually:

```text
Generation Capacity ↑↑↑
          ↓
Candidate Volume ↑↑↑
          ↓
Evaluation Demand ↑↑↑
```

The Evaluator Bottleneck Hypothesis does not claim that evaluation is always the dominant bottleneck.

It proposes that evaluation may become increasingly important as generation and search scale.

---

## Evaluator Scarcity Hypothesis

The broader hypothesis that trustworthy machine-operable evaluation may become relatively scarce and valuable as candidate generation becomes abundant.

This hypothesis motivates the SRSI concept of an emerging evaluator-centered engineering frontier.

---

## Evaluator Plane

A computational layer containing multiple evaluators and the mechanisms needed to route, compose, compare, and interpret their outputs.

Example:

```text
Candidate
   ↓
Evaluator Router
   ├── Performance Evaluator
   ├── Structural Evaluator
   ├── Regression Evaluator
   ├── Counter-Evaluator
   ├── Trajectory Evaluator
   └── Policy Evaluator
           ↓
    Structural Judgment
```

The Evaluator Plane avoids assuming that one evaluator should answer every improvement question.

---

## Evaluator Portfolio

A collection of evaluators that examine a candidate from different perspectives.

An Evaluator Portfolio may include:

```text
Performance

Safety

Structure

Cost

Regression

Trajectory

Policy

Counter-Evidence
```

Evaluator diversity can reduce dependence on a single evaluation proxy.

---

## Evaluator Pack

A reusable collection of domain-specific evaluators.

Examples:

### AI Coding Evaluator Pack

```text
Compiler
Tests
CallingGraph
Runtime
Performance
Security
Architecture
```

### Scientific Evaluator Pack

```text
Evidence
Prediction
Replication
Counterexample Search
Mechanism
Uncertainty
```

Evaluator Packs are proposed as one possible reusable infrastructure unit for domain-specific SRSI.

---

## Evaluator Routing

The process of selecting appropriate evaluators based on candidate type, context, risk, structure, or improvement stage.

```text
Candidate
   ↓
Type / Context / Risk
   ↓
Evaluator Router
   ├── E1
   ├── E2
   └── E3
```

Evaluator Routing can reduce unnecessary evaluation cost while increasing relevant coverage.

---

## Evaluator Composition

The process of combining multiple evaluators sequentially or in parallel.

Example:

```text
Fast Evaluation
      ↓
Structural Evaluation
      ↓
Counter-Evaluation
      ↓
Deep Verification
      ↓
Policy Evaluation
```

Composition may also preserve disagreement rather than immediately compressing all outputs into one scalar.

---

## Evaluator-of-Evaluators

A meta-evaluator that evaluates the reliability, calibration, coverage, robustness, or historical performance of other evaluators.

Questions include:

```text
How often did this evaluator promote bad candidates?

How often did it reject good candidates?

Under which contexts is it reliable?

How easily can it be gamed?
```

Evaluator-of-Evaluators supports recursive improvement of evaluation infrastructure itself.

---

## Evaluator Reputation

A context-bound record of evaluator performance accumulated over time.

Example:

```text
Evaluator E7

Coding: High Reliability
Security: Medium Reliability
Long-Horizon Prediction: Low Reliability
Adversarial Robustness: High
```

Evaluator Reputation can influence future evaluator routing and weighting.

---

## Evaluator Engineering

The engineering discipline concerned with designing, implementing, composing, validating, securing, benchmarking, and evolving evaluators.

In SRSI, Evaluator Engineering is treated as potential core AI infrastructure rather than merely a support activity.

---

## Evaluator Security

The protection of evaluators and evaluation pipelines against manipulation.

Possible threats include:

* evaluator gaming,
* benchmark overfitting,
* evidence manipulation,
* evaluator poisoning,
* counter-evidence suppression,
* routing manipulation,
* policy bypass.

---

## Evaluator Economy

A speculative SRSI term describing a possible ecosystem in which evaluators, Evaluator Packs, benchmarks, routing systems, certification mechanisms, and evaluator security become reusable and economically valuable infrastructure.

This is a research hypothesis, not a claim that such a market already exists in mature form.

---

# 4. Evidence and Falsification Terms

## Evidence

Information supporting the claim that a candidate represents improvement relative to a baseline, objective, context, or policy.

Evidence may include:

* benchmark improvement,
* successful tests,
* runtime observations,
* structural consistency,
* lower cost,
* improved trajectory.

---

## Counter-Evidence

Information that challenges an improvement claim.

Examples include:

* counterexamples,
* regression,
* failure contexts,
* incompatible dependencies,
* long-horizon degradation,
* evaluator exploitation.

Counter-evidence is treated as first-class improvement information.

---

## Counter-Evidence Search

An active process that searches for reasons a candidate may **not** represent genuine improvement.

Instead of only asking:

> Why is B better?

Counter-Evidence Search asks:

> **Where does B fail, regress, conflict, or exploit the evaluator?**

It is one of the principal Anti-Goodhart mechanisms proposed in SRSI.

---

## Counter-Evaluator

An evaluator whose role is to challenge, falsify, or stress-test the conclusions of another evaluator.

Conceptually:

```text
Primary Evaluator
        ↕
Counter-Evaluator
```

The objective is not automatic disagreement.

The objective is to create structured challenge.

---

## Cross-Perspective Evaluation

Evaluation of the same candidate from multiple structural, contextual, objective, or policy perspectives.

A candidate may be:

```text
better for performance

worse for reliability

neutral for cost

uncertain for long-horizon behavior
```

SRSI attempts to preserve these differences rather than immediately hiding them inside a single score.

---

# 5. Goodhart and Anti-Goodhart Terms

## Goodhart's Law

A general principle often summarized as:

> When a measure becomes a target, it can cease to be a good measure.

In RSI, stronger optimization can increase pressure on evaluator weaknesses.

---

## RSI Goodhart Amplifier

A working SRSI term describing a recursive failure pattern:

```text
Evaluator Weakness
       ↓
Candidate Exploits Weakness
       ↓
Candidate Is Promoted
       ↓
Improved Optimizer
       ↓
More Effective Exploitation
       ↓
...
```

Recursive optimization can therefore recursively amplify evaluator error.

---

## Anti-Goodhart RSI

An SRSI architecture intended to reduce recursive exploitation of evaluator weaknesses through mechanisms such as:

* evaluator diversity,
* Counter-Evidence Search,
* Counter-Evaluators,
* cross-perspective evaluation,
* structural A/B comparison,
* verification,
* policy gates,
* runtime observation.

Anti-Goodhart RSI does not imply that Goodhart problems can be eliminated.

Its purpose is to make evaluator weakness more visible and contestable.

---

# 6. Comparison and Search Terms

## Structural A/B Evaluation

Comparison between current structure `A` and candidate structure `B` that preserves meaningful differences instead of producing only a winner.

```text
A
↕
Structural Comparison
↕
B
```

Possible outputs include:

* shared structure,
* A-specific strengths,
* B-specific strengths,
* regressions,
* contextual differences,
* unresolved differences.

---

## Two-Way CCC

A DBM-SI structural comparison mechanism used in SRSI as a possible implementation of Structural A/B Evaluation.

Rather than forcing:

```text
A vs. B
   ↓
Winner
```

Two-Way CCC can preserve:

```text
Shared

A-Specific

B-Specific

Difference

Unresolved
```

This supports promotion, rejection, branching, localization, and Leftover.

---

## Structural Search

Search performed over explicit structures rather than an undifferentiated candidate space.

Structural Search may answer:

```text
Where is the failure?

Which node should be improved?

Which previous structure is similar?

Which branch contains relevant experience?
```

SRSI uses Structural Search for both improvement localization and memory retrieval.

---

## Structural Search Plane

A computational layer that transforms observations into searchable structural representations.

A generic DBM-SI form is:

```text
Raw Evidence
    ↓
Structural Representation
    ↓
Metric / Differential Structure
    ↓
CCC
    ↓
Dispatch / Trigger
    ↓
Outcome
```

Within SRSI, this can support candidate localization, evaluator routing, and improvement-memory retrieval.

---

# 7. Localization Terms

## Localization

The process of identifying the specific node, branch, behavior, path, evaluator, or subsystem responsible for an observed opportunity or failure.

Localization converts:

```text
Improve the system
```

into:

```text
Improve this structure.
```

---

## Localized RSI

Recursive improvement applied to a bounded part of a larger system.

Canonical form:

```text
Locate
  ↓
Generate Local Candidate
  ↓
Evaluate
  ↓
Counter-Evaluate
  ↓
Verify Integration
  ↓
Promote Locally
```

Localized RSI is proposed as a practical alternative to whole-system self-replacement.

---

## Per-Node RSI

A form of Localized RSI in which individual nodes maintain or access local:

* intelligence,
* evaluators,
* memory,
* policies,
* improvement histories.

This allows recursive improvement to occur across a distributed structure.

---

## Per-Node Intelligence

A Structural Intelligence concept in which intelligence is associated with individual structural nodes rather than existing only at the global system level.

In SRSI, Per-Node Intelligence provides a natural substrate for localized evaluation and improvement.

---

# 8. Structural Growth Terms

## Structural Growth

Improvement through expansion, differentiation, refinement, or branching of a computational structure.

Instead of:

```text
A → B → C
```

Structural Growth may produce:

```text
       Root
      / |  \
     A  B   C
       / \
      B1 B2
```

---

## Recursive Structural Differentiation and Growth

A central SRSI interpretation of self-improvement.

Rather than repeatedly replacing the entire current system, recursive improvement can create context-specific branches and selectively preserve alternatives.

This supports the principle:

> **Self-improvement does not have to mean self-replacement.**

---

## Branch

A structural alternative preserved for a particular context, specialization, uncertainty state, or deployment scope.

A candidate can therefore become:

```text
Global Replacement

Local Branch

Experimental Branch

Context-Specific Branch
```

rather than simply winning or losing.

---

## Leftover

An explicit structural state for unresolved candidates, evidence, or cases.

A Leftover is neither automatically accepted nor rejected.

Example:

```text
Evidence: Positive
Counter-Evidence: Significant
Uncertainty: High
        ↓
LEFTOVER
```

Later evidence may trigger re-evaluation.

---

## 3-Cat Learning

A DBM-SI structural learning pattern in which new observations can be organized through shared structure and differentiated alternatives rather than simple binary classification.

Within SRSI, 3-Cat Learning can support structural growth and branching.

---

# 9. Memory Terms

## Improvement Memory

Stored experience about previous improvement attempts.

An Improvement Memory may preserve:

```text
Baseline

Candidate

Context

Difference

Evidence

Counter-Evidence

Decision

Deployment Scope

Runtime Outcome

Rollback Outcome
```

This allows future improvement cycles to reuse prior experience.

---

## Structural Memory

Memory organized around explicit computational relationships, differences, contexts, branches, and outcomes.

Structural Memory supports retrieval based on similarity and relevance rather than only chronological storage.

---

## Structural Folding

The process of compressing or organizing validated runtime experience into reusable structural memory.

In SRSI:

```text
Improvement Attempt
      ↓
Runtime Evidence
      ↓
Validation
      ↓
Fold
      ↓
Reusable Improvement Structure
```

---

## Structural Unfolding

The process of retrieving and adapting folded structural experience to a new runtime context.

```text
New Context
    ↓
Search Structural Memory
    ↓
Retrieve Relevant Structure
    ↓
Unfold
    ↓
Adapt / Evaluate
```

Folding and Unfolding together support cumulative improvement.

---

## Structural Improvement Capital

A working SRSI term describing the accumulated value of validated improvements, rejected candidates, counterexamples, evaluator histories, runtime outcomes, and rollback knowledge.

Unlike raw candidate generation, Structural Improvement Capital accumulates through repeated operational experience.

---

## Negative Improvement Memory

Stored information about failed, rejected, regressive, or misleading improvement attempts.

Negative Improvement Memory can answer:

```text
What looked promising but failed?

Which context caused the failure?

Which evaluator was fooled?

Which counter-evidence mattered?
```

Failed improvements can therefore become reusable intelligence.

---

# 10. Governance Terms

## Improvement Governance

The policies and computational mechanisms that determine whether a validated candidate may be promoted, where it may operate, and under which conditions.

Improvement Governance separates:

```text
Candidate Capability
        ≠
Validated Improvement
        ≠
Authorized Promotion
        ≠
Authorized Action
```

---

## Improvement Governance Plane

A dedicated computational layer for decisions such as:

```text
PROMOTE-GLOBAL

PROMOTE-LOCAL

BRANCH

SHADOW

EXPERIMENTAL

HOLD

LEFTOVER

REJECT

ROLLBACK
```

The Improvement Governance Plane prevents technical evaluation from automatically becoming deployment authority.

---

## Promotion

The process by which a candidate becomes an authorized active structure.

Promotion may be:

* global,
* local,
* context-bound,
* temporary,
* experimental.

---

## Promotion Gate

A policy-controlled decision point between validated improvement and deployment.

```text
Validated Candidate
        ↓
Promotion Gate
        ↓
Authorized Deployment
```

---

## Improvement Authority

The permission to modify, replace, branch, promote, or otherwise alter an intelligent system or its improvement infrastructure.

Improvement Authority is distinct from Action Authority.

---

## Action Authority

The permission to perform actions in the external or operational environment.

SRSI distinguishes:

```text
Action Authority
       ≠
Improvement Authority
```

A system may be allowed to act without being allowed to modify the evaluator or policy governing future actions.

---

## PDS — Policy Decision System

A DBM-SI policy and decision structure.

Within SRSI, PDS can serve as one possible:

* Promotion Control Plane,
* Improvement Governance Plane,
* policy evaluation mechanism.

---

## Rollback

The controlled restoration of an earlier structure after a promoted candidate causes unacceptable runtime outcomes.

Rollback is a core requirement for reversible improvement.

---

## Improvement Provenance

The traceable history of an improvement.

It may include:

```text
Who or what generated it?

Which baseline was used?

Which evaluators tested it?

What evidence existed?

What counter-evidence existed?

Who authorized promotion?

Where was it deployed?

What happened afterward?
```

Improvement Provenance supports auditability and governance.

---

# 11. DBM-SI Structural Terms Used in SRSI

## DBM-SI

A broader Structural Intelligence research program containing computational mechanisms for structural representation, comparison, search, localization, trajectories, folding/unfolding, policy, and runtime intelligence.

Within this repository:

> **DBM-SI is treated as one possible provider of SRSI infrastructure, not as the exclusive route to Structural Recursive Self-Improvement.**

---

## MDT — Metric Differential Tree

A structural mechanism for organizing objects or states according to metric differences.

Within SRSI, MDT can function as a:

* differential evaluator,
* structural localization mechanism,
* candidate search structure.

---

## CCC

A recurring DBM-SI structural representation and organization mechanism.

Within SRSI, CCC can support:

* structural consistency,
* comparison,
* localization,
* routing,
* structural memory.

---

## UTN — Universal Typing / Naming

A DBM-SI mechanism concerned with structural identity, naming, typing, and compatibility.

Within SRSI, UTN can support:

* candidate identity,
* evaluator compatibility,
* context binding,
* local/global integration.

---

## CallingGraph

A graph representation of calling relationships among software functions or computational components.

Within SRSI, CallingGraph can act as a behavioral-path evaluator.

---

## CallingGraph Delta — CG Delta

The structural difference between two CallingGraph states.

Within AI Coding SRSI, CG Delta can identify:

```text
what changed

where

which paths were affected

what integration risk exists
```

---

## Trajectory Intelligence

A DBM-SI perspective in which behavior is evaluated across sequences, paths, trajectories, or long-horizon evolution rather than only at isolated decision points.

Within SRSI, Trajectory Intelligence can serve as a long-horizon evaluator.

---

## DNA Dispatch / Trigger

A DBM-SI structural dispatch concept used to route runtime inputs, candidates, or contexts toward appropriate structural branches or actions.

Within SRSI, similar mechanisms can support:

* evaluator routing,
* candidate routing,
* branch selection.

---

# 12. Runtime Terms

## Runtime Evidence

Evidence collected after a candidate has entered an experimental, local, shadow, or production runtime.

Runtime Evidence is especially important because offline evaluation may not capture all operational behavior.

---

## Shadow Deployment

Deployment in which a candidate observes or processes real runtime inputs without receiving full operational authority.

Shadow deployment can provide evidence before promotion.

---

## Selective Deployment

Deployment restricted by:

* context,
* node,
* user class,
* risk tier,
* environment,
* time window,
* policy.

Selective Deployment is a key mechanism for Localized RSI.

---

## Integration Verification

Testing whether a local improvement remains compatible with the larger system.

A candidate may pass local evaluation but fail integration verification.

Therefore:

```text
Local Improvement
       ≠
Global Compatibility
```

---

# 13. AI-SI-RSI Frontier Terms

## AI-SI-RSI

A conceptual convergence of:

### AI

Candidate generation, reasoning, prediction, planning, coding, and hypothesis generation.

### SI

Structural evaluation, comparison, localization, search, memory, dispatch, and governance.

### RSI

Repeated recursive improvement.

Conceptually:

```text
AI
 ↓
Generate

SI
 ↓
Evaluate / Structure / Search / Remember

RSI
 ↓
Improve Recursively
```

---

## AI-SI-RSI Gold Rush

A metaphor introduced in this project for a possible engineering wave in which Rich Evaluators, Structural Search, Improvement Memory, and Improvement Runtimes become increasingly valuable as AI candidate generation becomes more abundant.

The term does **not** imply:

* inevitable intelligence explosion,
* guaranteed AGI,
* guaranteed economic abundance,
* guaranteed safety.

It identifies a possible shift in technological scarcity.

---

## Evaluator Rush

The possible engineering race to create better machine-operable evaluators.

Core question:

> **Is B really better than A?**

---

## Structural Search Rush

The possible engineering race to efficiently locate improvement opportunities and retrieve relevant historical experience.

Core questions:

> **Where should improvement occur?**

and:

> **Which previous improvement is relevant?**

---

## Improvement Runtime Rush

The possible engineering race to connect:

```text
Generate
→ Evaluate
→ Counter-Evaluate
→ Verify
→ Govern
→ Deploy
→ Observe
→ Fold
→ Repeat
```

into reliable domain-specific improvement runtimes.

---

## Collective Recursive Improvement

Recursive improvement performed by an ecosystem rather than a single isolated AI.

Example:

```text
AI proposes
      ↓
Evaluators challenge
      ↓
Humans govern
      ↓
Runtime verifies
      ↓
Structures preserve
      ↓
Other systems reuse
```

This provides an alternative to purely monolithic interpretations of RSI.

---

## Improvement Network

A network through which systems exchange validated structural improvement experience.

The exchanged object may include:

```text
Candidate Structure

Context

Evidence

Counter-Evidence

Evaluation History

Runtime Outcome
```

rather than raw data alone.

---

# 14. MET Terms

## MET — Minimum Engineering Test

A small executable or experimentally testable system designed to validate one structural hypothesis without requiring a complete production architecture.

A minimal SRSI MET might be:

```text
Generate Candidates
       ↓
Evaluate
       ↓
Counter-Evaluate
       ↓
Promote One Local Improvement
       ↓
Observe
       ↓
Fold
       ↓
Reuse
```

The purpose is to test whether the improvement loop actually produces measurable cumulative benefit.

---

## AI Coding SRSI MET

A proposed early SRSI experiment using software engineering because the domain already contains strong machine-operable evaluators.

Example:

```text
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
Runtime Evaluation
      ↓
Promotion Gate
      ↓
Fold Result
```

---

## Scientific RSI

A domain-specific SRSI pattern applied to scientific discovery.

```text
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

---

# 15. Important Distinctions

## Generation vs. Improvement

```text
Generation
    =
Producing a candidate

Improvement
    =
Establishing that a candidate is preferable
under defined evidence, context, verification,
and governance conditions
```

Therefore:

> **Generation is not improvement.**

---

## Evaluation vs. Governance

Evaluation asks:

> Is this candidate technically better?

Governance asks:

> Should this candidate be promoted, where, and under what authority?

Therefore:

```text
Evaluation
    ≠
Governance
```

---

## Capability vs. Improvement

A candidate may gain capability while introducing unacceptable regressions.

Therefore:

```text
More Capability
      ≠
Validated Improvement
```

---

## Improvement vs. Deployment

A validated improvement may still be inappropriate for unrestricted deployment.

Therefore:

```text
Validated Improvement
        ≠
Authorized Deployment
```

---

## Self-Improvement vs. Self-Replacement

SRSI does not assume:

```text
A must die
when
B improves something.
```

Instead:

```text
A
├── B1
├── B2
└── Leftover
```

may preserve multiple valid structures.

---

## Search vs. Structural Search

General search asks:

```text
Which candidate wins?
```

Structural Search additionally asks:

```text
Where should we search?

Which structure matters?

Which context applies?

Which previous structure is relevant?
```

---

## Explanation vs. Machine-Operable Evaluation

Human-readable explanation is useful.

But a Rich Evaluator should ideally produce structured outputs that downstream systems can:

```text
search

compare

route

verify

govern

fold

reuse
```

Thus Rich Evaluation is not merely explainability.

---

# 16. Canonical SRSI Vocabulary

For consistency across this repository, the preferred terms are:

```text
Structural Recursive Self-Improvement
SRSI
Rich Evaluator
Evaluator Richness
Evaluator Bottleneck
Evaluator Plane
Evaluator Pack
Counter-Evidence
Counter-Evaluator
Anti-Goodhart RSI
Structural A/B
Localized RSI
Per-Node RSI
Structural Growth
Leftover
Improvement Memory
Structural Folding
Improvement Governance
Improvement Authority
Improvement Runtime
Structural Improvement Capital
AI-SI-RSI Gold Rush
Collective Recursive Improvement
```

---

# 17. Terms to Use Carefully

The following expressions should be used cautiously unless supported by empirical evidence:

```text
Solved RSI

Complete RSI Architecture

Guaranteed Self-Improvement

Autonomous Intelligence Explosion

Perfect Evaluator

Safe RSI

Optimal Improvement

Exhaustive Search of Intelligence
```

Preferred language includes:

```text
Research Framework

Engineering Hypothesis

Candidate Architecture

Structural Mechanism

Possible Bottleneck

Proposed Runtime

Research Direction

Minimum Engineering Test
```

This distinction is important because SRSI v1.0 establishes a research framework rather than claiming a completed general RSI implementation.

---

# 18. Canonical SRSI Equations and Relations

The following relations summarize the project conceptually.

## Candidate vs. Improvement

```text
Candidate Generation
        ≠
Validated Improvement
```

## Capability vs. Authority

```text
Candidate Capability
        ≠
Validated Improvement
        ≠
Authorized Promotion
        ≠
Authorized Action
```

## Search and Evaluation

```text
More Compute
      +
Weak Evaluation
      ≠
Reliable Improvement
```

## Structural RSI

```text
SRSI
≈
Generation
+
Rich Evaluation
+
Counter-Evidence
+
Structural Search
+
Localization
+
Verification
+
Structural Memory
+
Governance
```

These are conceptual relations, not formal mathematical equalities.

---

# 19. Canonical SRSI Loop

```text
Runtime Evidence
       ↓
Structural Search
       ↓
Localization
       ↓
Candidate Generation
       ↓
Rich Evaluation
       ↕
Counter-Evidence
       ↓
Structural Comparison
       ↓
Verification
       ↓
Improvement Governance
       ↓
Promote / Branch / Leftover / Reject
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

---

# 20. Canonical SRSI Principles

### Principle 1

> **Generation proposes change. Evaluation determines whether the change deserves to become improvement.**

### Principle 2

> **Compute determines how hard RSI can search. Evaluators determine what RSI learns to become.**

### Principle 3

> **Every powerful improvement engine needs a powerful falsification engine.**

### Principle 4

> **Self-improvement does not have to mean self-replacement. It can mean recursive structural growth.**

### Principle 5

> **Candidate Capability ≠ Validated Improvement ≠ Authorized Promotion ≠ Authorized Action.**

### Principle 6

> **The next scarce AI resource may be trustworthy machine-operable judgment.**

---

# 21. One-Sentence Definition

If only one definition is retained from this glossary:

> **Structural Recursive Self-Improvement is recursive improvement organized around rich evaluation, counter-evidence, structural localization, verification, cumulative memory, and governed promotion rather than candidate generation alone.**

---

# 22. Related Repository Documents

For the conceptual introduction:

[`README.md`](README.md)

For the 10-minute reading guide:

[`START-HERE.md`](START-HERE.md)

For the full document map:

[`CONTENTS.md`](CONTENTS.md)

For visual terminology:

[`FIGURE-INDEX.md`](FIGURE-INDEX.md)

For open research questions and future work:

[`FUTURE-DIRECTIONS.md`](FUTURE-DIRECTIONS.md)
