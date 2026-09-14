# FUTURE DIRECTIONS — Structural Recursive Self-Improvement

**Project:** Structural Recursive Self-Improvement
**Acronym:** SRSI
**Repository:** `Structural-Recursive-Self-Improvement`

---

# 1. Purpose

SRSI v1.0 introduces a structural framing of Recursive Self-Improvement centered on:

```text
Rich Evaluation
        +
Counter-Evidence
        +
Localization
        +
Verification
        +
Structural Memory
        +
Improvement Governance
```

The next phase should not attempt to “solve RSI” in one step.

A more productive roadmap is to progressively test the individual mechanisms that make recursive improvement:

* measurable,
* falsifiable,
* localizable,
* cumulative,
* reversible,
* governable.

The guiding research question remains:

> **What computational structures make recursive improvement evaluable, falsifiable, localizable, auditable, cumulative, reversible, and governable?**

---

# 2. Future Direction Map

The main future directions can be organized into seven research fronts.

```text
SRSI
│
├── 1. Rich Evaluator Theory
├── 2. Anti-Goodhart RSI
├── 3. Localized and Per-Node RSI
├── 4. Structural Improvement Memory
├── 5. Improvement Governance
├── 6. SRSI Runtime and METs
└── 7. Evaluator Ecosystems and Collective Improvement
```

These fronts are strongly connected.

The long-term goal is not a collection of isolated mechanisms.

It is a coherent improvement infrastructure.

---

# 3. Rich Evaluator Theory

The first major research direction is to make the concept of the **Rich Evaluator** more precise.

SRSI currently defines evaluator richness through dimensions such as:

```text
Difference
Context
Evidence
Counter-Evidence
Regression
Structure
Trajectory
Uncertainty
Policy
Deployment
Audit
```

Future work should determine which dimensions are actually necessary for different classes of improvement problems.

---

## 3.1 Evaluator Richness Metrics

A core open question is:

> **Can Evaluator Richness itself be measured?**

Possible research dimensions include:

```text
Coverage

Context Sensitivity

Counterexample Detection

Regression Detection

Structural Resolution

Temporal Stability

Uncertainty Calibration

Policy Awareness

Auditability
```

A future SRSI benchmark could compare:

```text
Scalar Evaluator
        vs.
Multi-Metric Evaluator
        vs.
Rich Structural Evaluator
```

and measure whether additional structure improves candidate-selection quality.

---

## 3.2 Evaluator Quality vs. Evaluator Cost

Rich evaluation is not free.

A practical runtime must balance:

```text
Evaluation Quality
        ↕
Evaluation Cost
```

This suggests research into:

* staged evaluation,
* evaluator routing,
* adaptive evaluator depth,
* risk-based evaluator selection,
* early rejection,
* selective deep verification.

Possible runtime pattern:

```text
Cheap Evaluator
      ↓
Potentially Promising?
      ↓
Rich Evaluator
      ↓
High Risk?
      ↓
Deep Verification
```

---

## 3.3 Evaluator Routing

Not every candidate requires every evaluator.

Future SRSI systems should investigate:

```text
Candidate Type
      +
Context
      +
Risk
      +
Structural Location
      ↓
Evaluator Router
```

Questions include:

* Which evaluators should run first?
* Which can be skipped?
* Which evaluator combinations are most informative?
* When should disagreement trigger deeper evaluation?

---

## 3.4 Evaluator Composition

Rich evaluation may require multiple evaluators operating:

```text
Serially

In Parallel

Conditionally

Adversarially
```

Future work should study whether evaluator composition behaves more like:

```text
Pipeline
```

or:

```text
Graph
```

or:

```text
Evaluator CallingGraph
```

This may become a major SRSI engineering topic.

---

## 3.5 Evaluator-of-Evaluators

Evaluators themselves can fail.

Therefore future SRSI should study:

> **How should evaluators be evaluated?**

Possible evidence includes:

