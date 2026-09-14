# SRSI-003 — DBM-SI as a Rich Evaluator and Improvement Infrastructure

## Reinterpreting Structural Intelligence as an Evaluation, Localization, Memory, and Governance Layer for Recursive Self-Improvement

**Project:** Structural Recursive Self-Improvement (SRSI)
**Repository:** `Structural-Recursive-Self-Improvement`
**Series:** SRSI-003
**Status:** Research Framework / Structural Mapping Paper

---

## Abstract

The first two papers in the Structural Recursive Self-Improvement (SRSI) series argued that Recursive Self-Improvement (RSI) requires more than increasingly powerful candidate generation and search.

A mature RSI system also requires rich evaluation, counter-evidence, structural localization, verification, memory, and governance.

This raises a practical question:

> **Where can such structures come from?**

This paper examines one concrete answer.

The DBM-SI research program has developed a family of structural mechanisms for intelligence, localization, comparison, search, memory, trajectory reasoning, CallingGraph analysis, typing, policy control, folding/unfolding, and per-node computation.

These mechanisms were not originally created as a unified RSI evaluation stack.

However, when viewed from the SRSI perspective, many of them acquire a second role:

> **They can function as machine-operable evaluators and improvement infrastructure.**

Examples include:

* Metric Differential Trees as differential and localization evaluators,
* Two-Way CCC as structural A/B comparison,
* Counter-Evidence Search as falsification infrastructure,
* UTN as identity and compatibility evaluation,
* CallingGraph and CallingGraph Delta as behavioral and change-impact evaluation,
* Trajectory Intelligence as long-horizon evaluation,
* Per-Node Intelligence as localized improvement,
* Structural Folding as cumulative improvement memory,
* PDS as improvement governance,
* Leftover branches as explicit unresolved-candidate preservation.

The purpose of this paper is not to claim that DBM-SI is the only path to SRSI.

Instead, it presents DBM-SI as a concrete example of how a broad family of existing structural computation can be reorganized into an **RSI Rich Evaluator and Improvement Infrastructure**.

The deeper implication is that structural intelligence may have an important dual role:

> **to perform intelligence, and to evaluate and govern the improvement of intelligence.**

---

# 1. From Structural Intelligence to Improvement Infrastructure

The DBM-SI research program has historically focused on questions such as:

```text id="j7qjss"
How can differences be localized?

How can structural patterns be folded?

How can behavior be represented as trajectories?

How can decisions be governed by policy?

How can CallingGraphs support reasoning?

How can identities remain stable across contexts?

How can local structures become intelligent?

How can evidence and counter-evidence coexist?

How can structural growth preserve branches and leftovers?
```

These are intelligence questions.

But RSI introduces a second interpretation.

A recursively improving system must also ask:

```text id="5yadwg"
What changed?

Where did it change?

Which structure improved?

Which structure regressed?

Which context applies?

What evidence supports promotion?

What counter-evidence exists?

Should the change remain local?

Should it become a branch?

Should it be rejected?

Should it be preserved?

Can it be rolled back?

How should the result influence the next improvement cycle?
```

The overlap is substantial.

This suggests a new interpretation:

> **Many structural-intelligence mechanisms are also improvement-evaluation mechanisms.**

That dual role is the focus of this paper.

---

# 2. DBM-SI Is Not Proposed as the Exclusive SRSI Architecture

A critical clarification is necessary.

SRSI is intended as an open framework.

Rich Evaluators can be built using many technologies:

* formal methods,
* testing systems,
* graph analysis,
* probabilistic models,
* symbolic reasoning,
* simulation,
* LLM critics,
* adversarial agents,
* policy engines,
* human review,
* domain-specific evaluators.

DBM-SI is therefore not presented as:

> the only valid implementation of SRSI.

Instead, the claim is narrower and more useful:

> **DBM-SI already contains a substantial collection of structural computation mechanisms that map naturally onto key SRSI responsibilities.**

This makes it a useful concrete provider and experimental substrate for SRSI.

---

# 3. The Structural Reinterpretation Principle

A useful principle is:

> **A structure designed to represent, localize, compare, search, govern, or preserve intelligence may also serve as a structure for evaluating and improving intelligence.**

For example:

A differential tree used to locate structural similarity can also locate improvement differences.

