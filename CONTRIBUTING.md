# Contributing to the SBOL Standard Website

This guide is for editors and community members who want to add or update content on [sbolstandard.org](https://sbolstandard.org). You do not need to know Hugo, SCSS, or any programming language — all content is written in plain Markdown with a short block of structured data at the top.

---

## Prerequisites

- A [GitHub account](https://github.com/join)
- Basic familiarity with editing files on GitHub (or cloning a repo locally)

Installing Hugo and running the site locally allows you to preview changes before submitting. See the main [README](README.md) for local setup instructions.

---

## How to Submit a Change

1. **Fork** the repository on GitHub.
2. **Create a branch** for your change (e.g. `add-pysbol-library`).
3. **Edit or add files** following the relevant guide below.
4. **Open a Pull Request** against `master`. An editor will review and merge it.

If you spot a problem but don't want to fix it yourself, [open an issue](https://github.com/SynBioDex/SbolStandardWebsite/issues/new) instead.

---

## Content Guides

Each guide below covers one type of content, with step-by-step instructions and a real example from the repo.

| What you want to add or change | Guide |
|---|---|
| News announcement or event notice | [Announcements](docs/editors/01-announcements.md) |
| Blog post | [Blog Posts](docs/editors/02-blog-post.md) |
| Software library | [Libraries](docs/editors/03-library.md) |
| Application or tool | [Applications](docs/editors/04-application.md) |
| GenAI tool or AI resource | [GenAI Tools](docs/editors/05-genai-tool.md) |
| Image in the Visual Gallery | [Visual Gallery](docs/editors/06-visual-gallery.md) |
| Person on the Leadership page | [Leadership](docs/editors/07-leadership.md) |
| Publication | [Publications](docs/editors/08-publication.md) |

---

## General Rules

- **Never put HTML, CSS, or JavaScript inside Markdown files.** All content files should contain only front matter (the `---` block at the top) and plain Markdown text. Styling and layout are handled by the templates.
- **Follow the folder structure exactly.** Each content type lives in a specific place; the guides show you where.
- **Use the existing entries as your template.** Every guide links to a real example in the repo.
- **Images go in the same folder as the content file** — not in `static/` or anywhere else.

---

## Questions

Ask on [Slack](https://join.slack.com/t/sbol-standard/shared_invite/zt-1ukcka8b8-Z4QoyiE_LwwoRBw2DzheSg) or open a GitHub issue.