```text
Historical Accuracy

False Promotion Rate

False Rejection Rate

Goodhart Vulnerability

Context Coverage

Calibration

Runtime Prediction Accuracy
```

This creates:

# **Evaluator-of-Evaluators**

The challenge is to improve evaluator quality without creating an infinite regress.

A practical solution may rely on bounded layers of verification and runtime evidence.

---

# 4. Evaluator Diversity and Correlated Blind Spots

Multiple evaluators are useful only if they do not all fail in the same way.

A major future direction is therefore:

# **Evaluator Diversity**

The important quantity may not be merely:

```text
Number of Evaluators
```

but:

```text
Independence of Failure Modes
```

Future work should study:

* correlated evaluator blind spots,
* evaluator monoculture,
* shared benchmark bias,
* shared training-data bias,
* evaluator diversity metrics,
* adversarial evaluator generation.

A strong evaluator portfolio should not simply contain many copies of the same judgment process.

---

# 5. Anti-Goodhart RSI

One of the most important SRSI directions is strengthening the machinery that can challenge improvement claims.

The central concern is:

```text
Optimizer Strength ↑
        ↓
Evaluator Exploitation Ability ↑
```

Future Anti-Goodhart research should therefore grow alongside optimization capability.

---

## 5.1 Counter-Evidence Search

Counter-Evidence Search should become a first-class experimental subsystem.

Possible research questions:

```text
How much counter-evidence is enough?

Which search strategies find regressions fastest?

Can counter-evidence be reused across candidate families?

Can historical counter-evidence predict future failure?
```

A future runtime might explicitly allocate:

```text
Improvement Search Budget

and

Counter-Evidence Search Budget
```

---

## 5.2 Recursive Counter-Evidence

If the improvement generator improves recursively, the challenger should also improve recursively.

This suggests:

# **Recursive Counter-Evidence**

```text
Candidate Generator Improves
          ↕
Counter-Evidence Engine Improves
```

This creates a co-evolutionary architecture.

The goal is not permanent balance by assumption.

The goal is to prevent one side from becoming structurally obsolete.

---

## 5.3 Adversarial Evaluators

Future SRSI systems may include evaluators whose explicit role is:

```text
Break the Candidate

Find Boundary Conditions

Find Hidden Regression

Find Evaluator Exploits

Find Unsafe Contexts
```

These can act as:

# **Improvement Red Teams**

This may be especially important for:

* policy changes,
* evaluator modifications,
* governance changes,
* high-impact code changes.

---

## 5.4 Evaluator Disagreement

Evaluator disagreement should be studied as a signal.

Instead of:

```text
E1 = 0.9
E2 = 0.4
      ↓
Average = 0.65
```

future SRSI systems should ask:

```text
Why do E1 and E2 disagree?

Which context causes disagreement?

Which evaluator is more reliable here?

Should this become a branch?
```

This connects evaluator disagreement directly to Structural A/B and Leftover.

---

# 6. Two-Way CCC as an Improvement Primitive

Two-Way CCC deserves deeper study as a canonical SRSI comparison primitive.

Future research should evaluate whether Two-Way CCC can systematically preserve:

```text
Shared Structure

A-Specific Strength

B-Specific Strength

Regression

Context Difference

Unresolved Difference
```

across multiple domains.

Potential domains include:

* software,
* scientific reasoning,
* policy systems,
* market strategies,
* trajectory decisions,
* evaluator comparison.

A major question is:

> **Can Structural A/B outperform winner-take-all evaluation in recursive improvement tasks?**

---

# 7. Localized RSI

Localized RSI may be one of the most practical paths toward real recursive improvement.

Future work should test the hypothesis:

> **Localize first, improve second.**

Instead of searching the entire system, identify the structurally relevant node or region first.

---

## 7.1 Per-Node RSI Runtime

A future runtime could maintain per-node:

```text
Evaluator

Memory

Candidate History

Counter-Evidence

Policy

Improvement State
```

Conceptually:

```text
Node_i
  ↓
Local Evidence
  ↓
Local Candidate
  ↓
Local Evaluation
  ↓
Counter-Evidence
  ↓
Integration Verification
  ↓
Promotion
```

This could make recursive improvement:

* cheaper,
* easier to audit,
* easier to roll back,
* more context-sensitive.

---

## 7.2 Global Coherence Evaluation

Localized improvement introduces a major risk:

```text
Local Improvement
        ≠
Global Improvement
```

Therefore future SRSI needs:

# **Global Coherence Evaluators**

These should test:

* global performance,
* cross-node compatibility,
* CallingGraph impact,
* trajectory effects,
* shared resource conflicts,
* policy conflicts.

The long-term architecture may require:

```text
Local Evaluators
        +
Global Coherence Evaluators
```

---

## 7.3 Improvement Blast Radius

CallingGraph Delta and dependency structures could be used to estimate:

# **Improvement Blast Radius**

Questions include:

```text
Which nodes depend on this change?

Which paths are affected?

How far can regression propagate?

Which tests should be triggered?
```

Improvement Blast Radius may become a useful runtime metric.

---

# 8. Structural Growth and Branch Lifecycle

If recursive improvement becomes structural growth, branch management becomes important.

Future SRSI systems should study:

```text
Create Branch

Evaluate Branch

Promote Branch

Merge Branch

Freeze Branch

Deprecate Branch

Delete Branch
```

Without branch lifecycle management, structural growth can become structural clutter.

---

## 8.1 Branch Merge

Two successful branches may later become compatible.

Future work should investigate:

```text
B1
 \
  → Merge → B*
 /
B2
```

This may require:

* structural compatibility checks,
* counter-evidence,
* regression testing,
* identity reconciliation,
* policy review.

---

## 8.2 Branch Pruning

Not every historical branch should remain active forever.

Future work should define pruning policies based on:

```text
Usage

Performance

Reliability

Redundancy

Risk

Maintenance Cost
```

Structural growth should include forgetting and consolidation.

---

# 9. Leftover as a Research Object

The Leftover state deserves more attention.

Rather than treating uncertainty as failure, SRSI preserves unresolved cases explicitly.

Future questions include:

```text
How long should a Leftover remain unresolved?

What new evidence should trigger re-evaluation?

Can Leftovers cluster into new categories?

Can repeated Leftovers reveal missing evaluators?
```

A powerful hypothesis is:

> **Repeated Leftover may reveal missing structure.**

This connects directly to:

* 3-Cat Learning,
* evaluator discovery,
* branch growth,
* new policy creation.

---

# 10. Structural Improvement Memory

Recursive improvement should accumulate experience.

Future SRSI needs a richer theory of:

# **Improvement Memory**

Possible stored elements include:

```text
Baseline

Candidate

Difference

Context

Evidence

Counter-Evidence

Evaluator Outputs

Decision

Deployment Scope

Runtime Result

Rollback Result
```

---

## 10.1 Positive and Negative Improvement Memory

Memory should preserve both:

```text
What worked
```

and:

```text
What failed
```

Negative improvement memory may be especially valuable because it prevents repeated exploration of known bad paths.

---

## 10.2 Improvement Memory Retrieval

Future research should investigate how runtime systems retrieve relevant improvement experience.

Possible keys include:

```text
Structural Similarity

Context Similarity

Failure Pattern

CallingGraph Region

Trajectory Pattern

UTN Identity

Evaluator Signature
```

This connects Structural Folding directly to future candidate generation.

---

## 10.3 Improvement Memory Compression

Large-scale recursive improvement may generate enormous history.

Future systems will need to decide:

```text
What should be preserved?

What should be folded?

What should be summarized?

What should remain raw?

What can be discarded?
```

This creates a new research area:

# **Improvement Memory Compression**

---

# 11. Evaluator Memory

Evaluators should also accumulate their own history.

Future systems may track:

```text
Evaluator E1

Past Decisions

Correct Decisions

Incorrect Decisions

Contexts of Failure

Goodhart Incidents

Calibration History
```