A CallingGraph used to represent execution structure can also evaluate the impact of code change.

A policy runtime used to decide actions can also decide whether an improvement should be promoted.

A folding mechanism used to preserve experience can also preserve validated improvement history.

This reinterpretation does not require changing the underlying structure.

It changes the role assigned to it.

---

# 4. DBM-SI Structures as SRSI Infrastructure

The mapping can be summarized as follows.

| DBM-SI Structure               | Original Structural Role                 | SRSI Role                              |
| ------------------------------ | ---------------------------------------- | -------------------------------------- |
| Metric Differential Tree (MDT) | Difference organization and localization | Differential evaluator                 |
| CCC                            | Structural relation and dispatch         | Structural consistency evaluator       |
| Two-Way CCC                    | A/B structural differentiation           | Comparative improvement evaluator      |
| Counter-Evidence Search        | Search for opposing structure            | Falsification evaluator                |
| UTN                            | Typing, naming, identity continuity      | Identity / compatibility evaluator     |
| CallingGraph                   | Execution-path structure                 | Behavioral-path evaluator              |
| CallingGraph Delta             | Structural code change                   | Change-impact evaluator                |
| Trajectory Intelligence        | Multi-step behavioral structure          | Long-horizon evaluator                 |
| Per-Node Intelligence          | Local structural intelligence            | Localized improvement engine           |
| Structural Search Plane        | Structure-guided retrieval               | Improvement candidate localization     |
| Structural Folding             | Experience compression and reuse         | Improvement memory                     |
| Folding / Unfolding            | Reuse and execution reconstruction       | Improvement reuse / deployment         |
| Leftover Branch                | Explicit unresolved structure            | Uncertainty-preserving evaluator state |
| 3-Cat Learning                 | Structural differentiation and growth    | Continual improvement branching        |
| DNA Dispatch / Trigger         | Structural routing                       | Evaluator and candidate dispatch       |
| PDS                            | Policy-controlled decision runtime       | Improvement governance plane           |

This table is not a proof.

It is a research map.

The remaining sections explain why these mappings are technically meaningful.

---

# 5. Metric Differential Tree as a Differential Evaluator

Recursive improvement depends on difference.

Suppose:

```text id="gxbh7c"
Current System = A
Candidate System = B
```

A primitive evaluator may compute:

```text id="60b7w3"
Score(B) > Score(A)
```

But an SRSI system often needs:

```text id="v9evw5"
Where are A and B different?

How large is the difference?

Which dimensions changed?

Which differences are meaningful?

Which changes correlate with improvement?

Which changes correlate with regression?
```

This is naturally a metric differential problem.

MDT can therefore support:

> **Differential Evaluation**

A simplified flow is:

```text id="lq7566"
A
│
├── Representation
│
B
│
↓
Metric Difference
↓
Differential Structure
↓
Localized Difference Nodes
↓
Improvement / Regression Analysis
```

Instead of treating the candidate as globally better or worse, MDT encourages explicit localization.

This is particularly useful when the candidate differs across many dimensions.

---

# 6. Two-Way CCC as Structural A/B Evaluation

Two-Way CCC is one of the strongest direct connections between DBM-SI and RSI.

Traditional A/B evaluation often asks:

```text id="l6q1sj"
Which performs better?
```

Two-Way CCC asks a richer question:

```text id="2v2j1b"
What is structurally shared?

What is structurally different?

Which differences belong to A?

Which differences belong to B?

Which branch should be preserved?
```

In an SRSI setting:

```text id="639l0c"
Current Structure A
        ↕
    Two-Way CCC
        ↕
Candidate Structure B
```

The output can support:

```text id="qjm0rw"
Shared structure
A-specific strength
B-specific strength
A-specific failure
B-specific failure
Context dependency
Branch opportunity
```

This transforms A/B comparison from simple winner selection into structural differentiation.

The result may be:

```text id="9hykml"
PROMOTE B
```

but it may also be:

```text id="6r2aql"
KEEP A

or

BRANCH A / B

or

LOCALIZE B

or

LEFTOVER B
```

Thus Two-Way CCC supports a key SRSI principle:

> **Improvement does not have to mean replacement.**

---

# 7. Counter-Evidence Search as a Falsification Evaluator

