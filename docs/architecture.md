# Public Product Architecture

Herline connects shows and other content, learning and participation paths, Herline App, and services for organizations. For individuals, content can reveal a skill worth learning and applying; participation should fit each program. For organizations, Herline aims to develop new customer-acquisition entry points and manage acquisition costs, with results established through actual business evidence.

This page maps the **public Herline App product layer** within that broader project. It explains user-facing responsibilities and permission boundaries, not the architecture of every show or organizational engagement. Show-specific submissions, discussions, and practice are a direction; this map does not represent them as released App features.

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

## Current public product-platform map

```text
User goal
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

AI output does not silently become user-approved fact. A successful tool call also does not prove that a real-world outcome occurred. Product documentation, code presence, or a merged change does not by itself prove release, deployment, adoption, or business impact.

## Data and permission boundaries

- Private inputs remain private unless the user takes an explicit sharing action.
- Access is scoped by account, role, purpose, and the current product contract.
- Youth and voice experiences use additional consent and safety controls.
- Invited operator tools do not grant access to learner content by default.
- External publication, commercial use, teaching delivery, and high-impact decisions require human review.

See [Data Handling](data-handling.md) and the live [Privacy Policy](https://herline.vip/legal/privacy).

## Availability and status

The private product system distinguishes released capabilities from work that is validating, limited, internal, experimental, or retired. This public repository only describes a capability as available when current release evidence and the user-facing product support that statement. Platform direction, product strategy, implementation evidence, and commercial results remain separate claims.

Availability can still vary by role, account, region, and rollout. The live product is the final source for what a particular user can access.

See the [Public Documentation Policy](public-documentation-policy.md) for this repository's publication criteria.

---

**See also**: [Glossary](glossary.md) · [FAQ](faq.md) · [Data Handling](data-handling.md) · [Main README](../README.md)
