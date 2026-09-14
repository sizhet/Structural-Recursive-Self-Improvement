# SRSI-004 — Two-Way CCC, Counter-Evidence, and Anti-Goodhart RSI

## From Winner-Take-All Optimization to Structural Comparison, Falsification, and Contestable Improvement

**Project:** Structural Recursive Self-Improvement (SRSI)
**Repository:** `Structural-Recursive-Self-Improvement`
**Series:** SRSI-004
**Status:** Research Framework / Mechanism Paper

---

## Abstract

Recursive Self-Improvement (RSI) creates a fundamental evaluation problem.

As an AI system becomes increasingly capable of generating and optimizing candidate improvements, it may also become increasingly capable of exploiting weaknesses in the evaluators used to judge those improvements.

A candidate can achieve a higher score without representing a correspondingly better system.

Repeated recursively, this gap can become self-reinforcing.

This paper calls that possibility the **RSI Goodhart Amplifier**.

Structural Recursive Self-Improvement (SRSI) therefore requires more than stronger primary evaluators. It requires computational mechanisms that preserve structural differences, actively search for counter-evidence, expose evaluator disagreement, and prevent premature winner-take-all promotion.

This paper develops two complementary mechanisms from the DBM-SI framework:

1. **Two-Way CCC** as a structural A/B comparison mechanism; and
2. **Counter-Evidence Search** as an explicit falsification mechanism.

Together they support an **Anti-Goodhart RSI** architecture in which candidate improvements are not accepted merely because they optimize a primary score.

Instead, the system asks:

> What changed?

> What became better?

> What became worse?

> Under which contexts?

> What evidence supports the candidate?

> What evidence opposes it?

> Which evaluator may be wrong?

> Should the candidate replace the current structure, become a specialized branch, remain unresolved, or be rejected?

The resulting architecture shifts recursive improvement from:

> **optimize → score → replace**

toward:

> **compare → differentiate → challenge → verify → branch or promote**

The deeper principle is:

> **The stronger the optimizer becomes, the more important it becomes to preserve disagreement and search for reasons why its apparent improvement may be false.**

---

# 1. The Core Problem: Optimizers Learn Their Evaluators

Suppose an RSI system repeatedly performs:

```text id="s1kjup"
Generate Candidate
       ↓
Evaluate Candidate
       ↓
Select Higher Score
       ↓
Promote
       ↓
Generate Again
```

Initially, this may work well.

But recursive optimization changes the relationship between generator and evaluator.

The generator does not remain static.

It learns.

Over repeated cycles:

```text id="bx3vkm"
Generator
   ↓
observes evaluation pressure
   ↓
discovers what receives high scores
   ↓
generates increasingly evaluator-optimized candidates
```

This is not inherently a failure.

It is exactly what optimization is supposed to do.

The problem appears when:

```text id="0ev4ac"
Evaluator Objective
       ≠
True Intended Objective
```

Even a small gap can become important under strong optimization pressure.

---

# 2. The RSI Goodhart Amplifier

A conventional Goodhart-like failure can be represented as:

```text id="k33gd6"
Intended Objective
       ↓
Proxy Metric
       ↓
Optimization
       ↓
Proxy improves
       ↓
Reality may not
```

RSI adds recursion:

```text id="65tpyy"
Weakness in Evaluator
        ↓
Candidate exploits weakness
        ↓
Candidate receives high score
        ↓
Candidate is promoted
        ↓
Improved optimizer
        ↓
Finds evaluator weakness more effectively
        ↓
Further promotion
        ↓
...
```

We call this:

# **The RSI Goodhart Amplifier**

The critical feature is recursion.

The system may not merely exploit a weak evaluator once.

It may promote systems that become progressively better at exploiting the evaluator.

Thus:

> **A small evaluator error can become a recursively amplified optimization direction.**

This makes evaluator robustness a first-class RSI problem.

---

# 3. Score Improvement Is Not Structural Improvement

Suppose:

```text id="26hf99"
Score(A) = 0.82

Score(B) = 0.89
```

A winner-take-all system concludes:

```text id="q04dsp"
B > A
```

But this statement hides many possibilities.

Perhaps:

```text id="9wz2nj"
B improves benchmark performance.

B degrades rare-case safety.

B uses 4× more compute.

B works only under Context C1.

B breaks compatibility under C2.

B introduces a long-horizon instability.

B learned to exploit the benchmark.
```

Therefore:

