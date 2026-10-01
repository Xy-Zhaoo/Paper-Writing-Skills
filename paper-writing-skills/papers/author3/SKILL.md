---
name: libo-abstract-intro-writing
description: Draft or revise English Abstracts and Introductions for vision, restoration, diffusion, and quantization papers using a scene-to-mechanism argument. Best when real-world degradation, data construction, physical modeling, and component-level restoration evidence are central.
---

# Libo Abstract and Introduction

Use this skill when the paper must connect a real capture or application scene to a new degradation, a data or modeling bottleneck, a restoration design, and practical evidence.

## Evidence contract

Extract task and scene, degradation, prior progress, target gap, observed failure, physical or algorithmic mechanism, data/resource facts, components, evidence, costs, and scope. Do not invent numbers, datasets, hardware, novelty, or guarantees. Mark missing essentials as `[NEED: ...]`.

## Choose the argument path

**Method/efficiency:** task and progress -> practical bottleneck -> candidate solution -> target-setting failure -> a small set of supported challenges -> method -> mapped components -> efficiency/evidence.

**Emerging phenomenon/data-restoration:** real scene -> degradation and consequence -> acquisition mechanism -> contrast with adjacent problems -> dataset/model gap -> data construction or simulation -> restoration method -> mapped components -> evidence and scope.

## Shared workflow

1. Define the scene, task, and consequence in concrete terms.
2. Credit adjacent methods and state the residual target-setting gap.
3. Show the observable failure and its cause.
4. Decompose only genuine barriers into parallel challenges.
5. Introduce the method with the organizing idea, then map components in challenge order.
6. State data, simulation, calibration, or deployment facts only when documented.
7. Close with bounded evidence and non-overlapping contributions.

## Abstract

Use `problem/scene -> gap/failure -> method -> component sequence -> data or practicalization -> evidence -> scope`. Include data construction before the model when data scarcity is a prerequisite bottleneck. Keep each component tied to a diagnosed difficulty.

## Introduction

Escalate across paragraphs: scene and stakes, prior progress and residual gap, target-setting failure, challenge block, method pivot, component mapping, practicalization/evidence, and optional contributions. Use two challenges when there are two; do not create symmetric filler.

## Libo-specific moves

- Make the physical, acquisition, or real-world origin of the degradation explicit when supported.
- Treat data construction, simulation, or calibration as a first-class method contribution when it enables the task.
- Use `component -> operation/mechanism -> immediate effect -> paper-level purpose` mapping.
- Separate restoration quality from realism, data coverage, deployment, and resource claims.
- State boundaries such as artifact type, capture setting, model regime, or benchmark scope.

## Revision gate

Remove author-style commentary, generic motivation, repeated component descriptions, and source-paper wording. Check that the gap is narrower than the problem, each challenge has a consequence, and every contribution bullet adds a distinct supported claim.

Use `references/phrase-bank.md` for fill-slot syntax. Compose new sentences; do not copy source papers.