One of the most important weaknesses of strong optimization is confirmation pressure.

Once a candidate appears promising, the system may accumulate evidence supporting it.

SRSI requires a complementary process:

> **Search explicitly for evidence against the candidate.**

DBM-SI Counter-Evidence Search provides a natural mechanism.

The loop becomes:

```text id="vo0q5z"
Candidate
    ↓
Evidence Search
    ↕
Counter-Evidence Search
    ↓
Structural Comparison
    ↓
Promotion Decision
```

The purpose is not to reject every candidate.

It is to make improvement claims survive structured challenge.

Counter-Evidence Search can look for:

```text id="7k1qjt"
Failure contexts

Opposing patterns

Regression branches

Historical exceptions

Structural incompatibilities

Trajectory instability

Policy conflicts
```

This gives DBM-SI a direct role in:

> **Anti-Goodhart evaluation.**

A candidate optimized for the primary evaluator must also survive counter-evaluation.

---

# 8. UTN as an Identity and Compatibility Evaluator

Recursive improvement creates identity problems.

If a structure changes, the system must determine:

```text id="2b6wj5"
Is this still the same functional object?

Is this a compatible replacement?

Does the new object preserve required type relationships?

Does the modification apply to this context?

Which identity should runtime dispatch use?
```

UTN provides a structural framework for:

* typing,
* naming,
* identity continuity,
* context-bound identity,
* cross-structure correspondence.

In SRSI, UTN can therefore support:

> **Identity-Preserving Improvement Evaluation**

For example:

```text id="r0g06d"
Function F
   ↓
Candidate F'
   ↓
UTN Identity / Type Check
   ↓
Compatible?
   ├── Yes → continue evaluation
   └── No  → branch / reject / remap
```

This is especially important when improvements are localized.

A local change should not silently destroy the structural identity expected by downstream components.

---

# 9. CallingGraph as a Behavioral-Path Evaluator

Software improvement is one of the clearest domains for early SRSI experiments.

A code candidate may pass tests while still altering important execution structure.

CallingGraph evaluation asks:

```text id="5woy8a"
Which calls changed?

Which paths were added?

Which paths disappeared?

Which functions became unreachable?

Which runtime behaviors changed?

Which structural dependencies shifted?
```

Thus CallingGraph analysis can act as:

> **Behavioral-Path Evaluation**

The comparison becomes:

```text id="6ardni"
CallingGraph(A)
      ↕
Structural Comparison
      ↕
CallingGraph(B)
```

The evaluator can detect changes that output-only tests may miss.

This helps bridge:

```text id="57jy1e"
External Behavior
```

and:

```text id="8p37zn"
Internal Structural Change
```

---

# 10. CallingGraph Delta as a Change-Impact Evaluator

CallingGraph Delta extends this further.

Instead of comparing entire programs, it focuses on change:

```text id="xwzr86"
Baseline CG
    ↓
Candidate Delta
    ↓
Affected Nodes
    ↓
Affected Paths
    ↓
Affected Runtime Regions
```

This is extremely relevant to localized RSI.

The core question becomes:

> **What is the structural blast radius of this candidate improvement?**

The evaluator can help determine:

```text id="v3y26h"
Local effect

Downstream effect

Cross-module effect

Hidden dependency effect

Regression surface
```

This supports:

* targeted verification,
* selective rollout,
* rollback,
* per-node improvement,
* lower-cost evaluation.

---

# 11. Trajectory Intelligence as a Long-Horizon Evaluator

Not all improvements can be judged at one step.

Many systems generate trajectories:

```text id="41f8ga"
State0
  ↓
Action1
  ↓
State1
  ↓
Action2
  ↓
State2
  ↓
...
```

A candidate may improve immediate performance while degrading long-horizon behavior.

Trajectory Intelligence therefore maps naturally to:

> **Long-Horizon Improvement Evaluation**

For example:

```text id="e8u6je"
Candidate A
   ↓
Trajectory TA

Candidate B
   ↓
Trajectory TB

TA ↔ TB
   ↓
Risk / Stability / Outcome Comparison
```

This can expose:

* delayed regressions,
* policy drift,
* unstable feedback,
* cumulative cost,
* trajectory divergence.

For agentic RSI, this is especially important.

