# Adding or Editing a Person on the Leadership Page

The Leadership page (`/community-leadership/`) is powered by Wowchemy's people widget. Each person has a profile folder under `content/authors/`. The same profiles are used for blog post attribution.

---

## Where the files live

```
content/authors/
└── firstname-lastname/
    ├── _index.md
    └── avatar.jpg    ← headshot photo
```

The folder name is the person's slug (used in blog `authors:` lists and internal links). Use lowercase with hyphens.

---

## Step-by-step

### Adding a new person

1. Create a new folder inside `content/authors/` (e.g. `content/authors/jane-smith/`).
2. Add `_index.md` with the front matter below.
3. Add a headshot photo named `avatar.jpg` or `avatar.png` in the same folder.

### Editing an existing person

Open the relevant `content/authors/<slug>/_index.md` and update the fields directly.

### Changing someone's group (e.g. moving a chair to Past Chairs)

Update the `user_groups` list in their `_index.md`. A person can belong to multiple groups and will appear in each section on the Leadership page.

---

## Template

```markdown
---
title: Jane Smith
role: "SBOL Editor (2024–present)"
weight: 10          # lower numbers appear first within a section
organizations:
  - name: University of Example
    url: "https://example.ac.uk"
social:
  - icon: envelope
    icon_pack: fas
    link: mailto:jane@example.ac.uk
  - icon: github
    icon_pack: fab
    link: https://github.com/janesmithgithub
  - icon: linkedin
    icon_pack: fab
    link: https://linkedin.com/in/janesmith
user_groups:
  - Current Editors
---

Optional short bio in plain Markdown. Appears on the person's profile page.
```

---

## Real example

`content/authors/prashant-vaidyanathan/_index.md`

```markdown
---
title: Prashant Vaidyanathan
role: "SBOL Chair (2023–present)"
weight: 10
organizations:
  - name: Oxford Biomedica
    url: ""
user_groups:
  - Current Chair
  - Past Editors
---
```

---

## Field reference

| Field | Required | Notes |
|---|---|---|
| `title` | Yes | Full name as it should appear on the site |
| `role` | No | Job title or SBOL role. For Past Chairs, include tenure dates (e.g. `SBOL Chair (2019–2022)`) |
| `weight` | No | Controls ordering within a section. Lower = appears earlier. Default is unordered |
| `organizations` | No | List of `name` + `url` pairs. `url` can be empty |
| `social` | No | List of social/contact links with Font Awesome icons |
| `user_groups` | Yes | Controls which section(s) on the Leadership page the person appears in |

### Valid `user_groups` values

| Value | Section on Leadership page |
|---|---|
| `Current Chair` | Current Chair |
| `Current Editors` | Current Editors |
| `Steering Committee` | Steering Committee |
| `Advisory Board` | Advisory Board |
| `Past Chairs` | Past Chairs |
| `Past Editors` | Past Editors |

A person can be in multiple groups (e.g. someone who is both a Steering Committee member and a Past Editor).

### `role` visibility

The `role` field is shown only in the **Past Chairs** section. In all other sections it is hidden, so the section heading itself provides the context. For Past Chairs, use the tenure format: `SBOL Chair (2019–2022)`.

---

## Common mistakes

- **File named `index.md` not `_index.md`** — author profiles must use `_index.md` (with the leading underscore). A file named `index.md` will not be picked up as an author profile.
- **Wrong `user_groups` value** — the value must match exactly (including capitalisation). A typo means the person does not appear on the Leadership page.
- **Avatar not found** — without `avatar.jpg` or `avatar.png`, a grey placeholder is shown. Add a headshot whenever possible.
- **`authors` vs `credit`** — when listing someone as a blog post author, use their slug in the post's `authors:` list, not their full name.