> **A higher evaluation score is evidence about improvement, not the complete structure of improvement.**

SRSI requires preservation of the differential structure between `A` and `B`.

---

# 4. From Winner-Take-All to Structural A/B

Traditional optimization often uses:

```text id="4ds5zv"
A vs. B
   ↓
Score
   ↓
Winner
```

Two-Way CCC proposes a different representation:

```text id="8n82md"
          A
          │
          ↕
     Two-Way CCC
          ↕
          │
          B
```

Instead of asking only:

> Which one wins?

the system asks:

```text id="yk0tah"
What do A and B share?

What exists in A but not B?

What exists in B but not A?

Under which context is A stronger?

Under which context is B stronger?

Which difference caused improvement?

Which difference caused regression?

Should both structures survive?
```

This transforms evaluation from ranking into differentiation.

---

# 5. Two-Way CCC as a Comparative Evaluator

Let:

```text id="cctibq"
A = Current System

B = Candidate Improvement
```

A Two-Way CCC comparison can conceptually produce:

```text id="rzld6q"
Shared(A, B)

A-only

B-only

A-better contexts

B-better contexts

Unresolved differences
```

This creates a richer improvement representation:

```text id="l77kpu"
A
│
├── Shared Structure ───── B
│
├── A-Specific Strength
│
└── A-Specific Weakness

B
│
├── B-Specific Strength
│
└── B-Specific Weakness
```

The result does not require immediate global replacement.

---

# 6. Five Possible Outcomes of Structural A/B

A structural comparison can produce at least five major outcomes.

## 6.1 Promote

```text id="k3tj5z"
A → B
```

Evidence strongly supports B across relevant contexts.

---

## 6.2 Reject

```text id="d9cwxp"
A remains
B rejected
```

The candidate fails evaluation.

---

## 6.3 Branch

```text id="kkgx7h"
       Root
      /    \
     A      B
    C2      C1
```

Both structures are useful under different contexts.

---

## 6.4 Localize

```text id="tz53lg"
System A
   │
   └── Node N
          ↓
         N'
```

Only a local part of B is adopted.

---

## 6.5 Leftover

```text id="iwnf62"
A remains active

B → LEFTOVER
```

Evidence is insufficient.

B is preserved for later re-evaluation.

These outcomes make improvement structurally richer than:

```text id="f1m1pc"
WIN / LOSE
```

---

# 7. Why Branching Matters for Anti-Goodhart RSI

Goodhart pressure is intensified by forced optimization toward a single winner.

If every evaluation must produce:

```text id="j5p38n"
Best Candidate
```

then the system continually compresses uncertainty and disagreement into one selected state.

Branching allows:

```text id="ll94ob"
Candidate A works under C1.

Candidate B works under C2.

Candidate C remains uncertain.
```

Instead of forcing:

```text id="8k35ba"
B is globally best.
```

the system can preserve:

```text id="u8ac4h"
C1 → A

C2 → B

C3 → unresolved
```

This reduces pressure to overgeneralize local evaluation results.

Thus:

> **Structural branching can act as an anti-Goodhart mechanism by preventing context-bound improvements from being falsely promoted as universal improvements.**

---

# 8. Counter-Evidence as the Second Half of Evaluation

Two-Way CCC preserves differences.

But another mechanism is needed.

Suppose B looks better.

The system should not ask only:

> What evidence confirms B?

It should also ask:

> **What evidence would invalidate B as an improvement?**

This is the role of:

# **Counter-Evidence Search**

The evaluation loop becomes:

```text id="97f7o3"
Candidate B
     ↓
Supporting Evidence
     ↕
Counter-Evidence
     ↓
Structural Judgment
```

This is fundamentally different from passive error detection.

Counter-Evidence Search is active.

---

# 9. Active Falsification

A conventional evaluator may run predefined tests.

Counter-Evidence Search goes further:

```text id="zqvfoq"
Given Candidate B:

Search for contexts where B fails.

Search for cases where A remains superior.

Search for historical counterexamples.

Search for structural incompatibilities.

Search for trajectory regressions.

Search for policy violations.

Search for evaluator blind spots.
```

The system is deliberately trying to defeat its own improvement claim.

This creates:

> **Active Falsification**

rather than passive validation.

---

# 10. Improvement Search and Counter-Evidence Search

A mature SRSI loop should therefore contain two opposing search processes:

```text id="ev27b5"
        Candidate B
            │
    ┌───────┴───────┐
    ↓               ↓
Improvement      Counter-Evidence
Search              Search
    ↓               ↓
Evidence         Opposition
    └───────┬───────┘
            ↓
      Structural Judgment
```

The first asks:

> How is B better?

The second asks:

> Where is B not better?

The tension between them is productive.

---

# 11. Scientific-Method-Like RSI

This creates an analogy with scientific reasoning.

A candidate improvement resembles a hypothesis:

> B is better than A.

Then:

```text id="c3y5ry"
Hypothesis
    ↓
Supporting Evidence
    ↓
Attempted Falsification
    ↓
Counter-Evidence
    ↓
Replication
    ↓
Context Variation
    ↓
Judgment
```

Therefore SRSI can move toward:

# **Scientific Recursive Self-Improvement**

The system does not merely optimize.

It proposes, challenges, tests, and revises improvement hypotheses.

---

# 12. The Candidate Improvement Engine

We can separate the RSI process into two engines.

The first is:

# **Candidate Improvement Engine**

```text id="p17e4h"
Problem / Opportunity
       ↓
Candidate Generation
       ↓
Search
       ↓
Optimization
       ↓
Candidate B
```

Its job is to produce better possibilities.

Modern AI and large-scale compute may make this engine extremely powerful.

But it should not govern itself alone.

---

# 13. The Candidate Falsification Engine

The second is:

# **Candidate Falsification Engine**

```text id="jsqjmr"
Candidate B
    ↓
Search for Failure
    ↓
Search for Regression
    ↓
Search for Counterexample
    ↓
Search for Context Conflict
    ↓
Search for Evaluator Exploitation
```

Its job is not to maximize candidate quality.

Its job is to attack the claim that the candidate is an improvement.

Together:

```text id="zdh8mz"
Candidate Improvement Engine
             ↕
Candidate Falsification Engine
             ↓
     Structural Judgment
```

This dual-engine architecture is one of the core mechanisms of Anti-Goodhart SRSI.

---

# 14. Primary Evaluator vs. Counter-Evaluator

A practical implementation may contain:

```text id="xllk1q"
Primary Evaluator
        ↕
Counter-Evaluator
```

For example:

```text id="uqg44c"
Primary:
Performance improved by 14%.

Counter:
Performance collapses under Context C7.
```

Or:

```text id="w7abjs"
Primary:
All benchmark tests pass.

Counter:
CallingGraph reveals a new unverified execution path.
```

Or:

```text id="qnpzhp"
Primary:
Market strategy improves historical return.

Counter:
Improvement disappears under high transaction cost.
```

The disagreement is valuable.

It identifies the structural boundary of the improvement.

---

# 15. Counter-Evidence Should Be Preserved

A common mistake is to treat counter-evidence as noise after a candidate is accepted.

SRSI should preserve it.

For example:

```text id="5fl1zs"
Candidate B

Evidence:
E1
E2
E3

Counter-Evidence:
CE1
CE2

Decision:
Local promotion only
```

Later, runtime evidence may show:

```text id="u49h58"
CE2 was predictive.
```

This information should improve future evaluation.

Thus Counter-Evidence becomes part of Structural Memory.

---

# 16. Counter-Evidence as Future Intelligence

Today's rejected evidence may become tomorrow's important branch.

Suppose:

```text id="s1ol81"
B wins 95% of contexts.

A wins 5%.
```

A naive optimizer may discard A.

But those 5% may represent:

* rare emergencies,
* new regimes,
* security edge cases,
* high-value exceptions,
* future environmental change.

Therefore:

> **Counter-evidence is not merely opposition to current optimization; it can be preserved future intelligence.**

This is especially important in non-stationary systems.

---

# 17. Anti-Goodhart Requires Multiple Perspectives

One primary evaluator and one counter-evaluator may still share the same blind spots.

Therefore:

```text id="rf5thf"
Primary Evaluator
Counter-Evaluator
```

should sometimes expand into:

```text id="7hzw9k"
Performance Evaluator

Structural Evaluator

Trajectory Evaluator

Counter-Evidence Evaluator

Adversarial Evaluator

Policy Evaluator

Runtime Evaluator
```

Each observes a different aspect of the candidate.

This creates:

> **Cross-Perspective Evaluation**

---

# 18. Evaluator Disagreement Should Not Be Collapsed Too Early

Suppose:

```text id="0s2wmy"
Performance: PASS

Structural Consistency: PASS

Trajectory Stability: UNCERTAIN

Counter-Evidence: FAIL

Policy: PASS
```