This supports:

* evaluator reputation,
* evaluator routing,
* evaluator replacement,
* evaluator improvement.

---

# 12. Recursive Evaluator Improvement

One of the deepest future directions is:

> **Can the evaluator improve recursively too?**

A mature SRSI loop should not only improve the candidate system.

It should also improve:

```text
Evaluators

Counter-Evaluators

Search

Routing

Memory

Governance
```

This creates a more complete recursive system.

But evaluator modification should carry higher governance sensitivity than ordinary local capability improvement.

---

# 13. Improvement Sensitivity Levels

Future SRSI could formalize different classes of self-modification.

For example:

```text
Level 0 — Cosmetic Change

Level 1 — Local Performance Change

Level 2 — Behavioral Logic Change

Level 3 — Policy Change

Level 4 — Evaluator Change

Level 5 — Improvement Runtime Change
```

Higher levels should require increasingly strong:

* evaluation,
* counter-evidence,
* verification,
* human review,
* rollback guarantees.

---

# 14. Improvement Governance

Improvement Governance is likely to become a major SRSI research area.

The central principle is:

```text
Validated Improvement
        ≠
Authorized Promotion
```

Future research should define machine-operable policies for:

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

---

## 14.1 Risk-Adaptive Promotion

Low-risk changes and high-risk changes should not follow the same promotion process.

Possible policy:

```text
Low Risk
   ↓
Fast Local Promotion

Medium Risk
   ↓
Staged Deployment

High Risk
   ↓
Deep Verification + Human Gate
```

Future SRSI should test such promotion ladders empirically.

---

## 14.2 Improvement Constitution

A mature SRSI system may require a relatively stable set of rules describing:

```text
What may self-modify?

What requires external approval?

Which evaluators must remain independent?

Which structures are immutable?

When is rollback mandatory?

Which evidence is required?
```

This can be called an:

# **Improvement Constitution**

It would define the boundaries of recursive self-modification.

---

## 14.3 Meta-Governance

If the system can modify its own governance rules, a deeper problem appears:

> **Who governs governance modification?**

Future SRSI should distinguish:

```text
Ordinary Improvement

Evaluator Improvement

Governance Improvement
```

with progressively stronger oversight.

---

# 15. Improvement Provenance

Every significant improvement should ideally preserve provenance.

A future provenance record may include:

```text
Candidate ID

Baseline ID

Generator

Evaluator Set

Counter-Evidence

Structural Difference

Verification Result

Promotion Authority

Deployment Scope

Runtime Outcome
```

This creates an auditable chain:

```text
Proposal
→ Evaluation
→ Promotion
→ Deployment
→ Outcome
```

Improvement Provenance may become central to:

* debugging,
* rollback,
* certification,
* accountability,
* evaluator benchmarking.

---

# 16. AI Coding SRSI Runtime

AI coding is one of the strongest candidates for an early SRSI MET.

A future runtime could implement:

```text
LLM Code Candidate
      ↓
Compile
      ↓
Unit Tests
      ↓
Integration Tests
      ↓
CallingGraph Delta
      ↓
Static Analysis
      ↓
Performance
      ↓
Security
      ↓
Counter-Evidence
      ↓
Promotion Gate
      ↓
Runtime Observation
      ↓
Structural Folding
```

This domain is attractive because evaluation is already highly machine-operable.

---

## 16.1 AI Coding MET-001

A minimal experiment:

```text
Baseline Function
       ↓
Generate 10 Candidate Patches
       ↓
Compile
       ↓
Tests
       ↓
CG Delta
       ↓
Rank
       ↓
Counter-Evidence
       ↓
Promote Best Local Candidate
```

Measure:

* selection quality,
* regression rate,
* evaluator disagreement,
* time cost,
* rollback rate.

---

## 16.2 AI Coding MET-002

Add Structural Memory.

```text
Previous Patch History
        ↓
Retrieve Similar Changes
        ↓
Generate New Candidate
        ↓
Evaluate
        ↓
Compare Search Cost
```