---

# 12. Per-Node Intelligence as Localized RSI

Whole-system self-improvement is expensive and risky.

Per-Node Intelligence introduces another model:

```text id="zr9zft"
System
├── Node A
├── Node B
├── Node C
└── Node D
```

Instead of:

```text id="k8mk8e"
Replace whole system
```

the system can:

```text id="4ksbmi"
Locate Node C
      ↓
Generate Candidate C'
      ↓
Evaluate C vs. C'
      ↓
Verify integration
      ↓
Promote locally
```

This is:

# **Localized RSI**

Localized RSI offers several advantages:

* smaller search space,
* lower evaluator cost,
* easier regression tracing,
* easier rollback,
* clearer causality,
* more targeted deployment.

This may be one of the most practical ways to implement recursive improvement before whole-system autonomous RSI becomes feasible.

---

# 13. Structural Search Plane as Improvement Localization

DBM-SI Structural Search is designed to locate relevant structures efficiently.

In SRSI, this capability can support:

```text id="93mh9y"
Where should improvement search begin?
```

Instead of generating modifications everywhere, the system may first identify:

```text id="nsutvi"
High-error branch

High-cost branch

Unstable branch

Low-confidence node

Frequently failing trajectory

Counter-evidence cluster

Policy-conflict region
```

Then improvement search is localized.

A possible flow is:

```text id="9dw9rs"
Runtime Evidence
      ↓
Structural Search
      ↓
Problem Region
      ↓
Candidate Generator
      ↓
Local Evaluation
```

This makes RSI structurally targeted rather than globally indiscriminate.

---

# 14. DNA Dispatch and Trigger as Improvement Routing

Once candidate generation, evaluation, and structural search become modular, routing becomes important.

A candidate may need different evaluators depending on:

```text id="x9t8rz"
Type
Context
Risk
Affected structure
Uncertainty
Deployment scope
```

DNA Dispatch / Trigger mechanisms can support:

> **Evaluator and Improvement Routing**

For example:

```text id="4g3l2h"
Candidate
   ↓
Structural Signature
   ↓
DNA Dispatch
   ├── MDT Evaluator
   ├── CG Evaluator
   ├── Trajectory Evaluator
   ├── Counter-Evidence Evaluator
   └── PDS Governance
```

This creates a practical bridge between Rich Evaluator theory and runtime execution.

---

# 15. Structural Folding as Improvement Memory

Recursive improvement becomes much more powerful when successful and unsuccessful attempts are preserved.

A candidate cycle generates:

```text id="yjdyjr"
Candidate
Context
Difference
Evidence
Counter-Evidence
Decision
Deployment
Runtime Outcome
```

Structural Folding can compress this into reusable experience.

The result is:

```text id="pw63n8"
Improvement Experience
        ↓
Structural Folding
        ↓
Reusable Improvement Unit
        ↓
Future Search / Dispatch / Evaluation
```

This transforms RSI from repeated isolated experimentation into cumulative improvement.

The system begins to remember:

```text id="t26pkj"
Which changes worked?

Where?

Under which contexts?

Which failed?

Why?

Which evaluators were reliable?

Which branches should be reused?
```

Structural Folding therefore provides:

> **Improvement Memory**

---

# 16. Folding and Unfolding as Improvement Reuse

Folding preserves experience.

Unfolding reactivates it.

In SRSI:

```text id="cik9c5"
Past Validated Improvement
        ↓
Folded Structural Memory
        ↓
Current Context
        ↓
Unfold
        ↓
Candidate / Policy / Runtime Structure
```

This means recursive improvement does not always require search from scratch.

The system can reuse prior validated improvement structures.

This creates a cycle:

```text id="1mlxh4"
Improve
  ↓
Validate
  ↓
Fold
  ↓
Reuse
  ↓
Adapt
  ↓
Improve Again
```

This is a major source of cumulative efficiency.

---

# 17. Leftover as an Explicit Uncertainty State

Many optimization systems force a decision:

```text id="jcw2in"
Accept
or
Reject
```

DBM-SI Leftover introduces a third possibility:

> **Not enough evidence yet. Preserve explicitly.**

In SRSI:

```text id="drnwyu"
Candidate
   ↓
Evaluation
   ↓
Evidence incomplete
   ↓
LEFTOVER
```

