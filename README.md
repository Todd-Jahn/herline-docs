<p align="center">
  <a href="https://herline.vip">
    <img src="assets/logo.svg" height="96" alt="Herline">
  </a>
</p>

<h1 align="center">Herline</h1>

<p align="center">
  <strong>The AI engine for super individuals.</strong><br>
  Turn your expertise into <b>keynotes</b>, <b>pitch decks</b>, and <b>full courses</b>.
</p>

<p align="center">
  <a href="https://herline.vip"><img src="https://img.shields.io/badge/website-herline.vip-5b8def?style=flat-square" alt="Website"></a>
  <img src="https://img.shields.io/badge/status-production-22c55e?style=flat-square" alt="Status">
  <img src="https://img.shields.io/badge/languages-EN%20%7C%20中文-6366f1?style=flat-square" alt="Languages">
  <a href="LICENSE"><img src="https://img.shields.io/badge/docs-CC%20BY%204.0-f59e0b?style=flat-square" alt="License"></a>
</p>

<p align="center">
  <a href="#what-is-herline">What</a> •
  <a href="#the-7-layer-pipeline">Pipeline</a> •
  <a href="#who-its-for">Who</a> •
  <a href="#use-cases">Use Cases</a> •
  <a href="#architecture">Architecture</a> •
  <a href="#roadmap">Roadmap</a> •
  <a href="#faq">FAQ</a> •
  <a href="README.zh-CN.md">中文</a>
</p>

---

## What is Herline

**Herline** is a vertical AI engine built for the **12M+ solopreneurs, independent consultants, and knowledge creators** who have deep expertise but struggle to turn it into external deliverables.

Unlike generic AI tools (ChatGPT, Claude, Notion AI) that help you *write words*, Herline runs a **7-layer pipeline** that turns your professional knowledge into the three forms of outbound expression every super individual actually uses — **speeches to deliver on stage, pitch decks to raise capital, and courses to teach paying students**.