Immediately converting this to:

```text id="phtsnv"
Final Score = 0.78
```

destroys information.

Instead, SRSI may preserve:

```text id="m56zqv"
PASS
PASS
UNCERTAIN
FAIL
PASS
```

and reason about the disagreement.

Possible response:

```text id="9izcrp"
Do not globally promote.

Search the failing context.

Run additional trajectory evaluation.

Preserve candidate as experimental.
```

This is:

> **Contestable Improvement**

An improvement claim remains open to structured challenge.

---

# 19. Evaluator-of-Evaluators

Anti-Goodhart RSI eventually reaches another question:

> What if the evaluator itself is wrong?

Then:

```text id="fh4l1a"
Candidate
    ↓
Evaluator E
    ↓
Judgment
```

must become:

```text id="mv8zcc"
Candidate
    ↓
Evaluator E
    ↓
Judgment
    ↓
Runtime Evidence
    ↓
Evaluate E
```

An evaluator can be judged by:

```text id="h8spqz"
Calibration

Predictive validity

False promotion rate

False rejection rate

Counter-evidence miss rate

Context coverage

Adversarial robustness

Runtime outcome accuracy
```

This creates:

# **Evaluator-of-Evaluators**

---

# 20. Evaluators Should Also Branch

Suppose Evaluator E works well in one context but poorly in another.

The response need not be:

```text id="qwt58w"
Delete E
```

It may be:

```text id="z9ch6x"
        Evaluator Root
          /       \
        E1         E2
       C1          C2
```

Thus the same structural branching principle can apply to evaluators themselves.

This creates:

> **Recursive Structural Evaluator Growth**

The evaluator infrastructure evolves alongside the target system.

---

# 21. Anti-Goodhart Is Not Anti-Optimization

An important clarification:

SRSI is not arguing against optimization.

Optimization is essential.

Without strong search:

```text id="fsy5aq"
many valuable improvements remain undiscovered.
```

The argument is:

> **Optimization should operate inside a sufficiently rich evaluation structure.**

Thus:

```text id="3skd0x"
Optimization
+
Counter-Evidence
+
Structural Comparison
+
Verification
+
Governance
```

is stronger than:

```text id="b5w36s"
Optimization alone.
```

Anti-Goodhart RSI is therefore not anti-scale.

It is an attempt to make scale directionally meaningful.

---

# 22. Two-Way CCC as an Anti-Compression Mechanism

There is another way to understand Two-Way CCC.

Winner-take-all optimization compresses:

```text id="hdufdo"
A
B
Differences
Contexts
Trade-offs
Uncertainty
```

into:

```text id="tif9ha"
B wins.
```

Two-Way CCC resists this premature compression.

It preserves:

```text id="ghrkhd"
Shared

A-specific

B-specific

Context-specific

Unresolved
```

Therefore Two-Way CCC acts as an:

> **Anti-Compression Mechanism for Improvement Evidence**

This is important because Goodhart-like failures often benefit from excessive compression of complex objectives into narrow proxies.

---

# 23. Leftover as an Anti-Goodhart State

Leftover also has an important role.

Suppose the evidence is contradictory:

```text id="jqz6pk"
Performance: strong

Counter-Evidence: significant

Trajectory: unknown

Policy: acceptable
```

A forced decision may promote B.

SRSI can instead choose:

```text id="6qk9xu"
LEFTOVER
```

meaning:

> We do not yet know enough.

This prevents uncertainty from being converted into false confidence.

Thus:

> **Explicit Leftover is an anti-Goodhart mechanism because it allows the system not to optimize through unresolved evidence.**

---

# 24. Local Promotion Instead of Global Promotion

Suppose:

```text id="55npga"
B > A under C1

A > B under C2
```

Global promotion is inappropriate.

Instead:

```text id="5z47y0"
C1 → B

C2 → A
```

This is:

# **Context-Bound Promotion**

Context-bound promotion reduces overgeneralization.

It also creates a direct connection between:

```text id="njbnuy"
Evaluation
↓
Localization
↓
Dispatch
```

This is one of the main advantages of Structural RSI.

---

# 25. Per-Node Anti-Goodhart Evaluation

The same principle applies inside large systems.

Suppose Candidate B improves Node N3.

Instead of:

```text id="ayb1da"
Replace System A with System B
```

we can perform:

```text id="n9y5am"
Locate N3
   ↓
Compare N3 vs. N3'
   ↓
Counter-Evidence
   ↓
Verify local dependencies
   ↓
Promote N3'
```

This reduces the scope over which an evaluator must be trusted.

A local evaluator can be narrower, more explicit, and easier to falsify.

Thus:

> **Localization can reduce the surface area of evaluator error.**

---

# 26. CallingGraph Delta as Counter-Evidence

AI coding provides a concrete example.

Suppose a candidate passes every existing unit test.

Primary evaluator:

```text id="azcrbk"
PASS
```

But CallingGraph Delta reveals:

```text id="pqh2k7"
new path:

Authentication
    ↓
Helper
    ↓
Unverified External Call
```

That structural delta is counter-evidence.

The candidate may still be useful.

But global promotion should stop until the new path is evaluated.

Thus structural differences can generate counter-evidence even when output metrics look good.

---

# 27. Trajectory Counter-Evidence

Similarly:

```text id="8xip4d"
Immediate Outcome:
better
```

does not imply:

```text id="sl1xrz"
Long-Horizon Outcome:
better
```

A trajectory evaluator may find:

```text id="7x24tf"
t0: improvement
t1: improvement
t2: instability
t3: failure
```

The later states become counter-evidence against immediate promotion.

This is especially important for:

* agents,
* markets,
* continual learning,
* policy systems,
* recursive evaluators themselves.

---

# 28. Counter-Evidence and Structural Folding

Counter-evidence should not disappear after evaluation.

The full record can be folded:

```text id="ldfv3m"
Candidate B

Context

Primary Evidence

Counter-Evidence

Structural Difference

Decision

Runtime Outcome
```

Later:

```text id="hx2llb"
New Candidate C
       ↓
Structural Search
       ↓
Similar to B
       ↓
Retrieve prior Counter-Evidence
```

Thus the system becomes harder to fool repeatedly in the same way.

This is:

> **Anti-Goodhart Memory**

---

# 29. Recursive Counter-Evidence

As the system improves, Counter-Evidence Search can improve too.

A first-generation system may search:

```text id="2gk7w0"
known failure cases.
```

A stronger system may generate:

```text id="p7cd9q"
novel adversarial contexts.
```

An even stronger system may search for:

```text id="zd13yi"
weaknesses in the evaluator architecture itself.
```

Therefore:

```text id="4gttgm"
Improvement Search improves
        ↕
Counter-Evidence Search improves
```

This co-evolution is desirable.

We do not want only the optimizer to recursively improve.

We also want its challenger to recursively improve.

---

# 30. The Red-Team Analogy

A useful analogy is:

```text id="qf8xwp"
Candidate Generator
        =
Builder

Counter-Evidence Search
        =
Red Team
```

But SRSI makes this relationship structural and continuous.

The red team is not an occasional external audit.

It can exist inside every important improvement cycle.

Thus:

> **Every sufficiently consequential RSI candidate should be capable of facing an improvement red team.**

---

# 31. Improvement Governance After Contest

Evaluation should not itself deploy the candidate.

After structural contest:

```text id="0et83a"
Primary Evidence
        ↕
Counter-Evidence
        ↓
Two-Way Comparison
        ↓
Verification
```

the result enters:

```text id="1ucjs3"
Improvement Governance
```

Possible decisions:

```text id="wybqxu"
PROMOTE

LOCAL-ONLY

BRANCH

EXPERIMENTAL

LEFTOVER

REJECT

ROLLBACK
```

This separation is essential.

A candidate can win a technical comparison without receiving global deployment authority.

---

# 32. Candidate Capability Is Not Deployment Authority

This leads to an important chain:

```text id="msm70a"
Candidate Capability
        ↓
Evaluated Capability
        ↓
Validated Improvement
        ↓
Governed Promotion
        ↓
Authorized Deployment
```

These stages should not be collapsed.

A recursively improving system becomes easier to govern when each transition is explicit.

---

# 33. A Canonical Anti-Goodhart SRSI Loop

The complete loop can now be represented as:

```text id="0qyrhn"
Current Structure A
        │
        ↓
Candidate Generator
        │
        ↓
Candidate Structure B
        │
        ↓
Primary Evaluation
        │
        ↓
Two-Way CCC
     A ↔ B
        │
        ↓
Structural Difference
        │
        ↓
Counter-Evidence Search
        │
        ↓
Cross-Perspective Evaluation
        │
        ↓
Verification
        │
        ↓
┌────────────────────────────┐
│ Promote                    │
│ Reject                     │
│ Branch                     │
│ Localize                   │
│ Experimental               │
│ Leftover                   │
└──────────────┬─────────────┘
               ↓
      Improvement Governance
               ↓
          Deployment
               ↓
       Runtime Evidence
               ↓
       Structural Folding
               ↓
        Next RSI Cycle
```

This is the core architecture proposed in this paper.

---

# 34. Anti-Goodhart as an Architectural Property

Goodhart resistance should not depend only on:

```text id="qxfrhr"
a better reward function.
```

It can also arise from architecture.

For example:

```text id="uvl9ya"
Multiple evaluators

Two-Way structural comparison

Counter-evidence search

Context preservation

Branching

Leftover

Localized promotion

Runtime monitoring

Rollback

Structural memory
```

Together these reduce dependence on any single proxy.

Thus:

> **Anti-Goodhart behavior can be an emergent property of evaluation architecture rather than a property of one perfect evaluator.**

This is a major SRSI proposition.

---

# 35. No Evaluator Should Be Sovereign

This leads to a strong design principle:

> **No single evaluator should automatically possess sovereign promotion authority over high-impact recursive improvement.**

A primary evaluator can recommend.

A counter-evaluator can challenge.

A structural evaluator can localize.

A policy evaluator can constrain.

Runtime evidence can overturn prior confidence.

This creates distributed epistemic control over improvement.

---

# 36. Evaluator Diversity as Structural Defense

If every evaluator shares the same model, benchmark, objective, and data, then nominal plurality provides little protection.

Therefore SRSI should seek evaluator diversity across:

```text id="ntn4jo"
Representation

Data

Method

Perspective

Time Horizon

Objective

Failure Search

Structural Level
```

For example:

```text id="trc07k"
LLM Critic
+
Unit Tests
+
CallingGraph Analysis
+
Runtime Trace
+
Counterexample Generator
+
Policy Engine
```

This is stronger than six copies of the same critic.

---

# 37. Evaluator Competition

In some settings, evaluators may themselves compete.

Suppose:

```text id="fd5ugj"
E1 predicts candidate success.

E2 predicts candidate failure.
```

Runtime evidence later shows:

```text id="03pz7q"
E2 was correct.
```

The system can update evaluator confidence.

Over time:

```text id="18u5b4"
Evaluator Portfolio
        ↓
Runtime Outcomes
        ↓
Evaluator Performance
        ↓
Weight / Branch / Retire
```

Thus evaluator quality becomes empirically grounded.

---

# 38. The Evaluator Must Not Become the New Black Box

There is a danger in solving black-box optimization with black-box evaluation.

If the evaluator itself becomes opaque:

```text id="6k37oh"
Candidate
   ↓
Huge Evaluator Model
   ↓
Trust Me
```

then important SRSI goals are lost.

Not every evaluator must be fully interpretable.

But high-impact evaluation should ideally expose enough structure to answer:

```text id="nqztyf"
What evidence mattered?

What counter-evidence existed?

Which context applied?

What structural difference was decisive?

Which policy authorized promotion?
```

This is why structural evaluators remain important even when powerful learned evaluators are available.

---

# 39. Human Evaluators Remain Part of the Portfolio

Anti-Goodhart SRSI does not require eliminating human evaluation.

Humans can remain useful for:

* high-impact ambiguity,
* policy decisions,
* novel failure modes,
* value conflicts,
* evaluator disagreement,
* governance escalation.

The goal is not:

```text id="p7gq9x"
Machine evaluators replace humans.
```

It is:

```text id="tf3qgm"
Machine-operable evaluation
+
Structural evidence
+
Human governance where appropriate
```

This can make human intervention more targeted and evidence-rich.

---

# 40. From Reward Hacking to Improvement Hacking

The familiar concept of reward hacking can be generalized.

An RSI system may engage in:

# **Improvement Hacking**

That is:

> producing modifications that satisfy the formal improvement process without delivering the intended substantive improvement.

Examples include:

```text id="rtzq5v"
Benchmark gaming

Test overfitting

Metric manipulation

Evaluator spoofing

Counter-evidence avoidance

Context narrowing

Selective reporting

Policy bypass

Structural camouflage
```

Anti-Goodhart SRSI is partly an architecture for resisting Improvement Hacking.

---

# 41. The Improvement Attack Surface