This has several advantages.

It prevents:

* premature rejection,
* premature promotion,
* forced binary decisions,
* loss of potentially useful candidates.

Later:

```text id="v0h1y1"
New evidence
      ↓
Re-evaluate Leftover
      ↓
Promote / Branch / Reject
```

This gives recursive improvement an important property:

> **Epistemic patience.**

---

# 18. 3-Cat Learning as Continual Improvement Growth

A structural learning system may classify candidate differences into:

```text id="fwgd1s"
A-like

B-like

New / Third Category
```

This becomes powerful in RSI.

Suppose a candidate does not fit the current structure.

Instead of forcing it into A or B:

```text id="pdiqgh"
Candidate C
   ↓
Third Category
   ↓
New Branch
```

This enables:

> **Recursive Structural Growth**

The system does not merely optimize existing branches.

It can create new structural categories when evidence demands them.

This is particularly important in non-stationary environments.

---

# 19. PDS as an Improvement Governance Plane

PDS provides perhaps the clearest bridge from evaluation to deployment.

An SRSI system must distinguish:

```text id="84ne9z"
Candidate generated

Candidate evaluated

Candidate validated

Candidate authorized

Candidate deployed
```

These are different states.

PDS can implement policy over promotion:

```text id="kir4a6"
Candidate
   ↓
Evaluation Result
   ↓
Risk
   ↓
Context
   ↓
Policy
   ↓
Decision
```

Possible outputs include:

```text id="rtzi93"
PROMOTE
LOCAL-ONLY
EXPERIMENTAL
BRANCH
HOLD
REJECT
ROLLBACK
```

Thus PDS can act as:

# **Improvement Governance Plane**

This is critical because:

> **Technical improvement does not automatically imply deployment authorization.**

---

# 20. From Action Governance to Improvement Governance

Action governance asks:

> Should the system perform this action?

Improvement governance asks:

> Should this candidate become part of the system that will perform future actions?

These are related but distinct.

A candidate can be technically effective yet inappropriate for:

* global deployment,
* high-risk contexts,
* autonomous activation,
* permanent promotion.

Thus:

```text id="9gj30f"
Capability
   ≠
Validated Improvement
   ≠
Authorized Promotion
   ≠
Authorized Action
```

This layered separation may become important in advanced RSI systems.

---

# 21. DBM-SI as an Evaluator Portfolio

The DBM-SI structures can now be reorganized into an SRSI Evaluator Portfolio.

```text id="m53r9a"
                       Candidate
                           │
                           ↓
                  Structural Dispatch
                           │
        ┌──────────────────┼──────────────────┐
        ↓                  ↓                  ↓
      MDT               Two-Way CCC          UTN
 Differential            A/B Compare       Identity
 Evaluator                                 Evaluator
        │                  │                  │
        ├──────────────────┼──────────────────┤
        ↓                  ↓                  ↓
 Counter-Evidence      CallingGraph       Trajectory
 Falsification         Path Impact        Long-Horizon
        │                  │                  │
        ├──────────────────┼──────────────────┤
        ↓                  ↓                  ↓
 Per-Node             Structural Folding      PDS
 Localization          Improvement Memory   Governance
        │                  │                  │
        └──────────────────┼──────────────────┘
                           ↓
                  Improvement Decision
```

This is not a rigid pipeline.

It is a composable evaluator infrastructure.

---

# 22. A Canonical DBM-SI SRSI Loop

A generic recursive improvement loop can be expressed as:

```text id="mafp71"
Runtime Evidence
      ↓
Structural Search
      ↓
Problem Localization
      ↓
Candidate Generation
      ↓
MDT Difference Analysis
      ↓
Two-Way CCC Comparison
      ↓
Counter-Evidence Search
      ↓
UTN Compatibility Check
      ↓
CG / Trajectory Verification
      ↓
Per-Node Integration
      ↓
PDS Promotion Governance
      ↓
Deployment
      ↓
Runtime Observation
      ↓
Structural Folding
      ↓
Next Improvement Cycle
```

This is a concrete example of Structural RSI.

---

# 23. Improvement as Structural Differentiation

One of the strongest implications of this architecture is that recursive improvement need not be linear.

