---
name: jz-abstract-intro
description: Draft or revise English Abstracts and Introductions for ML systems papers with an evidence-first, mechanism-driven argument. Best for quantization, sparse attention, acceleration, and inference papers where local component gains and end-to-end trade-offs must be explicit.
---

# JZ Abstract and Introduction

Use this skill when the paper's argument depends on a measurable systems bottleneck and an explanation of why a natural optimization fails.

## Evidence contract

Before writing, extract: target regime, bottleneck, prior direction, exact gap, failed direct solution, failure mechanism, component-to-challenge mapping, local benefits, end-to-end evidence, cost or guarantee, and evaluated scope. Never invent numbers, baselines, hardware, quality claims, or mechanisms. Mark missing essentials as `[NEED: ...]` or omit them.

## Shared workflow

1. State the regime and bottleneck in concrete computational terms.
2. Credit the strongest relevant prior direction, then narrow the unresolved object or regime.
3. Show a direct-transfer failure before introducing the method.
4. Explain the mechanism behind the failure, preferably as one causal sentence.
5. Map each challenge to one design choice in the same order.
6. Attach local benefit or cost to a component when evidence exists.
7. Close with metric, baseline, setting, cost/guarantee, and bounded scope.

## Abstract

Use the compact chain `bottleneck -> gap/failure -> mechanism or observation -> method -> hard evidence -> cost/guarantee -> scope`. Keep one claim per sentence when numbers are present. Mention kernel/operator gains and end-to-end gains separately when both support the systems claim. End with evidence or a limitation, never with an unquantified adjective.

## Introduction

Build a necessity proof: regime and scaling bottleneck, relevant prior solutions, concrete failure of the strongest direct baseline, mechanism diagnosis, challenge-to-method mapping, local effects, and quantitative closure. Use `C1 -> M1` style mapping when there are multiple challenges. Do not turn the section into a survey or a component inventory.

## JZ-specific moves

- Prefer complexity, latency share, memory, sequence/model scale, or hardware constraints over broad motivation.
- Make the gap object-specific: what remains high precision, unaccelerated, unsupported, or unexplained.
- Use observation -> explanation -> design implication when an analysis drives the method.
- Separate local operator/kernel benefit from end-to-end benefit, and state implementation overhead explicitly.
- Bound every claim by model, task, sequence length, hardware, and inference/training setting supplied by the user.

## Revision gate

Remove repeated motivation, generic academic advice, author commentary, and claims that belong in the phrase bank. Check that the final draft contains a concrete failure, a mechanism, a visible mapping, and at least one supported metric with baseline and setting.

Use `references/phrase-bank.md` for fill-slot syntax. Compose new sentences; do not copy source papers.
