# Adding a Library

Libraries appear on the **Ecosystem → Libraries** page, organised into SBOL 2 and SBOL 3 tabs. Each library has a category that controls where it appears within a tab.

---

## Where the files live

```
content/libraries/
└── your-library-slug/
    ├── index.md
    └── featured.png   ← logo or screenshot (recommended)
```

---

## Step-by-step

1. Create a new folder inside `content/libraries/` (lowercase, hyphenated).
2. Add `index.md` with the front matter below.
3. Optionally add `featured.png` — a logo or screenshot shown on the card.
4. Write a description of the library in Markdown below the closing `---`.

---

## Template

```markdown
---
title: "Library Name"
summary: "One sentence describing what the library does."
tags:
  - Libraries
sbol_versions: ["3"]        # "2", "3", or ["2", "3"] for both
lib_category: library       # see categories below
date: "2026-06-01T00:00:00Z"

external_link: ""

image:
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: GitHub
    url: https://github.com/your-org/your-repo
  - icon: edge
    icon_pack: fab
    name: Documentation
    url: https://your-docs-url.com
---

Write a description of the library here. Explain what it does, what language it targets, and any relevant background.
```

---

## Real example

`content/libraries/sbol3-py/index.md`

```markdown
---
title: Python
summary: Python interfaces and implementations for SBOL
tags:
  - Libraries
sbol_versions: ["3"]
lib_category: primary
date: "2022-02-15T16:30:18Z"
external_link: ""
image:
  focal_point: Smart
links:
  - icon: github
    icon_pack: fab
    name: Github
    url: https://github.com/SynBioDex/pySBOL3
  - icon: edge
    icon_pack: fab
    name: API & Documentation
    url: https://pysbol3.readthedocs.io
---

[pySBOL3](https://opensource.org/licenses/MIT) provides Python interfaces...
```

---

## Field reference

| Field | Required | Notes |
|---|---|---|
| `title` | Yes | Displayed as the library name |
| `summary` | Yes | One-line description shown in the card |
| `sbol_versions` | Yes | Controls which tab the library appears in. Use `["2"]`, `["3"]`, or `["2","3"]` |
| `lib_category` | Yes | Controls the section within the tab (see below) |
| `date` | Yes | ISO 8601 format. Used for ordering within a section |
| `links` | No | List of icon buttons shown on the card. See icon packs below |
| `external_link` | No | If set, the card title links here instead of to the detail page |

### `lib_category` values

| Value | Where it appears |
|---|---|
| `primary` | "Primary Libraries" — actively maintained core implementations |
| `library` | "Libraries" — community-contributed implementations |
| `resource` | "Resources" — notebooks, utilities, and other tooling |

### Link icon packs

Icons come from Font Awesome. Use `icon_pack: fab` for brand icons (GitHub, npm) and `icon_pack: fas` for solid icons (tools, bug, code). Browse available icons at [fontawesome.com](https://fontawesome.com/icons).

---

## Common mistakes

- **Wrong `sbol_versions` format** — must be a YAML list: `["3"]` not just `3`.
- **Unknown `lib_category`** — only the three values above are recognised; typos cause the entry to be silently omitted.
- **Image not named `featured`** — the card image must be `featured.png` or `featured.jpg`.
