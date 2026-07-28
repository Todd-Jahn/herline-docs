# Public Documentation Policy

This repository is Herline’s public documentation surface. Its job is to give users, partners, researchers, and contributors enough accurate information to understand the product without publishing the private codebase or internal operating context.

## Source hierarchy

Maintainers update public claims in this order:

1. current user-facing product and legal pages;
2. current product strategy approved for external use;
3. released-capability and runtime evidence;
4. public examples reviewed for their stated purpose.

Code presence, a merged branch, a feature flag, a design document, or an internal test does not by itself prove public availability.

## Allowed public content

- approved product positioning and audience descriptions;
- user-facing surfaces, Agent names, and workflow responsibility boundaries;
- capabilities supported by current release evidence and public product behavior;
- general trust, privacy, safety, and human-review principles already reflected in live policy;
- public examples clearly labelled as illustrative rather than guaranteed benchmarks;
- contact, contribution, and security-reporting paths.

## Content that must stay private

- source code and private repository paths;
- provider identities or routing when disclosure is not already an approved public fact;
- prompts, internal evaluations, thresholds, hidden policies, and unpublished benchmarks;
- infrastructure topology, credentials, environment variables, internal endpoints, and runbooks;
- customer or participant data, account lists, private program assets, and support records;
- internal economics, fundraising analysis, partner terms, negotiation positions, and sales pipelines;
- unreleased roadmaps, experiments, shadow systems, scaffolds, and validation-stage work presented as available;
- implementation success presented as deployment, customer adoption, or production proof.

## Status language

- **Live / released**: supported by current user-facing behavior and release evidence.
- **Limited / role-scoped**: released for a defined audience, account class, or program.
- **Under evaluation**: may be discussed only when an external explanation is useful; it must not be presented as available or promised.
- **Internal / experimental / retired**: omitted from public product claims unless a public correction or safety notice requires mention.

Dates, prices, quotas, performance numbers, model/provider names, and availability change faster than documentation. Prefer linking to the live product instead of copying them.

## Review checklist

Before publishing a change, confirm:

1. Who is the external reader and what do they need to act?
2. Is each availability claim backed by current public or release evidence?
3. Does the change expose security-sensitive, commercial, personal, or operational information?
4. Does it distinguish product direction, implementation, release, and real-world outcome?
5. Do English and Chinese entry points describe the same product and boundaries?
6. Are links valid and Markdown checks green?

When evidence is incomplete, narrow or omit the claim. Public documentation should never be used to make an internal capability appear released.