Question:

> Does folded improvement history reduce future search cost?

---

## 16.3 AI Coding MET-003

Add evaluator improvement.

Track which evaluators predicted runtime success best.

Then update evaluator routing.

Question:

> Can the improvement system improve its own evaluation process?

---

# 17. Scientific Recursive Self-Improvement

Scientific reasoning is another major SRSI direction.

A possible loop is:

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
Structural Differential
   ↓
Promotion / Rejection / Branch
   ↓
Knowledge Folding
   ↓
Next Hypothesis
```

Future work should explore:

* scientific Evaluator Packs,
* counterexample search,
* replication evaluators,
* mechanism consistency,
* uncertainty preservation,
* hypothesis memory.

---

# 18. Domain-Specific Evaluator Packs

One of the most practical future directions is building domain Evaluator Packs.

Potential packs include:

```text
AI Coding Evaluator Pack

Scientific Reasoning Evaluator Pack

Manufacturing Evaluator Pack

Market Evaluator Pack

Safety Evaluator Pack

Policy Evaluator Pack

Engineering Design Evaluator Pack
```

Each pack should define:

```text
Input

Evaluator Set

Counter-Evaluators

Decision Structure

Uncertainty State

Promotion Interface
```

Evaluator Packs could become a reusable bridge between general AI generation and domain-specific recursive improvement.

---

# 19. Evaluator Benchmarking

If evaluators become core infrastructure, they need benchmarks.

Future benchmark questions include:

```text
Does the evaluator detect real regressions?

Does it detect evaluator gaming?

How context-sensitive is it?

How often does it disagree with runtime outcomes?

How robust is it to adversarial candidates?

How reusable is it across domains?
```

This may lead to a new class of benchmarks focused on:

# **Improvement Judgment Quality**

rather than raw model capability.

---

# 20. Evaluator Security

Evaluator infrastructure creates a new attack surface.

Potential threats include:

```text
Evaluator Poisoning

Benchmark Gaming

Evidence Forgery

Counter-Evidence Suppression

Routing Manipulation

Policy Bypass

Evaluator Collusion
```

Future SRSI should therefore develop:

* evaluator isolation,
* independent verification,
* evidence provenance,
* evaluator diversity,
* protected policy gates.

---

# 21. Improvement Attack Surface

A future SRSI security model should explicitly represent:

# **Improvement Attack Surface**

This includes every component capable of influencing what becomes promoted:

```text
Generator

Evaluator

Counter-Evaluator

Search

Memory

Router

Verification

Governance

Deployment
```

The more recursive the system becomes, the more consequential compromise of these components may become.

---

# 22. Improvement Budgets

Recursive improvement consumes resources.

Future systems may need explicit budgets for:

```text
Generation

Evaluation

Counter-Evidence

Verification

Runtime Experiment

Memory

Human Review
```

This suggests a resource allocation problem:

> **Where should the system spend its next unit of improvement compute?**

Possible strategies include:

* highest expected gain,
* highest uncertainty,
* highest risk,
* highest reuse potential.

---

# 23. Improvement Queues

Large systems may contain many possible improvement targets.

Future runtimes may maintain:

```text
Improvement Queue
```

with priorities based on:

```text
Severity

Frequency

Impact

Confidence

Risk

Cost

Expected Benefit
```

This would turn RSI into a managed runtime service rather than uncontrolled recursive search.

---

# 24. Structural Search for Improvement

Structural Search itself deserves deeper optimization.

Possible future questions:

```text
Can MDT reduce candidate search space?

Can UTN improve candidate compatibility search?

Can CallingGraph identify high-value improvement nodes?

Can Counter-Evidence redirect search away from false optima?

Can Structural Memory guide future search?
```

The long-term objective is:

> **search where improvement is structurally plausible.**

---

# 25. Improvement Search vs. Candidate Search

Future work should distinguish:

```text
Candidate Search
```

from:

```text
Improvement Search
```

Candidate Search asks:

> Which candidate scores highest?

Improvement Search asks:

```text
Where is improvement needed?

