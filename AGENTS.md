# AGENTS.md

## Project Context

This is a static website for Slim Power Advisory (SPA), an electrical and power consulting business. The site is a single-page Bootstrap HTML site in `docs/index.html`.

The site is served via GitHub Pages from the `docs/` folder on the `main` branch. All published files (HTML, CSS, images) must live under `docs/`.

## Code Style

- Keep edits simple, explicit, and easy to review.
- Prefer small, focused changes over broad refactors.
- Preserve the existing Bootstrap-based structure unless there is a clear reason to change it.
- Use double quotes for HTML attributes.
- Keep indentation consistent with the existing file: two spaces.
- Avoid comments that simply restate what the markup already says.

## Web Design Guidelines

- Use Bootstrap classes and components as much as possible for layout, spacing, typography, responsive behaviour, and common UI patterns.
- Create or update `docs/assets/style.css` only for extra styling that Bootstrap cannot express cleanly.
- Keep custom CSS small, project-specific, and easy to scan.
- Avoid duplicating Bootstrap utility classes in custom CSS.
- Prefer Bootstrap responsive grid and utility classes before adding custom media queries.
- Keep the visual style restrained, professional, and suitable for an advisory business.
- Use the existing colour palette:
  - navy: `#0d2137`
  - gold: `#f0b429`
  - Bootstrap neutrals
- Avoid decorative clutter, gradients, and unnecessary visual effects.

## Content Guidelines

- Keep copy professional, clear, and business-focused.
- Use Australian spelling where applicable, such as `organisation`, `optimise`, and `favour`.
- Do not invent credentials, employment history, locations, contact details, or client claims.
- If content is taken from LinkedIn, screenshots, or other supplied references, stay faithful to the provided material.
- Keep Sarah Lim's profile content aligned with:
  - energy infrastructure leadership
  - business cases
  - regulation
  - asset management
  - innovation
  - commercially sound investment decisions
  - Australia's energy transition

## Images

- Store project images in `docs/assets/`.
- Use descriptive filenames, for example `sarah-lim.png`.
- Reference images with paths relative to `docs/index.html`, for example `assets/sarah-lim.png`.
- Prefer local images over remote hotlinks.
- When replacing an image, verify the file renders correctly and is referenced from `docs/index.html`.

## Verification

After edits, check:

- The page still loads as plain static HTML.
- Navigation anchor links still work.
- The team section renders cleanly on desktop and mobile widths.
- Image paths are valid.
- External links use `target="_blank"` and `rel="noopener noreferrer"`.

## Git / Safety

- Do not revert unrelated user changes.
- Do not run destructive git commands unless explicitly requested.
- Keep diffs focused on the requested change.
