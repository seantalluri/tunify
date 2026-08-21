# Tunify

**A public, single-file agentic AI prototype for turning a singer's melody into a reviewable arrangement recommendation—with explicit human approval, uncertainty handling, evaluations, and rights safeguards.**

> **Public source · GitHub Pages demo · synthetic data only**

Tunify is intentionally small enough to inspect end-to-end. The prototype demonstrates the shape of an agentic product rather than hiding the important behavior behind a polished mockup.

## What It Demonstrates

A complete human-governed loop:

```text
INPUT
  melody / request
      ↓
CONTEXT
  musical data + policies + rights
      ↓
DECISION
  recommendation + confidence + reasons
      ↓
OUTPUT
  proposed arrangement direction
      ↓
HUMAN REVIEW
  Approve · Edit · Escalate
```

Nothing consequential is treated as final until a human reviews it.

## Trust & Safety Behavior

The prototype makes boundaries visible in the product experience rather than leaving them as prompt text.

Examples include:

- unusable or corrupted input stops the workflow instead of producing a confident guess;
- low-confidence key or tempo detection is surfaced as uncertainty;
- harmony conflicts stop after a bounded number of automatic correction attempts;
- unauthorized third-party voice cloning is refused;
- direct imitation of a named living artist is refused in favor of non-identifying musical attributes;
- human approval is required before an arrangement is considered complete;
- metered generation can require explicit cost approval.

## Evaluation Cases

The project includes synthetic eval cases covering:

1. a clear happy path;
2. low-confidence but recoverable audio;
3. unusable audio;
4. unresolved harmony after bounded correction attempts;
5. an unauthorized voice-cloning request.

The goal is not a perfect scoreboard. The goal is **observable expected behavior, honest verdicts, and a system that knows when to stop.**

## Why It Is Public

Most of my larger production applications are intentionally private. Tunify provides a compact public example where the complete artifact, policies, synthetic test data, evaluation cases, and front-end behavior can be inspected directly.

## Implementation

- static HTML/CSS/JavaScript
- no framework required to run the prototype
- synthetic CSV context and policy files
- browser-based interface
- deployable as a static GitHub Pages site
- multiple visual skins, including accessible/high-contrast behavior

## Portfolio Context

Tunify is a prototype—not a production SaaS platform. Its role in this portfolio is different from pm.gold, Ezra, Koinonia, and Christ Everywhere:

**it is the public proof-of-code artifact.**

It demonstrates that the same principles used in the larger private systems—human control, explicit policies, visible context, refusal behavior, evaluation, and bounded autonomy—can be represented in a small implementation that anyone can inspect.