What structure is responsible?

Which candidate is relevant?

What counter-evidence exists?

What deployment scope is appropriate?
```

This distinction may become fundamental to SRSI.

---

# 26. Evaluator Discovery

A particularly interesting future direction is whether repeated improvement failures can reveal missing evaluators.

Example:

```text
Candidate repeatedly passes
        ↓
Runtime repeatedly fails
        ↓
Missing evaluation dimension suspected
        ↓
New evaluator discovered
```

This suggests:

# **Evaluator Discovery**

The system not only improves candidates.

It learns what should be evaluated.

---

# 27. Leftover-Driven Evaluator Discovery

Repeated Leftover cases may contain strong signals.

If many unresolved candidates share the same structure:

```text
Leftover Cluster
       ↓
Common Missing Dimension
       ↓
Candidate New Evaluator
```

This creates a possible path from uncertainty to new intelligence structure.

---

# 28. Evaluator Markets and Evaluator Economy

If machine-operable judgment becomes valuable, evaluator infrastructure may develop into a broader ecosystem.

Possible components include:

```text
Evaluator Providers

Evaluator Benchmarks

Evaluator Certification

Evaluator Packs

Evaluator Routers

Evaluator Reputation

Evaluator Security
```

This is the basis of the SRSI concept:

# **Evaluator Economy**

Future work should explore whether evaluator quality becomes a distinct source of competitive advantage.

---

# 29. Open Evaluator Infrastructure

Open-source evaluators may play an important role.

Potential benefits include:

* transparency,
* reproducibility,
* evaluator diversity,
* reduced monopoly pressure,
* easier benchmarking,
* shared scientific progress.

A major open question is:

> **Can open evaluator ecosystems become shared infrastructure for safe and productive recursive improvement?**

---

# 30. Evaluator Monopoly Risk

If one evaluator architecture becomes dominant, recursive systems may inherit the same blind spots.

Future SRSI should therefore study:

```text
Evaluator Concentration

Evaluator Monoculture

Shared Failure Modes

Benchmark Lock-In
```

This motivates:

# **Evaluator Pluralism**

---

# 31. Collective Recursive Improvement

A major long-term direction is moving beyond single-system RSI.

Possible architecture:

```text
System A learns Improvement X
        ↓
Structural Memory
        ↓
Validated Improvement Package
        ↓
System B
        ↓
Context Re-Evaluation
        ↓
Adapt / Reject / Branch
```

This creates:

# **Collective Recursive Improvement**

The key is that transferred improvement should remain subject to local evaluation and governance.

---

# 32. Improvement Networks

Future systems may exchange structured improvement packages containing:

```text
Candidate Structure

Context

Evidence

Counter-Evidence

Evaluator History

Runtime Outcome

Policy Constraints
```

This could form:

# **Improvement Networks**

Such networks would differ from ordinary model sharing because they exchange validated improvement experience rather than only parameters or raw data.

---

# 33. Structural Improvement Capital

Repeated recursive improvement may create a durable asset:

```text
Validated Changes

Rejected Changes

Failure Histories

Evaluator Histories

Counterexamples

Runtime Outcomes
```

This is:

# **Structural Improvement Capital**

Future research should investigate whether this accumulated structural memory:

* improves future search,
* reduces repeated failure,
* accelerates adaptation,
* supports transfer across systems.

---

# 34. Improvement Capital Transfer

A further question is whether Structural Improvement Capital can be transferred between:

```text
Models

Agents

Organizations

Domains

Versions
```

Transfer may require:

* UTN compatibility,
* context matching,
* evaluator re-validation,
* policy adaptation.

This could become a major research area.

---

# 35. SRSI and Non-Stationary Environments

Many domains change over time.

Therefore:

```text
Yesterday's Improvement
        ≠
