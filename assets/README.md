# Assets

Static assets referenced by documentation in this repository.

## Current Contents

- `logo.svg` — approved red staircase master mark, embedded as a transparent PNG in SVG for consistent display. Referenced in both README headers.
- `architecture-diagram.svg` — Public map of Herline App's reading, course creation, presentation, and rehearsal surfaces.
- `social-preview.svg` + `social-preview.png` — 1280x640 social media preview card. The PNG has been rendered from the current SVG and visually checked. GitHub Settings → Social preview requires a separate upload; changing this file does not update that setting.
- `share-wechat.svg` + `share-wechat.png` — 800x800 Chinese-language sharing card. The PNG has been rendered from the current SVG and visually checked. Both cards use the approved red staircase master mark.

## Optional — Future Additions

### `logo-128.png` (optional)

PNG fallback for the logo. 128x128px. Useful for surfaces that don't render SVG (rare on modern GitHub).

### `screenshots/` (optional)

Product screenshots, if the team wants to include them. Keep public-safe:

- Use demo data, not real user data
- No admin surfaces
- No internal-only features

## Formatting Standards

### SVG

- ViewBox-based (scalable)
- Embedded text should use web-safe fonts or be converted to paths
- Keep file size reasonable (under 50KB for diagrams)

### PNG

- 72 DPI is fine for web display
- PNG-24 with transparency where appropriate
- Optimize with tools like `pngquant` before committing

### Naming

- Use lowercase with hyphens: `architecture-diagram.svg`, not `ArchitectureDiagram.svg`
- Descriptive, not cryptic: `logo-dark-mode.svg`, not `logo2.svg`
- Size suffixes only when multiple sizes exist: `logo-128.png`, `logo-512.png`

## Contributing Assets

If you contribute visual assets:

- Ensure you have rights to all artwork (no stock photo violations, no copyrighted logos)
- Submit through a PR with clear description
- Include the source file (Figma link, Illustrator file) separately if possible, for future edits
- Use demo data only; do not include customer, account, or private workspace content

See [CONTRIBUTING.md](../CONTRIBUTING.md) for general contribution guidelines.

---

*All assets in this folder are licensed under [CC BY 4.0](../LICENSE), same as the rest of the repository.*
