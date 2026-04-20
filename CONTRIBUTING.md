# Contributing to Herline's Public Repository

Thanks for considering contributing! This repository is **public documentation**, not Herline's product source code. The following contributions are welcomed:

## What We Welcome

### 🌐 Translations
Help translate documentation into more languages. Open a PR with `README.<locale>.md` or `docs/<topic>.<locale>.md`.

Currently available: **English** + **简体中文**.
Priority locales we'd love help with: **繁體中文**, **日本語**, **한국어**, **Español**, **Português**.

### 📝 Documentation Improvements
- Typo fixes
- Clarifications to confusing sections
- Broken link fixes
- Factual corrections (please cite sources)
- Improvements to `docs/glossary.md`, `docs/faq.md`, `docs/architecture.md`

### 🎓 Use Case Contributions
Have a great example of using Herline? Open an issue first so we can align on format, then submit a PR to `examples/`. Each example should include:
- `README.md` — what the example demonstrates, target audience, skill level
- `input.md` — the raw inputs provided to Herline
- `output-*.md` — the Herline output (lightly polished, showcase quality)
- `generation-notes.md` — timing, human edits applied, lessons learned

### 🐛 Documentation Bugs
If something in this repo is wrong or misleading, open an issue with the `documentation` label.

## What We Don't Accept Here

- **Core product feature requests** → use `hi@herline.vip` or [herline.vip/feedback](https://herline.vip)
- **Bug reports about the product itself** → use the in-app bug report or email `hi@herline.vip`
- **Source code for the Herline engine** — the core engine is proprietary and not accepting contributions
- **Promotional content disguised as docs** — we'll reject PRs that read like advertising

## Pull Request Process

1. **Fork** this repository to your account
2. **Create a branch**:
   ```bash
   git checkout -b docs/<short-description>
   ```
   Use prefixes: `docs/`, `translate/`, `example/`, `fix/`
3. **Make your changes** — keep each PR focused on one logical change
4. **Ensure markdown lints clean** — GitHub Actions will run `markdownlint` on all `.md` files
5. **Test links** — make sure internal links resolve (relative paths, anchor fragments)
6. **Submit a PR** with a clear description:
   - What changed
   - Why it matters
   - How to verify
7. **Respond to review feedback** — we aim to review within 7 days

All contributions are licensed under [CC BY 4.0](LICENSE).

## Style Guide

### Markdown
- Use ATX-style headers (`# H1`, `## H2`)
- Wrap lines naturally — no hard wrap at 80 chars
- Code blocks must specify language (` ```python`, ` ```bash`)
- Links: prefer descriptive anchor text over raw URLs
- Tables: use standard markdown tables, no HTML

### Language
- English docs: plain, direct. Avoid jargon. Short paragraphs.
- Chinese docs: 简洁、直接，避免翻译腔。优先短句。
- Both: no marketing puffery. Concrete examples over abstract claims.

### Tone
- Respectful, professional, warm
- We don't trash competitors — we describe what Herline is, not what others aren't
- First-person plural ("we") is fine for the Herline team
- Second-person ("you") addresses the reader directly — use it

## Code of Conduct

By participating, you agree to follow our [Code of Conduct](CODE_OF_CONDUCT.md).

## Questions?

- Open a [GitHub Discussion](https://github.com/Todd-Jahn/herline-docs/discussions)
- Email `hi@herline.vip`

We're glad you're here.
