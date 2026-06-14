# Adding an Announcement

Announcements appear in the **News → Announcements** section of the site and on the homepage feed. Use them for event notices, new releases, calls for abstracts, and other time-sensitive community news.

---

## Where the files live

```
content/post/
└── your-announcement-slug/
    └── index.md
```

Each announcement is a folder inside `content/post/`. The folder name becomes part of the URL (e.g. `content/post/combine-2026/` → `sbolstandard.org/post/combine-2026/`). Keep it short, lowercase, and hyphenated.

---

## Step-by-step

1. Create a new folder inside `content/post/` with a short descriptive name.
2. Inside that folder, create a file called `index.md`.
3. Copy the front matter template below and fill in the fields.
4. Write the body of the announcement in plain Markdown below the closing `---`.

---

## Template

```markdown
---
title: "Your Announcement Title"
date: 2026-06-01
summary: >
  One or two sentences that appear in the card preview on the homepage
  and listings page. Keep it under 200 characters.
tags:
  - Events          # add relevant tags; common ones: Events, Release, Community
---

Write the full announcement here in plain Markdown.

You can use headings, bullet lists, tables, bold text, and links.
```

---

## Real example

`content/post/combine-2026/index.md`

```markdown
---
title: "COMBINE 2026 — Workshop at Keele University, UK"
date: 2026-05-09
summary: >
  The 2026 COMBINE Workshop will be held at Keele University, UK, from
  7–10 September 2026. Registration and abstract submission are now open.
tags:
  - Events
  - COMBINE
  - Community
---

The **Computational Modeling in Biology Network (COMBINE)** ...
```

---

## Field reference

| Field | Required | Notes |
|---|---|---|
| `title` | Yes | Shown as the heading on the post page and in cards |
| `date` | Yes | ISO format (`YYYY-MM-DD`). Used for ordering — most recent appears first |
| `summary` | Yes | Short preview text shown in cards and the homepage feed |
| `tags` | No | Freeform list. Common values: `Events`, `Release`, `Community`, `COMBINE`, `HARMONY` |

---

## Common mistakes

- **Wrong folder** — files must be inside `content/post/`, not `content/blog/`. Blog posts and announcements are separate sections.
- **Missing `index.md`** — the file must be named exactly `index.md` (lowercase).
- **Date in the future** — Hugo will still publish it, but double-check the date is what you intend.