Traditional model:

```text id="vapvhy"
A
↓
B
↓
C
↓
D
```

Structural model:

```text id="o1dxpy"
          Root
       /   |   \
      A    B    C
     / \        |
   A1  A2       C1
```

Different branches may serve different contexts.

The improvement process becomes:

> **Recursive Structural Differentiation and Growth**

This is a natural outcome of:

* Two-Way CCC,
* context evaluation,
* 3-Cat Learning,
* Leftover,
* UTN,
* PDS.

The system does not have to converge prematurely to one global winner.

---

# 24. Improvement as Structural Memory Growth

A second implication is that RSI can be understood as memory growth.

Every validated improvement adds:

```text id="dvom3o"
New difference

New branch

New context mapping

New evaluator result

New counter-evidence

New policy

New runtime evidence
```

These are folded into structural memory.

Therefore:

> **Recursive improvement can be viewed as recursive growth of validated structural memory.**

This connects SRSI directly with Structural Folding and Continual Structural Learning.

---

# 25. Improvement as Local Search Rather Than Global Reinvention

A third implication is computational.

If the system can locate:

```text id="dbmtt6"
where failure occurs
```

then it can search:

```text id="b7vtxd"
where improvement is needed
```

This reduces the problem from:

```text id="12gbbz"
Search entire system
```

to:

```text id="gmxf0g"
Locate
↓
Search locally
↓
Evaluate locally
↓
Verify globally
```

This is likely to be much more scalable.

It also aligns with practical software engineering.

---

# 26. The Importance of Structural Auditability

A major advantage of DBM-SI-style structures is that many operations can leave explicit artifacts.

For example:

```text id="s2q7nt"
Difference Tree

A/B Branch

CallingGraph Delta

Counter-Evidence Set

Trajectory Trace

Policy Decision

Folded Improvement Record
```

These artifacts create an audit trail.

A system can answer:

```text id="3zlkdb"
Why was this candidate promoted?

What evidence supported it?

What counter-evidence existed?

Which evaluator disagreed?

Which branch was changed?

Which policy authorized deployment?

What happened afterward?
```

This is valuable for:

* debugging,
* research,
* safety,
* governance,
* rollback,
* human oversight.

Thus:

> **Structural auditability is itself an SRSI capability.**

---

# 27. DBM-SI as a Machine-Operable Improvement Language

Taken together, the structures begin to resemble a language for improvement.

They can express:

```text id="c6taz7"
Difference

Identity

Branch

Context

Evidence

Counter-Evidence

Trajectory

Policy

Memory

Promotion State
```

This is more than a collection of algorithms.

It suggests the possibility of a:

> **Machine-Operable Improvement Representation**

Such a representation could allow AI systems to reason explicitly about their own candidate modifications.

---

# 28. Example: AI Coding

AI coding provides a concrete SRSI example.

Suppose an AI proposes:

```text id="kbyo8v"
Code Candidate B
```

The DBM-SI evaluator stack may process:

```text id="zlwhxs"
Compile
   ↓
Tests
   ↓
CallingGraph Delta
   ↓
MDT Difference
   ↓
Two-Way CCC
   ↓
Counter-Evidence Search
   ↓
Runtime Trajectory
   ↓
UTN Compatibility
   ↓
PDS Promotion Gate
   ↓
Deploy Locally
   ↓
Observe
   ↓
Fold Result
```

This is already implementable in partial form.

It therefore provides a practical research platform for SRSI before general autonomous RSI.

---

# 29. Example: Structural Market Intelligence

A second example is structural market intelligence.

Suppose an RSI system generates a new market strategy.

A rich evaluator can examine:

```text id="8di1ku"
Return

Risk

Drawdown

Regime dependence

Pattern differential

Counterexamples

Liquidity

Crowding

Trajectory stability

Policy constraints
```

Structural Folding can preserve successful context-bound strategies.

Counter-Evidence can search for failing regimes.

Two-Way CCC can compare competing strategies.

PDS can restrict deployment scope.

This illustrates how RSI may accelerate domain-specific improvement without requiring global AGI.

---

# 30. Example: Scientific Reasoning

A scientific candidate may be evaluated by:

```text id="c6r19w"
Evidence fit

Mechanism

Counterexample

Replication

Cross-domain consistency

Prediction

Uncertainty

Structural compatibility
```

