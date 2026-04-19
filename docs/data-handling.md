# Data Handling

A plain-language overview of how Herline handles your data. This is not a legal document — the full privacy policy lives at [herline.vip/privacy](https://herline.vip/privacy).

## Core Principles

### 1. Your Knowledge Graph Belongs to You

Every Claim, Concept, and Method extracted from your deep-reads belongs to you. Every course you generate, every keynote you produce — all yours. We store them on your behalf to power the product; we never repackage, resell, or use them without your instruction.

### 2. We Don't Train On Your Private Data

Your private knowledge graph, course drafts, and deep-read results **are not used to train machine learning models** — ours or anyone else's. The compounding intelligence in your personal graph only makes Herline smarter **for you specifically**, not for the platform at large.

### 3. Export Is Always Available

You can export your knowledge graph at any time, in formats that don't require Herline to consume (Markdown, JSON, structured text). Your ability to leave is a first-class product feature, not an afterthought.

### 4. Portability Over Lock-In

Our moat is the depth and fit of your personal graph, not the difficulty of leaving. Generated deliverables (keynotes, decks, courses) are yours to use commercially without royalty. Source material attribution follows standard copyright conventions.

## What Data We Process

### You provide
- **Account info**: email, password (hashed), payment info (processed by external PCI-compliant providers — we don't see card numbers)
- **Profile data**: Assessment results, stated domains, preferences
- **Source material**: books, articles, transcripts you upload or link to
- **Generated artifacts**: courses, keynotes, decks you create

### We derive
- **Knowledge blocks**: Claims/Concepts/Methods extracted from your sources
- **Embeddings**: vector representations enabling cross-book RAG
- **Usage telemetry**: aggregated patterns for product improvement (anonymized)

### We don't collect
- Your browsing activity outside Herline
- Social graph data from third parties
- Device fingerprinting beyond what's needed for fraud prevention

## Where Data Lives

### Data Residency
- **Users in mainland China**: data stored in mainland-China cloud infrastructure, compliant with local regulations
- **International users**: data stored in international cloud infrastructure
- **Cross-border transfers**: only occur when legally permitted and necessary for service delivery (e.g., TTS providers that operate internationally)

### Storage Providers
We use established cloud providers with enterprise-grade security certifications. Specific provider names and certifications are available on request and listed in our full privacy policy.

## What We Share

### With service providers
Limited, purpose-scoped data sharing with:
- Payment processors (transaction data only)
- Email providers (for account notifications)
- TTS synthesis providers (course narration text, results)
- Analytics providers (anonymized usage data)

### With law enforcement
Only when legally compelled, and we notify users where legally permitted.

### Never
- To advertisers
- To data brokers
- To train third-party AI models
- For any purpose not essential to service delivery

## Security

- **Encryption in transit**: TLS 1.3 everywhere
- **Encryption at rest**: all user data encrypted at the storage layer
- **Access controls**: Herline staff access to user data is minimized, logged, and audited
- **Incident response**: see [SECURITY.md](../SECURITY.md) for vulnerability reporting

## Retention & Deletion

### While active
Data retained as long as your account is active, to power the product.

### After cancellation
- **30-day grace period**: full export access retained
- **After 30 days**: account data deleted except where retention is required by law (financial records, etc.)
- **Aggregated/anonymized telemetry**: may persist for product analytics but is not tied to your identity

### Deletion on request
You can request complete deletion at any time via `privacy@herline.vip`. We honor deletion requests promptly, subject to legal retention requirements.

## Your Rights

Depending on your jurisdiction, you may have rights to:
- Access your personal data
- Correct inaccurate data
- Delete your data
- Export your data in portable format
- Object to certain processing
- Withdraw consent

Herline honors these rights globally, not only where locally required. Submit requests to `privacy@herline.vip`.

## Enterprise / Institutional Compliance

For institutional partners and enterprise customers, we offer:
- **Data Processing Agreements** (DPAs)
- **Audit logs** with configurable retention
- **SSO** with major identity providers
- **Data residency commitments** per contract
- **Compliance attestations** (on request, per jurisdiction)

Contact `partners@herline.vip` for institutional agreements.

## Changes to This Document

When we update this document:
- Material changes are announced via in-product notification
- Change history is maintained in this repository's Git log
- Users can review the Git blame to see when any specific principle was adopted

---

**Full privacy policy**: [herline.vip/privacy](https://herline.vip/privacy)
**Questions**: `privacy@herline.vip`
**Data deletion requests**: `privacy@herline.vip`
**Security vulnerabilities**: `security@herline.vip` (see [SECURITY.md](../SECURITY.md))

---

**See also**: [Architecture](architecture.md) · [Glossary](glossary.md) · [FAQ](faq.md) · [Main README](../README.md)
