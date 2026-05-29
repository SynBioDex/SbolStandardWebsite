# Adding an Application

Applications appear on the **Ecosystem → Applications** page. These are tools, platforms, and software that use or support SBOL — distinct from libraries (which are code packages developers import into their own projects).

---

## Where the files live

```
content/applications/
└── your-app-slug/
    ├── index.md
    └── featured.png   ← screenshot or logo (recommended)
```

---

## Step-by-step

1. Create a new folder inside `content/applications/` (lowercase, hyphenated).
2. Add `index.md` with the front matter below.
3. Add `featured.png` — a screenshot or logo is strongly recommended as it appears on the card.
4. Write a description in Markdown below the closing `---`.

---

## Template

```markdown
---
title: "Your Application Name"
summary: "One sentence describing what the tool does."
tags:
  - Design         # see common tags below
date: "2026-06-01T00:00:00Z"
active: true       # set to false to move to the Deprecated section

external_link: ""

image:
  focal_point: Smart

links:
  - icon: edge
    icon_pack: fab
    name: Website
    url: https://your-tool-url.com
  - icon: github
    icon_pack: fab
    name: GitHub
    url: https://github.com/your-org/your-repo
---

Write a description of the application here.
```

---

## Real example

`content/applications/synbiohub/index.md`

```markdown
---
title: SynBioHub
summary: A registry for storing and sharing genetic circuit designs using the SBOL2 standard
tags:
  - Repository
  - Visualization
date: "2020-06-30T00:00:00Z"
external_link: ""
image:
  focal_point: Smart
links:
  - icon: edge
    icon_pack: fab
    name: Link
    url: https://synbiohub.org/
  - icon: github
    icon_pack: fab
    name: GitHub
    url: https://github.com/SynBioDex/SynBioHub
---

SynBioHub is a repository for sharing genetic designs...
```

---

## Field reference

| Field | Required | Notes |
|---|---|---|
| `title` | Yes | Name of the application |
| `summary` | Yes | One-line description shown in the card |
| `tags` | Yes | Used by the filter bar on the Applications page. See common tags below |
| `date` | Yes | ISO 8601 format. Used for ordering |
| `active` | No | Defaults to `true`. Set to `false` to move to the Deprecated section at the bottom of the page |
| `external_link` | No | If set, clicking the card goes directly here instead of a detail page |

### Common tags

`Design`, `Repository`, `Visualization`, `Simulation`, `Conversion`, `Validation`, `Education`, `Notebook`

You can introduce new tags — they will automatically appear in the filter bar. Keep them concise (one or two words).

---

## Common mistakes

- **No `featured.png`** — applications without an image display a blank card, which looks unfinished. Add a screenshot or logo.
- **Too many tags** — two or three tags per application is enough. More dilutes the filter bar.
- **Using `active: false` instead of deleting** — prefer `active: false` for deprecated tools so the history is preserved on the site.