Counter-Evidence Search becomes especially important.

Structural memory can preserve:

```text id="7l3a3x"
Supported hypothesis

Rejected hypothesis

Conditional hypothesis

Unresolved hypothesis
```

Thus the same SRSI framework can support scientific improvement loops.

---

# 31. A New Interpretation of DBM-SI

The SRSI perspective suggests a broader interpretation of DBM-SI.

Previously:

> DBM-SI provides computational structures for intelligence.

Now:

> **DBM-SI may also provide computational structures for judging, localizing, preserving, and governing the improvement of intelligence.**

This is a significant shift.

It means that structural intelligence may participate in two levels:

```text id="k71oqe"
Level 1:
Perform intelligent computation

Level 2:
Evaluate and improve intelligent computation
```

The second level is the SRSI connection.

---

# 32. The Dual-Use Structural Principle

Many DBM-SI structures therefore exhibit a dual role.

For example:

```text id="vfr2ay"
MDT
  Intelligence Role:
    locate structural similarity/difference

  RSI Role:
    locate improvement/regression difference
```

```text id="xdspyp"
PDS
  Intelligence Role:
    govern action selection

  RSI Role:
    govern improvement promotion
```

```text id="6tl3om"
Folding
  Intelligence Role:
    preserve experience

  RSI Role:
    preserve validated improvement
```

This motivates:

> **The Dual-Use Structural Principle**

A structure capable of organizing intelligent behavior may often also help organize intelligent improvement.

---

# 33. What DBM-SI Does Not Yet Solve

It is equally important to state what remains open.

DBM-SI does not yet provide a complete autonomous RSI system.

Open problems include:

```text id="l1rwpu"
Evaluator calibration

Evaluator conflict resolution

Adversarial evaluator testing

Formal guarantees

Cross-domain evaluator transfer

Large-scale runtime integration

Evaluator learning

Evaluator corruption detection

Improvement rollback protocols

Multi-agent improvement governance

Resource-aware evaluator scheduling
```

These are important research directions.

The purpose of this paper is not to claim completion.

It is to identify a structural foundation.

---

# 34. From Structural Components to a Structural RSI Runtime

The next engineering step is to integrate these components into a runtime.

A possible architecture is:

```text id="05z7cy"
┌─────────────────────────────────────┐
│        AI Candidate Generator       │
├─────────────────────────────────────┤
│     Structural Search / Routing     │
├─────────────────────────────────────┤
│          Rich Evaluator Plane       │
│ MDT / CCC / UTN / CG / Trajectory   │
├─────────────────────────────────────┤
│       Counter-Evidence Plane        │
├─────────────────────────────────────┤
│       Localization / Per-Node       │
├─────────────────────────────────────┤
│        Verification Runtime         │
├─────────────────────────────────────┤
│       PDS Governance Plane          │
├─────────────────────────────────────┤
│          Deployment Layer           │
├─────────────────────────────────────┤
│       Runtime Evidence Layer        │
├─────────────────────────────────────┤
│      Structural Folding Memory      │
└─────────────────────────────────────┘
                 │
                 └────→ Next Cycle
```

This is a candidate architecture for DBM-SI-enabled SRSI.

---

# 35. Why This Matters for the Broader RSI Community

The importance of this mapping extends beyond DBM-SI.

It demonstrates a broader lesson:

> **RSI may benefit from reusing existing computational structures rather than waiting for one universal self-improvement algorithm.**

Many fields already contain useful evaluators.

For example:

```text id="cw62e5"
Software:
tests, graphs, traces, static analysis

Science:
replication, prediction, falsification

Markets:
risk, regime, counterfactuals

Engineering:
constraints, simulation, reliability

Governance:
policy, authorization, audit
```

SRSI can integrate such structures into richer improvement loops.

DBM-SI provides one example of this compositional strategy.

---

# 36. Toward an Evaluator Ecosystem

No single evaluator is likely to be sufficient.

The future may look more like:

```text id="0ik8pz"
Evaluator Ecosystem
│
├── Differential Evaluators
├── Structural Evaluators
├── Counter-Evaluators
├── Trajectory Evaluators
├── Identity Evaluators
├── Policy Evaluators
├── Runtime Evaluators
└── Human / External Evaluators
```

