# Public Product Architecture

This document explains how Herline’s public product concepts fit together. It intentionally does not reproduce the private codebase, service topology, deployment design, provider routing, schemas, prompts, credentials, feature flags, or operational runbooks.

## Responsibility model

| Type | Meaning | Examples |
| --- | --- | --- |
| Surface | A user-facing place where work happens | Atlas, Library, Studio, Courses, Prep, Assistant, Boost, Hypatia |
| Agent | A named conversational role with a bounded responsibility | Helena, Holly, Hera, Harmon, Hylia, Hypatia |
| Workflow | A long-running, stateful production process | D2B deep reading, B2C course generation, research |
| Service domain | Supporting product capability | Assessment, sharing, membership, support |
| Artifact | A versioned output a user can inspect or reuse | Knowledge block, course brief, report version, presentation |
| Policy | Rules governing access, approval, safety, billing, and retention | Role access, guardian consent, sharing scope |

A surface is not automatically an Agent, and an Agent is not automatically a workflow. This distinction keeps responsibility and user expectations clear.

## Current public product map

```text
Profile / intent
      │
      ├─ Atlas + Helena ─────────────── reading and source planning
      │          │
      │          ▼
      ├─ Library + D2B ──────────────── deep reading and reusable knowledge
      │          │
      │          ├─ Studio + Holly ──── course brief and learning design
      │          │          │
      │          │          ▼
      │          ├─ Courses + B2C ───── lessons, scripts, audio, assessment
      │          │
      │          └─ Prep + Hera ─────── keynote and teaching deliverables
      │
      ├─ Assistant + Harmon ─────────── voice rehearsal and revision
      ├─ Hypatia ────────────────────── evidence-based research workspace
      └─ Boost + Hylia ──────────────── role-scoped distribution

All paths produce inspectable artifacts and remain subject to account,
role, purpose, region, and product-availability checks.
```

## Information flow

1. The user supplies a goal, source material, or practice scenario.
2. Herline selects only the context allowed for that account and task.
3. An Agent or workflow produces a draft, structured artifact, or recommendation.
4. The user reviews, corrects, accepts, or rejects it.
5. Approved work can be exported, shared, rehearsed, or used as input to another product surface.
6. Failures, interruptions, and new versions remain distinguishable from completed work.

AI output does not silently become user-approved fact. A successful tool call also does not prove that a real-world outcome occurred.

## Data and permission boundaries

- Private inputs remain private unless the user takes an explicit sharing action.
- Access is scoped by account, role, purpose, and the current product contract.
- Youth and voice experiences use additional consent and safety controls.
- Invited operator tools do not grant access to learner content by default.
- External publication, commercial use, teaching delivery, and high-impact decisions require human review.

See [Data Handling](data-handling.md) and the live [Privacy Policy](https://herline.vip/legal/privacy).

## Availability and status

The private product system distinguishes released capabilities from work that is validating, limited, internal, experimental, or retired. This public repository only describes a capability as available when current release evidence and the user-facing product support that statement.

Availability can still vary by role, account, region, and rollout. The live product is the final source for what a particular user can access.

## What stays private

- application source code and private repository paths;
- model/provider routing and fallback topology;
- prompts, evaluation sets, internal quality thresholds, and unpublished benchmarks;
- database schemas, infrastructure addresses, credentials, environment variables, and security controls that would increase attack surface;
- customer data, account allowlists, private program assets, and support records;
- internal economics, fundraising material, partner negotiations, and unpublished roadmaps;
- code-complete or validation-pending work presented as released.

See the [Public Documentation Policy](public-documentation-policy.md) for the maintenance contract.

---

**See also**: [Glossary](glossary.md) · [FAQ](faq.md) · [Data Handling](data-handling.md) · [Main README](../README.md)
