# Adding a Blog Post

Blog posts appear in the **News → Blog** section. Use them for longer-form content: tutorials, perspectives, tool spotlights, or community stories. Unlike announcements, blog posts are not primarily time-sensitive — they are evergreen articles.

---

## Where the files live

```
content/blog/
└── your-post-slug/
    ├── index.md
    └── featured.png   ← optional cover image
```

---

## Step-by-step

1. Create a new folder inside `content/blog/` with a short descriptive name (lowercase, hyphenated).
2. Inside that folder, create `index.md`.
3. Optionally add a cover image named `featured.png` or `featured.jpg` in the same folder.
4. Fill in the front matter and write the post body in Markdown.

---

## Template

```markdown
---
title: "Your Post Title"
date: 2026-06-01
authors:
  - your-author-slug    # must match a folder name under content/authors/
tags:
  - SBOL
  - Tutorial
summary: "One or two sentences describing the post. Shown in the card preview."
featured: false
image:
  caption: ""
  focal_point: "Smart"
---

Write your post here in plain Markdown.
```

---

## Real example

`content/blog/sample-post/index.md`

```markdown
---
title: "Welcome to the SBOL Blog"
date: 2026-05-17
authors:
  - prashant-vaidyanathan
tags:
  - synthetic biology
  - SBOL
  - community
summary: "Introducing the new SBOL community blog..."
featured: false
image:
  caption: ""
  focal_point: ""
---

Welcome to the SBOL community blog...
```

---

## Field reference

| Field | Required | Notes |
|---|---|---|
| `title` | Yes | Heading shown on the post page and in cards |
| `date` | Yes | ISO format (`YYYY-MM-DD`) |
| `authors` | No | List of author slugs from `content/authors/`. Leave blank to omit author attribution |
| `tags` | No | Freeform list used for filtering |
| `summary` | Yes | Short preview shown in card listings |
| `featured` | No | Set to `true` to pin as the lead article at the top of the blog page |
| `image.focal_point` | No | Where to crop the cover image. Options: `Smart`, `Center`, `Top`, `Bottom`, `Left`, `Right` |

---

## Author slugs

Author slugs are the folder names under `content/authors/`. For example, `prashant-vaidyanathan` corresponds to `content/authors/prashant-vaidyanathan/`. If you are a new author, see the [Leadership guide](07-leadership.md) for how to create an author profile — the same profile is used for blog attribution.

---

## Common mistakes

- **Wrong folder** — blog posts go in `content/blog/`, not `content/post/`. Posts in `content/post/` appear as announcements.
- **Author slug not found** — if the slug doesn't match an existing folder under `content/authors/`, the author line is silently dropped. Check the folder name carefully.
- **Cover image wrong name** — the image must be named `featured.png` or `featured.jpg` exactly. Any other name will be ignored.