Today's Improvement
```

Future SRSI needs mechanisms for:

* context drift,
* evaluator drift,
* branch expiration,
* policy change,
* memory decay,
* re-validation.

This is especially important in:

* markets,
* cybersecurity,
* evolving software ecosystems,
* scientific knowledge.

---

# 36. Reversibility-Aware Improvement

Future SRSI should treat reversibility as a design dimension.

A candidate that offers slightly less gain but much easier rollback may sometimes be preferable.

This suggests evaluating:

```text
Expected Benefit

Risk

Rollback Cost

Recovery Time

State Preservation
```

together.

This can be called:

# **Reversibility-Aware Improvement**

---

# 37. Improvement Contracts

Localized improvement may benefit from explicit contracts.

A structural node could declare:

```text
Inputs

Outputs

Dependencies

Safety Constraints

Performance Requirements

Allowed Mutation Scope
```

A candidate must satisfy the contract before promotion.

This suggests:

# **Structural Improvement Contracts**

UTN and CallingGraph structures may provide useful foundations.

---

# 38. Formal Verification

Some high-impact improvements may require stronger guarantees.

Future SRSI could integrate:

* formal verification,
* proof-carrying code,
* symbolic constraints,
* invariant checking,
* model checking.

Formal methods are unlikely to replace all empirical evaluation.

But they may provide strong evidence for selected structures.

---

# 39. Bounded Guarantees

A realistic SRSI objective may not be:

```text
Prove the whole system safe forever.
```

Instead:

```text
Prove this change preserves these invariants
within this scope
under these assumptions.
```

This suggests:

# **Bounded Structural Guarantees**

These may be much more practical.

---

# 40. Human Participation

SRSI does not require removing humans from improvement loops.

Humans may contribute as:

```text
Evaluator Designers

Counter-Evidence Sources

Policy Authorities

Domain Experts

Promotion Approvers

Audit Reviewers
```

Future research should identify where human judgment provides the highest leverage.

---

# 41. Human–AI Evaluator Composition

Human and machine evaluators may have complementary strengths.

Possible pattern:

```text
Machine Evaluation
      ↓
Structural Summary
      ↓
Human Review
      ↓
Policy Decision
```

or:

```text
Human Concern
      ↓
Counter-Evidence Search
      ↓
Machine Verification
```

This may become an important form of hybrid intelligence.

---

# 42. SRSI Before AGI

A major research proposition remains:

> **Recursive improvement can be studied and engineered before AGI.**

Future work should prioritize narrow domains where the full loop can already be executed.

Possible early environments:

```text
AI Coding

Database Optimization

Compiler Optimization

Scientific Workflow

Manufacturing Process

Policy Simulation

Market Strategy Research
```

---

# 43. Minimum Engineering Tests

SRSI should advance through METs.

A canonical sequence could be:

## MET-001 — Rich Evaluation

Compare scalar evaluation with Rich Evaluation.

## MET-002 — Counter-Evidence

Measure whether active counter-evidence reduces false promotion.

## MET-003 — Localization

Measure whether local search reduces cost and regression.

## MET-004 — Structural Memory

Measure whether folded history improves future cycles.

## MET-005 — Governance

Measure staged promotion and rollback effectiveness.

## MET-006 — Recursive Evaluator Improvement

Allow evaluator selection or weighting to evolve.

This progression would convert SRSI from framework into testable engineering evidence.

---

# 44. SRSI Benchmark Suite

A future benchmark suite could evaluate full improvement loops.

Candidate metrics include:

```text
True Improvement Rate

False Promotion Rate

False Rejection Rate

Regression Rate

Rollback Rate

Evaluation Cost

Search Cost

Improvement Latency

Memory Reuse Rate

Counter-Evidence Detection Rate

Long-Horizon Stability
```

Such benchmarks could compare different improvement architectures.

---

# 45. Validated Improvement Loop as a Unit of Progress

AI progress is often measured by:

```text
Model Size

Benchmark Score