🌐 **Live at [herline.vip](https://herline.vip)** — free tier available.

---

## Why Herline Exists

Smart people read 50 books a year and still can't teach what they learned. Not because the books are bad — but because **from "I read it" to "I can teach it", an entire workflow is missing**:

- **Deconstruct** — knowledge networks broken into reusable blocks, not just summaries
- **Recompose** — blocks reorganized by learning arc, not outline stacking
- **Deliver** — expressed in the right medium (a keynote ≠ a course ≠ a short video)
- **Persist** — saved as a personal knowledge graph, not forgotten after the chat closes

Generic AI tools break down at step one. Herline is the pipeline that closes the loop.

The mission: **make every knowledge worker a viable one-person company.**

---

## The 7-Layer Pipeline

```
    ┌─────────────┐
    │ Assessment  │  →  Capture your professional profile
    └──────┬──────┘
           ↓
    ┌─────────────┐
    │    Atlas    │  →  Personalized book & content planning
    └──────┬──────┘
           ↓
    ┌─────────────┐
    │   Library   │  →  Deconstruct books into reusable knowledge blocks
    │    (D2B)    │      (Claims / Concepts / Methods)
    └──────┬──────┘
           ↓
    ┌─────────────┐
    │   Studio    │  →  Design course strategy from your knowledge graph
    └──────┬──────┘
           ↓
    ┌─────────────┐
    │   Courses   │  →  Auto-generate full courses with scripts,
    │    (B2C)    │      TTS audio, and assessments
    └──────┬──────┘
           ↓
    ┌─────────────┐
    │    Prep     │  →  Export keynotes, pitch decks, teaching materials
    └──────┬──────┘
           ↓
    ┌─────────────┐
    │    Boost    │  →  Adapt content for multi-platform distribution
    └─────────────┘
```

Each layer is usable standalone. Or chain them end-to-end: **one book in, a complete set of deliverables out**.

📖 See [`docs/architecture.md`](docs/architecture.md) for a deeper walkthrough.

---

## Who It's For

| Persona | Core Pain | What Herline Solves |
|---|---|---|
| **Independent Consultant** | 10 years of expertise reassembled from scratch for every proposal | Personal knowledge graph → reusable callable blocks |
| **Content Creator / Lecturer** | 2–4 weeks to prepare a single course | D2B → Studio → B2C pipeline compresses it to 1–2 days |
| **Solo Founder** | Pitch decks eat creative energy before product work | Expertise + one book → pitch deck ready for iteration |
| **Institution / School** | Need 10 curricula/year, can only produce 2 | One teacher's expertise auto-expands into a curriculum matrix |

---

## What Makes Herline Different

- 🧠 **Persistent personal knowledge graph** — grows with every book, every deep-read, every course. Cross-book RAG surfaces insights at intersections you'd never find manually.
- 🏗️ **End-to-end vertical pipeline** — not another AI chat box. Seven specialized layers, each addressing a specific workflow break.
- 🌐 **Bilingual native** — Chinese and English are first-class throughout, not bolted-on translation layers.
- 📦 **Export to deliverables, not documents** — PDFs with timing notes, PPTX templates with speaker structure, curriculum-ready assessments.
- 🎯 **Built for super individuals** — 12M+ one-person companies, domain experts, educators. Not for teams, not for enterprises (yet).
- 🔐 **Data ownership** — your knowledge database belongs to you. The system gets smarter with use; we never repackage your content. See [`docs/data-handling.md`](docs/data-handling.md).

---

## Use Cases

### 📣 Book → Keynote
**Input**: a book you've read + a short bio.
**Output**: a 30–45 min keynote script with timing annotations, slide deck template, and quote cards.
**Typical time**: ~30 minutes end-to-end.

👉 [See full example](examples/book-to-keynote/)

### 💼 Expertise → Pitch Deck
**Input**: your professional profile + target audience.
**Output**: 15–20 page pitch deck with narrative arc and speaker notes.
**Typical time**: ~45 minutes end-to-end.

### 🎓 Book → Full Course
**Input**: a book + target learner profile.
**Output**: 3–7 unit course with scripts, TTS audio narration, and assessments.
**Typical time**: 1–2 hours end-to-end.

### 📚 Knowledge Graph Over Time
Every read, course, and deck persists in your personal knowledge database. Cross-book RAG surfaces connections you'd never find manually. The longer you use Herline, the smarter it gets for you specifically.

---

## Architecture

At a high level:

| Layer | Stack |
|---|---|
| Frontend | React 18 · Next.js 16 · TypeScript · Tailwind CSS |
| Backend | FastAPI · SQLAlchemy (async) · Python 3.11 |
| AI orchestration | **LangGraph 1.0** — multi-step workflows across specialized agents |
| Data | MySQL 8 (metadata) · Redis 7 (cache/queue) · Milvus 2.6 (vector) |
| Async processing | **ARQ** on Redis Streams — long-running D2B / B2C generation jobs |
| Speech synthesis | Cloud-based TTS for audio course generation |

Under the hood:
- LangGraph-orchestrated multi-step pipelines with state checkpointing
- Dual-LLM strategy: generative models for synthesis, reasoning models for structured output
- Cross-book RAG via Milvus with custom embedding strategies
- Token-aware cost management across 10M+ monthly token operations
- Structured knowledge-block schema (Claims / Concepts / Methods) that enables cross-book composition

The deconstruction and generation engines are proprietary. This repository exists for public documentation, not source distribution. See [`docs/architecture.md`](docs/architecture.md) for a deeper walkthrough.

---

## Roadmap

### ✅ Shipped (Q1 2026)
- 7-layer pipeline — production-ready
- Prep export: PDF / PPTX / DOCX
- Cross-book RAG over personal knowledge graph
- Elective courses marketplace
- Sharing & collaboration primitives

### 🚧 In Progress (Q2 2026)
- GCYSC — Global Chinese Youth Speaking Competition school partnerships
- Domestic GTM: city partner program V1
- Marketing agent (Boost) for automated multi-platform distribution
- Sentiment & citation tracking for brand visibility in AI search

### 🔭 Exploring (Q3+ 2026)
- **MCP Server** — native Claude / ChatGPT / Cursor integration
- **Public OpenAPI spec** — enable external tool integrations
- GPT Store presence for "Course Planner by Herline"
- International expansion (EN / ES / JA)
- Creator monetization layer

---

## FAQ

### Is Herline open source?
**No.** This repository is public documentation and community resources only. The engines that power Herline's deconstruction and generation are proprietary — they represent years of domain-specific research and are what differentiate Herline from generic AI wrappers. We may open specific peripheral components (like MCP integration and OpenAPI spec) over time.

### How is Herline different from ChatGPT / Claude?
Generic AI tools are one-shot. You ask, they respond, and the context evaporates. Herline is a **pipeline with persistent state** — your personal knowledge database grows with every use. Long-term Herline users become significantly more productive than ad-hoc AI users because of this compounding effect.

### Does Herline support English content?
Yes. The pipeline is bilingual throughout. You can deep-read English books, generate English courses, and export English-language keynotes. Native support, not translation layers.

### Can I use Herline for institutional / academic curriculum?
Yes. The institution tier supports curriculum matrices and teacher collaboration. One teacher's expertise auto-expands into a full curriculum matrix. Contact `partners@herline.vip` for institutional inquiries.

### What's the data ownership model?
Your knowledge database belongs to you. We never repackage your content, never train models on your private data, and never sell data. You can export your knowledge graph at any time. See [`docs/data-handling.md`](docs/data-handling.md).

### How long does a typical generation take?
- **D2B deep read**: 8–15 minutes per book (Claims / Concepts / Methods extraction)
- **B2C course generation**: 30–90 minutes for a 3–7 unit course with audio
- **Prep export**: under 2 minutes per format
- Long runs execute asynchronously — you can queue multiple jobs.

### Is there a free tier?
Yes. Sign up at [herline.vip](https://herline.vip) — the free tier covers the assessment, first deep-read, and a course generation trial.

### What about privacy and enterprise compliance?
See [herline.vip/privacy](https://herline.vip/privacy) for the full privacy policy. Enterprise compliance features (SSO, audit logs, data residency) are available on higher tiers — contact `partners@herline.vip`.

More questions? See [`docs/faq.md`](docs/faq.md) for the extended FAQ.

---

## Resources

- 🌐 **Product** — [herline.vip](https://herline.vip)
- 📖 **Documentation** — [`docs/`](docs/) (architecture · glossary · FAQ · data handling)
- 🏛️ **Architecture walkthrough** — [`docs/architecture.md`](docs/architecture.md)
- 📚 **Glossary** — [`docs/glossary.md`](docs/glossary.md)
- 🎓 **Example outputs** — [`examples/`](examples/)
- 📋 **Awesome Super Individual** — [curated resources for solopreneurs](https://github.com/Todd-Jahn/awesome-super-individual) (companion list, CC0)
- 💬 **Discussions** — [GitHub Discussions](https://github.com/Todd-Jahn/herline-docs/discussions)
- 📧 **Contact** — hi@herline.vip
- 🤝 **Partner / institutional inquiries** — partners@herline.vip

---

## Contributing

We welcome translations, documentation improvements, and case study contributions. See [`CONTRIBUTING.md`](CONTRIBUTING.md).

Core product feature requests go to `hi@herline.vip` or [herline.vip/feedback](https://herline.vip) — not via this repo.

---

## About

Herline is built by a small team operating out of **East Asia and beyond**, shipping production infrastructure for a global audience of super individuals.

We believe the defining challenge of the next decade isn't "can AI generate content" — it's **can every knowledge worker turn their expertise into products that compound**. Herline is our answer.

**Mission**: make every knowledge worker a viable one-person company — by closing the workflow gap between what they know and what they can deliver.

---

## License

The content in this repository (documentation, diagrams, examples, and resources) is licensed under **[CC BY 4.0](LICENSE)**. You are free to share and adapt, with attribution.

**Herline's core engine is proprietary** and not part of this repository. See [herline.vip/terms](https://herline.vip/terms) for product terms of service.
