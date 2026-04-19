# Assets

Static assets referenced by documentation in this repository.

## Current Contents

- `architecture-diagram.svg` — A simple vector diagram of the 7-layer pipeline, referenced from the main README and `docs/architecture.md`.

## Needed — TODO (add these before publishing)

These assets need to be created and dropped into this folder. Once added, the `README.md` references will resolve correctly.

### `logo.svg` (required)
Herline's logo as SVG. Referenced in README header. Target: clean, monochrome or subtle two-color version. Vector format for crispness at any size.

### `logo-128.png` (recommended)
PNG fallback for the logo. 128x128px. Some GitHub surfaces render PNG more reliably than SVG.

### `social-preview.png` (recommended)
Social media preview image for the GitHub repo. **1280x640px**. Shown when the repo is linked on Twitter, LinkedIn, Discord, etc. Should feature:
- Herline name and tagline
- Clean, legible design
- Consistent with brand identity

Upload in GitHub repo Settings → Options → Social preview.

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

See [CONTRIBUTING.md](../CONTRIBUTING.md) for general contribution guidelines.

---

*All assets in this folder are licensed under [CC BY 4.0](../LICENSE), same as the rest of the repository.*
