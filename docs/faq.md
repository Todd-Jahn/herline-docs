# Frequently Asked Questions

Extended FAQ — for the short version see the [main README](../README.md#faq).

## Product Basics

### What is Herline?
Herline is an AI engine that turns your professional expertise into three forms of outbound deliverables — **keynote speeches, pitch decks, and full courses**. It runs a 7-layer pipeline specifically for the "expertise → outbound product" workflow.

### How is Herline different from ChatGPT or Claude?
Generic AI tools are one-shot: you ask, they respond, context evaporates. Herline is a **pipeline with persistent state**. Your personal knowledge database grows with every book, deep-read, and course you build. Long-term Herline users see compounding productivity that ad-hoc AI users don't.

### What are the 7 layers, briefly?
Assessment → Atlas → Library (D2B) → Studio → Courses (B2C) → Prep → Boost. Full walkthrough in [architecture.md](architecture.md).

### Do I have to use all 7 layers?
No. Each layer is usable standalone. Common entry points:
- **Start with Assessment + Atlas** if you want personalized book recommendations
- **Start with Library (D2B)** if you have a specific book you want deconstructed
- **Start with Studio + Courses** if you have a clear course goal in mind
- **Start with Prep** if you already have course material and need delivery-format exports

### Is there a free tier?
Yes. The free tier covers Assessment, a first deep-read, and a course generation trial. Sign up at [herline.vip](https://herline.vip). No credit card required.

### Where should I start if I'm new?
1. Complete the Assessment (5–10 minutes)
2. Pick one book you've already read well
3. Run a deep-read in Library
4. Use Studio to plan a 3-unit mini-course
5. Generate it in Courses
6. Export a keynote version in Prep

This 1–2 hour end-to-end walk-through shows the full pipeline in action.

## Who It's For

### Am I a "super individual"?
If you have specialized professional knowledge and want to turn it into outbound products (speeches, decks, courses), yes. Typical profiles:
- Independent consultants with 5+ years of domain expertise
- Content creators building a personal brand
- Domain experts who teach or train
- Solo founders raising capital or building thought leadership

If you're in a large team producing content collaboratively, Herline may not be the best fit (yet).

### Can teams use this?
Currently, Herline is optimized for single users building personal knowledge graphs. Multi-user collaboration is on the roadmap but not a current priority. Teams have used Herline effectively when each member maintains their own knowledge graph and shares finished deliverables.

### Can institutions (schools, training orgs) use this?
Yes — the institution tier supports curriculum matrices and teacher collaboration. One teacher's deep-read expertise can auto-expand into a full curriculum. Contact `partners@herline.vip`.

### What about students?
Students benefit most when they're **producing** (writing papers, preparing presentations, building portfolio projects) rather than just consuming. Herline's pipeline is productive-side; students in producer mode fit well.

### Is Herline useful if I don't read books?
The Library (D2B) layer is book-centric but accepts other long-form inputs — transcripts, articles, research reports, course notes. Source material needs enough structure to yield Claims/Concepts/Methods. A tweet thread won't; a 30-page whitepaper will.

## Data & Privacy

### Does Herline train AI models on my data?
**No.** Your private data is never used for model training. Full details in [data-handling.md](data-handling.md).

### Can I export my knowledge graph?
Yes. Export is always available in formats that don't require Herline to consume. Your knowledge belongs to you.

### Where is my data stored?
Data is stored in region-appropriate infrastructure. Users in mainland China have data stored in mainland-China cloud providers; international users have data in international providers. Full details in our [privacy policy](https://herline.vip/privacy).

### What if I cancel my account?
You retain access to export for 30 days after cancellation. After that, data is deleted per our retention policy. See [data-handling.md](data-handling.md).

### What about intellectual property of generated content?
**You own what you create.** Herline's output (courses, keynotes, pitch decks built from your knowledge) is yours to use commercially without royalty. Source material (books, articles) retains its original copyright — you can't redistribute raw extracted content from copyrighted books without permission, just as you couldn't redistribute your own notes.

## Technical Questions

### What languages are supported?
- **Input**: English and Chinese (Simplified + Traditional) fully supported. Other languages in exploratory state.
- **Output**: English and Chinese with high-fidelity TTS. Other languages available with machine translation (quality varies).

### What file formats can I import?
- **Books**: EPUB, PDF (text-extractable), TXT
- **Articles**: PDF, Markdown, plain text, URL fetches
- **Structured content**: DOCX, various e-reader exports

Scanned PDFs require OCR first; we recommend external OCR (our internal OCR is limited).

### How long does generation take?
- **Deep-read (D2B)**: 8–15 minutes per book (varies with length and density)
- **Course generation (B2C)**: 30–90 minutes for 3–7 unit course with audio
- **Prep export**: under 2 minutes per format (PDF / PPTX / DOCX)
- **Keynote generation**: ~30 minutes end-to-end

Long jobs run async — you can queue multiple and come back later.

### Is there an API?
Not yet public. A public API with stable versioning is on the Q3+ roadmap. Institutional partners can get custom API access — contact `partners@herline.vip`.

### What happens if a generation fails partway through?
Jobs are checkpointed. Failures resume from the last checkpoint on retry rather than restarting. Token costs for resumed jobs are only incurred on the remaining work.

## Integrations

### Does Herline integrate with Notion / Obsidian / Logseq?
Not natively yet. You can export Herline outputs in formats those tools accept (Markdown, PDF), but bidirectional sync is not built. It's on the roadmap but not committed.

### Will there be an MCP (Model Context Protocol) server?
Yes, this is on our Q3+ roadmap. When ready, Claude / ChatGPT / Cursor users will be able to call Herline capabilities directly from their AI clients.

### Can I integrate Herline via webhook?
Webhooks for generation events (course generation complete, export ready) are available on higher tiers. Contact support for access.

## Business / Team

### Who's behind Herline?
A small team operating out of East Asia and beyond. We're a product-first team with deep focus on knowledge-work infrastructure.

### How can I partner with Herline?
- **Content IP partnerships** (books, shows, communities): `partners@herline.vip`
- **Educational institutions**: `partners@herline.vip`
- **Distribution / reseller**: `partners@herline.vip`
- **Press / media**: `hi@herline.vip`

### Is Herline open source?
Core engines are **proprietary** — they represent years of domain-specific research and are what differentiate Herline from generic AI tools. This repository (public documentation, examples, resources) is open under CC BY 4.0. Peripheral components (MCP server, OpenAPI spec) may be open-sourced over time.

### How can I invest in / partner with Herline?
We're not running a public funding round at time of writing. Qualified parties can reach out to `hi@herline.vip`.

## Support

### How do I get help with the product?
- **In-product**: use the help menu on [herline.vip](https://herline.vip)
- **Email**: `hi@herline.vip`
- **Discussion (documentation issues only)**: [GitHub Discussions](https://github.com/herline/herline/discussions)

### How do I report a bug?
- **Product bugs**: use in-app "Report a Bug" or email `hi@herline.vip`
- **Documentation bugs (this repo)**: [open a GitHub issue](https://github.com/herline/herline/issues/new/choose)

### How do I report a security vulnerability?
Email `security@herline.vip` — see [SECURITY.md](../SECURITY.md) for the full process.

### How do I request a feature?
- **Product features**: email `hi@herline.vip` or use in-product feedback
- **Documentation enhancements**: [open a GitHub issue](https://github.com/herline/herline/issues/new/choose)

---

**Still have questions?** Email `hi@herline.vip` — we read and respond to everything.

**See also**: [Architecture](architecture.md) · [Glossary](glossary.md) · [Data Handling](data-handling.md) · [Main README](../README.md)