DBM-SI can contribute multiple members to this ecosystem.

Other frameworks can contribute others.

This open architecture is preferable to treating SRSI as a closed stack.

---

# 37. The Structural RSI Thesis

The main argument of this paper can be summarized as follows.

### Thesis 1

> **Many DBM-SI structures already satisfy key requirements of Rich Evaluator infrastructure.**

### Thesis 2

> **Structural comparison, localization, counter-evidence, trajectory analysis, identity, policy, and memory are all directly relevant to recursive improvement.**

### Thesis 3

> **DBM-SI can therefore be reinterpreted as one practical provider of Structural RSI infrastructure.**

### Thesis 4

> **This does not make DBM-SI the exclusive SRSI architecture; rather, it demonstrates how existing structural computation can be composed into recursive improvement systems.**

### Thesis 5

> **Structural Intelligence may have a dual role: performing intelligence and governing the improvement of intelligence.**

---

# 38. Central Mapping

The core mapping of this paper is:

```text id="oix30b"
DBM-SI
│
├── Difference        → MDT
├── Comparison        → Two-Way CCC
├── Falsification    → Counter-Evidence
├── Identity          → UTN
├── Behavior          → CallingGraph
├── Change Impact     → CG Delta
├── Long Horizon      → Trajectory
├── Localization      → Per-Node Intelligence
├── Search            → Structural Search
├── Routing           → DNA Dispatch
├── Memory            → Structural Folding
├── Uncertainty       → Leftover
├── Growth            → 3-Cat Learning
└── Governance        → PDS
                         │
                         ↓
               Structural RSI
```

This is the main conceptual contribution of SRSI-003.

---

# 39. Conclusion

Recursive Self-Improvement needs more than a generator.

It needs infrastructure capable of determining what changed, whether the change is genuine improvement, where it applies, what evidence supports it, what counter-evidence challenges it, what downstream structures are affected, and whether the change should be promoted.

The DBM-SI research program already contains many structures that address precisely these computational responsibilities.

Reinterpreted through the SRSI lens:

```text id="fx8gaq"
MDT becomes a Differential Evaluator.

Two-Way CCC becomes a Comparative Evaluator.

Counter-Evidence becomes a Falsification Evaluator.

UTN becomes an Identity Evaluator.

CallingGraph becomes a Behavioral-Path Evaluator.

CG Delta becomes a Change-Impact Evaluator.

Trajectory Intelligence becomes a Long-Horizon Evaluator.

Per-Node Intelligence becomes Localized RSI.

Structural Folding becomes Improvement Memory.

PDS becomes Improvement Governance.
```

The deeper lesson is broader than DBM-SI.

> **Recursive improvement may require an ecosystem of explicit computational structures for evaluation, localization, falsification, memory, and governance.**

DBM-SI provides one concrete example of how such an ecosystem can be assembled.

This gives Structural Intelligence a new possible role:

> **not only to compute intelligence, but to help intelligence evaluate and improve itself.**

---

## SRSI Principle

> **Structures that make intelligence inspectable can also make improvement inspectable.**

And:

> **The path from AI to RSI may run through explicit structural evaluation.**

---

## Project Navigation

This document is the third paper in the **Structural Recursive Self-Improvement (SRSI)** series.

### Previous

**SRSI-002 — Rich Evaluators: The Missing Infrastructure of RSI**

Introduces the Evaluator Bottleneck, Evaluator Richness, Evaluator Portfolio, Counter-Evaluation, and the Rich Evaluator Plane.

### Next

**SRSI-004 — Two-Way CCC, Counter-Evidence, and Anti-Goodhart RSI**

Focuses on structural A/B comparison, adversarial evaluation, falsification, and the problem of evaluator exploitation under strong recursive optimization.

### SRSI Core Progression

```text id="4m4kjg"
Recursive Self-Improvement
          ↓
Rich Evaluator Requirement
          ↓
DBM-SI Structural Mapping
          ↓
Differential Evaluation
          ↓
Two-Way Comparison
          ↓
Counter-Evidence
          ↓
Localization
          ↓
Structural Memory
          ↓
Improvement Governance
          ↓
Structural RSI Runtime
```