Training Compute
```

SRSI suggests another possible unit:

# **Validated Improvement Loop**

A strong loop repeatedly demonstrates:

```text
Generate
→ Evaluate
→ Challenge
→ Verify
→ Promote
→ Observe
→ Learn
```

Future AI systems may be judged not only by what they can do once, but by how reliably they can improve.

---

# 46. Scale × Structure

Future work should avoid framing structural intelligence as the opposite of scaling.

A more productive research direction is:

```text
Scale
  ×
Structure
```

More compute can support:

* broader search,
* deeper evaluation,
* more counter-evidence,
* more simulation.

Structure can make that compute more targeted and interpretable.

---

# 47. Open Research Questions

The following questions remain central.

### Evaluation

* What makes an evaluator rich enough?
* How should evaluator quality be measured?
* How should evaluator disagreement be interpreted?

### Goodhart

* How quickly do strong generators learn evaluator weaknesses?
* Can Counter-Evidence Search materially reduce false promotion?

### Localization

* How accurately can improvement targets be localized?
* When does local improvement cause global regression?

### Memory

* What improvement history should be preserved?
* How should negative improvement memory be retrieved?

### Governance

* Which changes require which level of authority?
* How should evaluator modifications be governed?

### Runtime

* Which domains support SRSI before AGI?
* What is the smallest closed improvement loop that produces cumulative benefit?

### Ecosystem

* Can Evaluator Packs become reusable infrastructure?
* Can validated improvements be transferred between systems?

---

# 48. Suggested Research Sequence

A practical next-stage roadmap is:

```text
Phase 1
Rich Evaluator MET
        ↓
Phase 2
Counter-Evidence MET
        ↓
Phase 3
Localized RSI MET
        ↓
Phase 4
Structural Memory
        ↓
Phase 5
Improvement Governance
        ↓
Phase 6
Recursive Evaluator Improvement
        ↓
Phase 7
Collective Improvement
```

This progression preserves engineering tractability.

---

# 49. Near-Term Priorities

For the immediate post-v1.0 phase, the highest-value directions are likely:

## Priority 1

**AI Coding SRSI MET**

Because strong evaluators already exist.

## Priority 2

**Rich Evaluator Benchmark**

Because the core SRSI thesis depends on evaluation quality.

## Priority 3

**Counter-Evidence Runtime**

Because Anti-Goodhart capability is essential.

## Priority 4

**Localized Per-Node RSI**

Because local improvement is more testable than whole-system replacement.

## Priority 5

**Improvement Memory**

Because recursive improvement becomes truly cumulative only when validated experience survives.

---

# 50. Long-Term Vision

A mature Structural Recursive Self-Improvement infrastructure may eventually look like:

```text
Runtime Evidence
      ↓
Structural Localization
      ↓
Candidate Generation
      ↓
Rich Evaluator Plane
      ↕
Counter-Evidence Plane
      ↓
Structural A/B
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
Evaluator Improvement
      ↓
Next Improvement Cycle
      ↺
```

This would not simply be a system that generates better versions of itself.

It would be a system that progressively improves:

```text
its candidates

its evaluators

its search

its memory

its governance

its ability to prove itself wrong
```

---

# 51. Final Direction

The deepest future direction of SRSI is not:

> How can AI modify itself faster?

It is:

> **How can recursive improvement become progressively better at determining what deserves to be called improvement?**

That question leads naturally to:

```text
Rich Evaluators

Counter-Evidence

Structural Search

Localized Improvement

Improvement Memory

Governed Promotion

Recursive Evaluator Improvement
```

The long-term SRSI objective is therefore:

> **not uncontrolled recursive optimization, but cumulative, contestable, reversible, and governable structural improvement.**

---

# Related Documents

For the project overview:

[`README.md`](README.md)

For the reading guide:

[`START-HERE.md`](START-HERE.md)

For repository navigation:

[`CONTENTS.md`](CONTENTS.md)

For terminology:

[`GLOSSARY.md`](GLOSSARY.md)

For figures:

[`FIGURE-INDEX.md`](FIGURE-INDEX.md)