Once evaluation determines recursive promotion, the entire improvement pipeline becomes an attack surface:

```text id="ukxdaz"
Candidate Generation

Evaluator Selection

Evaluator Inputs

Metric Calculation

Counter-Evidence Search

Verification

Promotion Policy

Structural Memory

Runtime Feedback
```

Failures can occur at any layer.

Therefore SRSI security must eventually include:

> **Improvement-Pipeline Security**

This is broader than model security alone.

---

# 42. The Importance of Reversibility

Even rich evaluation cannot predict everything.

Therefore:

```text id="szk7zb"
Validated
```

should not imply:

```text id="d9sg71"
Irreversible.
```

SRSI should favor:

```text id="6s8v39"
Versioned structures

Local deployment

Branch preservation

Rollback

Runtime monitoring
```

especially for high-impact changes.

Reversibility converts some uncertainty from a pre-deployment impossibility into a manageable runtime process.

---

# 43. Anti-Goodhart RSI Is a Moving Target

No evaluator architecture can be assumed permanently sufficient.

As candidate generators improve:

```text id="g0isxs"
new evaluator weaknesses emerge.
```

As environments change:

```text id="p8e46a"
new counter-evidence appears.
```

As systems become more complex:

```text id="uf2rlz"
new structural interactions arise.
```

Therefore Anti-Goodhart RSI must itself be adaptive.

The goal is not:

> solve Goodhart once.

It is:

> **maintain an evolving contest between optimization and evaluation.**

---

# 44. Co-Evolution of Optimizer and Evaluator

This leads to a central SRSI dynamic:

```text id="o5x8wq"
Optimizer improves
      ↓
Evaluator pressure increases
      ↓
Evaluator improves
      ↓
Counter-Evidence improves
      ↓
Optimizer faces stronger judgment
      ↓
Higher-quality improvements survive
      ↓
Optimizer improves again
```

This is:

# **Optimizer–Evaluator Co-Evolution**

A healthy RSI system should recursively improve both sides.

---

# 45. From Optimization Race to Epistemic Arms Race

There is a potentially important consequence.

RSI may not produce only:

```text id="j6fdtm"
a race for better generators.
```

It may also produce:

```text id="tzw47m"
a race for better evaluators.
```

And eventually:

```text id="mh9zx0"
Generator
↕
Evaluator
↕
Counter-Evaluator
↕
Evaluator-of-Evaluators
```

This could become an **epistemic arms race** inside advanced AI engineering.

The desirable outcome is not endless complexity.

It is increasingly reliable improvement judgment.

---

# 46. The Anti-Goodhart Structural Stack

The mechanisms discussed in this paper can be summarized as:

```text id="3p37f2"
┌───────────────────────────────────┐
│      Candidate Generation         │
├───────────────────────────────────┤
│       Primary Evaluation          │
├───────────────────────────────────┤
│      Two-Way CCC Comparison       │
├───────────────────────────────────┤
│      Counter-Evidence Search      │
├───────────────────────────────────┤
│    Cross-Perspective Evaluation   │
├───────────────────────────────────┤
│     Structural Localization       │
├───────────────────────────────────┤
│ Verification / Adversarial Tests  │
├───────────────────────────────────┤
│      Improvement Governance       │
├───────────────────────────────────┤
│      Reversible Deployment        │
├───────────────────────────────────┤
│       Runtime Observation         │
├───────────────────────────────────┤
│ Counter-Evidence / Result Folding │
└───────────────────────────────────┘
                  │
                  └────→ Next Cycle
```

This is an architectural approach to Anti-Goodhart RSI.

---

# 47. Five Anti-Goodhart Principles for SRSI

The discussion can be reduced to five principles.

## Principle 1 — Preserve Difference

> Do not reduce A/B comparison to a score before understanding the structural difference.

## Principle 2 — Search for Opposition

> Every important improvement claim should face active Counter-Evidence Search.

## Principle 3 — Preserve Context

> A local improvement should not automatically become a global improvement.

## Principle 4 — Preserve Uncertainty

> Branch and Leftover are legitimate improvement states.

## Principle 5 — Separate Evaluation from Promotion

> An evaluator may establish evidence of improvement without possessing authority to deploy it.

Together these form a minimal Anti-Goodhart discipline for SRSI.

---

# 48. Open Research Questions

This framework creates several important research problems.

### 48.1 Counter-Evidence Generation

How can a system generate high-value counterexamples rather than merely random failures?

