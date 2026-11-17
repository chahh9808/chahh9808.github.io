# Unused automation archive

Archived on 2026-11-17 after the owner confirmed that Netlify deployment and
BibTeX publication imports are not used. GitHub Pages remains the active
deployment workflow.

## Contents

- `netlify/netlify.toml`: former Netlify deployment configuration.
- `netlify/module-reference.txt`: the removed Netlify Hugo import, pinned Go
  dependency/checksums, and previous home output formats.
- `github/import-publications.yml`: former BibTeX-to-Markdown GitHub workflow.

These paths are outside `.github/workflows/` and Hugo's content roots, so the
archived files do not run or publish as website pages. The referenced Netlify
module source remains an external dependency; it is not vendored here.

## Restore only when needed

For Netlify, restore `netlify.toml` at the repository root, restore the module
import and dependency recorded in `module-reference.txt`, and re-enable the
`headers` and `redirects` home output formats. Run Hugo's module tidy command and
verify both hosting configurations before deploying.

For BibTeX imports, move the archived workflow back to
`.github/workflows/import-publications.yml`, add a valid root `publications.bib`,
and review the importer permissions and pull request settings before running it.
