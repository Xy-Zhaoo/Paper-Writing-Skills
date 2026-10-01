---
name: kl-abstract-intro
description: Draft or revise English Abstracts and Introductions for practical ML papers by connecting deployment pressure to a hard-regime failure, an overlooked factor, a derived design, and a deployment contract. Best for quantization, caching, lightweight models, generative inference, and capability benchmarks.
---

# KL Abstract and Introduction

Use this skill when the central story is that an attractive practical direction breaks under a demanding regime because an overlooked variable or mismatch is not controlled.

## Evidence contract

Extract the practical pressure, attractive prior direction, hard regime, observable failure, overlooked factor, causal mechanism, method principle, component roles, deployment cost, quantitative evidence, and scope. Never invent metrics, comparisons, hardware, novelty, or guarantees. Use `[NEED: ...]` for missing facts.

## Shared workflow

1. Open with capability or deployment pressure.
2. Explain why the chosen prior direction is attractive.
3. Pin the failure to a hard regime rather than criticizing the field globally.
4. Name the overlooked factor or representation/supervision mismatch.
5. Derive the method from that observation.
6. Present only components with distinct causal roles.
7. State what the method avoids or preserves, then close with measured quality, efficiency, and scope.

## Abstract

Use `capability -> deployment cost -> promising direction -> hard-regime failure -> overlooked factor -> method -> practical guarantee -> quantitative closure`. For quantization, expose the distribution or grouping mismatch; for acceleration, expose error accumulation or schedule mismatch; for reasoning/benchmark work, expose the supervision or grounding defect. End with a deployment-relevant metric and a verified cost statement.

## Introduction

Create an expectation that the natural solution should work, then break it with evidence. Explain the hidden factor briefly, and make the proposed design a direct response. Use a minimal component chain such as `detect/estimate -> transform -> compensate` or `ground -> relate -> reason` only when supported by the method.

## KL-specific moves

- Keep the practical contract visible: no retraining, no architecture change, no extra model evaluations, offline absorption, or bounded overhead only when verified.
- Treat an overlooked factor as the story's organizing variable, not as a decorative observation.
- Distinguish coupled error sources or stages that prior methods collapse into one approximation path.
- Compare hard-regime quality and deployment cost together; do not end with a naked superiority claim.
- Preserve the paper's target capability while stating the exact evaluated regime.

## Revision gate

Delete generic background, repeated transition prose, survey-only language, and unsupported superlatives. Confirm that a reader can answer what breaks, why it breaks, what the hidden factor is, how the design controls it, and what deployment cost remains.

Use `references/phrase-bank.md` for fill-slot syntax. Compose new sentences; do not copy source papers.