### 48.2 Evaluator Diversity

How much independence between evaluators is necessary to reduce correlated blind spots?

### 48.3 Evaluator Conflict

How should persistent disagreement between strong evaluators be represented and resolved?

### 48.4 Promotion Thresholds

When is evidence strong enough for global, local, experimental, or no deployment?

### 48.5 Evaluator Evolution

How should evaluator structures themselves branch, merge, decay, or retire?

### 48.6 Adversarial Candidate Search

How should an RSI system deliberately search for candidates that fool its own evaluator?

### 48.7 Counter-Evidence Memory

How should historical failures be folded so future candidates cannot repeatedly exploit the same weakness?

### 48.8 Localized Goodhart Effects

Can per-node optimization create global failure even when every local evaluator reports improvement?

These questions are central to a mature SRSI runtime.

---

# 49. Central Thesis

The argument of this paper can be summarized as follows.

### Thesis 1

> **Strong recursive optimization amplifies the consequences of evaluator weakness.**

### Thesis 2

> **A higher score should be treated as evidence of improvement, not as the complete definition of improvement.**

### Thesis 3

> **Two-Way CCC can preserve structural differences that winner-take-all optimization would discard.**

### Thesis 4

> **Counter-Evidence Search can turn evaluation from confirmation into active falsification.**

### Thesis 5

> **Branch, Localize, and Leftover are important alternatives to global replacement.**

### Thesis 6

> **Anti-Goodhart behavior can arise from a rich evaluation architecture rather than from one supposedly perfect evaluator.**

### Thesis 7

> **Recursive improvement should include recursive improvement of the evaluator and counter-evaluator infrastructure itself.**

---

# 50. Conclusion

Recursive Self-Improvement creates a paradox.

The better an AI becomes at optimization, the less safe it is to assume that a simple evaluator will continue to represent the intended objective.

The optimizer learns.

The evaluator is therefore under increasing pressure.

A mature RSI architecture must respond by making evaluation richer, more contestable, more structural, and more adaptive.

Two-Way CCC provides one mechanism for preserving the structural difference between the current system and its candidate successor.

Counter-Evidence Search provides another mechanism for actively challenging the claim that the candidate is better.

Together they change the improvement process from:

```text id="rdxj9c"
Generate
   ↓
Score
   ↓
Winner
   ↓
Replace
```

into:

```text id="2sg6fd"
Generate
   ↓
Compare
   ↓
Differentiate
   ↓
Search Evidence
   ↕
Search Counter-Evidence
   ↓
Localize
   ↓
Verify
   ↓
Promote / Reject / Branch / Leftover
   ↓
Govern
   ↓
Observe
   ↓
Fold
```

This is a more demanding improvement process.

But stronger RSI makes that additional structure more—not less—important.

The central Anti-Goodhart principle of SRSI is therefore:

> **The stronger the optimizer becomes, the stronger its challenger must become.**

And the deeper architectural principle is:

> **Do not ask only whether the candidate wins. Preserve enough structure to understand where it wins, where it loses, why it wins, why it may be wrong, and whether it deserves to become part of the next system.**

That is the role of Two-Way CCC, Counter-Evidence, and Anti-Goodhart Structural RSI.

---

## SRSI Principle

> **Every powerful improvement engine needs a powerful falsification engine.**

And:

> **Recursive Self-Improvement should recursively improve not only the optimizer, but also the machinery capable of proving the optimizer wrong.**

---

## Project Navigation

This document is the fourth paper in the **Structural Recursive Self-Improvement (SRSI)** series.

### Previous

**SRSI-003 — DBM-SI as a Rich Evaluator and Improvement Infrastructure**

Maps DBM-SI structures onto the Rich Evaluator, localization, memory, and governance requirements of SRSI.

### Next

**SRSI-005 — Localized RSI, Structural Growth, and Improvement Governance**

Develops the transition from whole-system recursive replacement toward per-node improvement, structural branching, reversible growth, and governed promotion.

### SRSI Core Progression

```text id="a9ys0u"
Recursive Optimization
        ↓
Evaluator Pressure
        ↓
RSI Goodhart Amplifier
        ↓
Two-Way CCC
        ↓
Structural Difference
        ↓
Counter-Evidence Search
        ↓
Cross-Perspective Evaluation
        ↓
Promote / Reject / Branch / Leftover
        ↓
Improvement Governance
        ↓
Anti-Goodhart Structural RSI
```
